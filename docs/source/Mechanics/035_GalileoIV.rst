Versión moderna del teorema IV de Galileo
============================================
**Objetivo**

El objetivo de esta actividad es estudiar una versión moderna del teorema IV de Galileo sobre el movimiento
uniformemente acelerado, tal como se encuentra en el tercer día de la obra
\" *Discourses and Mathematical Demonstrations Relating to Two New Sciences* \" de Galileo [#f1]_

.. _GalileoIVRec:

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.geogebra.org/m/kqRFm4vW <https://www.geogebra.org/m/kqRFm4vW>`_.

**Situación**

La :numref:`GalileoIV` muestra un plano inclinado de longitud :math:`L` constante y altura :math:`h` variable. Un cuerpo se suelta del reposo desde la parte superior del plano, el tiempo :math:`\Delta t` que gasta el cuerpo en llegar a la base del plano dependerá de la distancia :math:`h`, y es claro que entre mayor es :math:`h` menor será el tiempo :math:`\Delta t`. La finalidad es encontrar la relación matemática entre :math:`\Delta t` y :math:`h`.

.. figure:: /images/Mecanica/GallileoIV/GalileoIV.png
   :alt:
   :scale: 50
   :align: center
   :name: GalileoIV

   Montaje experimental usado por Galileo (Teorema IV).


**Mediciones y procedimientos**

Las mediciones de tiempo tienen una incertidumbre de 0.1 s por defecto.

   #. Abra el programa que realiza la simulación cuyo enlace se encuentra en la sección de Recursos.
   #. Selecione la opción TEOREMA IV
   #. Selecione la opción *Point particle* y *Point particle appearance* :math:`\rightarrow` ball.
   #. Establezca la altura :math:`h` del plano inclinado con la barra de desplazamiento rotulada como :math:`h`. La altura :math:`h` la puede variar en el rango :math:`0<h\leq2\,\text{m}`.
   #. Realice simulaciones para diferentes valores de :math:`h`, registrando los diferentes valores de :math:`\Delta t` en la  :numref:`tab:GalileoIV` .
       .. csv-table:: Relación entre :math:`\Delta t` y :math:`h`
          :header: ":math:`h`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoIV
          :align: center

          0.2,
          0.4,
          0.6,
          0.8,
          1.0,
          1.2,
          1.4,
          1.6,
          1.8,
          2.0,

   #. Proponga un modelo para la dependencia de :math:`\Delta t` con la altura :math:`h`, basado en el tipo de gráfica obtenido en el inciso anterior.
   #. Haga uso de sus conocimientos de linelalización de una función para encontrar una ecuación matemática que relacione las variables :math:`\Delta t` y :math:`h`.
   #. Verifique que la ecuación encontrada en el inciso anterior predice el tiempo de descenso de la partícula a lo largo del plano inclinado para diferentes valores de :math:`h` de la  :numref:`tab:GalileoIV`.
   #. Repita los mismos pasos anteriores, pero esta vez seleccionando una esfera en lugar de la partícula puntual. Para ello, seleccione la opción *Finite size ball* y seleccione el radio de la esfera igual :math:`R=0.2` m en el primer caso y :math:`R=0.4` m en el segundo caso. Registre los valores de sus mediciones en la :numref:`tab:GalileoIV_1` y la :numref:`tab:GalileoIV_2` respectivamente.
       .. csv-table:: :math:`R=0.2\,\text{m}`
          :header: ":math:`h`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoIV_1
          :align: center

          0.2,
          0.4,
          0.6,
          0.8,
          1.0,
          1.2,
          1.4,
          1.6,
          1.8,
          2.0,

       .. csv-table:: :math:`R=0.4\,\text{m}`
          :header: ":math:`h`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoIV_2
          :align: center

          0.2,
          0.4,
          0.6,
          0.8,
          1.0,
          1.2,
          1.4,
          1.6,
          1.8,
          2.0,


**Análisis y Preguntas**

Basado en los datos de la simulación y las ecuaciones que relacionan las variables :math:`\Delta t` y :math:`h`:


   #. En sus propias palabras: enuncie el teorema IV de Galileo.
   #. Proponga un modelo para la dependencia de :math:`\Delta t` con la altura :math:`h`, basado en el tipo de gráfica obtenido en el inciso anterior.
   #. Haga uso de sus conocimientos de linelalización de una función para encontrar una ecuación matemática que relacione las variables :math:`\Delta t` y :math:`h`.
   #. Verifique que la ecuación encontrada en el inciso anterior predice el tiempo de descenso de la partícula a lo largo del plano inclinado para diferentes valores de :math:`h` de la  :numref:`tab:GalileoIV`.
   #. Repita los mismos pasos anteriores, pero esta vez seleccionando una esfera en lugar de la partícula puntual. Para ello, seleccione la opción *Finite size ball* y seleccione el radio de la esfera igual :math:`R=0.2` m en el primer caso y :math:`R=0.4` m en el segundo caso. Registre los valores de sus mediciones en la :numref:`tab:GalileoIV_1` y  la :numref:`tab:GalileoIV_2` respectivamente.

.. rubric:: Nota

.. [#f1] Galileo Galilei (1564-1642) fue un astrónomo, filósofo, matemático y físico italiano, relacionado estrechamente con la revolución científica.
