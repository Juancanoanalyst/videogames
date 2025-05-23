# 🎮 Análisis de Ventas de Videojuegos para la Tienda Ice

## 📌 Descripción del Proyecto

Contexto:
Ice es una tienda online que vende videojuegos a nivel mundial. La empresa busca comprender qué factores influyen en el éxito de un videojuego, con el fin de optimizar sus campañas publicitarias y estrategias de ventas.

Objetivo del análisis:
Identificar patrones en los datos históricos de videojuegos —incluyendo reseñas de usuarios y críticos, géneros, plataformas y ventas por región— que permitan predecir si un videojuego será exitoso.

## 🧠 Objetivo

- Analizar los datos de ventas y reseñas.
- Determinar qué plataformas y géneros son más rentables.
- Evaluar el impacto de las reseñas y calificaciones ESRB en las ventas.
- Formular y comprobar hipótesis estadísticas.

---

## 📁 Dataset

- Fuente: `/datasets/games.csv`
- Columnas principales:
  - `name`: Nombre del videojuego
  - `platform`: Plataforma (Xbox, PS, etc.)
  - `year_of_release`: Año de lanzamiento
  - `genre`: Género
  - `na_sales`, `eu_sales`, `jp_sales`, `other_sales`: Ventas por región (en millones USD)
  - `critic_score`: Calificación de críticos (0-100)
  - `user_score`: Calificación de usuarios (0-10)
  - `rating`: Clasificación ESRB

---

## 🧹 Preparación de los Datos

- Conversión de tipos de datos (por ejemplo, fechas y calificaciones).
- Limpieza de valores nulos y valores "TBD".
- Cálculo de ventas totales por consola (`total_sales`).

📊 Resultado:


<p align="center">
  <img src="imagenes_proyecto/imagen_1.png" alt="Distribución por Año" width="75%" >
</p>


---

## 📊 Análisis Exploratorio

### Juegos por Año
Se visualiza la cantidad de juegos publicados por año para determinar qué periodos son significativos.


<p align="center">
  <img src="imagenes_proyecto/imagen_2.png" alt="Juegos por Año" width="75%" >
</p>


### Plataformas más Populares
Identificamos las plataformas con mayores ventas totales, observando su ciclo de vida.


<p align="center">
  <img src="imagenes_proyecto/imagen_3.png" alt="Top Plataformas" width="47%" />
  <img src="imagenes_proyecto/imagen_4.png" alt="Ventas por Plataforma en el Tiempo" width="45%" />
</p>


### Diagrama de Caja de Ventas Globales


<p align="center">
  <img src="imagenes_proyecto/imagen_5.png" alt="Boxplot por Plataforma" width="75%" >
</p>


---

## 💬 Análisis de Reseñas

Se explora la correlación entre calificaciones de usuarios y críticos vs. ventas, usando como ejemplo **PS4**.


<p align="center">
  <img src="imagenes_proyecto/imagen_6.png" alt="Correlación PS4 User" width="45%" />
  <img src="imagenes_proyecto/imagen_7.png" alt="Correlación PS4 Críticos" width="46%" />
</p>

---

## 🎯 Análisis por Región

### América del Norte, Europa y Japón
---
- Top 5 plataformas y géneros.


<p align="center">
  <img src="imagenes_proyecto/imagen_8.png" alt="Top Plataformas NA" width="30%" />
  <img src="imagenes_proyecto/imagen_9.png" alt="Top Plataformas EU" width="30%" />
  <img src="imagenes_proyecto/imagen_10.png" alt="Top Plataformas JP" width="30%" />
</p>



---
- Preferencias por región.



<p align="center">
  <img src="imagenes_proyecto/imagen_gna.png" alt="Géneros por Región NA" width="30%" />
  <img src="imagenes_proyecto/imagen_geu.png" alt="Géneros por Región EU" width="30%" />
  <img src="imagenes_proyecto/imagen_gjp.png" alt="Géneros por Región JP" width="30%" />
</p>



---
- Influencia del ESRB.


<p align="center">
  <img src="imagenes_proyecto/imagen_pna.png" alt="Impacto del ESRB NA" width="30%" />
  <img src="imagenes_proyecto/imagen_peu.png" alt="Impacto del ESRB EU" width="30%" />
  <img src="imagenes_proyecto/imagen_pjp.png" alt="Impacto del ESRB JP" width="30%" />
</p>




## 🧪 Pruebas de Hipótesis

Se probaron las siguientes hipótesis:

1. Las calificaciones promedio de usuarios para Xbox One y PC son diferentes.
2. Las calificaciones promedio de usuarios para los géneros Acción y Deportes son iguales.

Método: Prueba t de Student con un nivel de significancia `α = 0.05`.

<p align="center">
  <img src="imagenes_proyecto/imagen_13.png" alt="Prueba Xbox-PC" width="45%" />
  <img src="imagenes_proyecto/imagen_14.png" alt="Prueba Acción-Deportes" width="45%" />
</p>

---

## 🛠 Tecnologías Usadas

- Python (Pandas, Matplotlib, Seaborn, SciPy)
- Jupyter Notebook
- Git y GitHub
- Estadística inferencial (prueba de hipótesis)

---


## 📌 Conclusiones

- El informe recomienda mantener un buen stock de juegos de PS4 y Xbox One por su tendencia actual y vida útil estimada. Se sugiere monitorear las tendencias de plataformas cada década, aprender de la pérdida de liderazgo de Nintendo en los 2000.

- También destaca la importancia de la crítica de expertos, el marketing con influencers y la atención a los juegos en  Esports. Franquicias como Call of Duty y GTA siguen siendo relevantes, al igual que el género shooter gracias al juego online.

- El análisis regional revela preferencias similares entre Europa y Norteamérica por acción y deportes (con Xbox más fuerte en NA y PlayStation en Europa), mientras que Japón prefiere juegos de Nintendo y RPGs.

- Finalmente, el informe enfatiza la necesidad de completar la información sobre el público objetivo de los juegos para mejorar la precisión del análisis.

---





