## Documentación
El primer paso para lograr la visualización de datos presentada fue la carga del dataset a Google Collab. En este caso utilicé la base de datos previamente limpiada **oscars_limpio_1997_2025-4.csv**, la cual contiene información de las nominaciones y ganadores de los premios Oscar desde 1997, el año que se inventó Netflix, hasta la ultima edición que fue este año. La base de datos muestra el o los distribuidores de cada película, las categorías y si es que la película ganó o no. Las variables principales son **Winner** (si es que ganó o solo fue nominado), los distribuidores y el año.

Para lograr identificar si una película fue distribuida por una plataforma de Streaming o no le pedí a Google Collab que buscara las palabras clave 'netflix', 'amazon', 'prime video', 'apple', 'hulu', 'disney+', las plataformas de streaming que han distribuido películas nominadas a los premios Oscar. A partir de esto se añadió una nueva columna booleana **is_streaming**, para diferenciar entre ambas categorías.

Luego agrupé los datos por año y según la columna **is_streaming**, calculando según dos métricas:
count: cantidad total de nominaciones.
sum: cantidad de premios ganados (donde winner == 1).
Para facilitar y simplificar la visualización cambie el formato a un *long format*, por lo que se separaron todas las filas según las métricas,(nominations o wins).

Para el formato busque un color rojo para representar streaming y azul para las distribuidoras tradicionales. Para el resto del formato no estaba muy sgeura como hacerlo asi que le pedi a ChatGPT que me diera una instrucción: mark_line(point=alt.OverlayMarkDef(filled=True, size=60))
x=alt.X('Year:O', title='Año')
y=alt.Y('Count:Q', title='Cantidad', axis=alt.Axis(labelFontSize=12, titleFontSize=14)), además me ayudó a ponerle un título y un subtítulo personalizados.

## Base de datos (CSV)
La base de datos que utilicé fue la que limpie a partir de los datos que adjuntaron las profesoras a partir de la página Kaggle y IMBd.
Para dejarla lista deje todas las ediciones de los premios desde 1997 hasta 2025, con todas las nominaciones, si habían ganado o no, sus productoras y las distribuidoras. Como dicho anteriormente, al hacer la visualización se tomaron en cuenta las plataformas de streaming como palabras claves para así lograr encontrar los resultados de manera más fácil.

## Preguntas
La visualización logra responder la pregunta que responde nuestra hipótesis: "las películas distribuidas por plataformas de streaming están superando, cada vez más, al resto de la industria cinematográfica, en la temporada de premios", en este caso en los premios Oscar desde 1997 a 2025. A través del tiempo las películas distribuidas por plataformas de streaming han visto un aumento exponencial en la cantidad de nominaciones y un aumento lineal en la cantidad de permios obtenidos. Por otro lado, las distribuidoras tradicionales han visto una baja drástica en sus nominaciones en los últimos 10 años y una baja más lineal en los premios obtenidos.

Otras preguntas que pueden ser respondidas son:
+ ¿En qué años las plataformas de streaming alcanzaron su punto más alto de reconocimiento?
+ ¿Existen diferencias claras entre el crecimiento de nominaciones y el de premios ganados por el streaming?
+ ¿Cómo se compara el rendimiento de las películas de streaming con el de los estudios tradicionales en términos de premios ganados?