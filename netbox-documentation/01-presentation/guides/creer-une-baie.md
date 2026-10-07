# Créer une baie (rack)

## Prérequis

- Un **Site** existant (*Organisation → Sites*).
- Optionnel : un **Emplacement / Location** (salle, étage) et un **Rôle de baie** (*Équipements → Rôles de baie*).

## Étapes

1. Aller dans **Équipements (DCIM) → Baies → Ajouter**.
2. Renseigner les champs :

| Champ | Exemple | Remarque |
|---|---|---|
| Nom | `BAIE-A01` | Obligatoire, unique dans l'emplacement |
| Site | `DC-Paris` | Obligatoire |
| Emplacement | `Salle 1` | Recommandé |
| Statut | `Active` | Actif, réservé, planifié… |
| Rôle | `Serveurs` | Optionnel |
| Type | `Baie 19" 4 montants` | Optionnel |
| Largeur | `19 pouces` | |
| Hauteur (U) | `42` | |
| Numéro d'U de départ | `1` | |
| Numérotation décroissante | à cocher si U1 est en haut | |
| Profondeur, poids max… | | Utile pour la planification |

3. Cliquer sur **Créer**.

## Placer un équipement dans la baie

1. **Équipements → Équipements → Ajouter**.
2. Choisir **Type d'équipement**, **Rôle**, **Site**.
3. Renseigner **Baie**, **Position** (numéro d'U) et **Face** (avant / arrière).
4. Enregistrer : l'équipement apparaît dans l'élévation de la baie.

## Astuces

- Plusieurs baies d'un coup : **Importer** (CSV / YAML / JSON) ou import en masse.
- Les **réservations de baie** (*Rack Reservations*) bloquent des U pour un projet futur.
- La vue de la baie affiche élévation avant / arrière, taux d'occupation et consommation électrique (si les ports d'alimentation sont renseignés).

## Plugins liés

- Déplacer les équipements par glisser-déposer → [Reorder Rack](../../03-plugins/niveau-1-indispensables/03-reorder-rack/README.md)
- Placer la baie dans un plan de salle → [Floorplan](../../03-plugins/niveau-3-specialises/15-floorplan/README.md)
- Suivre le matériel réel (série, achat) → [Inventory](../../03-plugins/niveau-1-indispensables/02-inventory/README.md)
