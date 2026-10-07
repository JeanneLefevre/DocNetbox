# Inventory : utilisation pas à pas

1. Créer les **Suppliers** (fournisseurs / revendeurs).
2. Créer un **Purchase** (fournisseur, date, numéro de commande) et, si besoin, une **Delivery**.
3. Créer les **Assets** à la réception : type de matériel, numéro de série, étiquette, achat associé, date de fin de garantie.
4. Laisser l'asset au statut **stocké** avec un lieu de stockage tant qu'il n'est pas installé.
5. À l'installation, **affecter l'asset à un équipement** (Device), un module ou une baie, puis passer le statut à **en service**.
6. Au retrait, passer au statut **retiré** (au lieu de supprimer) pour garder l'historique.

## Astuce

Charger un parc existant : *Assets → Importer* (CSV) avec les colonnes série, étiquette, type de matériel, fournisseur.

↩ [README du plugin](README.md)
