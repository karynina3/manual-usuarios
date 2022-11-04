.. _Tethys-logos:

.. |logo1| image:: _static/imgs/Tethys/geoglows.png
    :width: 50
.. |logo2| image:: _static/imgs/Tethys/hydroviewer.png
    :width: 50
.. |logo3| image:: _static/imgs/Tethys/hvt.png
    :width: 50
.. |logo4| image:: _static/imgs/Tethys/nwlf.png
    :width: 50
.. |logo5| image:: _static/imgs/Tethys/wde.png
    :width: 50
.. |logo6| image:: _static/imgs/Tethys/mde.png
    :width: 50
.. |logo7| image:: _static/imgs/Tethys/grace.png
    :width: 50
.. |logo8| image:: _static/imgs/Tethys/reservoir.png
    :width: 50
.. |logo9| image:: _static/imgs/Tethys/watermappingapp.png
    :width: 50
.. |logo10| image:: _static/imgs/Tethys/floodimpactviewer.png
    :width: 50

.. |logo11| image:: _static/imgs/Tethys/hydrostats.png
    :width: 50

.. |logo12| image:: _static/imgs/Tethys/climateapp.png
    :width: 50


MANUAL DE USUARIOS DE LA PLATAFORMA TETHYS-INAMHI-ECUADOR
############################################################

Este website contiene una guía para el manejo de las aplicaciones contenidas en la plataforma Tethys del INAMHI (Instituto
Nacional de Meteorología e Hidrología).
Tethys fue probada mediante la implementación de portales web para socios de la iniciativa de sostenibilidad del agua del
Grupo de Observaciones de la Tierra (GEO) y de la Universidad Brigham Young University (BYU).
En Ecuador, la implementación y personalización de la plataforma Tethys ha sido posible con la colaboración del
INAMHI, Fundación EcoCiencia y el Centro Internacional de Agricultura Tropical (CIAT), mediante el programa SERVIR-Amazonia.

Caja de herramientas GEOGloWS
********************************

La caja de herramientas GEOGloWS es una colección de herramientas de aplicación web de apoyo a la toma de decisiones en
materia de recursos hídricos. Se basa en lo que se está organizando en GEOGloWS como un **Almacén de Aplicaciones** que
se puede considerar similar a las tiendas de aplicaciones de Apple o tiendas de aplicaciones Android. Estas aplicaciones
fundamentales se extraen del almacén de aplicaciones que crecerá con el tiempo, las cuales pueden descargarse y combinarse
en portales personalizados con aplicaciones personalizadas para satisfacer las necesidades específicas de los diferentes
partes interesadas.

Plataforma Tethys INAMHI
*************************

.. image:: _static/imgs/Tethys/tethysPlat.jpeg

La plataforma Tethys alberga aplicaciones para pronóstico hidrológico, meteorológico, visualización y descarga de datos
relacionadas a variables hidrometeorológicas.

    1. **Aplicaciones para pronóstico hidrológico:** GEOGloWS ECMWF Streamflow Hydroviewer, Hydroviewer Ecuador,
                                                     Historical Validation Tool, National Water Level Forecast.
    2. **Aplicaciones para pronóstico meteorológico:** Met Data Explorer
    3. **Aplicación para visualización de datos:** Water Data Explorer



A continuación, se describe brevemente cada una de las aplicaciones contenidas en la plataforma Tethys de INAMHI.

|logo1| :doc:`GEOGloWS HydroViewer </content/AplicacionesHidrologicas>`
            El GEOGloWS ECMWF Streamflow provee el acceso a la simulación histórica de 40 años y al pronóstico de caudal con una
            previsión de 15 días para cerca de 1,000,000 de ríos a nivel mundial.

|logo2| :doc:`HydroViewer-Ecuador </content/hydroviewer-ecuador>`
            El Hydroviewer-Ecuador permite la visualización de pronósticos de caudal para cualquier río en Ecuador y permite
            visualizar alertas.

|logo3| :doc:`Historical Validation Tool </content/historical-validation>`
            El Historical Validation Tool permite visualizar pronósticos de caudal en los lugares estaciones hidrológicas de INAMHI
            que posean datos históricos de caudal con el fin de aplicar una corrección a la simulación de caudales.

|logo4| :doc:`National Water Level Forecast </content/national-water-level-forecast>`
            El National Water Level Foercast permite visualizar pronósticos de nivel solo donde existen datos históricos usando
            corrección de sesgo.

|logo5| :doc:`Water Data Explorer </content/water-data-explorer>`
            Aplicación para visualizar, descargar, y graficar datos observados en formato csv, Water ML, jpg y png

|logo6| :doc:`Met Data Explorer </content/met-data-explorer>`
         Aplicación para descubris, visualizar, garficar y descargar pronósticos meteorológicos en netCDF, Grib y geoTIFF.

|logo7| :doc:`GRACE Groundwater </content/groundwater-tools>`
        Utiliza información satelital para comprender las anomalías de las aguas subterráneas.
        Esta aplicación aún está en desarrollo.

|logo11| :doc:`HydroStats </content/hydrostats>`
         Esta aplicación permite procesar series de tiempo (merge, interpolaciones, graficar).

|logo12| :doc:`Tendencias de Clima </content/tendencias-clima>`
         La aplicación permite comparar datos obtenidos de información satelital y compararlo para diferentes variables.

|logo8| :doc:`Reservorios </content/Reservorios>`
         La aplicación permite visualizar y descargar datos de pronóstico de caudal para reservorios de agua.

|logo9| :doc:`Water Mapping App</content/historical-WaterMappingApp>`
         La aplicación usa datos Sentinel 1 para visualizar eventos de inundación pasados en un lugar determinado.

|logo10| :doc:`Flood Impact Viewer </content/historical-floodImpactViewer>`
         La aplicación permite visualizar el impacto de inundaciones. La aplicación aún está en desarrollo para Ecuador.

.. note:: **Páginas de Interés**

             Página de INAMHI:
            `INAMHI <https://www.inamhi.gob.ec/>`_
            Página de SERVIR-Amazonia:
            `SERVIR-Amazonia <https://servir.ciat.cgiar.org/?lang=es>`_
            Página de Fundación EcoCiencia:
            `Fundacion EcoCiencia <https://ecociencia.org/>`_
            Página de Laboratorio de Hydroinformática Brigham Young University:
            `Video BYU <https://hydroinformatics.byu.edu/>`_
            Video de Brigham Young University-GEOGloWS:
            `Video BYU <https://youtu.be/PLG8U8AQmXY>`_

.. toctree::
   :maxdepth: 6
   :caption: Contents:

   content/AplicacionesHidrologicas
   content/hydroviewer-ecuador
   content/historical-validation
   content/national-water-level
   content/water-data-explorer
   content/met-data-explorer

Indice
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

.. _link-to-geoglows-model-page

.. rst shortcut to make a link