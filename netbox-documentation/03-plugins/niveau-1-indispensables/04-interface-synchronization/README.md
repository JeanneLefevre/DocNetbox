# NetBox Interface Synchronization (rang 4 · niveau 1)

## À quoi ça sert

Quand on modifie un **type d'équipement** (ajout d'interfaces, correction de noms…), les équipements **déjà créés** ne sont pas mis à jour automatiquement. Le plugin compare les composants réels de chaque équipement avec ceux du modèle et propose de les resynchroniser.

## Composants concernés

Interfaces, ports console, ports série, alimentations, baies de modules, ports avant / arrière.

## Pièges

- Ne **pas supprimer** une interface déjà câblée ou portant une IP sans l'avoir vérifié.
- Pour un grand nombre d'équipements, travailler par lots et dans une [branche](../01-branching/README.md).

## Complémentarité

Après un import de découverte ([IP Fabric](../../niveau-2-importants/07-ip-fabric/README.md), [Slurpit](../../niveau-2-importants/08-slurpit/README.md)), permet de remettre les composants en cohérence.

↩ [Niveau 1](../README.md) · [utilisation.md](utilisation.md)
