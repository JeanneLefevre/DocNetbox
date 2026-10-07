# NetBox Inventory (rang 2 · niveau 1)

## À quoi ça sert

Ajoute la notion d'**actif physique (asset)**. Dans NetBox, un *Device* est un équipement logique à un endroit donné ; un *Asset* est l'objet réel avec son numéro de série, sa provenance et son état. Permet de suivre aussi ce qui est **en stock** ou **retiré**.

## Objets principaux

- **Assets** : numéro de série, étiquette d'actif, statut (stocké, en service, retiré…), lieu de stockage.
- **Types de matériel** : liens vers types d'équipement / modules / éléments d'inventaire.
- **Fournisseurs (Suppliers)**, **Achats (Purchases)**, **Livraisons (Deliveries)**.
- **Groupes** d'éléments d'inventaire.

## Cas d'usage

- Suivre les équipements en **stock** avant installation.
- Retrouver l'origine d'un matériel (commande, date, garantie).
- Faire des **audits** : documenté vs réellement installé.

## Bon usage

- Donne la « vérité physique » ; à combiner avec [Lifecycle](../../niveau-3-specialises/13-lifecycle/README.md) pour les contrats de support.
- Utiliser l'import CSV pour charger un parc existant en masse.
- Des options de configuration permettent de synchroniser numéro de série / étiquette entre l'asset et l'équipement 🔎.

↩ [Niveau 1](../README.md) · [utilisation.md](utilisation.md)
