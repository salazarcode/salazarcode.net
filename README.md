# SalazarCode.net - Landing Page & Catálogo de Proyectos

Sitio web personal y portal de proyectos de **SalazarCode** ([https://salazarcode.net](https://salazarcode.net)). Presenta los servicios en producción, estado de la infraestructura y fichas técnicas detalladas de cada solución.

## Proyectos Destacados

- **[Legal RAG Venezuela](https://legal.salazarcode.net):** Asistente conversacional de inteligencia artificial y recuperación semántica de alta precisión especializado en la legislación venezolana (.NET 8, PostgreSQL 16 + pgvector HNSW, Ollama y Angular 18). [Ficha técnica](legal-rag.html) • [Repositorio](https://github.com/salazarcode/legal-rag-venezuela).
- **[Mapa Interactivo de Venezuela](https://mapa.salazarcode.net):** Cartografía vectorial SVG interactiva con navegación jerárquica multinivel de 4 niveles (País ➔ Estados ➔ Municipios ➔ Parroquias) construida con D3.js y GeoJSON estandarizado (OCHA / ONU). [Ficha técnica](mapa-venezuela.html) • [Repositorio](https://github.com/salazarcode/mapa-venezuela).

## Estructura del Sitio

```
├── index.html               # Portada principal y showcase de proyectos
├── legal-rag.html           # Exposición técnica completa del motor RAG
├── mapa-venezuela.html      # Exposición técnica del visualizador geoespacial
├── css/
│   └── style.css            # Estilos modernos con tema oscuro, glassmorphism y diseño responsivo
├── js/                      # Scripts auxiliares
├── docker/
│   └── conf/
│       └── default.conf     # Configuración de Nginx para servir estáticos con gzip y SPA routing
├── docker-compose.yml       # Orquestación con Nginx Alpine
└── README.md
```

## Despliegue Local con Docker

```bash
docker compose up -d
```

El sitio estará disponible en `http://localhost:8080`.
