# NetBox Kea (rang 17 · niveau 3)

## À quoi ça sert

Connecte NetBox à un ou plusieurs serveurs **DHCP ISC Kea** pour **consulter** (et selon les cas gérer) baux, réservations et sous-réseaux.

## Prérequis 🔎

- Kea avec le **Control Agent** actif et joignable depuis NetBox.
- Les modules (*hooks*) Kea nécessaires aux commandes (baux, sous-réseaux, hôtes) selon les fonctions utilisées.

## Intérêt

Repérer les écarts entre l'IPAM NetBox et ce que distribue réellement le DHCP (IP distribuée mais non documentée).

↩ [Niveau 3](../README.md) · [utilisation.md](utilisation.md)
