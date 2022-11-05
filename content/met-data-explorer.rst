.. _Met Data Explorer:

.. |logo| image:: _static/imgs/met-data-explorer/logo.png
    :width: 70

.. |botonaladomde| image:: _static/imgs/met-data-explorer/botonaladomde.png
    :width: 30

.. |coordenadas| image:: _static/imgs/met-data-explorer/coordenadasboton.png
    :width: 30

.. |latandlong| image:: _static/imgs/met-data-explorer/latandlong.png
    :width: 30

.. |areadefinida| image:: _static/imgs/met-data-explorer/areadefinida.png
    :width: 30

.. |areaindefinida| image:: _static/imgs/met-data-explorer/areaindefinida.png
    :width: 30

.. |puntoespecifico| image:: _static/imgs/met-data-explorer/areapuntual.png
    :width: 30

.. |barramapa| image:: _static/imgs/met-data-explorer/barramapa.png
    :width: 50

.. |botonesgrafico| image:: _static/imgs/met-data-explorer/botonesgrafico.png
    :width: 70

.. |botonespantalla| image:: _static/imgs/met-data-explorer/botonespantalla.png
    :scale: 50
.. |seleccionmapa| image:: _static/imgs/met-data-explorer/seleccionmapa.png
    :scale: 50

|logo| MET DATA EXPLORER (MDE)
#########################################


.. note:: **Información General**

    Met Data Explorer (MDE) es una app de código abierto que permite descubrir, acceder, visualizar y descargar datos
    grillados. Utiliza un THREDDS server el cual brinda acceso en tiempo real a conjuntos de datos grillados y
    metadatos utilizando varios protocolos de acceso estándar.


La interfaz de la app MDE se divide en algunas secciones: panel de visualización, visualizador del mapa y de datos.
A continuación, se detalla cada una de las partes del MDE:

1. Panel
================
El panel de navegación lateral enumera los archivos que se han cargado en el MDE mediante catálogos.

 **Catálogo**
Permite visualizar la información de interés agrupado en diferente grupos. Según las credenciales de usuario, permite
agregar o eliminar capas y grupos en el catálogo.

.. image:: _static/imgs/met-data-explorer/catalogos.png
   :width: 300
   :align: center

El área de extracción se puede especificar como un marcador, un cuadro delimitador, un polígono o por coordenadas
(latitud, longitud). La ventana de mapa se utiliza para visualizar y animar los datos y para definir el área sobre
la cual extraer los datos.

Localización de áreas de interés
******************************

Los botones para localizar áreas de interés se encuentran en los botones a la izquierda del mapa |botonespantalla|.
Los primeros dos botones permiten realizar el zoom de un área de interés, y los dos últimos botones permiten borrar una
selección de área definida previamente.

Para localizar un área de interés se puede acceder de algunas maneras:
    • Ingresando las coordenadas |coordenadas|. Al hacer clic en este botón se abrirá una pequeña ventana emergente |latandlong|,
    una vez llenada la informaciòn en el mapa se ubicará el punto.
    • Dibujando un área de interés: con un área definida |areadefinida| o sin definir |areaindefinida|
    • Marcando un punto específico en el mapa |puntoespecifico|
    • Shapefile: puede seleccionar el shapefile de su interés, en el siguiente gráfico se muestran las provincias del
      Ecuador.

.. image:: _static/imgs/met-data-explorer/aguaprecipitable.png
   :width: 200
   :align: center

2. Visualización
=========================

Para visualizar el mapa ó el cuadro de información de diferente tamaño de manera vertical conforme se mueva la barra
plomo del centro |barramapa|.
Derecha: se desplegará el mapa en toda la pantalla.

Izquierda: se visualizará la tabla de contenidos.

Medio: se visualizará la pantalla y cuadro de opciones.

.. image:: _static/imgs/met-data-explorer/mde.png
   :width: 200
   :align: center

Haciendo clic en la barra junto al nombre de la aplicación |botonaladomde| se puede visualizar la pantalla completa de
manera horizontal:

.. image:: _static/imgs/met-data-explorer/mdepantallacompleta.png
   :width: 200
   :align: center


Se puede agregar diferentes tipos de mapas |seleccionmapa|.

Además, el MDE permite la animación de la capa de interés, se puede acelerar o desacelerar la animación.

También en el gráfico a la derecha del mapa, se puede observar la barra de valores de la capa seleccionada.

.. image:: _static/imgs/met-data-explorer/barradecolores.png
   :width: 100
   :align: center


Descubrimiento de datos
============================
Para visualizar los datos en el mapa, seleccione un file del catálogo, y la capa aparecerá en el mapa. La primera variable
listada en el archivo será seleccionada por defecto. La variable seleccionada se puede cambiar utilizando el menú
desplegable Variable. La forma en que se muestran los datos en el mapa se puede modificar cambiando la configuración de
visualización ubicada en la parte inferior de la ventana de gráficos.

**File options**
En este cuadro se puede seleccionar las fechas de interés, seleccionar un shapefile  como la división política nacional
o estaciones convencionales de INAMHI. Para graficar los datos del àrea seleccionada, haga clic en *Plot time series*.

.. image:: _static/imgs/met-data-explorer/fileanddimensions.png
   :width: 200
   :align: center

**Display settings**

Permite modificar las opciones de la capa de interés como la opacidad, colores u ocultar la capa. Al finalizar de
establecer la configuración de la visualización de la capa, hacer clic en el botón verde.

.. image:: _static/imgs/met-data-explorer/layeropacity.png
   :width: 200
   :align: center


Una vez que se haya especificado una ubicación sobre la cual extraer los datos, y realizado las configuraciones requeridas
haga clic en el botón *Plot Time Series* para extraer y graficar los datos.

La serie temporal se trazará en la ventana del gráfico, en la siguiente ventana emergente.

**Gráfico de la serie de tiempo**
Una vez seleccionado el punto o área de interés, en la ventana emergente desplegada se visualizarán los datos
graficados en scatter o box plot. A continuación, se muestra el gráfico de dispersión para la serie de tiempo:

.. image:: _static/imgs/met-data-explorer/graficoplot.png
   :width: 500
   :align: center

A continuación, se muestra para la misma serie de tiempo el gráfico de box plot:
.. image:: _static/imgs/met-data-explorer/boxplot.png
   :width: 800
   :align: center

Realizar zoom, restaurar el gráfico cuando se haya realizado un zoom en una fecha determinada.
Visualización de los datos, al acercar el cursor del mouse se puede visualizar los datos de un punto determinado.
En la parte derecha del gráfico se muestra la leyenda la cual puede ser activada o desactivada.

No se olvide de *Limpiar el área de gráfico anterior*, en caso que desee visualizar una sola variable.

**Calculadora**
Sirve para realizar la conversión de unidades de una variable en específico.

.. image:: _static/imgs/met-data-explorer/calculadora.png
   :width: 500
   :align: center

Para lo cual se debe ingresar el nombre la nueva variable en New Dataset ID y posteriormente realizar el cálculo con la
variable seleccionada, como se muestra en la gráfica:

.. image:: _static/imgs/met-data-explorer/temperaturakelvin.png
   :width: 500
   :align: center

Una vez realizada la transformación de unidades, haga clic en *Apply* y podrá visualizar el gráfico de la serie de tiempo
en las dos unidades ya sea a manera de box plot o de dispersión:

.. image:: _static/imgs/met-data-explorer/comparaciondetemperaturas.png
   :width: 500
   :align: center

En el gráfico se muestra la temperatura en unidades Celsius y Kelvin. Puede activar o descativar las lìneas haciendo clic
en el nombre de la serie de tiempo.

3. Descarga de datos
===================
La aplicación permite descargar los datos en diferentes formatos:  csv, JSON, Html, Python Notebook

.. image:: _static/imgs/met-data-explorer/descargadatos.png
   :width: 800
   :align: center

En la parte superior derecha del gráfico se muestra una serie de botones |botonesgrafico|, para descargar los datos seleccione
el botón en forma de cámara (botón número 2), y se decargará la imagen en .png


Recursos Adicionales
********************

- `MDE Source Code <https://github.com/BYU-Hydroinformatics/Met-Data-Explorer>`_

- `Grids Source Code <https://github.com/rileyhales/grids>`_

- `Grids Documentation <https://tsgrids.readthedocs.io/en/stable/>`_

- `Grids Demo <https://gist.github.com/rileyhales/79761303df16127e0195e11425fc2d9d>`_

- `CF Conventions <https://cfconventions.org/cf-conventions/cf-conventions.html>`_

- `NCML Cookbook <https://docs.unidata.ucar.edu/thredds/ncml/current/ncml_cookbook.html>`_
