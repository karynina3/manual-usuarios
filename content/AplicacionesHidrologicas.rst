APLICACIONES HIDROLÓGICAS
##########################
`Video Inundaciones: herramientas de pronóstico de inundaciones <https://www.youtube.com/watch?v=lCTsUr9G3j0&t=4s>`_

Las aplicaciones hidrológicas usan el modelo  GEOGloWS ECMWF Streamflow Hydroviewer. El modelo es parte de la iniciativa de
GEOGloWS: `Iniciativa GEOGloWS <https://www.geoglows.org/>`_

El modelo GEOGloWS ECMWF streamflow es un modelo hidrológico global que consta de 52 ensambles.

La previsión hidrológica se calcula con el sistema de previsión meteorológica del ECMWF, que tiene 51 miembros
de 18 km de resolución para los 10 primeros días (días 1 a 10) y 36 km de resolución para los 5 días siguientes
(días 11 a 15). Estas previsiones meteorológicas se convierten en escorrentía mediante el modelo hidrológico HTESSEL.
A continuación, estos resultados se reducen mediante una metodología de ponderación de áreas entre cuadrículas y vectores y,
posteriormente, mediante el modelo RAPID, se dirigen a la red de drenaje. Posteriormente, los resultados de esta simulación
histórica se utilizan para definir los periodos de retorno con los que se establecen los niveles de alerta para cada
tramo de río simulado. Los valores de descarga corresponden a 2, 5, 10, 25, 50 y 100 años y se calculan utilizando la
distribución de probabilidad de Gumbel.

Estos servicios están disponibles para casi todos los ríos del mundo (cerca de un millón de ríos) con áreas de drenaje
inferiores a 200 km2, y se pueden acceder a ellos a través de servicios web, un enfoque que denominamos Hydrologic
Modeling as a Service (HMaaS).
A continuación se muestran las zonas en las que actualmente funciona el modelo.



El modelo presenta una simulación histórica desde el 01/01/1979 hasta el presente (2 - 3 meses de retraso) con resolución diaria.




Los miembros máximos y mínimos están representados por las líneas discontinuas azules.
Los percentiles 75 y 25 se muestran como la parte superior e inferior del rango verde, respectivamente.
La media de los ensambles es la línea azul continua.
El pronóstico de alta resolución se presenta en una línea negra.
Los periodos de retorno de 2,5,10,25 y 100 años se muestran respectivamente como las zonas horizontales amarilla, roja y morada.


`GEOGloWS Toolbox Presentation <https://docs.google.com/presentation/d/1Ur45mm11KcIYxz0rEHVMxO7loHWobvCtclcV5BW9nsU/edit?usp=sharing>`_

.. _Hydroviewer Ecuador:

.. |logohydro| image:: _static/imgs/hydroviewer/hydroviewer.png
    :width: 50


HYDROVIEWER-ECUADOR
##########################################


.. note:: **Información General**
    Hydroviewer Ecuador |logohydro| muestra el pronóstico de caudal para cualquier río en el Ecuador. La red de ríos
    obtenida resulta de la extracción de ríos global del GEOGloWS ECMWF.


La interfaz de usuario muestra la delimitación de los ríos en color azul.

.. image:: _static/imgs/hydroviewer/hydroviewer.png
   :width: 500
   :align: center

Además, puede ver triángulos de diferentes colores en función del período de retorno que ha sido excedido por la media
del pronóstico en cualquier momento con 15 días de antelación.

.. image:: _static/imgs/hydroviewer/panelcuencas.png
   :width: 70
   :align: center

Al seleccionar los botones de las alertas, en caso de existir alguna en el mapa base se observarán triángulos de alerta
según el periodo de retorno como se muestra en la imagen:

.. image:: _static/imgs/hydroviewer/hydroviewer-alertas.png
   :width: 500
   :align: center

En el siguiente ejemplo, se muestra una alerta generada para un periodo de retorno de 2 años en el *Río Yaupi*, localizado
en la provincia de Morona Santiago.

.. image:: _static/imgs/hydroviewer/alertarioyaupi2anios.png
   :width: 500
   :align: center

En la pantalla de visualización puede observar los botones desplegables para seleccionar una provincia de interés |desplegable|

.. image:: _static/imgs/hydroviewer/provinciasejemplo.png
   :width: 500
   :align: center

*En la imagen de ejemplo, se muestra la selección para la provincia de Morona Santiago.*

También puede seleccionar una cuenca, en el ejemplo de la imagen se muestra la demarcación:

.. image:: _static/imgs/hydroviewer/ejemplodemarcacion.png
   :width: 500
   :align: center

Seleccione un río de interés, puede encontrarlo por su ID o coordenadas. Una vez seleccionado el río se desplegará una
pantalla emergente con la identificación del río y se visualizarán 4 pestañas:  pronóstico, simulación histórica,
estadísticos y descarga.

.. image:: _static/imgs/hydroviewer/botonesventanaemergente.png
   :width: 300
   :align: center

Pronósticos
===============
El pronóstico proviene de 51 simulaciones diferentes y uno de alta resolución, incluye los períodos de retorno que se
activan de forma predeterminada cuando la previsión supera un umbral.
Los valores de umbral del período de retorno se muestran al pasar el cursor sobre ellos en el borde derecho del gráfico.

.. image:: _static/imgs/hydroviewer/forecast.png
   :width: 500
   :align: center

A continuación se describe cada una de las partes del pronóstico visualizado en el gráfico:

1. **Calendario:** puede seleccionar un pronóstico anterior al de la fecha, hasta con un periodo de 40 días aproximadamente.
2. Se muestra el pronóstico con una previsión para 15 días, y se muestran los periodos de retorno. Incluye el promedio,
los percentiles de caudal 25-75, los caudales máximo y mínimo, y un único pronóstico de mayor resolución.
3.La leyenda se puede ver a la derecha y las diferentes capas se pueden activar y desactivar. El valor real de caudal de
datos para cada período de tiempo se puede mostrar al pasar el cursor sobre el gráfico.
4.Todos los gráficos desplegados en la ventana emergente presentan una barra en la esquina superior derecha de los mismos:
descarga en la opción de la cámara, zoom, pan, zoom in, zoom out, autoscale, reset axes.

.. image:: _static/imgs/hydroviewer/botonesdescargagrafico.png
   :width: 200
   :align: center

5.En la parte inferior de la ventana emergente desplegada se puede visualizar un cuadro del porcentaje de Ensambles que
exceden el periodo de retorno.

Simulación histórica
=====================
El gráfico desplegado en esta opción es la simulación histórica de los últimos 40 años. Los diferentes colores en el
gráfico representan los diferentes períodos de retorno que se calculan a partir de la simulación histórica de 40 años.
Los periodos de retorno pueden ser activados o desactivados según considere. También puede realizar zoom en un fecha
específica utilizando el cursor del mouse.

.. image:: _static/imgs/hydroviewer/historicalsimulation.png
   :width: 700
   :align: center


Estadísticas de simulación histórica
===========================================
En esta opción se puede observar: curva de duración de caudales, estacionalidad diaria y estacionalidad mensual.

.. image:: _static/imgs/hydroviewer/historicalsimulationstatistics.png
   :width: 700
   :align: center

Descarga
===========
En esta opción le permite descargar el pronóstico y la simulación histórica en formato .csv

.. image:: _static/imgs/hydroviewer/descargadatoscsv.png
   :width: 500
   :align: center

.. _Historical Validation Tool:

.. |logo| image:: _static/imgs/hydroviewer/hvt.png
    :width: 70


HISTORICAL VALIDATION TOOL (HVT)
######################################

.. note:: **Información General**
    Esta aplicación usa los datos observados de caudal históricos de las estaciones monitoreadas por INAMHI para ajustar
    los Servicios de GEOGloWS ECMWF Streamflow Prediction para las estaciones hidrológicas en Ecuador.

**En esta aplicación se puede visualizar pronóstico de caudal con un horizonte de 15 días y adicional se muestra la
corrección de sesgo.**

La corrección de sesgo usada se basa en curvas de duración de caudales mensuales descrito por Sanchez- Lozano
 (`<https://doi.org/10.3390/hydrology8020071>`_).

Para cada estación, el usuario puede ver series de tiempo y calcular métricas de error. La interfaz de usuario muestra
la delimitación de los ríos en azul y de las estaciones con mediciones de caudales identificados con puntos en rojo.

.. image:: _static/imgs/historical-validation/hvt.png

A manera de ejemplo, seleccione una estación al hacer clic. Para este ejemplo, haga zoom en la Estación Napo en Nuevo
Rocafuerte (Station Code: H1136, estación COMID (ID de río): 9026410).


Al hacer clic en la estación, aparecerá una ventana emergente con los datos de la misma. La ventana emergente, mostrarán
4 pestañas diferentes: hidrograma, análisis visual, reporte de métricas y pronóstico.



Hidrograma
================
.. image:: _static/imgs/historical-validation/hvt.png

La pestaña muestra el hidrograma con los valores observados de caudal, la simulación histórica y la simulación histórica
corregida. Este gráfico muestra la mejora entre el hidrograma de datos históricos simulados (rojo) y el hidrograma de
datos con corrección de sesgo (verde). El usuario puede activar y desactivar cada una de las opciones del hidrograma.

Análisis visual
=====================

La segunda pestaña en la ventana emergente es el análisis visual: promedio diario, promedio mensual, diagrama de
dispersión, diagrama de dispersión usando escala logarítmica, diagrama de análisis de volumen (simulación histórica de
40 años combinada con el volumen total que pasó por la estación, el cual fue calculado utilizando el caudal diario) y
tabla de análisis de volumen un determinado lugar.

Informe de métricas
======================
La tercera pestaña en la ventana emergente es el informe de métricas. El informe de métricas tiene una lista de
métricas predeterminadas, pero los usuarios pueden agregar métricas adicionales de las disponibles en el paquete
HydroStats. La interfaz proporciona métricas de error que pueden cuantificar la comparación y la evaluación de
la mejora entre la simulación histórica corregida por sesgo y la simulación histórica original de acuerdo con las
diversas métricas de error.

Pronóstico
===============

La pestaña muestra el pronóstico original y el pronóstico corregido por sesgo en los gráficos superior e inferior,
respectivamente. El gráfico superior muestra el pronóstico original antes de la corrección del sesgo, los umbrales de
los períodos de retorno calculados a partir de la simulación histórica. El gráfico de pronóstico inferior muestra el
pronóstico corregido sesgado, con umbrales de períodos de retorno calculados a partir de la simulación histórica corregida
por sesgo. Los dos gráficos de pronósticos provienen de 51 simulaciones diferentes, muestran los percentiles de caudal
25 y 75, caudales máximo y mínimo y un pronóstico de alta resolución. La leyenda desplegada en la derecha muestra las
diferentes capas se pueden activar y desactivar de los periodos de retorno calculados para la simulación histórica y la
simulación histórica corregida por sesgo. Los datos de cada período de tiempo aparecen al pasar el cursor sobre el gráfico.
Los datos pueden ser descargados desde la pestaña final.


.. note:: **Recursos Adicionales**

    Uso de la API - GEOGloWS ECMWF Streamflow Services - Ecuador

    `Material: <https://colab.research.google.com/drive/1LSEySZoTGm1mETqeMlbL7NxFBDLbyL0R?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/1XkgVRIlULSZhCyWPlfRgo-lclZ1itqzE/view?usp=sharing>`_

    Correción del Sesgo - GEOGloWS ECMWF Streamflow Prediction Services - Ecuador

    `Material: <https://drive.google.com/file/d/1L4BraZzLNfXsDCvoXxtKgi7v2grxUmJu/view?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/1L91tVe3jNpFvFxhZK4uWO1oNgBcEjoil/view?usp=sharing>`_

    Evaluación del desempeño de los pronósticos del modelo GESS - Ecuador
    *****************************************************************************
    `Material: <https://drive.google.com/drive/folders/1-9X0J50X9joOwp8Kzct540Q5ExJgvEJl?usp=sharing>`_
    `Video: <https://drive.google.com/file/d/168iamcxcHl2GbMwlnt8z3fZ3GIcGGuZ8/view?usp=sharing>`_

.. _National Water Level Forecast:

.. |logonwlf| image:: _static/imgs/nwlf/nwlf.png
    :width: 50

.. |desplegable| image:: _static/imgs/hydroviewer/provincias.png
    :width: 30


NATIONAL WATER LEVEL FORECAST
#########################################






