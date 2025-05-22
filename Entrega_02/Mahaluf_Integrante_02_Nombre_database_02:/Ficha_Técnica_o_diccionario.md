# 📄 Ficha Técnica: Base de Datos sobre Nominaciones a los Premios Emmy (2020–2024)

## 1. Fuente de los datos
La información fue recopilada manualmente desde diversas fuentes periodísticas confiables, incluyendo:

- Vogue México (categorías completas de nominaciones Emmy 2020, 2021, 2022)
- Artículos actualizados sobre los Emmy 2023 y 2024 de sitios como *Variety*, *The Hollywood Reporter*, *Emmys.com* y otras revistas de entretenimiento.

## 2. Metodología de la construcción de la base
- Se levantaron todas las nominaciones en las principales categorías de los Emmy desde 2020 hasta 2024.
- Se identificaron el nombre del programa, persona nominada (si aplica) y la plataforma de emisión principal.
- A cada entrada se le asignó una etiqueta binaria para indicar si corresponde a una producción de plataforma de streaming (`✅ Sí` / `❌ No`).
- En casos de emisión mixta (TV tradicional + streaming), se consideró TV tradicional si la emisión principal fue por televisión abierta o cable.
- La codificación fue manual, contrastando la información con fuentes oficiales y bases de datos como IMDb.

## 3. Alcance de los datos
- **Años considerados**: 2020, 2021, 2022, 2023, 2024.
- **Categorías**: Todas las categorías principales de los Emmy (actuación, dirección, guion, programas, variedades, realities, talk shows).
- **Unidad de análisis**: Cada nominación individual.
- Solo se consideraron nominaciones oficiales confirmadas por fuentes confiables.

## 4. Características de los datos
- Datos categóricos y nominales.
- Estructura de tabla plana con una fila por nominación.
- Información orientada a analizar la participación de plataformas de streaming en los Emmy.

## 5. Variables incorporadas

| Variable                  | Descripción                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| Año                       | Año de la premiación                                                        |
| Categoría                | Nombre de la categoría (ej: Mejor actriz en serie dramática)               |
| Nombrado/a                | Nombre de la persona nominada (si aplica)                                   |
| Título del programa       | Serie, película, documental o show nominado                                 |
| Plataforma principal      | Plataforma de emisión original (Netflix, HBO, Prime Video, etc.)            |
| ¿Es de streaming?         | Variable binaria que indica si es original de una plataforma de streaming (`✅` o `❌`) |

## 6. Otras observaciones
- En casos de coproducción o emisión múltiple, se priorizó la plataforma de estreno original.
- La categoría "streaming" se refiere exclusivamente a plataformas digitales nativas: Netflix, Prime Video, Hulu, Disney+, Apple TV+, etc.
- No se consideran como "streaming" los servicios on demand de canales tradicionales (ej: HBO Max cuando acompaña un estreno de HBO lineal).
- La disponibilidad de contenidos puede variar por región, pero se utilizó como referencia su estreno en EE. UU.

