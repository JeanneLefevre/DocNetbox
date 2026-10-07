# IP Fabric pour NetBox (rang 7 · niveau 2)

## À quoi ça sert

[IP Fabric](https://ipfabric.io) est une plateforme qui **découvre** automatiquement le réseau réel (équipements, interfaces, IP, VLAN, VRF…). Le plugin importe ces données dans NetBox pour **aligner la documentation sur la réalité**.

## Prérequis

- Une **instance et une licence IP Fabric** avec un jeton d'API.
- [Branching](../../niveau-1-indispensables/01-branching/README.md) : les imports sont normalement faits dans une branche à relire avant fusion 🔎.

## Notions

| Notion | Rôle |
|---|---|
| **Source** | Connexion à IP Fabric (URL, token) |
| **Snapshot** | Photographie du réseau à une date donnée |
| **Transform Maps** | Règles de correspondance entre champs IP Fabric et objets NetBox |
| **Sync** | Tâche d'import (manuelle ou planifiée) |
| **Ingestion** | Résultat d'une exécution, avec les changements proposés |

## Différence avec Slurpit

Même besoin (« réalité → NetBox »). IP Fabric passe par Branching ; [Slurpit](../08-slurpit/README.md) a sa propre zone de staging. **On en utilise généralement un seul.**

↩ [Niveau 2](../README.md) · [utilisation.md](utilisation.md)
