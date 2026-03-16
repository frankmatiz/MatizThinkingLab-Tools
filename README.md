# MATIZ Knowledge Platform

Plataforma de herramientas interactivas desarrollada por **MATIZ – Leadership & Thinking Lab**.

## Estructura

```
matiz-tools/
├── index.html                              ← Hub principal con búsqueda
├── netlify.toml                            ← Configuración Netlify
├── thinking/
│   ├── index.html                          ← Categoría: Thinking
│   └── simulador-inversiones/
│       └── index.html                      ← Simulador de inversiones
├── cybersecurity/
│   └── index.html                          ← Categoría: Cybersecurity
├── process-transformation/
│   └── index.html                          ← Categoría: Process Transformation
└── technology/
    └── index.html                          ← Categoría: Technology
```

## Categorías

| Categoría | Color | Herramientas activas |
|---|---|---|
| Thinking | Dorado `#f5c542` | 1 |
| Cybersecurity | Cyan `#22d3ee` | 0 (próximamente) |
| Process Transformation | Naranja `#fb923c` | 0 (próximamente) |
| Technology | Azul `#60a5fa` | 0 (próximamente) |

## Agregar una herramienta nueva

1. Crea la carpeta: `{categoria}/{nombre-herramienta}/`
2. Agrega `index.html` con el password gate incluido
3. Actualiza el catálogo en `index.html` raíz (array `CATALOG`)
4. Agrega la tarjeta en la página de categoría correspondiente
5. Sube los cambios → Netlify despliega automáticamente

## Acceso

Las herramientas individuales están protegidas por clave. La clave se configura en cada `index.html` de herramienta buscando `var PASS=`.

## Clave actual

`matiz2026` — cámbiala en cada tool antes de publicar en producción.

## Despliegue

Conectado a Netlify vía GitHub. Cualquier push a `main` despliega automáticamente.

---

© 2026 MATIZ – Leadership & Thinking Lab · Todos los derechos reservados
