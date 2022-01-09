Movimiento de partículas en un campo magnético
================================================

**Objetivo**

El propósito de esta práctica es determinar los factores que afectan la trayectoria de una partícula cargada cuando se mueve en un campo magnético.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://www.thephysicsaviary.com/Physics/Programs/Labs/ChargeinMagFieldLab/ <http://www.thephysicsaviary.com/Physics/Programs/Labs/ChargeinMagFieldLab/>`_.

**Resumen teórico**

Cuando una partícula con carga electrica :math:`q`, masa :math:`m` y velocidad :math:`\overrightarrow{v}`  se mueve en una zona del espacio donde existe un campo magnético :math:`\overrightarrow{B}`, ésta experimenta una fuerza denominada fuerza magnética dada por la expresión

.. math::
   :label: Ec:Mov_q_B_01

   \begin{equation}
    \overrightarrow{F}=q\overrightarrow{v}\times \overrightarrow{B}
   \end{equation}

La fuerza magnética posee las siguientes características:

   #. es perpendicular al plano que contiene los vectores :math:`\overrightarrow{v}` y :math:`\overrightarrow{B}` y su dirección está determinada por la regla de la mano derecha o regla del tirabuzón.
   #. es nula si la partícula es neutra, tiene la misma dirección de :math:`\overrightarrow{v}\times\overrightarrow{B}` para :math:`q>0` y dirección opuesta si :math:`q<0`.
   #. no realiza trabajo sobre la carga eléctrica, lo que implica que su rapidez y en consecuencia su energía cinética no se alteran.
   #. para el caso particular cuando el campo magnético :math:`\overrightarrow{B}` es uniforme y la velocidad :math:`\overrightarrow{v}` es perpendicular a :math:`\overrightarrow{B}`, es decir, :math:`\overrightarrow{v}\perp \overrightarrow{B}`, la partícula describe una trayectoria circular con rapidez constante.

Dado que la fuerza magnética implica el uso de una representación tridimensional para visualizar las direcciones de los vectores que en ella intervienen, es necesario definir una convención simbólica para representar las líneas de fuerza de un campo perpendicular a la superficie sobre la que escribimos. Para ello se representa el campo magnético saliente con círculos y el entrante con equis, tal y como se muestra en la :numref:`Fig:convention`.

.. figure:: /images/Electromagnetismo/Move_q_B/convention_B.png
   :scale: 80
   :align: center
   :name: Fig:convention

   :math:`\circ`: campo magnético perpendicular y saliendo del plano de la página, \texttt{x}: campo magnético perpendicular y entrando al plano de la página


**Descripción de la interfaz de la aplicación**

La :numref:`setup_01` muestra la interfaz gráfica del usuario que permite estudiar los factores que afectan la trayectoria de una partícula cargada cuando se mueve en un campo magnético de manera perpendicular. Desde la interfaz se pueden seleccionar los valores de la rapidez de la partícula en el rango comprendido entre 50 y 400 km/s, la magnitud del campo magnético entre 0 y 400 mT y la masa de la partícula entre 1 y 20 unidades de masa atómica (amu) con los botones de color rojo, azul y verde en forma de flecha ubicados en la parte inferior de la interfaz. Las flechas pequeñas permiten hacer variaciones finas. El signo de la carga (+ o -), dirección del campo (:math:`\circ` o \textbf{\texttt{x}}) y la magnitud de la carga en múltiplos enteros de la carga del electrón se cambian al presionar con el ratón los rótulos llamados \textbf{Charge is}, \textbf{B field is}, \textbf{Magnitud of charge is} respectivamente. Al presionar con el ratón, el rótulo llamado \textbf{Grid is} se activa o desactiva una grilla con resolución de 1 mm. Finalmente, al presionar el botón \textbf{Fire} ubicado en la parte superior izquierda de la interfaz, por la parte izquierda de la interfaz ingresa una partícula con los parámetros establecidos previamente y el simulador mide el tiempo en milisegundos que la partícula dura moviéndose en el campo magnético.

.. figure:: /images/Electromagnetismo/Move_q_B/gui_01.png
   :scale: 100
   :align: center
   :name: setup_01

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

**Variación de la velocidad**

   #. Fije valores que desee para la carga, masa y campo magnético. De igual manera el tipo de carga y dirección del campo magnético. No cambie estos valores para esta parte del laboratorio.
   #. Selecione dos velocidades: una muy grande y otra muy pequeña. Dispare la partícula para estas velocidades y asegúrese de que la partícula describa la semicircunferencia más grande posible que se pueda observar. Si no es así, ajuste los anteriores parámetros para que la trayectoria semicircular se pueda visualizar para todo el rango de velocidades que usará.
   #. Una vez que esté seguro de que el rango de velocidades que está examinando funciona, registre todas las cantidades anteriores para esta parte del laboratorio.
   #. Construya una tabla donde liste las velocidades que utilizará, el tiempo de viaje y el radio de la semicircunferencia. Debe considerar 8 velocidades diferentes.
   #. Construya gráficos de radio en función de la velocidad y tiempo en función de la velocidad. A partir de las gráficas y de sus conocimientos sobre linealización de funciones encuentre las ecuaciones que relacionan estas variables.


**Variación de la carga**

   #. Fije valores que desee para la velocidad, la masa y el campo magnético. De igual manera el tipo de carga y dirección del campo magnético. No cambie estos valores para esta parte del laboratorio.
   #. Antes de recopilar datos, asegúrese de que la combinación de parámetros le permita recopilar datos para todos los posibles valores de carga que utilizará. Establezca la carga en 1e y dispárela. Si el círculo que describe la carga no cabe en el área de visualización, ajuste los parámetros hasta que pueda ver el arco completo de la partícula con carga 1e.
   #. Una vez que esté seguro de que el rango de cargas que está examinando funciona, registre todas las cantidades para esta parte del laboratorio.
   #. Cree una tabla donde liste las cargas que utilizará, el tiempo de viaje y el radio de la semicircunferencia. Considere 8 cargas diferentes.
   #. Construya gráficos de radio en función de la carga y tiempo en función de la carga. A partir de las gráficas y de sus conocimientos sobre linealización de funciones encuentre las ecuaciones que relacionan estas variables.

**Variación de la masa**


   #. Fije valores que desee para la carga, la velocidad y el campo magnético. De igual manera el tipo de carga y dirección del campo magnético. No cambie estos valores para esta parte del laboratorio.
   #. Selecione dos masas: una muy grande y otra muy pequeña. Dispare la partícula para estas masas y asegúrese de que su partícula no salga del rango de prueba. Si es así, ajuste los anteriores parámetros para que la trayectoria semicircular de la partícula se pueda visualizar para todo el rango de masas que usará.
   #. Una vez que esté seguro de que el rango de masas que está examinando funciona, registre todas las cantidades para esta parte del laboratorio.
   #. Cree una tabla donde liste las masas que utilizará, el tiempo de viaje y el radio de la semicircunferencia. Considere 8 masas diferentes.
   #. Construya gráficos de radio en función de la masa y tiempo en función de la masa.  A partir de las gráficas y de sus conocimientos sobre linealización de funciones encuentre las ecuaciones que relacionan estas variables.

**Variación del campo magnético**

   #. Fije valores para la carga, velocidad, masa, tipo de carga y dirección de campo que desee. No los cambie para esta parte del laboratorio.
   #. Selecione dos valores de campo magnético: un valor grande y otro muy pequeño. Dispare la partícula para estas intensidades de campo y asegúrese de que su partícula no salga del rango de prueba. Si no es así, ajuste los anteriores parámetros para que la trayectoria semicircular se pueda visualizar para todo el rango de intensidades que usará.
   #. Una vez que esté seguro de que el rango de intensidades de campo que está examinando funciona, registre todas las cantidades para esta parte del laboratorio.
   #. Cree una tabla donde liste las intensidades de campo que utilizará, el tiempo de viaje y el radio de la semicircunferencia. Debe considerar 8 intensidades de campo diferentes.
   #. Construya gráficos de radio en función de la fuerza y tiempo en función de la fuerza. A partir de las gráficas encuentre las ecuaciones que relacionan estas variables.


**Análisis y preguntas**

Teniendo en cuenta los resultados de los cuatro apartados anteriores escriba:

   #. Una ecuación que relacione las magnitudes de la fuerza magnética, con la velocidad, la carga y la intensidad del campo magnético.
   #. Una ecuación que relacione el radio de la semicircunferencia con la masa, la velocidad, la carga y la intensidad del campo magnético.
   #. ¿Cómo se pueden utilizar los resultados de esta experiencia para determinar el signo de las partículas cargadas eléctricamente de manera experimental?
   #. ¿Cómo funciona un espectrómetro de masas?
   #. ¿Qué son los cinturones de Van Allen? ¿De qué nos protegen? ¿Dónde están ubicados? ¿Por qué en la zona ecuatorial no se tiene algo parecido?



