# Inventaire dynamique Ansible depuis NetBox

C'est l'approche la plus simple : Ansible interroge NetBox pour construire son inventaire.

## 1. Créer un token d'API

*Profil utilisateur → Jetons d'API → Ajouter*. Préférer un token en **lecture seule**.

## 2. Installer la collection

```bash
ansible-galaxy collection install netbox.netbox
pip install pynetbox
```

## 3. Créer le fichier d'inventaire `netbox_inv.yml`

```yaml
plugin: netbox.netbox.nb_inventory
api_endpoint: https://netbox.example.com
token: "{{ lookup('env', 'NETBOX_TOKEN') }}"
validate_certs: true
config_context: false
group_by:
  - sites
  - device_roles
  - platforms
query_filters:
  - status: active
compose:
  ansible_host: primary_ip4.address | ansible.utils.ipaddr('address')
```

## 4. Vérifier l'inventaire

```bash
export NETBOX_TOKEN="xxxxxxxx"
ansible-inventory -i netbox_inv.yml --graph
```

## 5. Lancer un playbook

```bash
ansible-playbook -i netbox_inv.yml playbooks/config_ntp.yml --limit "device_roles_switch"
```

Exemple de playbook minimal :

```yaml
---
- name: Configurer NTP sur les switchs
  hosts: device_roles_switch
  gather_facts: false
  tasks:
    - name: Pousser le serveur NTP
      cisco.ios.ios_config:
        lines:
          - ntp server 10.0.0.1
```

↩ [Retour à l'automatisation](../README.md)
