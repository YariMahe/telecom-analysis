# telecom-analysis

Este repositorio contiene el análisis realizado durante el Sprint 7 del caso de ConnectaTel donde se evaluó el comportamiento de los clientes de esta empresa de telecomunicaciones en Latinoamérica, a través de un proceso que incluía la exploración, limpieza y análisis de datos para construir un perfil estadístico de los clientes, detectar comportamientos atípicos y crear una segmentación de clientes basada en la edad y comportamiento. Todo este proceso permitió identificar patrones de consumo, diseñar estrategias de retención y sugerir mejoras en los distintos planes ofrecidos por la empresa. Los datos analizados abarcaron desde el año 2022 hasta el 2024 y se encontraron en 3 datasets: el primero llamado "plans" donde había datos relevantes de los planes que ofrece a compañía, su precio, minutos incluidos, GB incluidos, costo extra, etc.; el segundo nombrado "users" que incluía información de los clientes como su nombre, edad, ciudad, fecha de registro, plan y fecha de dada de baja (churn); así como "usage" donde se presentó registros sobre el uso real de los servicios como el número de llamadas y mensajes realizados por cliente, el número de minutos por llamada y demás.


## 📂 Contenido del repositorio

`S7 Version-Estudiante-Project-ConnectaTel.ipynb`
  → Notebook principal con limpieza, análisis exploratorio de datos, distribuciones, outliers y conclusiones.


## 📝 Etapas del análisis 
  1. Cargar y explorar los datasets: plans, users_latam y usage.
  2. Identificar problemas en la calidad de los datos: revisar nulos, inválidos y sentineles.
  3. Revisar y estandarizar fechas: dar formato a tipo fecha e identificar años fuera de rango.
  4. Corregir sentinels y fechas imposibles: reemplazar, en este caso, la edad con la mediana y catalogar sentinels como NA, así como las fechas fuera de rango.
  5. Decidir que hacer con los valores nulos: según la proporción y relevancia elegir que hacer con estos datos y justificar la decisión.
  6. Agrupar por comportamiento de uso: crear tabla del comportamiento de usuarios con número total de mensajes y llamadas, así como minutos por llamada.
  7. Crear resumen estadístico por usuario para el 2024: analizar columnas numéricas y categóricas para identificar rangos, valores extremos y distribución de los datos.
  8. Visualizar distribuciones: crear histogramas para observar las variables "uso" y "clientes", observar si existen diferencias entre el tipo de plan y analizar la forma de distribución.
  9. Identificar outliers: elaborar boxplots para detectar valores entremos en "uso" y "clientes" y decidir si quieren limpieza o revisión adicional.
  10. Segmentación de clientes: clasificar a cada usuario de acuerdo a su uso de llamadas y mensajes en bajo, medio o alto uso; así como clasificarlos de acuerdo a su edad, joven si es menor de 30 años, adulto si es menor que 60 años y adulto mayor para el resto de las edades.
  11. Visualizar segmentación de clientes: crear gráficos de barras que permitan ver la clasificación de "uso" y "edad" anteriores.
  12. Crear insights para stakeholders: traducir los hallasgos del análisis en conclusiones accionables para el negocio enfocadas en segmentación, patrones de uso y oportunidades comerciales. 


## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](S7 Version-Estudiante-Project-ConnectaTel.ipynb)

O:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**


## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S7 Version-Estudiante-Project-ConnectaTel.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos
- Analizar comportamientos, distribuciones y outliers
- Presentar a través de gráficos la información más relevante
- Generar insights para los stakeholders

