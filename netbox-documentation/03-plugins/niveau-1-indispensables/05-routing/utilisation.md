# Routing : utilisation pas à pas

## Exemple BGP

1. Vérifier que l'**ASN** existe (*IPAM → ASN*) et que les équipements ont leurs interfaces / IP.
2. Menu **Routing** : créer les **paramètres BGP** du routeur (équipement + ASN, éventuellement VRF).
3. Créer un **groupe de voisins** pour factoriser les paramètres communs (AS distant, politiques).
4. Créer chaque **voisin** (peer) : adresse locale, adresse distante, AS distant, groupe.
5. Ajouter les **familles d'adresses** (IPv4 / IPv6 unicast…) si nécessaire.
6. Relier aux **listes de préfixes** / **route-maps** pour documenter les politiques d'import / export.

## Exemple route statique

*Routing → Static routes → Ajouter* : équipement (et VRF), préfixe de destination, prochain saut, métrique.

↩ [README du plugin](README.md)
