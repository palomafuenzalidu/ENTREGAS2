El proceso comenzó con la recolección de datos desde diversas fuentes confiables como Vogue México y artículos especializados en medios estadounidenses. Estos datos estaban disponibles en formato HTML y fueron copiados manualmente para construir una base de datos con las nominaciones a los premios Emmy desde 2020 a 2024.

A continuación, se utilizaron herramientas como Excel y Google Sheets para estructurar y limpiar los datos. Los pasos fueron los siguientes:

1. Copiar y pegar la información desde los sitios web fuente.
2. Eliminar celdas vacías o categorías repetidas.
3. Normalizar nombres de plataformas (por ejemplo, “HBO Max” y “HBO” se unificaron como “HBO”).
4. Dividir categorías múltiples en columnas separadas si una celda contenía más de una nominación.
5. Validar que no existieran filas duplicadas.
6. Crear nuevas columnas como “Año”, “Plataforma”, “Categoría” y “Programa” para estandarizar la base.

La limpieza final se guardó en un archivo CSV, que puede ser usado para análisis en Python o Google Colab.

- Vogue México: https://www.vogue.mx/alfombra-roja/articulo/emmys-2022-la-lista-completa-de-nominados
- Vogue México: https://www.vogue.mx/estilo-de-vida/articulo/premios-emmy-2021-nominados
- Vogue México: https://www.vogue.mx/alfombra-roja/articulo/emmy-2020-nominados-ganadores-fecha-y-donde-verlo-en-vivo

Estas fuentes fueron elegidas por ser confiables, completas, y por publicar la lista completa de nominaciones organizadas por año y categoría.

1. ¿Qué plataforma de streaming obtuvo más nominaciones entre 2020 y 2024?
2. ¿En qué categorías ha sido más fuerte Netflix en comparación con HBO?
3. ¿Qué actores o actrices han sido más nominados/as durante estos cinco años?
