Segunda ley de Newton
======================

**OBJETIVO**

El propósito de esta práctica es estudiar y analizar la segunda ley de Newton.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `{https://www.walter-fendt.de/html5/phen/newtonlaw2_en.htm <{https://www.walter-fendt.de/html5/phen/newtonlaw2_en.htm>`_.

**Resumen teórico**

La segunda ley de Newton establece \ que la rata de cambio de momentum de un
sistema es igual a la fuerza neta :math:`\overrightarrow{F}` que actua sobre el
sistema. Explícitamente, :math:`\overrightarrow{F}=\frac{d\overrightarrow{p}}{dt}`, donde :math:`\overrightarrow{p}` es el momentum del sistema. Si la masa :math:`m` del
sistema es constante entonces :math:`\overrightarrow{F}=\frac{d(m\overrightarrow{v})}{dt}=m\overrightarrow{a}`, donde :math:`\overrightarrow{a}=\frac{d\overrightarrow{v}}{dt}` es la aceleración del cuerpo. En otras palabras la
aceleración del sistema es proporcional a la fuerza aplicada al mismo.

**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:new1fig4`. Supongamos que el sistema está en movimiento y
que existe una fuerza de rozamiento :math:`f` entre la mesa y el bloque de masa :math:`M`. Además, consideremos que la polea tiene masa despreciable. La :numref:`fig:new1fig3` muestra las fuerzas que actuan sobre cada uno de los bloques. Usando la segunda ley de Newton a los dos bloques de masas :math:`M` y :math:`m` resulta

.. math::
   :label: Ec:Newton_2_Law.1

   \begin{equation}
    T-f=Ma
   \end{equation}

.. math::
   :label: Ec:Newton_2_Law.2

   \begin{equation}
    mg-T=ma
   \end{equation}

.. figure:: /images/Mecanica/Newton_1/new1fig4.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:new1fig4

   Sistema compuesto por dos bloques de masas :math:`M` y :math:`m`


.. figure:: /images/Mecanica/Newton_1/new1fig3.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:new1fig3

   Fuezas sobre los bloques de masas :math:`M` y :math:`m`, la polea tiene masa despreciable.

donde :math:`a` representa la aceleración de los bloques. Obsérvese, que la
tensión de la cuerda es la misma en todos sus puntos.

De las  expresiones :eq:`Ec:Newton_2_Law.1`, :eq:`Ec:Newton_2_Law.2` se obtiene

.. math::
   :label: Ec:Newton_2_Law.4

   \begin{equation}
    a=\frac{g}{M_t}m-\frac{\mu Mg}{M_{t}}
   \end{equation}

donde :math:`M_t=m+M`

.. math::
   :label: Ec:Newton_2_Law.4a

   \begin{equation}
    M_t=m+M
   \end{equation}

Al despejar :math:`M` de la ecuación :eq:`Ec:Newton_2_Law.4a` y reemplazar su valor en la ecuación :eq:`Ec:Newton_2_Law.4` resulta

.. math::
   :label: Ec:Newton_2_Law.4b

   \begin{equation}
    a=\frac{g(1+\mu)}{M_t}m-\mu g
   \end{equation}

La expresión :eq:`Ec:Newton_2_Law.4b` permite determminar la acelaración de las masas en función de :math:`m`. Obsérvese que si :math:`M_t` se mantiene constante entonces la relación entre :math:`a` y :math:`m` es lineal.

El valor de la aceleración :math:`a` se obtiene directamente del simulador, valor que se obtiene de la curva de posición en función del tiempo.

**Descripción de la interfaz de la aplicación**


La :numref:`fig:Newton_2_Law_01` muestra la interfaz gráfica del usuario, que permite estudiar la segunda ley de Newton. La interfaz simula el movimiento de dos cuerpos conectados mediante una cuerda que pasa por una polea de masa despreciable y que no presenta fricción. Las masa del cuerpo que permanece sobre la mesa (*Mass of the  wagon*) es :math:`M`  y el que pende de la cuerda (*Hanging mass*) es :math:`m` ; estas masas se pueden fijar al escribir valores en las casillas de entrada ubicadas en el panel derecho de la interfaz. El coeficiente de rozamiento :math:`\mu` entre el cuerpo de masa :math:`M` y la superficie se puede variar en el rango comprendido entre 0 y 1.00. La fotocelda rotulada **LB** se puede desplazar de manera horizontal con el apuntador del ratón y esta registra el tiempo que gasta el cuerpo de masa :math:`M` desde que parte del reposo hasta que la interrumpe, este tiempo es registrado por el cronómetro en forma rectangular. Una vez que se han seleccionado los valores de :math:`M`, :math:`m` y :math:`\mu` apropiados y se ha fijado la posición de la fotocelda, al presionar el botón **Start** la animación comienza y esta se detiene después de que el cuerpo de masa :math:`M` ha recorrido una distancia de 1 m, es decir, cuando ha llegado al tope derecho de la mesa, en este momento se registra un punto de coordenadas (distancia, tiempo) en la gráfica de posición en función del tiempo. Al presionar el botón **Record data**, las coordenadas de este punto se registran la tabla rotulada **Data** ubicada en la parte inferior derecha de la interfaz. Si se quiere repetir la medida o cambiar la posición de la fotocelda se puede hacer y se está listo para seguir tomando datos. Al presionar, el botón *Reset*, la información contenida en la tabla se borra.

.. figure:: /images/Mecanica/Newton_1/Newton_1_gui_01.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:Newton_2_Law_01

   Interfaz gráfica del usuario


**Mediciones y procedimientos**

   #. Fije el valor del coeficiente de rozamiento por ejemplo 0.005 y los valores de :math:`M` y :math:`m` de modo que su suma sea contante, por ejemplo 100 gramos. Varíe el valor de :math:`m` y para cada valor registre el correspondiente valor de la aceleración en la :numref:`tab:second_newton_Law_01`.
   #. A partir de los datos obtenidos en el inciso 1, construya la gráfica de :math:`a` como función de :math:`m`. Si :math:`p_1` y :math:`b_1` representan la pendiente y punto de corte de la recta con el eje vertical compruebe que :math:`\mu=-\frac{b_1}{g}` y  :math:`M_t=\frac{g-b_1}{p_1}`.

.. csv-table:: Datos de la simulación.
         :header: ":math:`m` (g)", ":math:`a\, \text{m/s}^2`"
         :widths: 1,1
         :width: 12 cm
         :name: tab:second_newton_Law_01
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


**Análisis y Preguntas**

   #. ¿Por qué razón considera que esta simulación si verifica la segunda ley de Newton?
   #. Veamos el siguiente argumento dado por un estudiante, 'La segunda ley de Newton establece que :math:`F=ma`, luego si :math:`F` se duplica entonces la aceleración se duplica, por su puesto para el mismo valor de la masa', a lo cual su profesor responde: su argumento es correcto. Ahora el profesor pregunta: en la simulación utilizada, con coeficiente de rozamiento cero, :math:`M=100` g y :math:`m= 1` g el valor de :math:`a=0.097\,\text{m/s}^{2}`. Ahora, si suplicamos :math:`m`, es decir :math:`m=2` g, el valor obtenido es :math:`a=0.192\,\text{m/s}^{2}`; claramente se ha duplicado la fuerza sobre :math:`M` pero su aceleración no se ha duplicado exactamente! y es más, si :math:`m=3` g el valor de :math:`a=0.0286\,\text{m/s}^{2}`, el cual no se ha triplicado! ¿Significa esto que la segunda ley no se cumple?  o ¿significa esto que quien desarrolló la simulación se equivocó? ¿Qué tiene que responder el estudiante?
