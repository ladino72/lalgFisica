Versión moderna del teorema II de Galileo
============================================
**Objetivo**

El objetivo de esta actividad es estudiar una versión moderna del teorema IV de Galileo sobre el movimiento
uniformemente acelerado, tal como se encuentra en el tercer día de la obra
\" *Discourses and Mathematical Demonstrations Relating to Two New Sciences* \" de Galileo [#f1]_

.. _GalileoIIRec:

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.geogebra.org/m/kqRFm4vW <https://www.geogebra.org/m/kqRFm4vW>`_.

**Situación**

La :numref:`GalileoII` muestra un plano que tiene longitud :math:`L` y altura :math:`h` constantes. Un cuerpo se suelta del reposo desde la parte superior del plano, el tiempo :math:`\Delta t` que éste gasta en recorrer cierta distancia :math:`\Delta s` a lo largo del plano dependerá de ésta distancia, y es claro que entre mayor sea ésta, mayor será el tiempo. La finalidad es encontrar la relación matemática entre el tiempo :math:`\Delta t` y la distancia :math:`\Delta s`.

.. figure:: /images/Mecanica/GallileoII/GalileoII.png
   :alt:
   :scale: 50
   :align: center
   :name: GalileoII

   Montaje experimental usado por Galileo (Teorema II).



**Mediciones y procedimientos**

Las mediciones de tiempo tienen una incertidumbre de 0.1 s por defecto.

   #. Abra el programa que realiza la simulación cuyo enlace se encuentra en la sección de :ref:`Recursos <GalileoIIRec>`.
   #. Selecione la opción TEOREMA II
   #. Selecione la opción *Point particle* y *Point particle appearance* :math:`\rightarrow` ball.
   #. Establezca la fracción de distancia que la partícula descenderá lo largo del plano inclinado y cuyo tiempo se medirá; ésta se selecciona con la barra de desplazamiento rotulada como :math:`f` Obsérvese que :math:`f` se define como :math:`f=\frac{\Delta s}{L}`, donde :math:`0\leq f \leq 1`. Así, cuando :math:`f=0` la partícula se encuentra en la cima del plano, cuando :math:`f=1` la partícula se encuentra en la base del plano y ha recorrido una distancia igual a :math:`L`, cuando :math:`f=0,5` la partícula ha recorrido una distancia igual a :math:`\frac{L}{2}`, etc.
   #. Realice simulaciones para diferentes valores de :math:`f`, registrando los diferentes valores de :math:`\Delta t` en la  :numref:`tab:GalileoII` .
       .. csv-table:: Relación entre :math:`\Delta t` y :math:`f`
          :header: ":math:`f`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoII
          :align: center

          0.1,
          0.2,
          0.3,
          0.4,
          0.5,
          0.6,
          0.7,
          0.8,
          0.9,
          1.0

   #. Realice una gráfica del tiempo :math:`\Delta t` en función de :math:`f`.
   #. Basado en el tipo de gráfica obtenido en el inciso anterior, proponga un modelo para la dependencia de :math:`\Delta t` en función de :math:`f`.
   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relacione las variables  :math:`\Delta t` y :math:`f`.
   #. Verifique que la ecuación encontrada en el inciso anterior predice el tiempo de descenso de la partícula a lo largo del plano inclinado para diferentes valores de :math:`f` de la  :numref:`tab:GalileoII` .
   #. Repita los mismos pasos anteriores, pero esta vez seleccionando una esfera en lugar de la partícula puntual. Para ello, seleccione la opción *Finite size ball* y seleccione el radio de la esfera igual :math:`R=0.2` m en el primer caso y :math:`R=0.4` m en el segundo caso. Registre los valores de sus mediciones en la :numref:`tab:GalileoII_1` y la :numref:`tab:GalileoII_2` respectivamente.
       .. csv-table:: :math:`R=0.2\,\text{m}`
          :header: ":math:`f`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoII_1
          :align: center

          0.1,
          0.2,
          0.3,
          0.4,
          0.5,
          0.6,
          0.7,
          0.8,
          0.9,
          1.0

       .. csv-table:: :math:`R=0.4\,\text{m}`
          :header: ":math:`f`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoII_2
          :align: center

          0.1,
          0.2,
          0.3,
          0.4,
          0.5,
          0.6,
          0.7,
          0.8,
          0.9,
          1.0


**Análisis y Preguntas**

Basado en los datos de la simulación y las ecuaciones que relacionan las variables :math:`\Delta t` y :math:`f`:


   #. En sus propias palabras: enuncie el teorema II de Galileo.
   #. Demuestre que si :math:`\Delta t_1` y :math:`\Delta t_2` son los tiempos de descenso para las correspondientes distancias :math:`\Delta s_1` y :math:`\Delta s_2`, entonces :math:`\frac{\Delta t_1}{\Delta t_2}=\frac{\sqrt{\Delta s_1}}{\sqrt{\Delta s_2}}`.
   #. ¿Qué concluye acerca de la dependencia entre las variables :math:`\Delta t` y :math:`f`, si se tiene en cuenta el tamaño del objeto que desciende por el plano inclinado?
   #. ¿En qué difieren las ecuaciones que relacionan las variables :math:`\Delta t` y :math:`f` para el caso de la partícula puntual y las esferas de diferentes tamaños?
   #. Argumente la validez de sus resultados.
   #. Establezca las posibles limitaciones del fenómeno estudiado a través de la simulación.

.. rubric:: Nota

.. [#f1] Galileo Galilei (1564-1642) fue un astrónomo, filósofo, matemático y físico italiano, relacionado estrechamente con la revolución científica.
