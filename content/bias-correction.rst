Bias Correction
===============

Los resultados de los modelos globales suelen mostrar sesgos a escala local o en lugares específicos.
Aunque el tiempo y otros parámetros generales de un evento de inundación pueden ser correctos, la magnitud real del
evento puede ser consistentemente más alta o más baja que los caudales reales.
Estas predicciones sesgadas impiden su uso a escala local porque el sesgo puede afectar significativamente a la
precisión de una inundación simulada y, si es incorrecta, puede hacer que los responsables de la toma de
decisiones pierdan la confianza en los modelos.


Un método de corrección del sesgo derivado del método presentado por
`Farmer et al.(2018) <https://hess.copernicus.org/articles/22/5741/2018/>`_, que se basa en la curva de duración del caudal,
se ha propuesto para corregir el sesgo en el flujo de corriente simulado por GEOGLoWS ECMWF. En primer lugar, la curva
de duración del flujo se calculada a partir de las series temporales simuladas históricas y de las series temporales de
caudales observados para cada mes. La curva de duración del caudal muestra el porcentaje acumulado de tiempo en el que
se ha superado un caudal determinado durante un periodo concreto. En el gráfico abajo, las curvas de duración del caudal
se muestran a la derecha. El amarillo son los datos originales simulados, el azul son los observados y el rojo son los
datos simulados después de rojo son los datos simulados después de la corrección del sesgo.

Utilizando la curva de duración del caudal, podemos estimar la probabilidad de no superación de cada valor simulado
para cada mes. Esto se muestra en el gráfico como la línea horizontal superior, que conecta los datos simulados con la
curva de duración del caudal simulado.
La línea vertical muestra esa misma probabilidad de no superación en la curva de duración del caudal de los datos observados.
La línea vertical muestra la misma probabilidad de no superación en la curva de duración del caudal de los datos observados.
Por último, corregimos el valor simulado sustituyéndolo por el caudal observado equivalente a la misma probabilidad de
no superación, que se muestra en la línea horizontal inferior.

Utilizando la curva de duración del caudal, podemos estimar la probabilidad de no superación de cada valor simulado para
cada mes.
Esto se muestra en el gráfico como la línea horizontal superior, que conecta los datos simulados con la curva de duración
del caudal simulado.
La línea vertical muestra esa misma probabilidad de no superación en la curva de duración del caudal de los datos observados.

Por último, corregimos el valor simulado sustituyéndolo por el caudal observado equivalente a la misma probabilidad de
no superación, que se muestra en la línea horizontal inferior.



.. image:: /_static/imgs/bias-correction/intro-flow-duration.png
   :width: 550
   :align: center

.. image:: /_static/imgs/bias-correction/bias-correction.png
   :width: 700
   :align: center

Puede utilizar los datos históricos observados que tiene para los sitios que le interesan para ajustar cualquier sesgo en la
simulación histórica y la previsión en ese punto (estamos trabajando en la ampliación de la corrección del sesgo a las zonas no aforadas). Los métodos de
métodos y los resultados de algunos estudios piloto se ofrecen en la presentación.


