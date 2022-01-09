Experimento de Millikan
========================

**Objetivo**

El propósito de esta práctica es estudiar la cuantización de la carga eléctrica a través del experimento de Millikan.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://www.thephysicsaviary.com/Physics/Programs/Labs/MillikanOilDropLab/index.html <http://www.thephysicsaviary.com/Physics/Programs/Labs/MillikanOilDropLab/index.html>`_.

.. index:: Millikan

**Resumen teórico**

Cuando una partícula de carga eléctrica :math:`q` se encuentra en presencia de un campo eléctrico :math:`\overrightarrow{E}`, esta experimenta una fuerza igual a :math:`\overrightarrow{F}=q\overrightarrow{E}`. Si la carga es positiva la dirección de la fuerza va en la misma dirección del campo eléctrico, mientras que si es negativa la fuerza va en dirección opuesta. La :numref:`Fig:Millikan_01` muestra una partícula con carga :math:`q` y masa :math:`m` en equilibrio en presencia de dos campos: el campo gravitacional y un campo eléctrico :math:`\overrightarrow{E}` uniforme creado por un par de placas metálicas paralelas separadas una distancia :math:`d` a las cuales se les aplica una diferencia de potencial :math:`V` mediante una batería. La relación entre :math:`E` y :math:`V` es :math:`E=\frac{V}{d}`. Dado que la partícula se encuentra en equilibrio se cumple:

.. figure:: /images/Electromagnetismo/Millikan_Experiment/Millikan_01.png
   :scale: 100
   :align: center
   :name: Fig:Millikan_01

   Fuerzas sobre una partícula en equilibrio de masa :math:`m` y carga :math:`q` en presencia de dos campos: eléctrico y gravitacional

.. math::
   :label: Millikan_Ec_01

   \begin{equation}
    mg=qE=q\frac{V}{d}
   \end{equation}

**Descripción de la interfaz de la aplicación**

La :numref:`Fig:Gui_Millikan_01` muestra la interfaz gráfica del usuario que permite estudiar la cuantización de la carga eléctrica. La interfaz consta de un sistema de placas metálicas paralelas (capacitor) separadas una distancia :math:`d=3.0\,\text{mm}`, a las cuales se les aplica una diferencia de potencial eléctrico :math:`V`; la placa superior se encuentra a mayor potencial que la placa inferior (la placa superior es positiva y la inferior es negativa). Mediante el atomizador de aceite se inyectan pequeñas gotas de aceite al espacio comprendido entre las placas. La inyección de gotas se realiza al hacer clic con el puntero del ratón sobre la perilla redonda del atomizador. Las micro gotas al pasar por la boquilla metálica del atomizador se cargan negativamente. Tan pronto se realiza la inyección algunas micro gotas se mueven hacia arriba mientras que otras caen; solamente quedan suspendidas o levitando aquellas donde se cumple que la fuerza eléctrica es igual a la fuerza gravitacional. La aplicación muestra solo una gota suspendida de las múltiples posibles. Al hacer clic sobre el microscopio, se observa la ampliación de la gota (color naranja) y es posible medir su radio en nanómetros (nm). La densidad del aceite usado en el atomizador es :math:`\rho=900\,\text{kg/m}^{3}`. Hecha la medición del radio, se regresa a la interfaz principal al hacer clic sobre el botón **Return main**. Cada vez que se inyectan gotas aparece una lectura diferente de la diferencia de potencial entre las placas.

.. figure:: /images/Electromagnetismo/Millikan_Experiment/Gui_Millikan_01.png
   :scale: 80
   :align: center
   :name: Fig:Gui_Millikan_01

   Sistema utilizado para realizar el experimento de Millikan

**Mediciones y procedimientos**

   #. Inyecte gotas de aceite entre las placas del capacitor. Cuando encuentre una gota que quede en reposo (levitando) entre las placas, use su lupa para determinar su radio lo más exactamente posible. De igual manera registre el valor de la diferencia de potencial para el cual se logra el equilibrio de la gota. Registre sus mediciones en la :numref:`tab:Millikan_V_v_r`.

      .. csv-table:: Datos simulados para determinar el valor de la carga elemental
         :header: "Radio, :math:`r` (mm)", "Dif.de pot., :math:`V` (V)", "Carga :math:`q` (C)", ":math:`\\frac{q}{|e|}`"
         :widths: 1,1,1,1
         :width: 16 cm
         :name: tab:Millikan_V_v_r
         :align: center

         . , ., .,.
         . , ., .,.
         . , ., .,.
         . , ., .,.
         . , ., .,.
         . , ., .,.

   #. Repita el procedimiento del inciso 1 varias veces hasta completar las dos primeras columnas de la :numref:`tab:Millikan_V_v_r`.
   #. Use la ecuación :eq:`Millikan_Ec_01` para demostrar que la carga de la gota de aceite es

      .. math::
         :label: Millikan_Ec_02

         \begin{equation}
          q=\frac{4\rho\pi r^{3}gd}{3V}
         \end{equation}

   #. A partir de los datos obtenidos en la :numref:`tab:Millikan_V_v_r` encuentre la carga :math:`q` de la gota en cada caso y escriba sus resultados en la tercera columna de la :numref:`tab:Millikan_V_v_r`.
   #. Divida cada una de la entradas de la columna 3 de la :numref:`tab:Millikan_V_v_r` entre el valor absoluto de la carga del electrón :math:`|e|=1.6\times 10^{-19}\,\text{C}` y escriba sus resultados en la cuarta columna de la :numref:`tab:Millikan_V_v_r`.


**Análisis y preguntas**

   #. Si los resultados obtenidos en la cuarta columna de la :numref:`tab:Millikan_V_v_r` se aproximan a números enteros, ¿qué se puede concluir?
   #. ¿Qué tiene que ver lo anterior con lo que se llama cuantización de la carga eléctrica?
   #. ¿Qué demuestra este experimento y por qué es tan importante?
   #. El experimento realizado con la simulación es una versión simplificada del experimento real realizado por Robert Millikan y Harvey Fletcher en 1911. Investigue como se realizó este experimento y compárelo con el que usted acaba de realizar.


