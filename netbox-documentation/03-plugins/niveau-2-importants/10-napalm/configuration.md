# NAPALM : configuration 🔎

Après la [procédure générique](../../installation-generique.md), dans `configuration.py` :

```python
PLUGINS_CONFIG = {
    "netbox_napalm_plugin": {
        "NAPALM_USERNAME": "compte_lecture",
        "NAPALM_PASSWORD": "••••••••",
        "NAPALM_TIMEOUT": 10,
    },
}
```

Puis dans NetBox :

1. Associer un **pilote NAPALM** (ex. `ios`, `junos`, `eos`) à chaque **plateforme** concernée (configuration de plateforme du plugin).
2. S'assurer que chaque équipement a une **IP principale** et la bonne plateforme.

↩ [README du plugin](README.md)
