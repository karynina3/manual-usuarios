.. _Hydroviewer Ecuador:

.. |logo| image:: _static/imgs/hydroviewer/hydroviewer.png
    :width: 60
.. |desplegable| image:: _static/imgs/hydroviewer/provincias.png
    :width: 30

|logo| HYDROVIEWER-Ecuador
===============================

.. note:: **Información General**
    Hydroviewer Ecuador muestra el pronóstico de caudal para cualquier río en el Ecuador. La red de ríos obtenida resulta
    de la extracción de ríos global del GEOGloWS ECMWF.


La interfaz de usuario muestra la delimitación de los ríos en color azul.

.. image:: _static/imgs/hydroviewer/hydroviewerpag.png
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
##########
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
######################
El gráfico desplegado en esta opción es la simulación histórica de los últimos 40 años. Los diferentes colores en el
gráfico representan los diferentes períodos de retorno que se calculan a partir de la simulación histórica de 40 años.
Los periodos de retorno pueden ser activados o desactivados según considere. También puede realizar zoom en un fecha
específica utilizando el cursor del mouse.

.. image:: _static/imgs/hydroviewer/historicalsimulation.png
   :width: 700
   :align: center


Estadísticas de simulación histórica
######################################
En esta opción se puede observar: curva de duración de caudales, estacionalidad diaria y estacionalidad mensual.

.. image:: _static/imgs/hydroviewer/historicalsimulationstatistics.png
   :width: 700
   :align: center

Descarga
##################
En esta opción le permite descargar el pronóstico y la simulación histórica en formato .csv

.. image:: _static/imgs/hydroviewer/descargadatoscsv.png
   :width: 500
   :align: center

