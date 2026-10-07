# Lancer un job via un bouton (Custom Link)

Un **Custom Link** (*Personnalisation → Liens personnalisés*) ajoute un bouton sur la fiche d'un objet (ex. un équipement). Il ouvre une URL, par exemple la page de lancement d'un job AWX, en passant des paramètres.

## Étapes

1. *Personnalisation → Liens personnalisés → Ajouter*.
2. Choisir le **type d'objet** (ex. `dcim | device`).
3. Renseigner le **texte du bouton** et l'**URL** avec des variables Jinja2 :

```
https://awx.example.com/#/templates/job_template/12/survey?hostname={{ object.name }}&ip={{ object.primary_ip4.address.ip }}
```

4. Choisir la position du bouton (groupe) et enregistrer.
5. Ouvrir une fiche d'équipement : le bouton apparaît.

## Quand l'utiliser

Actions **manuelles ciblées** : redémarrer un service, relancer une sauvegarde, ouvrir une session de diagnostic.

↩ [Retour à l'automatisation](../README.md)
