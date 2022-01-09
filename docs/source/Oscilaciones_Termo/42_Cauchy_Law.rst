.. _Cauchy_Law:

Ley de Cauchy
==============

**Objetivo**

El propósito de esta práctica es encontrar la dependencia del índice de refracción de materiales transparentes (vidrio y agua) de la longitud de onda de la luz.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html <https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html>`_. *Bending Light: More Tools*

**Resumen teórico**

La velocidad :math:`v` de propagación de la luz dentro de un material transparente se define como el cociente :math:`\frac{c}{n}`, donde :math:`n` es el índice de refracción del material y :math:`c` es la velocidad de la luz en el vacío. Por otra parte, el índice de refracción es una función de la longitud de onda de la luz, lo que implica que la velocidad de propagación de la luz en un material transparente depende de la longitud de onda de la luz.
Supondremos que la relación entre :math:`n` y :math:`\lambda` tiene la forma

.. math::
   :label: Ec:Cauchy01

   \begin{equation}
    n=A+\frac{B}{\lambda ^2}
   \end{equation}


donde :math:`A` y :math:`B` son constantes que dependen de la naturaleza del medio.


**Montaje experimental**

La :numref:`fig:Cauchy_setup_01` muestra la interfaz del usuario que permite la toma de datos para la determinación de la dependencia de :math:`n` de :math:`\lambda`. En la parte superior izquierda se puede seleccionar la longitud de onda de la luz emitida por la fuente de luz al desplazar el botón de color rojo. El rango de longitudes de onda va desde 380 a 700 nm, que corresponde al visible.  El ángulo de incidencia del rayo de luz con respecto a la normal se puede variar al girar la fuente de luz.  En la interfaz también se encuentran un medidor de intensidad de la luz, uno de velocidad, un transportador (uno digital y otro mecánico) y un osciloscopio rudimentario.  Además, en la parte derecha central se dispone de dos cajas consolas idénticas, con un par de botones que permiten seleccionar el tipo de material y el correspondiente índice de refracción. En esta práctica solo usaremos el medidor de velocidad de la luz.

.. figure:: /images/Oscilaciones_Termo/Cauchy_Law/Cauchy_01.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:Cauchy_setup_01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

   #. Encienda la fuente de luz
   #. Fije el ángulo de incidencia de la luz con respecto a la normal, por ejemplo en :math:`45\,^o`. Obsérvese la trayectoria de los rayos refractado y reflejado. Verifique que se cumple la ley de Snell.
   #. Coloque el medidor de velocidad de la luz rotulado **Speed** tal como indica la :numref:`fig:Cauchy_setup_02`. El valor mostrado por el medidor indica que la velocidad de la luz en el vidrio con índice de refracción n=1.5 es de 0.67 veces la velocidad de la luz, cuando la longitud de onda es de 650 nm

      .. figure:: /images/Oscilaciones_Termo/Cauchy_Law/Cauchy_02.png
         :alt:
         :scale: 110
         :align: center
         :name: fig:Cauchy_setup_02

         Configuración inicial.


   #. Varíe la longitud de onda y observe el nuevo valor del índice de refracción. Registre los valores de :math:`\lambda` y :math:`n` en la :numref:`tab:Cauchy_01`.

      .. csv-table:: Datos medidos de :math:`\lambda` y :math:`n`, (víidrio)
         :header: "Longitud de onda :math:`\\lambda` (nm)", "Indice de refracción, :math:`n` "
         :widths: 1,1
         :width: 12 cm
         :name: tab:Cauchy_01
         :align: center

         380,.
         400,.
         425,.
         450,.
         475,.
         500,.
         550,.
         600,.
         650,.
         700,.

   #. Realice una gráfica de :math:`n` en función de lamba con los datos de la :numref:`tab:Cauchy_01`. Utilice sus conocimientos de linealización y el modelo propuesto por la ecuación :eq:`Ec:Cauchy01` para encontrar los valores de :math:`A` y :math:`B`.
   #. Sin cambiar las condiciones anteriores cambie la naturaleza del medio de la parte inferior, seleccione ahora agua y repita los pasos de los incisos 3, 4  y 5 solo que ahora debe registrar los datos en la :numref:`tab:Cauchy_02`.

      .. csv-table:: Datos medidos de :math:`\lambda` y :math:`n`, (agua)
         :header: "Longitud de onda :math:`\\lambda` (nm)", "Indice de refracción, :math:`n` "
         :widths: 1,1
         :width: 12 cm
         :name: tab:Cauchy_02
         :align: center

         380,.
         400,.
         425,.
         450,.
         475,.
         500,.
         550,.
         600,.
         650,.
         700,.


**Preguntas**

   #. Con referencia a los valores de  :math:`A` y :math:`\lambda`B`:

      a. ¿Cuáles son sus unidades?
      b. ¿Por qué razón sus valores son diferentes para el vidrio y el agua?

   #. La ecuación :eq:`Ec:Cauchy01` es una versión simplificada de la ley de Cauchy, ¿qué establece la ley de Cauchy?
   #. Explique la razón por la cual cuando luz blanca incide sobre un prisma ésta es descompuesta en sus colores, es decir, aparece un espectro de colores.
   #. Explique la razón por la cual la luz roja se dispersa menos que la luz violeta.
