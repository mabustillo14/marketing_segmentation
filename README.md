# Segmentación de Clientes para optimización de Campañas de Marketing

Una empresa de alimentos desea obtener el mayor beneficio posible para la próxima campaña de marketing directo, programada para el próximo mes.

El objetivo del proyecto es desarrollar un modelo que prediga el comportamiento de los clientes y aplicarlo al resto de la base de clientes. Además, más allá de maximizar el beneficio de la campaña, estudiar las características de los clientes dispuestos a comprar el gadget.

Se espera mejorar el ROI de la próxima campaña mediante un modelo predictivo que permita identificar clientes propensos a aceptar una oferta.

**Fuente:** [iFood](https://github.com/ifood/ifood-data-analyst-case)

## <br> Objetivo 🎯
El objetivo es analizar los datos históricos de las últimas 5 campañas de marketing, junto con el comportamiento de los clientes y su perfil, para:

* Identificar características clave de los clientes que aceptan la oferta.
* Optimizar las futuras campañas para mejorar la tasa de conversión y reducir los costos.
* Maximizar los ingresos y lograr una campaña rentable.

## <br> Tecnologías ⚙️
Este proyecto se ha desarrollado utilizando Python en un entorno de Jupyter Notebook.
* **Bibliotecas:** Pandas, NumPy, Scikit-learn
* **Herramientas de visualización:** Matplotlib, Seaborn
* **Exploración de Datos:** funpymodeling

### ¿Cómo usar el programa? 💻
0. Instala las librerías de funpymodeling y ProfileReport de Python.
```
# Instalar funpymodeling
!pip install -U ydata-profiling

# Instalar ProfileReport
!pip install funpymodeling
```
1. Agrega el path donde se encuentra guardado el archivo `data_campaign.csv` con los datos
```
path_ddbb = "PATH DEL ARCHIVO CSV"
```
2. Asignar el path de donde se guardarán los gráficos y archivos .CSV de las listas optimizadas de clientes

```
path_images = "PATH DE OUTPUT GRÁFICOS"

path_files = "PATH DE OUTPUT DE ARCHIVOS"
```
> En mi caso lo trabaje en un entorno de Google Collab, por lo que debes otorgale acceso a los archivos de Google Drive para trabajar todo en ese entorno.

3. Ejecuta el análisis con `marketing_segmentation.py`

# <br> Análisis de Negocio 🌟

Se realizó un análisis detallado utilizando los siguientes datos:

### 1. Exploración de Datos 🔍
- En esta etapa, se realizó una exploración inicial de los datos para obtener una visión general de las campañas anteriores y comprender mejor el perfil de los clientes.

Para el Perfil del Cliente se compararon dos grupos principales:
  - Clientes que aceptaron al menos una oferta: Análisis del comportamiento y características comunes de este grupo.
  - Clientes que no aceptaron ninguna oferta: Estudio de las diferencias clave entre estos clientes y los que aceptaron.

### 2. Segmentación 👥
- Basado la Recencia, Frecuencia y Valor Monetario (RFM) de los clientes, segmentamos a los clientes en 5 grupos: Top, Alto, Medio, Bajo e Inferior.

- Se emplearon técnicas de segmentación, como clustering con K-Means, para identificar grupos de clientes con comportamientos similares. Estos grupos se utilizarán para dirigir las futuras campañas de manera más eficaz, reduciendo el costo y aumentando las conversiones.

- Del mismo modo se planteo un grupo selecto de los Mejores Clientes, a los cuales se centrarán las campañas reduciendo los costos de contacto y aumentando el ROI de campañas.

### 3. Modelo Predictivo 🎯
- Para maximizar el beneficio de la próxima campaña, se desarrolló un modelo predictivo que ayuda a identificar qué clientes podrían aceptar la oferta.

- Se desarrolló un modelo predictivo con Random Forest que clasifica si el cliente aceptará las ofertas o no.

- Se evaluó la precisión del modelo utilizando métricas estándar (como precisión y F1 score), asegurando que el modelo puede hacer predicciones confiables.

### 4. Conclusiones 🚀
- Con base en los resultados del análisis y el modelo predictivo, se formularon conclusiones y recomendaciones para optimizar las futuras campañas de marketing directo. Estas incluyen mejorar la segmentación, enfocar el presupuesto en clientes con mayor probabilidad de conversión, y reducir la pérdida económica de la campaña.

Todo la documentación y análisis de negocios del caso se encuentra en [Versión en Español](https://github.com/mabustillo14/marketing_segmentation/blob/main/iFood%20Business%20Case%20Study%20-%20Mario%20Bustillo%20-%20Spanish.pdf) y [Versión en Inglés](https://github.com/mabustillo14/marketing_segmentation/blob/main/iFood%20Business%20Case%20Study%20-%20Mario%20Bustillo%20-%20English.pdf)
 
# <br> Contacto 🌟
Ante consultas, me puedes consultar por mi perfil de [Linkedin](https://www.linkedin.com/in/mario-bustillo/).
