# NetBox WDM (rang 18 · niveau 3)

> Correction : le plugin s'appelle **WDM** (et non « WDW »).

## À quoi ça sert

**WDM** = *Wavelength Division Multiplexing* (multiplexage en longueur d'onde) : plusieurs canaux optiques circulent sur une même fibre, chacun sur sa longueur d'onde (DWDM / CWDM). Le plugin `netbox-wdm` apporte la **gestion des longueurs d'onde** dans NetBox.

D'après sa description publique (PyPI), il couvre :

- les **plans de canaux ITU** (grilles de longueurs d'onde) ;
- l'**édition de ROADM** (*Reconfigurable Optical Add-Drop Multiplexer*) ;
- le **contrôle de cohérence des positions** (*position stack enforcement*).

🔎 Les détails (modèles exacts, menus, règles de cohérence) ne figurent pas dans cette documentation faute de source détaillée : à compléter à partir du dépôt du plugin.

## Quand l'utiliser

Uniquement si vous exploitez un **réseau optique WDM** (liaisons DWDM / CWDM, multiplexeurs, ROADM). Sinon, ce plugin n'a pas d'intérêt.

## Complémentarité

Rattacher les canaux aux **circuits** et au **câblage** NetBox. Pour la documentation des câbles physiques, voir aussi [Topology Views](../../niveau-1-indispensables/06-topology-views/README.md).

## Fiche à compléter

| Élément | Valeur |
|---|---|
| Dépôt / source | `netbox-wdm` (PyPI) |
| Version installée | `à renseigner` |
| Menus / objets ajoutés | `à renseigner` |
| Dépendances | `à renseigner` |
| Fréquence d'usage réelle | `à renseigner` |

↩ [Niveau 3](../README.md) · [utilisation.md](utilisation.md)
