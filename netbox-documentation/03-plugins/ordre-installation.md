# Ordre d'installation conseillé

L'ordre limite les problèmes de dépendances et apporte de la valeur progressivement.

1. **[Branching](niveau-1-indispensables/01-branching/README.md)** en premier (configuration de base de données : mieux vaut le faire tôt).
2. **[Inventory](niveau-1-indispensables/02-inventory/README.md)**, **[Interface Synchronization](niveau-1-indispensables/04-interface-synchronization/README.md)**, **[Reorder Rack](niveau-1-indispensables/03-reorder-rack/README.md)** : améliorent le quotidien sans prérequis lourds.
3. **[Routing](niveau-1-indispensables/05-routing/README.md)**, **[Topology Views](niveau-1-indispensables/06-topology-views/README.md)** : une fois le câblage et les IP bien renseignés.
4. **[IP Fabric](niveau-2-importants/07-ip-fabric/README.md)** *ou* **[Slurpit](niveau-2-importants/08-slurpit/README.md)** (un seul) : alimenter la donnée automatiquement.
5. **[NAPALM](niveau-2-importants/10-napalm/README.md)**, **[Config Diff](niveau-2-importants/09-config-diff/README.md)** : vérification en direct (accès aux équipements requis).
6. **[Security](niveau-2-importants/11-security/README.md)**, **[Data Flows](niveau-2-importants/12-data-flows/README.md)** : selon les projets sécurité.
7. **[Lifecycle](niveau-3-specialises/13-lifecycle/README.md)**, **[Contract](niveau-3-specialises/14-contract/README.md)**, **[Floorplan](niveau-3-specialises/15-floorplan/README.md)**, **[Lists](niveau-3-specialises/16-lists/README.md)**, **[Kea](niveau-3-specialises/17-kea/README.md)**, **[WDM](niveau-3-specialises/18-wdm/README.md)** : selon le besoin.

↩ [Retour aux plugins](README.md)
