Ley de Snell
=============

**Objetivo**

El propósito de esta práctica es determinar el índice de refracción de un material transparente a través de la ley de Snell.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html <https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html>`_. *Bending Light: More Tools*

**Resumen teórico**

La luz cuando se propaga en el vacío, lo hace a velocidad constante y de forma rectilínea, pero cuando llega a un material la velocidad de la luz cambia debido a su interacción con el sólido. El índice de refracción es un parámetro óptico característico de cada material homogéneo que se define como el cociente entre la velocidad de la luz en el vacío, :math:`c`, y la velocidad de la luz
en el material, :math:`v`: [#f1]_, [#f2]_

.. math::
   :label: Ec:Snell_01

   \begin{equation}
    n= \frac{c}{v}
   \end{equation}

Las leyes de la Óptica Geométrica permiten estudiar los fenómenos de interacción de la luz con los materiales:


   #. Ley de la propagación rectilínea: en un medio homogéneo, los rayos de luz se propagan en línea recta.
   #. Leyes de la reflexión establecen que:

      a. el rayo incidente, la normal y el rayo reflejado están en un mismo plano.
      b. el ángulo incidente :math:`\theta_i` y el ángulo reflejado :math:`\theta_r` tienen el mismo valor, con respecto a la normal.

      .. figure:: /images/Oscilaciones_Termo/Snell/Snell_01.png
         :alt:
         :scale: 80
         :align: center
         :name: fig:Snell_01

         Rayos incidente y reflejado

   #. Ley de la refracción: cuando una onda incide sobre la superficie de separación entre dos medios, parte de la onda se refleja y parte entra en el segundo medio. El rayo transmitido está contenido en el plano de incidencia pero cambia de dirección (rayo refractado) formando un ángulo :math:`\theta_t`  con la normal a la superficie, dado por la Ley de Snell:

      .. math::
         :label: Ec:Snell_02

         \begin{equation}
         n_1\sin(\theta_i)=n_2\sin(\theta_t)
         \end{equation}

      .. figure:: /images/Oscilaciones_Termo/Snell/Snell_02.png
         :alt:
         :scale: 80
         :align: center
         :name: fig:Snell_02

         :math:`n_1` y :math:`n_2` son los índices de refración de los medios 1 y 2.


Según la Ley de Snell, cuando el rayo pasa a un medio con menor índice de refracción se aleja de la normal, es decir, el ángulo de refracción es mayor que el de incidencia. El valor máximo que puede tomar el seno es 1, por lo que hay un ángulo de incidencia límite tal que para ángulos mayores la refracción no se produce:

.. math::
   :label: Ec:Snell_03

   \begin{equation}
    n_1\sin(\theta_c)=n_2\sin(\frac{\pi}{2})
   \end{equation}

Ese ángulo de incidencia límite se denomina ángulo crítico :math:`\theta_c`

.. math::
   :label: Ec:Snell_04

   \begin{equation}
    \theta_c=\arcsin{\big(\frac{n_2}{n_1}\big)}
   \end{equation}

.. figure:: /images/Oscilaciones_Termo/Snell/Snell_03.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Snell_03

   Reflexión total interna.

Para ángulos mayores que este ángulo crítico no existe rayo refractado, toda la energía de la onda se refleja. Este fenómeno se denomina *reflexión total interna*.


**Montaje experimental**


La :numref:`fig:Snell_Setup_01` muestra la interfaz del usuario que permite la toma de datos para estudiar la ley de Snell. En la parte superior izquierda se puede seleccionar la longitud de onda de la luz emitida por la fuente de luz al desplazar el botón de color rojo. El rango de longitudes de onda va desde 380 a 700 nm, que corresponde al visible.  El ángulo de incidencia del rayo de luz con respecto a la normal se puede variar al girar la fuente de luz.  En la interfaz también se encuentran un medidor de intensidad de la luz, uno de velocidad, un transportador (uno digital y otro mecánico) y un osciloscopio rudimentario. Además, en la parte derecha central se dispone de dos cajas consolas idénticas, con un par de botones que permiten seleccionar el tipo de material y el correspondiente índice de refracción.

.. figure:: /images/Oscilaciones_Termo/Snell/Snell_Setup_01.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:Snell_Setup_01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

.. _Dep_v_n:

**Dependencia de** :math:`v` de :math:`n`

   Para determinar la efecto del índice de refracción del medio en la velocidad de propagación de la luz, realice el montaje que se muestra en la figura :numref:`fig:Snell_Setup_02`. Se medirá la velocidad de la luz :math:`v` como función del índice de refracción :math:`n`. Pare ello, varíe el indice de refracción del medio 2 en pasos de 0.05 comenzando desde 1 hasta 1.6 y complete la :numref:`tab:Snell_01`.

   .. figure:: /images/Oscilaciones_Termo/Snell/Snell_Setup_02.png
      :alt:
      :scale: 35
      :align: center
      :name: fig:Snell_Setup_02

      Interfaz gráfica del usuario.


   .. csv-table:: Datos medidos de :math:`n` y :math:`v`
      :header: "Ind. de refracción :math:`n`", "Velocidad, :math:`v (\\times c)`"
      :widths: 1,1
      :width: 12 cm
      :name: tab:Snell_01
      :align: center

      1.00,.
      1.05,.
      1.10,.
      1.15,.
      1.20,.
      1.25,.
      1.30,.
      1.35,.
      1.40,.
      1.45,.
      1.50,.
      1.55,.
      1.60,.

   #. Realice una gráfica de :math:`v` como función de :math:`n`.
   #. Utilice sus conocimientos de linealización para comprobar a partir de los datos medidos que la gráfica de :math:`v` como función de :math:`\frac{1}{n}` corresponde a una línea recta con pendiente :math:`c`.

.. _Snell_Law:

**Ley d Snell**

   Para determinar la relación entre los ángulos de incidencia y refración, realice el montaje que se muestra en la figura :numref:`fig:Snell_Setup_03`. Se medirán los ángulos de incidencia :math:`\theta_i` y refracción :math:`\theta_t` para cuando la luz pasa del aire al vidrio. Pare ello, varíe el ángulo :math:`\theta_i` en pasos de :math:`10^o` comenzando desde 0 hasta 90, complete la :numref:`tab:Snell_02`.

   .. figure:: /images/Oscilaciones_Termo/Snell/Snell_Setup_03.png
      :alt:
      :scale: 35
      :align: center
      :name: fig:Snell_Setup_03

      Interfaz gráfica del usuario.


   .. csv-table:: Datos medidos de :math:`\theta_i` y :math:`\theta_t`
      :header: "Angulo de incidencia :math:`\\theta_i`", "Angulo de refracción :math:`\\theta_t`"
      :widths: 1,1
      :width: 12 cm
      :name: tab:Snell_02
      :align: center

      0,.
      10,.
      20,.
      30,.
      40,.
      50,.
      60,.
      70,.
      80,.
      90,.

   #. Verifique que la grafica de :math:`\sin(\theta_i)` en función de :math:`\sin(\theta_t)` es una línea recta.

.. _RefTI:

**Reflexión total interna**

   Para determinar el ángulo crítico cuando la luz pasa de un medio de mayor a menor íncide de refracción, realice el montaje que se muestra en la figura :numref:`fig:Snell_Setup_04`. Se medirán los ángulos de incidencia :math:`\theta_i` y refracción :math:`\theta_t` para cuando la luz pasa del vidrio al aire. Pare ello, varíe :math:`\theta_i` y registre el correspondiente valor de :math:`\theta_t`, complete la :numref:`tab:Snell_03`.

   .. figure:: /images/Oscilaciones_Termo/Snell/Snell_Setup_04.png
      :alt:
      :scale: 35
      :align: center
      :name: fig:Snell_Setup_04

      Interfaz gráfica del usuario.


   .. csv-table:: Datos medidos de :math:`\theta_i` y :math:`\theta_t`
      :header: "Angulo de incidencia :math:`\\theta_i`", "Angulo de refracción :math:`\\theta_t`"
      :widths: 1,1
      :width: 12 cm
      :name: tab:Snell_03
      :align: center

      0,.
      5,.
      10,.
      15,.
      20,.
      25,.
      30,.
      35,.
      38,.
      40,.
      :math:`\vdots`,:math:`\vdots`

   #. Verifique que la grafica de :math:`\sin(\theta_i)` en función de :math:`\sin(\theta_t)` es una línea recta.


**Análisis y Preguntas**

   #. En la sección :ref:`Dependencia de v de n <Dep_v_n>` se probó la validez de la ecuación :eq:`Ec:Snell_01`. Por otra parte, si la frecuencia de la luz no cambia cuando pasa de un medio a otro, justifique la razón por la cual se cumple que :math:`\lambda=\frac{\lambda_0}{n}`, donde :math:`\lambda_0` y :math:`\lambda` representan las longitudes de onda de la luz en el vacío y en el medio con índice de refracción :math:`n`. Si se desea estudiar esta dependencia se recomienda estudiar la :ref:`Ley de Cauchy <Cauchy_Law>`.
   #. Demuestre que la ley de Snell dada por la ecuación :eq:`Ec:Snell_02` tambien se puede escribir como :math:`v_2\sin(\theta_i)=v_1\sin(\theta_t)`, donde :math:`v_1` y :math:`v_2` represntan las velocidades de la luz en los medios con índices de refracción :math:`n_1` y :math:`n_2` respectivamente.
   #. En la sección :ref:`Ley de Snell <Snell_Law>` al graficar :math:`\sin(\theta_i)` en función de :math:`\sin(\theta_t)` se obiene una línea recta, ¿ por qué razón la pendiente de esta línea es :math:`\frac{3}{2}`?
   #. En la sección :ref:`Reflexión total interna <RefTI>` al graficar :math:`\sin(\theta_i)` en función de :math:`\sin(\theta_t)` se obiene una línea recta, ¿ por qué razón la pendiente de esta línea es :math:`\frac{2}{3}`?
   #. ¿En qué consiste la reflexión especular y la reflexión difusa? Suministre ejemplos.
   #. La fibra óptica es un componente básico en optoelectrónica y en general es un instrumento muy flexible que permite llevar la luz a cualquier sitio, como por ejemplo al interior del cuerpo humano en aplicaciones médicas.


.. [#f1] Jenkins F.A., White H.E., (1950) *Fundamentals of Optics*, McGraw-Hill, Nueva York
.. [#f2] ‎Eugene Hecht, *Optics*, Addison-Wesley; 4a edición (1 Agosto 2001)