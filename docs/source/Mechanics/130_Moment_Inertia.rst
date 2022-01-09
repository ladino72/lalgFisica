+Momento de inercia de un disco
================================

**Objetivo**

El propósito de esta práctica es doble:

   #. determinar experimentalmente el valor del momento de inercia :math:`I` de un disco homogéneo con respecto a un eje perpendicular a su superficie y que pasa por su centro.
   #. hallar el valor del torque :math:`\tau` ejercido por la fuerza de rozamiento  sobre el eje. Para ello, se enrolla un hilo muy delgado sobre el disco, de cuyo otro extremo pende un cuerpo; al descender éste último el disco gira y se mide su aceleración tangencial en función del peso del cuerpo que pende. A partir de estas mediciones y junto con el modelo dinámico propuesto se determinan los valores de :math:`I` y :math:`\tau`.

**Recursos**


   #. Un disco de acrílico transparente.
   #. Un juego de pesas.
   #. Un trozo de hilo de coser.
   #. Una balanza.
   #. Un fotointerruptor conectado al computador mediante una interfase para la medición de tiempos.
   #. Una regla graduada en mm.
   #. Un pedazo de cinta para asegurar el hilo al disco.


**Resumen teórico**

La segunda ley de Newton aplicada a la rotación de un sólido establece que la tasa de cambio de la  cantidad de movimiento angular de un sistema es igual al momento de fuerza o torque neto :math:`\overrightarrow{\tau}` que actúa sobre el
sistema. Explicitamente, :math:`\overrightarrow{\tau}=\frac{d\overrightarrow{L}}{dt}`, donde :math:`\overrightarrow{L}` es la cantidad de movimiento angular sistema. Si :math:`\overrightarrow{L}` y :math:`\overrightarrow{\omega}` son paralelos, es decir, :math:`\overrightarrow{L}=I\overrightarrow{\omega}`, siendo :math:`I` el momento de inercia se tiene :math:`\overrightarrow{\tau}=\frac{d(I\overrightarrow{\omega}%
)}{dt}=I\overrightarrow{\alpha}`, donde :math:`\overrightarrow{\alpha}=\frac{d\overrightarrow{\omega}}{dt}` es la aceleración angular del sistema. En otras palabras la aceleración angular del sistema es proporcional al momento de fuerza o torque neto aplicada al mismo.

**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:moment_Inertia_01`. Supongamos que el sistema está en movimiento. La :numref:`fig:moment_Inertia_02` muestra las fuerzas que actúan sobre la polea y la masa el cuerpo colgante. Al aplicar la segunda ley de Newton al cuerpo de masa :math:`m` resulta


.. math::
   :label: Ec:M_of_I2.1

   \begin{equation}
    mg-T=ma
   \end{equation}

.. figure:: /images/Mecanica/Moment_Inertia/moment_Inertia_01.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:moment_Inertia_01

   Sistema compuesto por un disco de masa :math:`m` y un cuerpo de masa :math:`m` que pende de un hilo delgado.


.. figure:: /images/Mecanica/Moment_Inertia/moment_Inertia_02.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:moment_Inertia_02

   Fuerzas sobre la polea (no se muestra la fuerza de rozamiento), y el cuerpo colgante de masa :math:`m`.


donde :math:`a`  representa la aceleración con la cuel desciende el cuerpo. Similarmente, aplicando la segunda ley de Newton a la polea que rota resulta

.. math::
   :label: Ec:M_of_I2.2

   \begin{equation}
   TR-\tau=I\alpha =I\frac{a}{R}
   \end{equation}

donde los torques se han medido con respecto al punto :math:`o`, :math:`I` es el momento de inercia de la polea, :math:`\alpha`  su aceleración angular y :math:`\tau` es el torque  ejercido por la fuerza de rozamiento. El peso de la polea :math:`mg` y la fuerza :math:`f` que ejerce su eje no producen torque. La relación entre la aceleración lineal :math:`a` y angular :math:`\alpha` es dada por la expresión :math:`a=\alpha R`.
De las expresiones :eq:`Ec:M_of_I2.1` y :eq:`Ec:M_of_I2.2` se obtiene

.. math::
   :label: Ec:M_of_I2.3

   \begin{equation}
    m(g-a)R=\frac{I}{R}a+\tau
   \end{equation}

La ecuación :eq:`Ec:M_of_I2.3` de puede reescribir de modo que tome la forma de la ecuación de una línea recta :math:`Y=nX+b`, con pendiente :math:`n` y punto de corte con el eje :math:`y` igual a :math:`b`, ver :numref:`fig:moment_Inertia_03`. Así si,

.. figure:: /images/Mecanica/Moment_Inertia/moment_Inertia_03.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:moment_Inertia_03

   Relación lineal entre las variables :math:`Y` y :math:`X`.


.. math::
   :label: Ec:M_of_I2.4

   \begin{equation}
    Y=IX+\tau
   \end{equation}

donde :math:`Y=m(g-a)R`, :math:`X=\frac{a}{R}` y

.. math::
   :label: Ec:M_of_I2.5

   \begin{equation}
   n=I
   \end{equation}

.. math::
   :label: Ec:M_of_I2.6

   \begin{equation}
    b=\tau  
   \end{equation}

**Mediciones**

Para la determinación del momento de inercia del disco y el torque debido a la fricción se utilizará el equipo mostrado en la :numref:`fig:moment_Inertia_04`. Este montaje consta de una disco que puede girar sobre un eje horizontal, un juego de pesas pequeñas de valores aproximadamente iguales a 5 g, 7 g, 9 g, 11 g, 13 g, 15 g, 17 g, 19 g, 21 g, 25 g [#f2]_; y un fotosensor. El disco posee una pequeña canal en su periferia sobre la cual se puede enrollar un hilo muy delgado.

.. figure:: /images/Mecanica/Moment_Inertia/moment_Inertia_04.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:moment_Inertia_04

   Montaje experimental usado para determinar :math:`I` y :math:`\tau`


El fotosensor  contiene un infrarrojo el cual es interrumpido por las franjas oscuras dispuestas de manera radial e igualmente espaciadas sobre la superficie del disco, ver :numref:`fig:moment_Inertia_05`. El haz infrarrojo al ser interrupido, el hardware procesa una señal eléctrica y envía al computador información que el software *CHRONOS* [#f3]_ utiliza para el cálculo de la rapidez de un punto del disco.


Para cada de las masas suministradas determine el valor de su aceleración de descenso. Para ello, enrolle el hilo dos o tres vueltas sobre la periferia del disco y por el otro extremo del hilo suspenda una de las masas. Deje que la masa descienda y mida el valor de la rapidez media :math:`\overline{v}` de los puntos del disco que ese encuentran a una distancia  :math:`r_2=45\,\text{mm}` del centro del disco como función del tiempo mediante el uso de *CHRONOS* operando en modo 2. Complete las tablas de datos :numref:`tab:a1a2`, :numref:`tab:a3a4`, :numref:`tab:a5a6`, :numref:`tab:a7a8` y :numref:`tab:a9a10`.  De la gráfica de :math:`\overline{v}` en función del tiempo determine la aceleración :math:`a'` de estos puntos. Note que el valor de la aceleración :math:`a` de los puntos de la periferia del disco (igual a la aceleración del cuerpo que pende) está relacionada con :math:`a'` mediante la expresión

.. math::
   :label: Ec:M_of_I2.7

   \begin{equation}
    a=\frac{R}{r_2}=\frac{55\,\text{mm}}{45\,\text{mm}}a'=\frac{11}{9}a'
   \end{equation}

Con la información extraída de las tablas de datos :numref:`tab:a1a2`, :numref:`tab:a3a4`, :numref:`tab:a5a6`, :numref:`tab:a7a8`, :numref:`tab:a9a10` y la ecuación :eq:`Ec:M_of_I2.7` complete la tabla :numref:`tab:ace`.

Ahora que se tienen los valores de aceleración para cada una de las masas complete la :numref:`tab:YX` y construya la gráfica de :math:`Y` como función de :math:`X`. De la gráfica obtenida y a partir de las ecuaciones :eq:`Ec:M_of_I2.5` y :eq:`Ec:M_of_I2.6` determine los valores de :math:`I` y :math:`\tau` .

Compare el valor de :math:`I` obtenido de manera indirecta via experimento con el valor teórico calculado a través de la expresión :math:`I=\frac{1}{2}mR^{2}` con :math:`m=0.106\,\text{kg}` y :math:`R=55\times10^{-3}\,\text{m}`, es decir, :math:`I=1.6\times10^{-4}\,\text{kgm}^{2}`
Discuta sus resultados.

.. figure:: /images/Mecanica/Moment_Inertia/moment_Inertia_06.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:moment_Inertia_05

   Diagrama del disco con sus dimensiones relevantes.


.. csv-table:: Datos para determinar :math:`a_1` y :math:`a_2` para :math:`m_1=_{........}` kg y :math:`m_2=_{........}` kg
   :header: ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v} \\,(\\text{m/s})`", ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v}\\,(\\text{m/s})`"
   :widths: 1,1,1,1,1,1
   :width: 15 cm
   :name: tab:a1a2
   :align: center

   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.

.. csv-table:: Datos para determinar :math:`a_3` y :math:`a_4` para :math:`m_3=_{........}` kg y :math:`m_4=_{........}` kg
   :header: ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v} \\,(\\text{m/s})`", ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v}\\,(\\text{m/s})`"
   :widths: 1,1,1,1,1,1
   :width: 15 cm
   :name: tab:a3a4
   :align: center

   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.

.. csv-table:: Datos para determinar :math:`a_5` y :math:`a_6` para :math:`m_5=_{........}` kg y :math:`m_6=_{........}` kg
   :header: ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v} \\,(\\text{m/s})`", ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v}\\,(\\text{m/s})`"
   :widths: 1,1,1,1,1,1
   :width: 15 cm
   :name: tab:a5a6
   :align: center

   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.

.. csv-table:: Datos para determinar :math:`a_7` y :math:`a_8` para :math:`m_7=_{........}` kg y :math:`m_8=_{........}` kg
   :header: ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v} \\,(\\text{m/s})`", ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v}\\,(\\text{m/s})`"
   :widths: 1,1,1,1,1,1
   :width: 15 cm
   :name: tab:a7a8
   :align: center

   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.


.. csv-table:: Datos para determinar :math:`a_9` y :math:`a_{10}` para :math:`m_9=_{........}` kg y :math:`m_{10}=_{........}` kg
   :header: ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v} \\,(\\text{m/s})`", ":math:`t \\text{(ms)}`", ":math:`\\Delta t \\,(\\text{ms})`", ":math:`\\overline{v}\\,(\\text{m/s})`"
   :widths: 1,1,1,1,1,1
   :width: 15 cm
   :name: tab:a9a10
   :align: center

   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.
   .,.,.,.,.,.


.. csv-table:: Aceleraciones :math:`a_1.....a_{10}` de las masas colgantes :math:`m_1.....m_{10}` respectivamente
   :header: ":math:`m \\,\\text{(kg)}`", ":math:`a \\,(\\text{m/s}^{2})`"
   :widths: 1,1
   :width: 10 cm
   :name: tab:ace
   :align: center

   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.

.. csv-table:: Datos para la contrucción de la gráfica de :math:`Y` en función de :math:`X`.
   :header: ":math:`Y=m(g-a)R\\,\\,\\text{(J)}`", ":math:`X\\,\\,(\\text{s}^{-2})`"
   :widths: 1,1
   :width: 12 cm
   :name: tab:YX
   :align: center

   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.

.. [#f2] Confirme los valores de las masas con la balanza suministrada y haga las correcciones pertinentes.
.. [#f3] *CHRONOS* se encuentra instalado en el computador de cada mesa de trabajo. Usted puede medir el valor de la aceleración de la misma manera que lo hizo cuando realizó las prácticas de la medición de la gravedad y leyes de Newton.