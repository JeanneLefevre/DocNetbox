# Plugins NetBox : vue d'ensemble et classement

Les plugins étendent NetBox avec de nouveaux modèles de données, vues et API. Le comportement exact dépend de la **version du plugin** et de sa **compatibilité avec votre version de NetBox** : toujours vérifier le dépôt du plugin.

## Méthode de classement

| Critère | Question posée |
|---|---|
| **Importance** | Que se passe-t-il sans ce plugin ? (risque, perte de fiabilité de la donnée, travail manuel) |
| **Fréquence** | À quelle cadence un exploitant l'utilise-t-il réellement ? |

> Le classement correspond à un usage typique en exploitation réseau / datacenter. Ajustez-le selon votre organisation (ex. licence IP Fabric ou Slurpit).

## Tableau récapitulatif

| Rang | Plugin | Niveau | Rôle en une phrase | Fréquence |
|---|---|---|---|---|
| 1 | [Branching](niveau-1-indispensables/01-branching/README.md) | 1 | Modifier NetBox dans une branche isolée, puis fusionner | Quotidienne |
| 2 | [Inventory](niveau-1-indispensables/02-inventory/README.md) | 1 | Gérer les actifs physiques (série, achat, stock, garantie) | Quotidienne |
| 3 | [Reorder Rack](niveau-1-indispensables/03-reorder-rack/README.md) | 1 | Réorganiser les équipements d'une baie par glisser-déposer | Hebdomadaire |
| 4 | [Interface Synchronization](niveau-1-indispensables/04-interface-synchronization/README.md) | 1 | Remettre les composants d'un équipement en phase avec son modèle | Hebdomadaire |
| 5 | [Routing](niveau-1-indispensables/05-routing/README.md) | 1 | Documenter routes statiques, BGP, OSPF | Hebdomadaire |
| 6 | [Topology Views](niveau-1-indispensables/06-topology-views/README.md) | 1 | Générer des schémas de topologie depuis le câblage | Hebdomadaire |
| 7 | [IP Fabric](niveau-2-importants/07-ip-fabric/README.md) | 2 | Importer la réalité du réseau découverte par IP Fabric | Planifiée |
| 8 | [Slurpit](niveau-2-importants/08-slurpit/README.md) | 2 | Importer les équipements découverts par Slurpit (avec validation) | Planifiée |
| 9 | [Config Diff](niveau-2-importants/09-config-diff/README.md) | 2 | Comparer config voulue (NetBox) et config réelle | Planifiée / à la demande |
| 10 | [NAPALM](niveau-2-importants/10-napalm/README.md) | 2 | Interroger un équipement en direct depuis sa fiche | À la demande |
| 11 | [Security](niveau-2-importants/11-security/README.md) | 2 | Modéliser zones, politiques et NAT de pare-feu | Par projet |
| 12 | [Data Flows](niveau-2-importants/12-data-flows/README.md) | 2 | Documenter les flux applicatifs (matrice de flux) | Par projet |
| 13 | [Lifecycle](niveau-3-specialises/13-lifecycle/README.md) | 3 | Suivre fin de vie, supports et licences | Mensuelle / annuelle |
| 14 | [Contract](niveau-3-specialises/14-contract/README.md) | 3 | Gérer contrats et factures liés à l'infra | Occasionnelle |
| 15 | [Floorplan](niveau-3-specialises/15-floorplan/README.md) | 3 | Plan de salle avec placement des baies | Occasionnelle |
| 16 | [Lists](niveau-3-specialises/16-lists/README.md) | 3 | Exposer des listes brutes (IP, préfixes) à d'autres outils | Automatique (machine) |
| 17 | [Kea](niveau-3-specialises/17-kea/README.md) | 3 | Consulter / gérer un DHCP Kea | Si Kea utilisé |
| 18 | [WDM](niveau-3-specialises/18-wdm/README.md) | 3 | Gestion des longueurs d'onde (plans de canaux ITU, ROADM) | Si réseau optique WDM |

## Autres documents de cette section

- [Installation générique d'un plugin](installation-generique.md)
- [Ordre d'installation conseillé](ordre-installation.md)
- [Dépendances et complémentarités](dependances.md)

## Structure des dossiers

Chaque plugin a son dossier `NN-nom/` contenant au minimum :

- `README.md` : à quoi ça sert, prérequis, intérêt, pièges (le « pourquoi »).
- `utilisation.md` : pas à pas (le « comment »).
- `installation.md` : uniquement quand la mise en place sort de la procédure générique.
