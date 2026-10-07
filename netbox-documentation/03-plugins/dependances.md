# Dépendances et complémentarités entre plugins

| Association | Pourquoi |
|---|---|
| **Branching + tout import en masse** | Relire avant d'appliquer |
| **Branching + IP Fabric** | IP Fabric s'appuie sur les branches pour valider l'import |
| **Inventory + Lifecycle** | L'asset physique reçoit les contrats / licences |
| **Lifecycle + Contract** | Technique / support d'un côté, commercial / financier de l'autre |
| **Security + Data Flows** | Chaque règle de pare-feu est justifiée par un flux documenté |
| **Routing + Config Templates + Config Diff** | Données de routage → config générée → contrôle de dérive |
| **NAPALM + Topology Views** | Comparer voisins LLDP réels et câblage documenté |
| **Floorplan + Reorder Rack** | Placement des baies dans la salle puis des équipements dans la baie |
| **IP Fabric / Slurpit + Interface Synchronization** | Importer la réalité, puis remettre les composants d'équipement en cohérence |
| **Lists + Security** | Alimenter automatiquement les pare-feu en listes d'adresses |
| **Kea + IPAM** | Comparer les baux DHCP et les adresses documentées |
| **Routing + Security** | Cohérence entre chemins de routage et zones / politiques |
| **WDM + Circuits NetBox** | Rattacher les canaux optiques aux circuits |

> **Slurpit et IP Fabric** répondent au même besoin (alimenter NetBox depuis la découverte réseau) : on n'en utilise en général qu'un seul.

↩ [Retour aux plugins](README.md)
