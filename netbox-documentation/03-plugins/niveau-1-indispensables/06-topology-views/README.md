# NetBox Topology Views (rang 6 · niveau 1)

## À quoi ça sert

Génère un **schéma réseau interactif** à partir des équipements et du câblage. Permet de documenter sans dessiner à la main.

## Prérequis essentiel

Un câblage **correctement saisi** dans NetBox. Sans câbles, pas de liens sur le schéma.

## Fonctionnalités

- Filtrage par site, emplacement, rôle d'équipement, tags.
- Affichage des liaisons entre équipements.
- Positionnement manuel des nœuds, sauvegarde possible des coordonnées.
- Export de l'image.

## Astuces 🔎

- Utiliser un **tag** ou un **rôle** pour exclure les équipements non pertinents (patch panels, PDU…).
- Options dans `PLUGINS_CONFIG` pour autoriser la sauvegarde des coordonnées et ignorer certains types de câbles.

## Complémentarité

Comparer avec les voisins LLDP réels via [NAPALM](../../niveau-2-importants/10-napalm/README.md).

↩ [Niveau 1](../README.md) · [utilisation.md](utilisation.md)
