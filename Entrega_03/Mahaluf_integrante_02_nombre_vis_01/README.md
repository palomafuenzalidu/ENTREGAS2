# README - Visualización Personal

## 1. Proceso de visualización

La visualización fue creada utilizando la librería **Altair** en Python, en un entorno Jupyter Notebook (Google Colab). A continuación, se detallan los pasos seguidos:

1. **Carga de datos**: Se utilizó la base de datos `oscars_limpio_1997_2025-F(in).csv`, que contiene información sobre nominaciones y premios en los Oscars desde 1997 hasta 2025.
2. **Exploración inicial**: Se revisaron las variables disponibles, como `Año`, `Categoría`, `Película`, `Ganador`, `País`, `Streaming`, entre otras.
3. **Limpieza y transformación**:
   - Se eliminaron filas con datos faltantes en campos clave.
   - Se agruparon las nominaciones por plataforma (`Streaming`) y año.
   - Se generaron nuevas variables para contar nominaciones y premios obtenidos.
4. **Visualización**:
   - Se diseñó un gráfico de barras agrupadas usando Altair para mostrar cuántas nominaciones tuvo cada plataforma por año.
   - Se exportó como `.html` (interactiva) y `.jpg` (imagen estática).
5. **Complemento narrativo**: Se redactó una crónica periodística que interpreta los datos visualizados, contextualizándolos con la transformación de la industria del cine y el streaming.

## 2. Base de datos utilizada

**Nombre:** `oscars_limpio_1997_2025-F(in).csv`  
**Fuente:** Elaboración propia a partir de datos públicos de los premios Oscars.  
**Período:** 1997 a 2025

### Procesamiento

- Se normalizó el nombre de las plataformas (`Netflix`, `Amazon Prime`, etc.).
- Se separaron las categorías principales (Mejor Película, Dirección, Actuación) de las técnicas.
- Se añadió una variable binaria para identificar si una plataforma ganó o solo fue nominada.

### Justificación

Esta base fue escogida porque permite estudiar cómo las plataformas de streaming han cambiado la dinámica de los Oscars en los últimos 25 años. Es relevante para analizar la consolidación de servicios como Netflix, Amazon o Apple TV+ como productores de contenido premiado.

## 3. Preguntas que responde la visualización

- ¿Qué plataformas de streaming han sido más nominadas en los Oscars desde 2015?
- ¿Ha aumentado la presencia de las plataformas digitales respecto al cine tradicional?
- ¿Qué plataforma ha ganado más premios en los últimos años?
- ¿Cuáles son los años en que más plataformas compitieron entre sí?

---

Este archivo se complementa con:
- La crónica periodística (`visualizacion/cronica.md`).
- La visualización interactiva (`visualizacion/vis_01.html`).
- La versión imagen de la visualización (`visualizacion/vis_01.jpg`).
- El script del proceso (`scripts/codigo_para_visualizar_1.ipynb`).
- La ficha técnica de la base (`Ficha_Técnica.md`).
