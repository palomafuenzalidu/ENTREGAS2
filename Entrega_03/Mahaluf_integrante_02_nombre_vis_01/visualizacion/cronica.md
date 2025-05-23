# De los datos al relato: el largo camino hacia la visualización de los Oscar

Cada año, los Premios Oscar capturan la atención del mundo con su desfile de celebridades, discursos emotivos y películas memorables. Pero detrás del espectáculo existe una maquinaria de decisiones, nominaciones y premios que, vista con lupa, puede revelar patrones mucho más profundos que el brillo de una estatuilla dorada. 

Este fue el punto de partida para esta visualización, cuyo objetivo fue explorar los datos de los Oscar desde 1997 hasta 2025 para entender, más allá de la narrativa oficial, cómo se han comportado las nominaciones a lo largo del tiempo. A través del análisis de una base limpia —con información detallada sobre cada nominación, categoría, año y resultados— busqué construir una visualización clara y efectiva que permitiera comunicar una pequeña historia dentro del universo de los datos.

## ¿Por qué esta historia?

Al revisar la base de datos, surgieron muchas posibilidades. ¿Cuál ha sido la evolución de ciertos estudios de cine? ¿Qué tan constantes son los actores o actrices más nominados? ¿Existen categorías dominadas por ciertos géneros o temáticas? Sin embargo, la que decidí abordar fue una más transversal: observar cómo han cambiado las nominaciones a lo largo del tiempo y detectar tendencias generales, a través de una visualización temporal.

Este enfoque me permitía construir una historia comprensible, visualmente atractiva y, al mismo tiempo, significativa para el espectador. La pregunta que guiaba el proceso fue: **¿qué nos dice la evolución de las nominaciones sobre las dinámicas de la industria cinematográfica en estos últimos 30 años?**

## El proceso detrás de la visualización

El primer paso fue seleccionar las variables clave: año, categoría, título, resultado (ganador o no), y el tipo de participación (persona o película). Luego de explorar los datos, realicé un proceso de limpieza adicional en Google Colab para asegurar que las columnas estuvieran estandarizadas, los años correctos y las categorías bien definidas.

Una vez lista la base, utilicé la librería Altair de Python para generar la visualización. Altair permite crear gráficos declarativos, lo que facilita construir visualizaciones limpias y fácilmente modificables. Me decidí por un gráfico de barras agrupadas por año y categoría, que muestra la cantidad de nominaciones en distintas categorías, permitiendo comparar rápidamente las más competitivas y cómo han variado.

El mayor desafío fue lograr un diseño legible pese a la gran cantidad de categorías y años. Para solucionarlo, utilicé filtros interactivos que permiten explorar los datos por partes, y exporté tanto una versión completa en HTML como una imagen en JPG que resume los principales hallazgos.

## ¿Qué revela esta visualización?

A simple vista, el gráfico permite identificar años con mayor o menor cantidad de nominaciones, categorías con mayor recurrencia y otras más inusuales, así como ciertos hitos: por ejemplo, los años con más cambios en categorías (como la inclusión de nuevas áreas técnicas) o una alta concentración de películas en determinadas categorías.

Esta visualización es una pieza más del proyecto mayor, pero busca cumplir un rol claro: **acercar los datos al público desde una mirada accesible, visual y con narrativa.** Así, se convierte en una herramienta no solo informativa, sino también reflexiva, que nos ayuda a entender cómo funciona uno de los eventos más importantes de la industria cultural contemporánea.

---

*Crónica realizada como complemento a la visualización desarrollada con la base de datos `oscars_limpio_1997_2025.csv`, empleando Python y la librería Altair.*
