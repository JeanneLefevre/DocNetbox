# Installation générique d'un plugin

> À adapter selon l'installation (paquet, Docker, `netbox-docker`…). Toujours lire le README du plugin.

## 1. Installer le paquet dans l'environnement virtuel de NetBox

```bash
source /opt/netbox/venv/bin/activate
pip install nom-du-plugin
echo "nom-du-plugin" >> /opt/netbox/local_requirements.txt   # pour survivre aux mises à jour
```

## 2. Déclarer le plugin dans `configuration.py`

```python
PLUGINS = ["nom_du_module"]          # Branching : toujours en dernier
PLUGINS_CONFIG = {
    "nom_du_module": {
        # options propres au plugin
    },
}
```

## 3. Migrations et fichiers statiques

```bash
cd /opt/netbox/netbox
python3 manage.py migrate
python3 manage.py collectstatic --no-input
```

## 4. Redémarrage

```bash
sudo systemctl restart netbox netbox-rq
```

## 5. Vérification

Le plugin doit apparaître dans le menu de NetBox (ou dans *Admin → Plugins* selon la version).

## Avec netbox-docker

- Ajouter le paquet dans le fichier de dépendances des plugins de l'image.
- Déclarer le plugin dans `configuration/plugins.py`.
- Reconstruire l'image, redémarrer les conteneurs, lancer les migrations.

## Avant chaque installation ou mise à jour

- **Sauvegarder** la base PostgreSQL.
- Vérifier la **compatibilité** de chaque plugin avec la version cible de NetBox.

↩ [Retour aux plugins](README.md)
