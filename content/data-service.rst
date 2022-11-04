Data Service (REST API)
=======================

La API REST permite consultar y descargar información de cualquier flujo basándose en la formación de una consulta con
parámetros como como parte de la URL. La documentación sobre las posibles consultas y cómo formarlas se encuentra en la
página principal del servicio GEOGloWS Streamflow https://geoglows.ecmwf.int/.

A continuación, se describirá brevemente cómo se utilizan los servicios:

REST API Documentation
***********************

1. Vaya a este sitio web donde puede encontrar la documentación de la API REST: https://geoglows.ecmwf.int
2. Haga clic en la pestaña de la parte superior llamada "REST API Documentation".
3. Haga clic en la barra azul que dice GET y el nombre del método de la API de caudal de agua.
4. Pulse el botón blanco "Try" situado debajo de la barra azul de la derecha.



5. Provide the necessary parameters. Usually, the only argument is either a reach_id or both a latitude and a longitude.



6. Press the blue “Execute” bar.



7. The website will then generate the appropriate curl command and URL to access the data you chose with the parameters
you provided.


8. After retrieving the streamflow information from the REST API, it will be presented as a preview under code 200
(which is a common response code for a successful query). A download button is found on the bottom right of that box.



9. You can copy and paste the URL you found in step 6 into a new tab of your web browser to retrieve the same result
without needing to use the documentation’s interactive tool.

Forecasted Datasets
-------------------

Each day, a new 15-day weather prediction is made by ECMWF. The weather forecast is composed of 52 ensemble members.
From that weather prediction, a surface runoff estimation is made using the precipitation forecast and a land surface
model, HTESSEL. Each of the 52 ensemble members is used to drive the GEOGloWS ECMWF hydrologic model producing 52
streamflow predictions called *ensembles*. The results of these streamflow predictions are available through the following
methods.

**ForecastStats**: Summarizes the 52 ensembles across each time step by reporting the minimum flow, 25th percentile flow,
average flow, 75th percentile flow, and maximum flow. Returns a time series of values for each of the 5 statistical
values.

**ForecastEnsembles**: Returns a time series of flows for each of the 52 ensemble members.

**ForecastWarnings**: Returns a CSV that summarizes when streams are expected to reach 2-, 5-, 10-, 25-, 50-, and 100-year return period level flows.

**ForecastRecords**: Each day, the average of the predicted flows from 52 forecast ensemble members is recorded and can be
retrieved to see a longer running record of streamflow predictions.

Historically Simulated Datasets
-------------------------------

ECMWF provides the ERA5 historically simulated runoff dataset. This dataset is also used to drive the GEOGloWS ECMWF
model and produce a historical streamflow simulation. This streamflow simulation covers from January 1, 1979 to the
present with only a few months lag. The historical streamflow and products derived from it are available through the
following methods:

**HistoricSimulation**: Returns a time series of daily average streamflow from 1979 through the near present.

**DailyAverages**: Returns a time series 366 steps long representing the average flow for each day of the year including
leap day. This is roughly equivalent to what an average year of streamflow looks like at the reach of interest.

**MonthlyAverages**: Returns a time series of 12 steps representing the average flow for each of the 12 months of the year
based on the historical simulation. Most useful in comparative analyses and validation metrics.

**ReturnPeriods**: Based on the historical simulation and the Gumbal distribution, returns an estimation of the 2-, 5-, 10-,
25-, 50-, and 100-year return period flows for the stream reach.