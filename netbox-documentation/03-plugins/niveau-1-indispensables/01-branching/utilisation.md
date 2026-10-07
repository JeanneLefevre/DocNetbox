# Branching : utilisation pas à pas

1. **Créer la branche** : *Plugins → Branching → Branches → Ajouter*. Nom explicite (ex. `ajout-baie-b12`).
2. **Attendre le provisionnement** : le statut passe de *New* / *Provisioning* à **Ready**.
3. **Activer la branche** : sélecteur de branche dans la barre supérieure. Un bandeau indique que vous travaillez dans la branche.
4. **Faire les modifications** normalement (baies, équipements, IP…).
5. **Relire** : fiche de la branche, onglet **Changes**.
6. **Synchroniser** (*Sync*) si la branche principale a évolué, pour récupérer ses changements et détecter les conflits.
7. **Fusionner** (*Merge*) : les changements sont appliqués à la production. Utiliser d'abord la simulation (*dry run*) si elle est proposée.
8. **Annuler au besoin** (*Revert*) après une fusion.
9. **Revenir sur la branche principale** via le sélecteur.

↩ [README du plugin](README.md)
