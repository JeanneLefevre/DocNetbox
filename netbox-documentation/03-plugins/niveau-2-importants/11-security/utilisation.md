# Security : utilisation pas à pas

Ordre recommandé : des briques vers l'assemblage.

1. Créer les **zones** (ex. `trust`, `untrust`, `dmz`) et les associer aux interfaces / équipements.
2. Créer les **adresses** (réutiliser les IP / préfixes de l'IPAM) puis les regrouper en **listes / ensembles**.
3. Créer les **applications** (protocole + ports) et les regrouper.
4. Créer la **politique** : zone source, zone destination, adresses source / destination, application, action (autoriser / refuser).
5. Si besoin, ajouter les **règles de NAT** (source, destination, statique) avec leurs pools.

↩ [README du plugin](README.md)
