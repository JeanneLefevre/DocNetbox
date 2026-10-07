# NetBox Lists (rang 16 · niveau 3)

## À quoi ça sert

Expose des **listes brutes** (IP, préfixes, équipements…) consommables par d'autres outils sans interprétation de l'API complète : par exemple un pare-feu qui lit une liste d'adresses à une URL.

## Intérêt

Mise à jour automatique de listes d'adresses (ex. « serveurs de production ») sans intervention manuelle. Complète [Security](../../niveau-2-importants/11-security/README.md).

## Point d'attention

Les points d'accès sont sous `/api/plugins/netbox_lists/` 🔎 : vérifier la liste exacte et les paramètres de filtre dans le README du plugin. (Cette correction remplace le chemin `/api/plugins/lists/` cité dans la première version.)

↩ [Niveau 3](../README.md) · [utilisation.md](utilisation.md)
