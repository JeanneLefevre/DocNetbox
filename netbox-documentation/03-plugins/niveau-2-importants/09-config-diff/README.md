# NetBox Config Diff (rang 9 · niveau 2)

## À quoi ça sert

Compare la **configuration voulue** (générée depuis NetBox avec les *Config Templates*) avec la **configuration réelle** de l'équipement (running-config) et affiche les **écarts**. Selon la version, peut aussi aider à déployer 🔎.

## Principe

```
Données NetBox + Config Template (Jinja2)  →  config "attendue"
Connexion à l'équipement                    →  config "réelle"
                    Comparaison → diff
```

## Prérequis 🔎

- Des **Config Templates** NetBox (fonction native : *Provisionnement → Config Templates*) associés aux équipements, rôles ou plateformes.
- Une **plateforme** correctement renseignée (pilote / type de connexion).
- Des **identifiants** d'accès (compte en lecture si possible) et un accès réseau depuis NetBox.

## Intérêt

Détecter la dérive de configuration (*drift*), contrôler après un changement.

↩ [Niveau 2](../README.md) · [utilisation.md](utilisation.md)
