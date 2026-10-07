# Automatisation avec NetBox

## Pourquoi utiliser un playbook avec NetBox ?

Sans NetBox, un playbook Ansible contient souvent des variables saisies à la main (IP, VLAN, hostnames…) qui divergent vite de la réalité. Avec NetBox :

- **Une seule source de vérité** : les variables viennent de NetBox, plus de doublons ni d'incohérences.
- **Inventaire dynamique** : la liste des équipements, leurs groupes (site, rôle, plateforme…) et leurs variables sont générés automatiquement.
- **Déclenchement piloté par les données** : un changement de statut ou la création d'un équipement peut lancer une automatisation.
- **Traçabilité** : on sait qui a modifié quoi dans NetBox et quel job a été lancé.
- **Moins d'erreurs humaines** : on modifie la donnée, le playbook applique.

## Trois approches possibles

| Approche | Principe | Quand l'utiliser | Détail |
|---|---|---|---|
| **Inventaire dynamique** | Ansible lit NetBox via `netbox.netbox.nb_inventory` | Le plus courant : Ansible va chercher les données | [inventaire-dynamique.md](ansible/inventaire-dynamique.md) |
| **Déclenchement par événement** | NetBox appelle AWX / AAP via une *Event Rule* (ex-*webhook*) | Réagir à une création / modification | [declenchement-awx.md](ansible/declenchement-awx.md) |
| **Lien personnalisé** | Un *Custom Link* ouvre / lance un job depuis une fiche | Action manuelle ciblée | [custom-link.md](ansible/custom-link.md) |

Bonnes pratiques communes → [ansible/bonnes-pratiques.md](ansible/bonnes-pratiques.md)

## Plugins qui renforcent l'automatisation

- [Config Diff](../03-plugins/niveau-2-importants/09-config-diff/README.md) : détecter la dérive de configuration.
- [NAPALM](../03-plugins/niveau-2-importants/10-napalm/README.md) : lire l'état réel des équipements.
- [Lists](../03-plugins/niveau-3-specialises/16-lists/README.md) : alimenter pare-feu / supervision en listes brutes.
- [Branching](../03-plugins/niveau-1-indispensables/01-branching/README.md) : relire avant d'appliquer des imports automatiques.
