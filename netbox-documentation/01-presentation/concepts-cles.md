# Concepts clés

## Ordre logique de modélisation (du plus global au plus précis)

```
Région → Site → Emplacement (Location) → Baie (Rack) → Équipement (Device) → Interfaces / Câbles / IP
```

## Objets de référence à créer AVANT les équipements

| Objet | Rôle | Exemples |
|---|---|---|
| **Fabricants** (Manufacturers) | Constructeurs | Cisco, Juniper, Dell |
| **Types d'équipement** (Device Types) | Modèle précis avec interfaces, ports, hauteur en U | Catalyst 9300-48P |
| **Rôles d'équipement** (Device Roles) | Fonction | switch, routeur, firewall, serveur |
| **Plateformes** (Platforms) | Système d'exploitation, utilisé aussi par l'automatisation | IOS-XE, JunOS, Linux |

## Autres objets fréquents

| Objet | Utilité |
|---|---|
| **Tenants** | Client / équipe propriétaire |
| **Tags** | Étiquettes libres pour filtrer |
| **Custom Fields** | Champs personnalisés ajoutés à n'importe quel objet |
| **Config Contexts** | Variables JSON attachées à des équipements (utiles à Ansible) |
| **Config Templates** | Modèles Jinja2 qui génèrent la configuration d'un équipement |
| **Journal / Changelog** | Historique des modifications |

## Voir aussi

- [Créer une baie](guides/creer-une-baie.md)
- [Ajouter un service](guides/ajouter-un-service.md)
