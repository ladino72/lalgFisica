Movimiento de un electrón en un campo eléctrico
=================================================

**Objetivo**

El propósito de esta práctica es determinar el efecto del campo eléctrico en el movimiento de una partícula cargada.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.thephysicsaviary.com/Physics/Programs/Labs/AcceleratingChargesWithCapacitor/ <https://www.thephysicsaviary.com/Physics/Programs/Labs/AcceleratingChargesWithCapacitor/>`_.

**Resumen teórico**

Cuando una partícula con carga eléctrica :math:`q`, se encuentra ya sea en reposo o en movimiento en una zona del espacio donde existe un campo eléctrico :math:`\overrightarrow{E}`, ésta experimenta una fuerza eléctrica dada por la expresión

.. math::
   :label: F_mag_01

   \begin{equation}
    \overrightarrow{F}=q \overrightarrow{E}
   \end{equation}

La fuerza eléctrica posee las siguientes características:

   #. es nula si la partícula es neutra, tiene la misma dirección de :math:`\overrightarrow{E}` si :math:`q>0` y dirección opuesta si :math:`q<0`.
   #. en general realiza trabajo sobre la carga eléctrica, lo que implica que su rapidez y en consecuencia su energía cinética se altera.
   #. para el caso particular cuando el campo eléctrico :math:`\overrightarrow{E}` es uniforme y la velocidad inicial :math:`\overrightarrow{v_0}` de la partícula es paralela a :math:`\overrightarrow{E}`, ésta describe una trayectoria rectilínea con aceleración uniforme.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Mov_q_E_1D_01` muestra la interfaz gráfica del usuario que permite estudiar los factores que afectan la dinámica de un electrón cuando se mueve de manera paralela a la dirección de un campo eléctrico uniforme. Desde la interfaz se puede seleccionar el valor de la diferencia de potencial aplicada a un par de placas paralelas a través de la fuente de voltaje en el rango comprendido entre 0 y 800 V. De igual manera la distancia de separación entre las placas se puede variar en el rango comprendido entre 15 mm y 60 mm. La aplicación cuenta con un medidor de tiempo, el cual mide el tiempo (en nano segundos) gastado por el electrón en ir de la placa izquierda a la derecha desde el momento de liberación al presionar el botón **Fire**. Cambios a la diferencia de potencial y distancia de separación entre placas es solo es posible después de presionar el botón **Reset**.

.. figure:: /images/Electromagnetismo/Move_q_E_1D/gui_01_mov_q_in_E.png
   :scale: 50
   :align: center
   :name: fig:Mov_q_E_1D_01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**


**Variación de la diferencia de potencial**

   #. Fije la distancia de separación entre las placas en :math:`d=20\,\text{mm}`.
   #. Aplique diferencias de potencial :math:`V` entre las placas y mida los corespondientes tiempo :math:`t_v` de viaje del electrón de una placa a la otra. Registre sus mediciones en la :numref:`tab:mov_q_in_E_01`.
   #. Construya la gráfica de tiempo de viaje :math:`t_v` en función de la diferencia de potencial :math:`V` aplicada a las placas. A partir de la gráfica y de sus conocimientos sobre linealización de funciones encuentre las ecuaciones que relacionan estas variables.
   #. Repita los procedimientos de los incisos 2 y 3  pero esta vez con :math:`d=50\,\text{mm}`.  Registre sus mediciones en la :numref:`tab:mov_q_in_E_02`. ¿Se mantiene la dependencia entre :math:`t_v` y :math:`V`?

      .. csv-table:: Diferencias de potencial :math:`V` y tiempos de vuelo :math:`t_v`, :math:`d=20\,\text{mm}`
         :header: ":math:`V` (V)", ":math:`t_v` (ns)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:mov_q_in_E_01
         :align: center

         0,
         100,
         200,
         300,
         400,
         500,
         600,
         700,
         800,

      .. csv-table:: Diferencias de potencial :math:`V` y tiempos de vuelo :math:`t_v`, :math:`d=50\,\text{mm}`
         :header: ":math:`V` (V)", ":math:`t_v` (ns)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:mov_q_in_E_02
         :align: center

         0,
         100,
         200,
         300,
         400,
         500,
         600,
         700,
         800,


**Variación de la distancia entre las placas**

   #. Fije la diferencia de potencial entre las placas en :math:`V=200\,\text{V}`.
   #. Varíe la distancia entre las placas y mida los correspondientes tiempos :math:`t_v` de viaje del electrón de una placa a la otra. Registre sus mediciones en la :numref:`tab:mov_q_in_E_03`.
   #. Construya la gráfica de tiempo de viaje :math:`t_v` en función de la distancia de separación :math:`d` entre las placas. A partir de la gráfica y de sus conocimientos sobre linealización de funciones encuentre las ecuaciones que relacionan estas variables.
   #. Repita los procedimientos de los incisos 1, 2 y 3 pero esta vez con :math:`V=700\,\text{V}`.  Registre sus mediciones en la :numref:`tab:mov_q_in_E_04`. ¿Se mantiene la dependencia entre :math:`t_v` y :math:`d`?

      .. csv-table:: Distacia de separación :math:`d` entre placas y tiempos de viaje :math:`t_v`, :math:`V=200\,\text{V}`
         :header: ":math:`d` (mm)", ":math:`t_v` (ns)"
         :widths: 1,1
         :width: 16 cm
         :name: tab:mov_q_in_E_03
         :align: center

         15,
         20,
         25,
         30,
         35,
         40,
         45,
         50,
         55,
         60,

      .. csv-table:: Distacia de separación :math:`d` entre placas y tiempos de viaje :math:`t_v`, :math:`V=700\,\text{V}`
         :header: ":math:`d` (mm)", ":math:`t_v` (ns)"
         :widths: 1,1
         :width: 16 cm
         :name: tab:mov_q_in_E_04
         :align: center

         15,
         20,
         25,
         30,
         35,
         40,
         45,
         50,
         55,
         60,

**Análisis y preguntas**

Teniendo en cuenta los resultados de los dos apartados anteriores:
   #. Escriba una ecuación que relacione la diferencia de potencial :math:`V` aplicada a las placas, distancia de separación :math:`d` entre las placas y tiempo de viaje :math:`t_v`.
   #. Escriba una ecuación que relacione el campo eléctrico :math:`E` con la diferencia de potencial :math:`V` entre las placas.
   #. Escriba una ecuación que relacione la distancia :math:`x` recorrida por el electrón en función del tiempo.
   #. Escriba una ecuación que relacione la velocidad del electrón con la diferencia de potencial.
   #. ¿Cómo se pueden utilizar los resultados de esta experiencia para determinar el signo de las partículas cargadas eléctricamente de manera experimental?
   #. ¿Cómo funciona un espectrómetro de masas?
   #. ¿Qué son los cinturones de Van Allen? ¿De qué nos protegen? ¿Dónde están ubicados? ¿Por qué en la zona ecuatorial no se tiene algo parecido?





