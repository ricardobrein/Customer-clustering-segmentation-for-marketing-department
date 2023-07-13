
 

## Caso de estudio: Apoyo al Departamento de Marketing para enviar campañas segmentadas a los clientes.

Clustering con K-means, realizado sobre los datos de los clientes de una entidad bancaria, para apoyar al departamento de marketing tomar decisiones estratégicas

###  Customer clustering segmentation for marketing department

El marketing desempeña un papel fundamental en el crecimiento y la sostenibilidad de cualquier negocio. Para tener un marketing efectivo, es crucial realizar campañas personalizadas que comprendan las necesidades de nuestros clientes. Esto es fundamental para fortalecer la imagen de la compañía, retener clientes existentes, atraer nuevos clientes, aumentar las ventas y, en última instancia, mejorar el rendimiento de la empresa.

En este contexto, en este caso de estudio el Departamento de Marketing de nuestra empresa nos requiere para enviar campañas segmentadas a los clientes. El objetivo es **utilizar la información y los datos disponibles** para identificar diferentes grupos de clientes con características y necesidades similares. **Debemos segmentarlos en al menos, 3 grupos distintivos** Al segmentarlos, podemos adaptar las estrategias y mensajes de marketing de manera más efectiva, brindando una experiencia personalizada que resuene con cada segmento.

**El análisis implicará el analisis de datos de los ultimos 6 meses** de los utilizando ténicas de análisis de datos y clustering para identificar los grupos y patrones relevantes. Esto permitirá la creación de segmentos de clientes significativos, lo que nos brindará información valiosa para desarrollar campañas más precisas y efectivas.

Esto acompañado de la posterior automatización y seguimiento de campañas segmentadas, nos permitirá implementar estrategias específicas para cada grupo de clientes, realizar un seguimiento de su rendimiento y ajustar nuestras acciones según los resultados obtenidos.

![marketing](media/img1.png)
# 

TL; DR

## Resumen:

Durante nuestro análisis que se encuentra detallado en  [este notebook](Kmeans_clustering_Segmentacion_de_clientes_para_marketing_.ipynb), realizamos las siguientes acciones:

1. Visualización de datos: Iniciamos visualizando los datos para tener una comprensión inicial de su distribución y características.

2. Imputación de datos: Identificamos la presencia de algunos valores faltantes y los imputamos utilizando la media de los valores existentes en esas variables.

3. Manejo de valores atípicos: Observamos la existencia de varios valores atípicos en los datos. Aunque eran atípicos, podían proporcionarnos información relevante.

4. Determinación del número de clusters: Realizamos una investigación para determinar el número óptimo de clusters. Encontramos que el rango adecuado oscilaba entre 3 y 6 clusters. Considerando nuestro objetivo, decidimos dividir los datos en 3 clusters que representaran de manera más precisa la distribución de los datos.

5. Evaluación de la separación de clusters: Utilizamos el índice de silueta para evaluar la calidad de la separación entre los clusters obtenidos. Obtuvimos valores de silueta alrededor de 0.50, lo cual indica una separación relativamente buena entre los clusters.

6. Aplicación de Análisis de Componentes Principales (PCA): Utilizamos las técnicas de PCA con sklearn y autoencoders para reducir la dimensionalidad de los datos. Esto nos permitió obtener datos con una menor cantidad de dimensiones, lo cual facilita la representación y generalización de cada cluster mediante el algoritmo de clustering K-means.

7. Creacion de clusters con K-means: Despues de aplicar K-means creamos clusters, y los visualizamos, luego agregamos cada punto de los nuevos clusteres a los datos originales para indicar en un dataframe a que cluster pertenece cada registro y asi poder procesarlos posteriormente y entender cuales son las caracteristicas que identifican mejor cada cluster.

**Conocimientos:**
- Kaggle
- Quantifying the quality of clustering via silhouetee plots - Python Machine Learning - Raschka & Mirjalili


## Gracias