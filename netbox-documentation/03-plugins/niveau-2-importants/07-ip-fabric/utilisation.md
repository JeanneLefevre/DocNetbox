# IP Fabric : utilisation pas à pas 🔎

1. Créer une **Source** (*Plugins → IP Fabric → Sources*) : URL, token, vérification SSL. Tester la connexion.
2. Vérifier les **Snapshots** disponibles (le dernier snapshot chargé est généralement utilisé).
3. Contrôler (ou adapter) les **Transform Maps** : types d'équipement, rôles, sites… doivent correspondre aux objets existants dans NetBox.
4. Créer une **Sync** : source, snapshot, sites / objets à importer, éventuellement une planification.
5. **Lancer** la synchronisation. Le plugin crée une branche et applique les changements dedans.
6. **Relire** l'ingestion (créations, modifications, erreurs).
7. **Fusionner** la branche si tout est correct.

## Conseils

- Commencer par **un seul site** pour valider les correspondances avant d'élargir.
- Définir au préalable les règles de nommage (sites, rôles) pour éviter les doublons.

↩ [README du plugin](README.md)
