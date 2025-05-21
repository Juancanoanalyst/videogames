# 🎮 Análisis de Ventas de Videojuegos para la Tienda Ice

## 📌 Descripción del Proyecto

Trabajas como analista de datos para **Ice**, una tienda online que vende videojuegos en todo el mundo. Contamos con datos históricos hasta 2016, incluyendo reseñas de usuarios y críticos, géneros, plataformas y ventas por región. El objetivo es **identificar patrones que determinen si un videojuego será exitoso**, para así planificar campañas publicitarias efectivas para el año siguiente (2017).

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

![Distribución por Año](imagenes_proyecto/imagen_1.png)

---

## 📊 Análisis Exploratorio

### Juegos por Año
Se visualiza la cantidad de juegos publicados por año para determinar qué periodos son significativos.

![Juegos por Año](imagenes_proyecto/imagen_2.png)

### Plataformas más Populares
Identificamos las plataformas con mayores ventas totales, observando su ciclo de vida.


<p align="center">
  <img src="imagenes_proyecto/imagen_3/.png" alt="Top Plataformas" width="45%" />
  <img src="imagenes_proyecto/imagen_4.png" alt="Ventas por Plataforma en el Tiempo" width="45%" />
</p>


### Diagrama de Caja de Ventas Globales

![Boxplot por Plataforma](imagenes_proyecto/imagen_5.png)

---

## 💬 Análisis de Reseñas

Se explora la correlación entre calificaciones de usuarios y críticos vs. ventas, usando como ejemplo **PS4**.


<p align="center">
  <img src="imagenes_proyecto/imagen_6/.png" alt="Correlación PS4 User" width="45%" />
  <img src="imagenes_proyecto/imagen_7.png" alt="Correlación PS4 Críticos" width="45%" />
</p>

---

## 🎯 Análisis por Región

### América del Norte, Europa y Japón
---
- Top 5 plataformas y géneros.


![Top Plataformas NA](imagenes_proyecto/imagen_8.png)  
![Top Plataformas EU](imagenes_proyecto/imagen_9.png)  
![Top Plataformas JP](imagenes_proyecto/imagen_10.png)  
---
- Preferencias por región.

![Géneros por Región NA](imagenes_proyecto/imagen_gna.png)
![Géneros por Región EU](imagenes_proyecto/imagen_geu.png)
![Géneros por Región JP](imagenes_proyecto/imagen_gjp.png)

---
- Influencia del ESRB.

![Impacto del ESRB NA](imagenes_proyecto/imagen_pna.png)
![Impacto del ESRB EU](imagenes_proyecto/imagen_peu.png)
![Impacto del ESRB JP](imagenes_proyecto/imagen_pjp.png)


## 🧪 Pruebas de Hipótesis

Se probaron las siguientes hipótesis:

1. Las calificaciones promedio de usuarios para Xbox One y PC son diferentes.
2. Las calificaciones promedio de usuarios para los géneros Acción y Deportes son iguales.

Método: Prueba t de Student con un nivel de significancia `α = 0.05`.

![Prueba Xbox-PC](imagenes_proyecto/imagen_13.png)  
![Prueba Acción-Deportes](imagenes_proyecto/imagen_14.png)

---

## 📌 Conclusiones

- El informe recomienda mantener un buen stock de juegos de PS4 y Xbox One por su tendencia actual y vida útil estimada. Se sugiere monitorear las tendencias de plataformas cada década, aprender de la pérdida de liderazgo de Nintendo en los 2000.

- También destaca la importancia de la crítica de expertos, el marketing con influencers y la atención a los juegos en  Esports. Franquicias como Call of Duty y GTA siguen siendo relevantes, al igual que el género shooter gracias al juego online.

- El análisis regional revela preferencias similares entre Europa y Norteamérica por acción y deportes (con Xbox más fuerte en NA y PlayStation en Europa), mientras que Japón prefiere juegos de Nintendo y RPGs.

- Finalmente, el informe enfatiza la necesidad de completar la información sobre el público objetivo de los juegos para mejorar la precisión del análisis.

---

## 🛠 Tecnologías Usadas

- Python (Pandas, Matplotlib, Seaborn, SciPy)
- Jupyter Notebook
- Git y GitHub
- Estadística inferencial (prueba de hipótesis)



