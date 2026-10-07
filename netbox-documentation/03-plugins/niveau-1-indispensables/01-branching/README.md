# NetBox Branching (rang 1 · niveau 1)

## À quoi ça sert

Fonctionne comme les branches Git : on crée une **copie de travail isolée** de NetBox, on y fait ses modifications sans toucher à la production, on les relit, puis on les **fusionne** (merge) dans la branche principale. On peut aussi **annuler** (revert) une fusion.

## Pourquoi c'est le plus important

C'est le filet de sécurité de toute la donnée. Une erreur dans une branche n'impacte personne. De plus, certains plugins (notamment [IP Fabric](../../niveau-2-importants/07-ip-fabric/README.md)) s'appuient dessus pour proposer des imports validables.

## Quand l'utiliser

- Gros changements (nouvelle baie complète, migration de VLAN…).
- Imports en masse (CSV, découverte automatique).
- Travail à plusieurs sur des sujets distincts.

## Prérequis 🔎

- NetBox **4.2 ou supérieur** (vérifier la matrice de compatibilité).
- Droit de **créer des schémas** pour l'utilisateur PostgreSQL de NetBox.
- Worker `netbox-rq` actif (provisionnement et fusion en dépendent).

## Pièges à éviter

- Ne pas laisser une branche vivre trop longtemps : les conflits s'accumulent.
- Une branche = un sujet précis.
- Sauvegarder PostgreSQL avant l'installation (la configuration touche à la base).

## Fichiers

- [installation.md](installation.md) : configuration spécifique (base de données)
- [utilisation.md](utilisation.md) : pas à pas

↩ [Niveau 1](../README.md)
