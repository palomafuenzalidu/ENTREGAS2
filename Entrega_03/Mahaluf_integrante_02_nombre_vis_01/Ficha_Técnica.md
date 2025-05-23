# Ficha Técnica - Base de Datos Oscar 1997-2025

## Nombre del archivo
`oscars_limpio_1997_2025-4(in).csv`

## Características generales
Base de datos con registros de películas nominadas a los Premios Oscar desde 1997 hasta 2025, incluyendo variables relevantes para análisis como nombre de la película, año, categoría, resultado (ganadora o no), y distribuidores asociados.

## Variables incluidas

| Variable          | Descripción                                                          |
|-------------------|----------------------------------------------------------------------|
| Year              | Año de la ceremonia de los Premios Oscar                             |
| Category          | Categoría en la que fue nominada la película                         |
| Nominee           | Persona, grupo o entidad nominada (puede ser actor, director, etc.)  |
| Film              | Título de la película nominada                                       |
| Winner            | 1 si ganó la categoría, 0 si solo fue nominada                       |
| distribuidor_1    | Primer distribuidor registrado para la película                      |
| distribuidor_2    | Segundo distribuidor registrado (si aplica)                          |
| distribuidor_3    | Tercer distribuidor registrado (si aplica)                           |
| distribuidor_4    | Cuarto distribuidor registrado (si aplica)                           |
| distribuidor_5    | Quinto distribuidor registrado (si aplica)                           |

## Observaciones

- Algunas películas tienen múltiples distribuidores.
- No todos los registros tienen 5 distribuidores; muchos tienen solo 1 o 2.
- Se agregó una columna nueva `is_streaming` durante el análisis para identificar si una película fue distribuida por una plataforma digital.
- Se recomienda normalizar los nombres de distribuidores para evitar inconsistencias ortográficas.
