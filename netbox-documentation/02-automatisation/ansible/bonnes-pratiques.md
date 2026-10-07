# Bonnes pratiques d'automatisation avec NetBox

- **Ne jamais stocker de mots de passe dans NetBox en clair** : utiliser Ansible Vault ou le coffre d'AWX.
- Utiliser des **Config Contexts** ou des **Custom Fields** pour porter les variables spécifiques (ex. serveurs DNS par site).
- **Restreindre** le token d'API (lecture seule pour l'inventaire).
- Tester avec `--check` / `--diff` avant d'appliquer.
- Écrire dans NetBox le **résultat** de l'automatisation (statut, date) pour garder la source de vérité fiable.
- Pour les imports massifs, passer par une **branche** ([Branching](../../03-plugins/niveau-1-indispensables/01-branching/README.md)) afin de relire avant fusion.
- Contrôler régulièrement la dérive avec [Config Diff](../../03-plugins/niveau-2-importants/09-config-diff/README.md).

↩ [Retour à l'automatisation](../README.md)
