### Análisis de ventas de Adidas.

##  INTRODUCCIÓN:
El conjunto de datos de ventas de Adidas es una recopilación de datos que incluye información sobre las ventas de productos de Adidas. 
Este conjunto de datos incluye detalles como la cantidad de unidades vendidas, las ventas totales, la ubicación de las ventas, el tipo de producto vendido y cualquier otra información relevante.
En este informe de análisis de ventas, analizamos en profundidad el desempeño de Adidas, una marca líder mundial de ropa deportiva, durante el año pasado. Aprovechando herramientas de análisis de datos como Excel, Python y Power Bi, nuestro objetivo es brindar información valiosa sobre el desempeño de ventas, las tendencias del mercado y las oportunidades de crecimiento de Adidas. 
Este informe destaca métricas clave, analiza el desempeño del producto, examina las tendencias de ventas regionales y ofrece recomendaciones estratégicas para optimizar las ventas y mantener una ventaja competitiva en la industria de la ropa deportiva. A través del uso de bibliotecas de Python, limpieza de datos, análisis exploratorio de datos y visualizaciones impactantes, obtuvimos información útil sobre los factores que impulsan el crecimiento de las ventas e identificamos oportunidades para una mayor optimización. Este análisis servirá como base para la toma de decisiones basada en datos y la planificación estratégica en Adidas.

##  BASE Y REQUISITOS:
El conjunto de datos utilizado para este proyecto se obtuvo de Kaggle y se denominó “Conjunto de datos de ventas de Adidas” y se convirtió de un archivo XLSX a un archivo CSV para facilitar su manejo. 
El aspecto analítico del proyecto se llevó a cabo dentro del entorno Python de Google Colaboratory, mientras que se aprovechó Microsoft Power BI para crear paneles interactivos. 
El conjunto de datos se recopiló en una hoja de cálculo (Microsoft Excel) con encabezados de columna que incluyen:
![image](https://github.com/user-attachments/assets/26ba0391-f223-4592-9a5b-beb3ce9bd0fb)

##  ANÁLISIS EXPLORATORIO DE DATOS (EDA)
El análisis exploratorio de datos (EDA) es un paso esencial para comprender y preparar los datos para el análisis. 
Durante el EDA, profundizamos en los diversos aspectos del conjunto de datos para descubrir información y patrones que puedan guiar nuestro análisis.
Este paso nos ayuda a identificar valores faltantes, valores atípicos, tendencias, correlaciones y posibles variables de interés. 
1. ¿Qué canales de venta generan mayores ingresos y crecimiento?
2. ¿Qué ciudades generan más ventas para el negocio?
3. ¿Cómo varía el rendimiento de ventas en diferentes regiones geográficas?
4. ¿Qué productos generan mayores ingresos por ventas?
5. ¿Qué meses o años tuvieron las cifras de ventas más altas y más bajas?
6. ¿Qué meses o años tuvieron las cifras de utilidad operativa más altas y más bajas?
7. ¿Cómo varía el rendimiento de ventas según los diferentes métodos de venta?
8. ¿Qué minorista realizó la compra más alta y la más baja?

## MÉTODOS UTILIZADOS:
### Limpieza y preprocesamiento de datos:
El primer paso en cualquier análisis de datos es garantizar la calidad y la fiabilidad de los mismos. 
La limpieza y el preprocesamiento de los datos son fundamentales para eliminar inconsistencias y preparar el conjunto de datos para el análisis.

1) Las bibliotecas de Python proporcionan funciones y herramientas predefinidas que simplifican varias tareas. 
En este paso, importamos bibliotecas como Pandas para la manipulación de datos, NumPy para operaciones numéricas, Matplotlib y Seaborn para la visualización de datos, Calendar para varias funcionalidades relacionadas con fechas y calendarios, Seasonal decompose para la descomposición de series temporales y ARIMA para implementar el modelo ARIMA (AutoRegressive Integrated Moving Average) para la previsión de series temporales. 
Estas bibliotecas ayudarán a realizar análisis de manera eficiente.

# Carga del conjunto de datos:

2) Este paso implica importar la biblioteca de Python necesaria, normalmente Pandas, para cargar el conjunto de datos desde un archivo CSV.
   Este es el primer paso para que los datos estén disponibles para su análisis.

### Comprobación de la forma del marco de datos:

3) Este es un paso básico para comprender el tamaño del conjunto de datos. Devuelve la cantidad de filas y columnas en el marco de datos.

### Comprobación de valores duplicados:

4) Este proceso implica identificar y contar las filas duplicadas en el conjunto de datos.Los datos duplicados pueden distorsionar los resultados del análisis y, si están presentes, se debe solucionar el problema.
   No había filas duplicadas en el conjunto de datos.
   
### Comprobación de la información de los datos:

5) La función ` .info()` proporciona información esencial sobre el conjunto de datos, como los tipos de datos de las columnas y la cantidad de valores no nulos.
 Esto ayuda a comprender la estructura y la calidad de los datos.

## ANÁLISIS DEL DESEMPEÑO FINANCIERO:

## En esta sección se analiza en profundidad el desempeño financiero de Adidas. 
Al examinar indicadores clave críticos como los ingresos promedio, el margen operativo promedio, 
las ganancias interanuales, las tendencias de ingresos anuales y los ingresos totales, 
obtenemos información que arroja luz sobre la salud financiera y la trayectoria de crecimiento de la empresa.
A través de estos análisis, buscamos descubrir patrones, tendencias y áreas potenciales para mejoras estratégicas.

## Insights 

1) Los ingresos totales brindan una visión general del tamaño financiero de la empresa y su presencia en el mercado. 
El seguimiento de esta métrica a lo largo del tiempo muestra la trayectoria de crecimiento de la empresa. 
Los picos o caídas repentinos en los ingresos totales pueden atribuirse a eventos importantes, lanzamientos de productos, cambios económicos o cambios en la demanda de los consumidores.

2) La métrica de ganancias interanuales nos permite evaluar el crecimiento o la disminución de las ganancias a lo largo del tiempo. 
Los valores positivos indican un aumento de las ganancias, mientras que los valores negativos sugieren una disminución. 
Este conocimiento ayuda a evaluar la salud financiera y el desempeño de Adidas e identificar tendencias en la rentabilidad.

3) La métrica de ingresos promedio brinda información sobre el valor típico de cada transacción de venta.Al analizar los ingresos promedio a lo largo del tiempo o en diferentes segmentos de clientes,
   podemos identificar cambios en el comportamiento de compra y medir la eficacia de las estrategias de marketing.

4) La métrica de ingresos de cada año permite identificar patrones cíclicos, variaciones estacionales o posibles picos de crecimiento.
   Al visualizar los ingresos por año, podemos detectar períodos de crecimiento o declive y evaluar el impacto de factores externos o estrategias comerciales en el desempeño de las ventas.
   Esta información es valiosa para anticipar períodos de alta demanda, planificar estrategias de marketing y alinear las operaciones comerciales con las tendencias de ingresos.

5)  Comparar los ingresos del mismo período en diferentes años ofrece información sobre la estacionalidad y los patrones cíclicos en el negocio de Adidas.
   Ayuda a identificar períodos de rendimiento alto o bajo constante, lo que contribuye a una gestión eficaz del inventario, el momento oportuno para la comercialización y la asignación de recursos.  

6)  El margen operativo promedio es una medida fundamental de la eficiencia con la que Adidas gestiona sus costos. Un margen operativo positivo sugiere rentabilidad, mientras que uno negativo podría indicar problemas con el control de costos.
    El seguimiento de esta métrica ayuda a optimizar las estrategias de precios y a gestionar los gastos de manera eficaz.

## CONCLUSIÓN DE LOS INSIGHT:

Al analizar estas métricas financieras, Adidas puede obtener una comprensión integral de su desempeño financiero, lo que permite tomar decisiones basadas en datos, 
una planificación estratégica informada y ajustes oportunos a la dinámica del mercado.


