# Documentation NetBox

Point d'entrée de la documentation. L'arborescence va **du plus général (racine) au plus spécifique (sous-dossiers profonds)**.

```
netbox-documentation/
├── README.md                      ← vous êtes ici (vue générale)
├── 01-presentation/               ← qu'est-ce que NetBox, concepts
│   └── guides/                    ← pas à pas : baie, service
├── 02-automatisation/             ← pourquoi / comment automatiser
│   └── ansible/                   ← playbooks, inventaire dynamique, AWX
└── 03-plugins/                    ← classement et vue d'ensemble des 18 plugins
    ├── niveau-1-indispensables/   ← usage quotidien / hebdomadaire
    │   └── NN-nom-du-plugin/      ← détail d'un plugin (README, utilisation…)
    ├── niveau-2-importants/
    └── niveau-3-specialises/
```

## Par où commencer ?

| Je veux… | Aller à |
|---|---|
| Comprendre à quoi sert NetBox | [01-presentation/README.md](01-presentation/README.md) |
| Connaître le vocabulaire et l'ordre de modélisation | [01-presentation/concepts-cles.md](01-presentation/concepts-cles.md) |
| Créer une baie | [01-presentation/guides/creer-une-baie.md](01-presentation/guides/creer-une-baie.md) |
| Ajouter un service | [01-presentation/guides/ajouter-un-service.md](01-presentation/guides/ajouter-un-service.md) |
| Comprendre pourquoi lancer un playbook depuis NetBox | [02-automatisation/README.md](02-automatisation/README.md) |
| Voir la liste et le classement des plugins | [03-plugins/README.md](03-plugins/README.md) |

> ⚠️ Les menus et options varient selon la version de NetBox (3.x / 4.x) et des plugins. Les passages marqués 🔎 sont à valider sur votre instance et dans le README du plugin concerné.
