# Análisis de visualizaciones

Este documento analiza cada una de las visualizaciones integradas en el reportaje **"El streaming en los premios Oscar"**, enfocándose en su mensaje, propósito informativo y vínculo con la narrativa general del proyecto.

---

## 1. Línea de tiempo: Hitos del streaming en los premios Oscar

### Descripción:
Una visualización cronológica que presenta los principales hitos de las plataformas de streaming desde 1997 hasta 2025.

### ¿Qué comunica?
Muestra la evolución del rol de las plataformas en la industria cinematográfica, destacando eventos como:
- Fundación de Netflix (1997)
- Primera nominación al Oscar (2014)
- Primer Oscar ganado (2017)
- Consolidación de Apple TV+ y Disney+

### Objetivo narrativo:
Funciona como introducción visual para contextualizar al usuario en el fenómeno. Reemplaza párrafos largos por puntos clave interactivos y refuerza la dimensión histórica del cambio.

---

## 2. Beeswarm chart: Nominaciones de plataformas de streaming

### Descripción:
Gráfico tipo "beeswarm" que muestra la distribución de nominaciones por año y plataforma.

### ¿Qué comunica?
Permite ver:
- En qué años aparecen ciertas plataformas
- La intensidad de participación por año
- La consolidación y crecimiento de ciertas marcas como Netflix, Amazon y Apple

### Objetivo narrativo:
Demuestra visualmente cómo el streaming pasa de ser una excepción a una constante en los Oscar. Aporta evidencia empírica que apoya la hipótesis del reportaje.

---

## 3. Comparación general por distribuidora

### Descripción:
Gráfico de barras que compara el número total de nominaciones y premios ganados por diferentes distribuidoras (tanto plataformas como estudios tradicionales).

### ¿Qué comunica?
- Netflix, Amazon y Apple tienen volúmenes comparables a estudios clásicos como Warner o Fox.
- El color dorado distingue premios ganados, mientras que el burdeos señala solo nominaciones.

### Objetivo narrativo:
Apoya la idea de que las plataformas digitales no solo participan, sino que también **compiten y ganan** en igualdad de condiciones con los grandes estudios.

---

## 4. Tabla interactiva de películas y nominaciones

### Descripción:
Tabla dinámica con filtros y paginación que permite explorar más de 20 años de datos sobre películas nominadas (nombre, distribuidora, categoría, año, etc.).

### ¿Qué comunica?
Permite al usuario hacer su propio análisis: buscar plataformas específicas, ver tendencias por década, observar cuántas películas de Netflix fueron nominadas a mejor documental, etc.

### Objetivo narrativo:
Aporta **transparencia y profundidad de información**. Refuerza la credibilidad del reportaje y abre posibilidades de análisis exploratorio.

---

## Datos y herramientas

- **Base de datos principal**: `oscars_distribuidoras_FINAL.csv`
- **Herramientas utilizadas**: Google Colab (Python, Pandas, Seaborn, Matplotlib, Altair), HTML+JS para integración web.
- **Librerías gráficas**: `Altair`, `Seaborn`, `Matplotlib`, `DataTables.js`

---

## Conclusión del análisis

Las visualizaciones no solo complementan el texto: **son el núcleo del argumento periodístico**. A través de una narrativa visual progresiva (línea de tiempo → tendencia histórica → comparación → exploración), se refuerza la hipótesis y se entrega al usuario una experiencia informativa y clara, fundamentada en datos y diseño.


