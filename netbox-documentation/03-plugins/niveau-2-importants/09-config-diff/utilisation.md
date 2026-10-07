# Config Diff : utilisation pas à pas 🔎

1. **Créer ou vérifier** le Config Template (modèle Jinja2) et l'associer au rôle / à la plateforme / à l'équipement.
2. **Prévisualiser** la configuration rendue sur la fiche de l'équipement (onglet *Render Config*) pour vérifier le modèle.
3. Configurer dans le plugin la **méthode de connexion** et les identifiants.
4. Lancer la **collecte** de la configuration réelle (tâche en arrière-plan).
5. Consulter le **diff** : lignes manquantes, en trop, différentes.
6. Décider : corriger **NetBox** (si la donnée est fausse) ou corriger **l'équipement** (si la configuration a dérivé).

↩ [README du plugin](README.md)
