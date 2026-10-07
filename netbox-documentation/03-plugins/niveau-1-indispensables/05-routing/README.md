# NetBox Routing (rang 5 · niveau 1)

## À quoi ça sert

Le cœur de NetBox ne décrit pas la couche routage. Ce plugin ajoute les **objets de routage** pour disposer d'une vision structurée des voisinages et des chemins.

## Objets typiques 🔎

- **Routes statiques** (préfixe, prochain saut, métrique, VRF).
- **BGP** : paramètres de routeur (ASN), groupes de voisins, **voisins** (peers), familles d'adresses.
- **OSPF** : instances, aires, interfaces.
- **Listes de préfixes** et **route-maps**.

## Intérêt

Audit rapide (« qui est voisin de qui ? »), source de données pour générer les configurations avec Ansible et [Config Templates](../../../01-presentation/concepts-cles.md).

↩ [Niveau 1](../README.md) · [utilisation.md](utilisation.md)
