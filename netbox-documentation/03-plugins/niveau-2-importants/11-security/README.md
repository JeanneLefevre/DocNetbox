# NetBox Security (rang 11 · niveau 2)

## À quoi ça sert

Modélise les **objets de sécurité** de pare-feu (approche de type Juniper SRX) : qui peut parler à qui, avec quelle application, et avec quel NAT.

## Objets 🔎

- **Zones** de sécurité
- **Adresses**, **listes** et **ensembles** d'adresses
- **Applications** et **groupes** d'applications
- **Politiques** de sécurité (règles)
- **NAT** : jeux de règles, règles, pools

## Intérêt

- Documenter les flux autorisés au même endroit que l'inventaire et l'IPAM.
- Réutiliser les préfixes / IP déjà dans NetBox.
- Base pour automatiser la configuration de pare-feu.

## Astuce

Coupler avec [Data Flows](../12-data-flows/README.md) pour justifier chaque règle par un flux applicatif documenté, et avec [Lists](../../niveau-3-specialises/16-lists/README.md) pour alimenter les pare-feu en listes d'adresses.

↩ [Niveau 2](../README.md) · [utilisation.md](utilisation.md)
