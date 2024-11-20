# Análisis de Redes Complejas en Colaboraciones Musicales

## Objetivo del Proyecto

Este proyecto analiza las colaboraciones entre artistas musicales utilizando técnicas de redes complejas. A través de esta investigación, buscamos comprender mejor las dinámicas de colaboración en la industria musical y responder preguntas relacionadas con la clasificación y predicción dentro de estas redes.

## Alumnos Participantes

| Nombre                          |
|---------------------------------|
| Sebastián Aaron Guevara Domínguez |
| Salvador Díaz Aguirre           |
| Marcelo Guerrero Iparraguirre  |

---

## Descripción del Dataset

El dataset utilizado proviene de la publicación **"Spotify Artist Feature Collaboration Network"** en Kaggle, con información extraída del API de Spotify y kworb.net. Incluye:

### Nodos
Representan artistas con las siguientes variables:

| Variable       | Descripción                                 |
|----------------|---------------------------------------------|
| `spotify_id`   | ID del artista en Spotify.                 |
| `name`         | Nombre del artista.                        |
| `followers`    | Número de seguidores.                      |
| `popularity`   | Nivel de popularidad.                      |
| `genres`       | Géneros musicales asociados.               |
| `chart_hits`   | Lista de éxitos en diferentes países.       |

### Aristas
Representan colaboraciones entre artistas con las siguientes variables:

| Variable       | Descripción                                 |
|----------------|---------------------------------------------|
| `id_0`         | ID del primer artista.                     |
| `id_1`         | ID del segundo artista.                    |

### Estadísticas del Dataset

| Métrica                | Valor       |
|------------------------|-------------|
| Número de artistas     | 156,422     |
| Número de colaboraciones | 300,386   |

---

## Preguntas de Investigación

1. ¿Es posible predecir el éxito de una colaboración entre dos artistas basándose en sus características individuales y su posición en la red de colaboraciones?
2. ¿Cómo se pueden clasificar los artistas en comunidades basadas en patrones de colaboración y qué información aporta esto sobre la estructura de la industria musical?
3. ¿Qué relación existe entre el número de seguidores y la popularidad de los artistas en sus colaboraciones?

---

## Técnicas Utilizadas

### 1. Detección de comunidades
- **Algoritmos implementados**: Louvain, Leiden y Label Propagation.
- Se extrajo la componente conexa más grande de la red para simplificar el análisis.

### 2. Predicción de enlaces
- **Métodos usados**: Vecinos Comunes, Índice de Jaccard y Adamic-Adar.
- Se evaluaron probabilidades de futuras colaboraciones basadas en datos históricos.

### 3. Visualización y análisis
- Representación gráfica de comunidades y colaboraciones utilizando bibliotecas como **NetworkX** y **matplotlib**.

---

## Conclusiones

### 1. Identificación de comunidades musicales
- Los algoritmos segmentaron la red en grupos de artistas que reflejan géneros o escenas musicales.

### 2. Predicción de colaboraciones futuras
- Se identificaron artistas con alta probabilidad de colaborar, lo cual puede ser útil para estrategias de marketing y planificación musical.

### 3. Impacto de las métricas de popularidad y seguidores
- Estas métricas juegan un papel importante en la visibilidad y éxito de las colaboraciones.

### 4. Limitaciones
- Se identificó la necesidad de incluir datos adicionales como temporalidad de colaboraciones e ingresos por asociaciones.

### 5. Impacto práctico
- Este análisis ofrece herramientas útiles para la industria musical y puede extenderse a otras áreas colaborativas.

### 6. Futuras investigaciones
- Incluir modelos avanzados como redes neuronales gráficas y análisis temporales.
