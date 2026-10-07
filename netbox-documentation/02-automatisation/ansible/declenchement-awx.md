# Déclencher un playbook depuis NetBox (Event Rule + AWX / AAP)

NetBox envoie un message à AWX / Ansible Automation Platform quand un objet est créé ou modifié ; AWX lance le job.

## Étapes

1. Dans AWX / AAP, créer un **Job Template** et noter l'URL de lancement (`/api/v2/job_templates/<id>/launch/`).
2. Dans NetBox : **Intégrations (ou Opérations) → Webhooks** → créer un webhook pointant vers cette URL, avec l'en-tête d'authentification (Bearer token).
3. Créer une **Event Rule** (NetBox 4.x) :
   - type d'objet (ex. `Device`) ;
   - événement (création / mise à jour / suppression) ;
   - conditions optionnelles (ex. statut = `active`) ;
   - action : *Webhook*.
4. À chaque événement, NetBox envoie le contenu de l'objet à AWX, qui lance le job.

> Sur NetBox 3.x, les *Event Rules* n'existent pas : on configure directement le webhook avec les types d'objets et événements.

## Précautions

- Éviter les **boucles** : un job qui modifie NetBox peut redéclencher la règle.
- Utiliser des **conditions** pour ne cibler que les changements utiles (ex. passage au statut `active`).
- Stocker le token dans un coffre, jamais en clair dans un dépôt.

↩ [Retour à l'automatisation](../README.md)
