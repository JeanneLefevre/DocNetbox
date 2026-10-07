# Qu'est-ce que NetBox ?

NetBox est une application web open source (Django / PostgreSQL) qui sert de **source de vérité (Source of Truth)** pour une infrastructure réseau. Deux grandes familles de fonctions :

- **DCIM** (Data Center Infrastructure Management) : sites, salles, baies, équipements, câblage, alimentation.
- **IPAM** (IP Address Management) : préfixes, adresses IP, VLAN, VRF, ASN, services.

On y trouve aussi la virtualisation (clusters, VM), les circuits opérateurs, les tenants, les tags, les champs personnalisés, etc.

## À quoi ça sert concrètement ?

| Besoin | Apport de NetBox |
|---|---|
| Savoir « ce qui existe et où » | Inventaire centralisé et à jour |
| Éviter les conflits d'IP / VLAN | IPAM structuré avec hiérarchie de préfixes |
| Documenter le câblage | Câbles, interfaces, ports de façade, traces de bout en bout |
| Planifier la place en baie | Visualisation des baies, unités libres, réservations |
| Automatiser | API REST / GraphQL, webhooks, scripts, inventaire dynamique Ansible |
| Tracer les changements | Journal des modifications (changelog) |

> **Principe :** on décrit l'infrastructure **cible** dans NetBox, et les outils d'automatisation (Ansible, scripts…) lisent ces données pour configurer ou vérifier les équipements.

## Pour aller plus loin

- Vocabulaire et ordre de modélisation → [concepts-cles.md](concepts-cles.md)
- Guides pas à pas → [guides/](guides/)
- Automatisation → [../02-automatisation/](../02-automatisation/README.md)
- Plugins → [../03-plugins/](../03-plugins/README.md)
