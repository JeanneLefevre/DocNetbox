# NetBox NAPALM (rang 10 · niveau 2)

## À quoi ça sert

Affiche des **informations en direct** lues sur l'équipement (via la bibliothèque NAPALM), directement depuis sa fiche NetBox. Idéal pour comparer « documenté » et « réel » sans ouvrir de session SSH.

Cette fonction était intégrée au cœur de NetBox dans les anciennes versions, puis a été déplacée dans un plugin.

## Informations typiques

Faits (modèle, version, uptime), état des interfaces, voisins LLDP, table ARP, environnement (CPU, mémoire, température).

## Prérequis 🔎

- Pilote NAPALM associé à chaque **plateforme** (`ios`, `junos`, `eos`…).
- **IP principale** renseignée sur l'équipement.
- Identifiants dans la configuration du plugin.
- Accès réseau depuis le serveur NetBox vers les équipements.

## Sécurité

Compte en **lecture seule**, mot de passe stocké de manière sécurisée, accès réseau restreint.

↩ [Niveau 2](../README.md) · [configuration.md](configuration.md) · [utilisation.md](utilisation.md)
