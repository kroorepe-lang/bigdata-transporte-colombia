# Proyecto Big Data – Transporte de Carga (Camiones de Tres Ejes)

##  Planteamiento del problema
El transporte de carga terrestre en Colombia es un eje estratégico para la competitividad nacional. En particular, los camiones de tres ejes cumplen un papel esencial en el movimiento de mercancías en las principales rutas del país.  

El RNDC (Registro Nacional de Despacho de Carga)** centraliza la información de los despachos, pero los datos se presentan en formatos extensos y poco amigables para el análisis directo. Esto genera retos como:  
- La identificación rápida de tendencias históricas de tarifas.  
- El seguimiento específico de rutas y tipos de vehículos.  
- La transformación de datos crudos en información útil para la toma de decisiones.  

Por ello, se plantea el desarrollo de una solución basada en Big Data, que permita:  
- Procesar los datos del RNDC en capas (bronze, silver, gold).  
- Filtrar y analizar las 10 rutas más transitadas del país para camiones de tres ejes.  
- Generar visualizaciones en Power BI que faciliten el análisis de tarifas históricas y comparaciones entre rutas.  



## Justificación
El transporte de carga terrestre es un componente vital para la economía colombiana, y los camiones de tres ejes representan una parte significativa del flujo de mercancías en las principales rutas del país.  
Aunque el RNDC centraliza la información de los despachos, esta se encuentra en formatos masivos que requieren procesamiento y organización para transformarse en conocimiento útil.  

La aplicación de técnicas de Big Data permite superar estas limitaciones, ofreciendo un sistema capaz de:  
- Procesar grandes volúmenes de datos de manera eficiente.  
- Filtrar información relevante para las 10 rutas más transitadas del país.  
- Proporcionar indicadores claros y visualizaciones interactivas que apoyen la toma de decisiones estratégicas en el sector transporte.  

Este proyecto no solo tiene un valor académico, sino también práctico, ya que responde a necesidades reales del sector en el que trabajamos, aportando herramientas modernas para mejorar la competitividad y la planificación logística.  



## Objetivos
- General: 
  Desarrollar un sistema de análisis de datos de transporte de carga en Colombia, enfocado en camiones de tres ejes y en las 10 rutas más transitadas, utilizando Databricks y Power BI.  

- Específicos:
  - Ingestar datos del RNDC mediante descargas abiertas o scraping.  
  - Organizar la información en capas de almacenamiento (*bronze*, *silver*, *gold*).  
  - Automatizar el flujo de procesamiento con **Jobs** en Databricks.  
  - Generar visualizaciones interactivas en Power BI para analizar tarifas históricas en las rutas seleccionadas.  



## ⚙️ Metodología
1. Ingesta (Bronze):
   - Recolección de datos del RNDC y fuentes oficiales.  
   - Almacenamiento en formato crudo.  

2. Transformación (Silver): 
   - Limpieza de columnas, normalización de tipos de datos.  
   - Filtrado exclusivo de camiones de tres ejes y selección de las 10 rutas más transitadas.  

3. Visualización (Gold/Power BI): 
   - Conexión de Power BI a Databricks.  
   - Creación de dashboards con KPIs: evolución de tarifas, comparación de rutas, costos promedio.  



## Herramientas
- **Databricks:** Plataforma de procesamiento y análisis de Big Data.  
- Power BI: Visualización interactiva de resultados.  
- GitHub: Control de versiones y documentación del proyecto.

- ##  Flujo del Proyecto

RNDC (Datos crudos) 
        │
        ▼
   [Bronze Layer]
   - Ingesta de datos
   - Almacenamiento inicial
        │
        ▼
   [Silver Layer]
   - Limpieza de columnas
   - Filtrado de camiones de 3 ejes
   - Selección de 10 rutas más transitadas
        │
        ▼
   [Gold Layer]
   - Dataset listo para análisis
        │
        ▼
   Power BI (Visualización)
   - Dashboards interactivos
   - KPIs de tarifas históricas
   - Comparación de rutas
