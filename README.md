# IronTrack Data Repository Template

Este directorio contiene la plantilla que debes subir a tu repositorio público en GitHub (por ejemplo `irontrack-data`).

## Estructura recomendada en GitHub

```text
irontrack-data/
├── catalog.json
└── assets/
    ├── routines/
    │   ├── ppl.webp
    │   ├── upper_lower.webp
    │   ├── full_body.webp
    │   └── glute_core.webp
    └── exercises/
        ├── bench_press.gif
        └── ...
```

## Cómo conectarlo a la app

1. Sube `catalog.json` y la carpeta `assets/` a tu repositorio de GitHub (rama `main`).
2. Reemplaza `TU_USUARIO` dentro de `catalog.json` por tu usuario real de GitHub.
3. En el proyecto Android (`app/src/main/java/com/irontrack/app/data/remote/GitHubConfig.kt`), `BASE_URL` apunta a:
   `https://raw.githubusercontent.com/alesr1704-glitch/irontrack-data/main/`
4. Recarga dentro de la app usando el botón de sincronización.
