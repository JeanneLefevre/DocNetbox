# Slurpit pour NetBox (rang 8 · niveau 2)

## À quoi ça sert

[Slurpit](https://slurpit.io) est un outil de découverte et d'inventaire réseau. Le plugin synchronise ses données (équipements, interfaces, préfixes, IP, VLAN) vers NetBox **avec une étape de validation** : les objets découverts arrivent d'abord dans une zone de transit (*staging*), puis on décide de les intégrer.

## Prérequis

Une instance Slurpit joignable et sa clé d'API.

## Différence avec IP Fabric

Slurpit utilise une zone de staging propre au plugin ; [IP Fabric](../07-ip-fabric/README.md) s'appuie sur [Branching](../../niveau-1-indispensables/01-branching/README.md). **On en utilise généralement un seul.**

↩ [Niveau 2](../README.md) · [utilisation.md](utilisation.md)
