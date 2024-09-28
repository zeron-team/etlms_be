# ETLMS BACKEND

## Estructura
```text 
etl_management/
│
├── core/                    # Núcleo del proyecto Django
│   ├── settings.py          # Configuraciones del proyecto
│   ├── urls.py              # Rutas del proyecto
│   └── wsgi.py              # Interfaz WSGI para el despliegue
│
├── apps/                    # Directorio para las aplicaciones Django
│   ├── data_sources/        # Gestión de fuentes de datos
│   │   ├── models.py        # Modelos de la aplicación
│   │   ├── views.py         # Vistas y lógica de negocio
│   │   ├── serializers.py   # Serializadores para la API REST
│   │   ├── urls.py          # Rutas de la aplicación
│   │   └── services.py      # Servicios específicos de la aplicación
│   │
│   ├── etl_processes/       # Gestión de procesos ETL
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── services.py
│   │
│   ├── transformations/     # Gestión de reglas de transformación
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── urls.py
│   │   └── services.py
│   │
│   └── executions/          # Gestión de ejecuciones de procesos
│       ├── models.py
│       ├── views.py
│       ├── serializers.py
│       ├── urls.py
│       └── services.py
│
├── requirements.txt         # Dependencias del proyecto
└── manage.py                # Comando de administración de Django
```
## Git
- echo "# etlms_be" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main
- git remote add origin https://github.com/zeron-team/etlms_be.git
- git push -u origin master