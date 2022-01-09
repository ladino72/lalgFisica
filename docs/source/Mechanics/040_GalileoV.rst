Versión moderna del teorema V de Galileo
============================================
**Objetivo**

El objetivo de esta actividad es estudiar una versión moderna del teorema V de Galileo sobre el movimiento
uniformemente acelerado, tal como se encuentra en el tercer día de la obra
\" *Discourses and Mathematical Demonstrations Relating to Two New Sciences* \" de Galileo [#f1]_

.. _GalileoVRec:

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.geogebra.org/m/kqRFm4vW <https://www.geogebra.org/m/kqRFm4vW>`_.

**Situación**

La :numref:`GalileoV` muestra dos planos inclinados de longitudes :math:`L_1`, :math:`L_2` y alturas :math:`h_1`, :math:`h_2` respectivamente. Cuerpos idénticos se sueltan del reposo desde la parte superior de cada plano, los tiempos :math:`\Delta t_1` que gastan los cuerpos en llegar a la base del plano dependerán la longitud del plano y la altura del mismo. La finalidad es encontrar la relación matemática entre :math:`\Delta t`, :math:`h` y :math:`L`.

.. figure:: /images/Mecanica/GallileoV/GalileoV.png
   :alt:
   :scale: 65
   :align: center
   :name: GalileoV

   Montaje experimental usado por Galileo (Teorema V).



**Mediciones y procedimientos**

Las mediciones de tiempo tienen una incertidumbre de 0.1 s por defecto.

.. _GalileoV_h:

**Dependencia de** :math:`\Delta t` con :math:`L`, :math:`h=\text{constante}`


   #. Selecione la opción TEOREMA V
   #. Selecione la opción *Point particle* y *Point particle appearance* :math:`\rightarrow` ball.
   #. Fije la altura del plano inclinado en :math:`h=1\,\text{m}` y varíe la longitud del plano el rango :math:`1<h=<8\,\text{m}`. Para cada longitud mida el tiempo :math:`\Delta t` que gasta el cuerpo en llegar a la base del plano. Registre sus mediciones en la :numref:`tab:GalileoV_a`.
       .. csv-table:: Relación entre :math:`\Delta t` y :math:`L`
          :header: ":math:`L`", ":math:`\\Delta t`` (s)"
          :widths: 1,1
          :width: 10 cm
          :name: tab:GalileoV_a
          :align: center

          1.5,
          2.5,
          3.5,
          4.5,
          5.5,
          6.5,
          7.5,
          8.0,


   #.  Realice una gráfica de :math:`\Delta t` en función de la altura :math:`L`.
   #.  Proponga un modelo para la dependencia de :math:`\Delta t` con la altura :math:`L`, basado en el tipo de gráfica obtenido en el inciso anterior.
   #.  Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relacione las variables :math:`\Delta t` y :math:`L`.  Asuma una relación de la forma :math:`\Delta t=aL^{m}`, donde :math:`a` y :math:`m` son constantes que debe encontrar.
   #. Verifique que la ecuación encontrada en el inciso anterior predice el tiempo de descenso de la partícula a lo largo del plano inclinado para diferentes valores de :math:`L` de la :numref:`tab:GalileoV_a`.


.. _GalileoV_L:

**Dependencia de** :math:`\Delta t` con :math:`h`, :math:`L=\text{constante}`

   #.  Abra el programa que realiza la simulación cuyo enlace se encuentra en la sección de Recursos.
   #.  Selecione la opción TEOREMA V
   #.  Selecione la opción *Point particle* y *Point particle appearance* :math:`\rightarrow` ball.
   #.  Fije la longitud del plano inclinado en :math:`L=1\,\text{m}` y varíe su altura en el rango :math:`0.5\leq h \leq2\,\text{m}`. Para cada longitud mida el tiempo :math:`\Delta t` que gasta el cuerpo en llegar a la base del plano. Registre sus mediciones en la :numref:`tab:GalileoV_b`.
        .. csv-table:: Relación entre :math:`\Delta t` y :math:`h`
           :header: ":math:`h`", ":math:`\\Delta t`` (s)"
           :widths: 1,1
           :width: 10 cm
           :name: tab:GalileoV_b
           :align: center

           1.5,
           2.5,
           3.5,
           4.5,
           5.5,
           6.5,
           7.5,
           8.0,

   #.  Realice una gráfica de :math:`\Delta t` en función de la altura :math:`h`.
   #.  Proponga un modelo para la dependencia de :math:`\Delta t` con la altura :math:`h`, basado en el tipo de gráfica obtenido en el inciso anterior.
   #.  Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relacione las variables :math:`\Delta t` y :math:`h`. Asuma una relación de a forma :math:`\Delta t=bh^{n}`, donde :math:`b` y :math:`n` son constantes que debe encontrar.
   #.  Verifique que la ecuación encontrada en el inciso anterior predice el tiempo de descenso de la partícula a lo largo del plano inclinado para diferentes valores de :math:`L` de la :numref:`tab:GalileoV_b`.


**Análisis y Preguntas**

   #. Basado en los resultados de los dos apartados anteriores escriba una relación entre :math:`\Delta t`, :math:`h` y :math:`L`. Ayuda: debe ser una relación de la forma :math:`\Delta t =Ah^{n}L^{m}`. Determine el valor de :math:`A`.
   #. Demuestre que si :math:`\Delta t_1` y :math:`\Delta t_2` son los tiempos de descenso para planos de altura :math:`h_1`, :math:`h_2` y longitudes :math:`L_1`, :math:`L_2` entonces se cumple que :math:`\frac{\Delta t_1}{\Delta t_2}=\frac{L_1}{L_2}\frac{\sqrt{h_2}}{\sqrt{h_1}}`.
   #. En sus propias palabras: enuncie el teorema V de Galileo.
   #. Argumente la validez de sus resultados.
   #. Establezca las posibles limitaciones del fenómeno estudiado a través de la simulación.


.. rubric:: Nota

.. [#f1] Galileo Galilei (1564-1642) fue un astrónomo, filósofo, matemático y físico italiano, relacionado estrechamente con la revolución científica.
