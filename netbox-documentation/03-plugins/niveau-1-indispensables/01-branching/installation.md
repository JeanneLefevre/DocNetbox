# Branching : installation

Cette configuration est plus invasive que celle des autres plugins car elle touche à la base de données. Suivre d'abord la [procédure générique](../../installation-generique.md), avec les adaptations ci-dessous 🔎.

## `configuration.py`

```python
from netbox_branching.utilities import DynamicSchemaDict

DATABASES = DynamicSchemaDict({
    "default": {
        # ... votre configuration PostgreSQL habituelle ...
    }
})

DATABASE_ROUTERS = [
    "netbox_branching.database.BranchAwareRouter",
]

PLUGINS = [
    # ... autres plugins ...
    "netbox_branching",   # à placer en DERNIER dans la liste
]
```

## Base de données

L'utilisateur PostgreSQL de NetBox doit pouvoir **créer des schémas** (chaque branche utilise son propre schéma).

## Finalisation

```bash
python3 manage.py migrate
python3 manage.py collectstatic --no-input
sudo systemctl restart netbox netbox-rq
```

↩ [README du plugin](README.md)
