# Ajouter un service

Un **service** représente un protocole et un ou plusieurs ports TCP / UDP / SCTP exposés par un équipement, une VM ou (selon la version) une application.

> Exemples : `SSH (TCP/22)`, `HTTPS (TCP/443)`, `DNS (UDP/53)`, `NTP (UDP/123)`.

## Ajouter un service sur un équipement ou une VM

1. Ouvrir la fiche de l'**équipement** (ou de la **machine virtuelle**).
2. Onglet **Services** → **Ajouter un service**.
3. Renseigner :

| Champ | Exemple |
|---|---|
| Nom | `HTTPS` |
| Protocole | `TCP` |
| Ports | `443` (plusieurs possibles : `80,443`) |
| Adresses IP | IP(s) sur lesquelles le service écoute (optionnel) |
| Description | `Interface d'administration` |

4. Enregistrer.

## Utiliser des modèles de service (Service Templates)

1. **IPAM → Modèles de service → Ajouter** (ex. `SSH`, `SNMP`, `HTTPS`).
2. Sur un équipement, choisir **Ajouter un service depuis un modèle**.

## Intérêt

- Cartographier ce qui est exposé et sur quelles IP.
- Alimenter la documentation de flux / règles de pare-feu.
- Exploiter ces données via l'API pour la supervision ou l'automatisation.

## Plugins liés

- Documenter les flux entre applications → [Data Flows](../../03-plugins/niveau-2-importants/12-data-flows/README.md)
- Modéliser les règles de pare-feu → [Security](../../03-plugins/niveau-2-importants/11-security/README.md)
