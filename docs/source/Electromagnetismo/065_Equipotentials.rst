+Equipotenciales
================

Determinar el conjunto de líneas equipotenciales para distintas configuraciones de electrodos conectados a una fuente de voltaje e inmersos en un líquido poco conductor. Comparar los resultados experimentales con los resultados provenientes de la solución de Laplace utilizando el método de relajación implementado en la hoja de cálculo Excel.

**Recursos**
   #. Cubeta rectangular  de vidrio de propundidad aproximadamente 4 cm
   #. Agua destilada.
   #. Dos fuentes de voltaje DC.
   #. Un voltímetro.
   #. Placas metálicas de (Cu, Al) para usar como electrodos.

**Resumen teórico**

El trabajo: math:`W` que se requiere para llevar una partícula :math:`q`  del punto :math:`A` al  punto :math:`B` a lo largo de una trayectoria :math:`C`  en una región donde existe un campo eléctrico :math:`E`  es dado por la integral de línea

.. math::
   :label: Ec:Equip_01

   \begin{equation}
    W=q\int \vec{E}\cdot d\vec{l}=q(V_A-V_B)
   \end{equation}

dónde :math:`V` es una función escalar denominada función potencial eléctrico y se expresa en voltios. El campo eléctrico es conservativo, es decir, el valor de :math:`W` no depende de la forma de la trayectoria que conecta los puntos :math:`A`  y :math:`B`. La relación entre :math:`\vec{E}` y :math:`V` es

.. math::
   :label: Ec:Equip_02

   \begin{equation}
      E_x = -\frac{\partial V}{\partial x}
   \end{equation}

.. math::
   :label: Ec:Equip_03

   \begin{equation}
      E_x  = -\frac{\partial V}{\partial y}
   \end{equation}

.. math::
   :label: Ec:Equip_04

   \begin{equation}
     E_z  = -\frac{\partial V}{\partial z}
   \end{equation}


Una línea de campo eléctrico es una recta o curva imaginaria trazada a través de una región en el espacio, de modo que el vector de campo eléctrico en un punto es tangente a la línea de campo eléctrico en ese punto.
Una línea o superficie equipotencial es una superficie imaginaria trazada a través de una región del espacio, de modo que todos sus puntos tienen el mismo valor de potencial eléctrico.

.. note::

   El general el campo eléctrico siempre es perpendicular a las superficies equipotenciales.

.. figure:: /images/Electromagnetismo/Equipotentials/Equipotentials_01.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:Equipotentials_01

   Líneas de campo eléctrico (líneas verdes) y superficies equipotenciales (Líneas azules y rojas) asociadas a dos cargas positivas  y dos cargas negativas)

El potencial eléctrico :math:`V(x,yz)` asociado a un campo eléctrico :math:`\vec{E}` cumple la ecuación de Poisson:

.. math::
   :label: Ec:Equip_05

   \begin{equation}
   \frac{\partial^2 V}{\partial x^2}+\frac{\partial ^2 V}{\partial y^2}+\frac{\partial ^2 V}{\partial z^2} =-\frac{\rho}{\epsilon_o}
   \end{equation}

En una región plana (:math:`z=0`) en ausencia de carga eléctrica: :math:`\rho=0`, la ecuación se convierte en la ecuación de Laplace

.. math::
   :label: Ec:Equip_06

   \begin{equation}
    \frac{\partial^2 V}{\partial x^2}+\frac{\partial ^2 V}{\partial y^2} =0
   \end{equation}

Un método simple para solucionar la ecuación: :eq:`Ec:Equip_06`, [#f3]_ consiste en discretizar  el plano :math:`xy`, es decir, se toma una malla bidimensional (ver :numref:`fig:discretization.png`)  de modo que las coordenadas :math:`x,y` se reemplazan por los índices :math:`i,j` y las derivadas que aparecen  :eq:`Ec:Equip_06` se reemplazan por

.. figure:: /images/Electromagnetismo/Equipotentials/discretization.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:discretization.png

   Discretización del plano.



.. math::
   :label: Ec:Equip_07

   \begin{equation}
   \frac{\partial V}{\partial x}\approx\frac{V_{i+1,j}-V_{i,j}}{h}
   \end{equation}

.. math::
   :label: Ec:Equip_08

   \begin{equation}
    \frac{\partial V}{\partial y}\approx\frac{V_{i,j+1}-V_{i,j}}{h}
   \end{equation}

y:

.. math::
   :label: Ec:Equip_09

   \begin{equation}
    \frac{\partial^2 V}{\partial x^2}\approx\frac{V_{i+1,j}-2V_{i,j}+V_{i-1,j}}{h^2}
   \end{equation}


.. math::
   :label: Ec:Equip_10

   \begin{equation}
   \frac{\partial^2 V}{\partial y^2}\approx\frac{V_{i,j+1}-2V_{i,j}+V_{i,j-1}}{h^2}
   \end{equation}

donde :math:`h` es el tamaño de la discretización o de la celda unitaria. De las ecuaciones :eq:`Ec:Equip_06`, :eq:`Ec:Equip_09`,  y :eq:`Ec:Equip_10`,  se encuentra que

.. math::
   :label: Ec:Equip_11

   \begin{equation}
   V_{i,j}=\frac{1}{4}\Big(V_{i+1,j}+V_{i-1,j}+V_{i,j+1}+V_{i,j-1}\Big)
   \end{equation}

.. Note::
   La ecuación :eq:`Ec:Equip_11` significa que el potencial en un punto dado del plano :math:`(i,j)` es igual al promedio del potencial de los cuatro puntos vecinos próximos.

El método de relajación hace uso de esta propiedad de la solución de la ecuación de Laplace. En una hoja de cálculo (Excel) el valor de una celda dada es el promedio de sus vecinas más próximas, excepto para aquellos puntos que tienen un potencial fijo (coincidente con el potencial de los electrodos), cuyos valores están establecidos por las condiciones de frontera y no varían. Luego se realizan las iteraciones hasta que los valores de las celdas no cambien, o hasta que su variación sea menor que un valor prefijado, digamos del 0.01%. Varios ejemplos de aplicación de este procedimiento se encuentran en las plantillas de Excel suminsitradas, [#f4]_.

**Condiciones de frontera**

Existen dos tipos de condiciones de frontera:

   #. *Dirichlet:* Este caso se usa en aquellas zonas donde el potencial se conoce como por ejemplo en los electrodos. En un electrodo todos los puntos de este se encuentran al mismo potencial eléctrico. Operacionalmente, esto se logra asignando un valor contante de potencial a todas aquellas celdas donde se encuentra el electrodo.
   #. *Neumann:* Este caso se usa en las paredes del recipiente (no conductoras), allí la corriente debe ser paralela a las paredes, la cuales definen la frontera. Operacionalmente, esta condición se logra haciendo que los valores de las celdas que definen los bordes del recipiente sean iguales a los valores de las celdas contiguas interiores. Por ejemplo, si la pared izquierda del recipiente coincide con el eje: math:`y`, las celdas que representan esta pared tienen índices :math:`(i=0,j)`, el valor del potencial sobre la pared debe cumplir :math:`V_{i=0,j}=V_{i=1,j}`.

**Montaje experimental**

Realice el montaje que se muestra en la :numref:`fig:Setup_02`. Este consta de una cubeta con agua destilada cuyo nivel no supera los 4 cm de altura en cuyo fondo se encuentran un par de electrodos conectados a las fuentes de voltaje y un voltímetro cuyo terminal negativo va conectado al punto común de conexión de las dos fuentes. El terminal positivo del voltímetro se utiliza como sonda y que al colocarlo en un punto :math:`P=(x,y)`, el voltímetro suministra el valor del potencial en dicho punto.  Note que la base de la cubeta posee un papel milimetrado.


.. figure:: /images/Electromagnetismo/Equipotentials/Equipotentials_02.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:Setup_02

   Montaje experimental.

**Mediciones**

   .. note::
      Las siguientes mediciones se harán fijando las fuentes de voltaje en 5.0 V, [#f2]_

   #. Utilice el montaje experimental :numref:`fig:Setup_02` y con terminal libre el voltímetro determine la familia de equipotenciales correspondientes a -5 V, -4 V, -3 V, -2 V, -1 V, 0 V, +1 V, +2 V, +3 V, +4 V y +5 V. Para cada línea equipotencial tome por lo menos 8 puntos con separaciones de aproximadamente 1 cm y una estos puntos con una línea continua. En total deben aparecer 11 líneas continuas. Una vez trazadas las líneas equipotenciales construya las líneas de campo eléctrico y determine las zonas donde el campo eléctrico toma el mayor valor.
   #. Usando la misma configuración anterior, coloque un cuadrado conductor en el centro de los electrodos y determine las nuevas líneas equipotenciales, ver :numref:`fig:Setup_03`. En particular determine las equipotenciales dentro y fuera del cuadrado. Determine la línea de campo eléctrico y el campo mismo sobre la superficie de los conductores.
   #. Utilice un montaje similar al usado en el inciso 1. Determine el potencial para todos los puntos de la cubeta usando un reticulado de aproximadamente 1 cm de lado. Represente los datos en una matriz bidimensional y realice una representación gráfica de los mismos. Calcule el potencial por el método de relajación discutido arriba. Represente los resultados numéricos usando el mismo criterio que el usado para representar los datos experimentales. Compare sus mediciones con la solución numérica.
   #. Repita el procedimiento del inciso 3, excepto que ahora debe tomar una cualquiera de las configuraciones mostradas en la :numref:`fig:Setup_04` y la :numref:`fig:Setup_05`.

.. figure:: /images/Electromagnetismo/Equipotentials/Equipotentials_03b.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:Setup_03

   Montaje experimental.

.. figure:: /images/Electromagnetismo/Equipotentials/Equipotentials_04.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:Setup_04

   Montaje experimental.

.. figure:: /images/Electromagnetismo/Equipotentials/Equipotentials_05.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:Setup_05

   Montaje experimental.


.. [#f2] Para prevenir la electrólisis, que alteraría las propiedades químicas del medio con el tiempo, se recomienda no matener encendida las fuentes por más de 30 minutos. Con cada nuevo experimento que realice cambie el agua por agua destilada fresca.
.. [#f3] *Experimental study of the Neumann and Dirichlet boundary conditionsin two-dimensional electrostatic problems*, Am. J. Phys., Vol. 70, No. 12, December 2002.
.. [#f4] Descarga de archivos: :download:`Relaxation.Zip <Downloadables/Relaxation/Relaxation.zip>`.









