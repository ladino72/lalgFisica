+Principio de Arquimedes
========================

**Objetivo**

El propósito principal de esta práctica es determinar la densidad de
un líquido (agua, alcohol o glicerina) usando  el principio de Arquímedes.

**Recursos**


  #. Agua, alcohol o glicerina.
  #. Beaker con capacidad de por lo menos 2 litros.
  #. Una probeta.
  #. Balanza digital.
  #. Una barra cilíndrica de metal.

**Resumen teórico**

El principio de Arquímedes es un principio físico que afirma que: Un cuerpo total o parcialmente sumergido en un fluido en reposo, recibe un empuje de abajo hacia arriba igual al peso del volumen del fluido que desaloja. Esta fuerza recibe el nombre de empuje hidrostático o de Arquímedes, y se mide en newtons (en el sistema internacional de unidades). El principio de Arquímedes se formula así:

.. math::
   :label: Ec:add0

   \begin{equation}
    E=\rho gV
   \end{equation}

donde :math:`E` es el empuje, :math:`\rho` es la densidad del fluido, :math:`V` el volumen de fluido desplazado por algún cuerpo sumergido parcial o totalmente en el mismo, :math:`g` la aceleración de la gravedad, de este modo, el empuje depende de la densidad del fluido, del volumen del cuerpo y de la gravedad existente en ese lugar. El empuje (en condiciones normales) y descrito de modo simplificado) actúa verticalmente hacia arriba y está aplicado en el centro de gravedad del fluido desalojado por el cuerpo; este punto recibe el nombre de centro de carena.



**Descripcion del Experimento**

Considere el sistema mostrado en la :numref:`fig:adfig1`, el cual consta de un vaso de vidrio con liquido de densidad :math:`\rho _{x}` desconocida colocado sobre una balanza electrónica. Una barra metálica de seccion transversal constante pende de un soporte y se encuentra parcialmente sumergida en el líquido.

.. figure:: /images/Mecanica/Arquimedes/adfig1.png
   :alt: Arquimedes
   :scale: 100%
   :align: center
   :name: fig:adfig1

   La lectura de la balanza corresponde a la suma de los pesos del vaso, el líquido, y el peso del volumen del líquido desplazado por la barra.


**Definiciones**

..

   :math:`A=` área de la sección transversal de la barra. :math:`\newline`

..

   :math:`m_{x}` y :math:`\rho _{x}` representan la masa y densidad del líquido cuya densidad se desea medir (alcohol o glicerina)

..

   :math:`m_{v}=` masa del vaso de vidrio.

..

   :math:`x =`  distancia que se encuentra sumergidada la barra en el líquido.

..

   :math:`L=` longitud de la barra metálica.

..

   :math:`g=` aceleración de la gravedad.


Si el sistema sse encuentra en equilibriio, la lectura de la balanza digital es

.. math::
   :label: Ec:ad1

   \begin{eqnarray}
    N &=& m_{v}g+m_{x}g+\rho_{x} gAx \\
      &=& b_{2}+px
   \end{eqnarray}

donde hemos definido

.. math::
   :label: Ec:Arq_Intercept_2

   \begin{equation}
    b_2 = m_{v}g+m_{x}g
   \end{equation}

.. math::
   :label: Ec:slope2

   \begin{equation}
    p =\rho_{x} gA
   \end{equation}

en la ecuación :eq:`Ec:ad1` el primer y segundo término corresponden a los pesos del vaso de vidrio y el líquido respectivamente. El tercer término dado por :math:`\rho_{x}gAx` es el peso del líquido desalojado por la barra.
El valor de :math:`N` es dado por :math:`mg`, donde :math:`m` es la lectura de la balanza. Obsérvese que :math:`N` depende linealmente de la profundidad :math:`x`; es decir,  el valor de :math:`N` varía linealmente con la propundidad :math:`x` que se sumerge la barra. De esta manera, una gráfica de :math:`N` en función de :math:`x` corresponde a una línea recta con pendiente :math:`p` igual a

.. math::
   :label: Ec:ad.2

   \begin{eqnarray}
    p= \rho_{x} gA
   \end{eqnarray}


de ésta última expresión el valor de la densidad :math:`\rho_{x}` se puede obtener a partir del valor :math:`p` medido experimentalmente

.. math::
   :label: Ec:Arq_Density_2

   \begin{equation}
    \rho_{x}=\frac{p}{gA}
   \end{equation}


**Mediciones**

Realice el montaje que se indica en la :numref:`fig:adfig1`. Se sugiere que complete la tabla de datos :numref:`table:Arqu_Densidad`. A partir de las mediciones obtenidas determine el valor del líquido usado.

.. csv-table:: Datos para determinar la densidad :math:`\rho` del líquido usado.
   :header: ":math:`N` (N)", ":math:`x` (m)"
   :widths: 1,1
   :width: 12 cm
   :name: table:Arqu_Densidad
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

**Preguntas**

   #. ¿Qué significa el valor del punto de intersección de la recta dado por la expresión :eq:`Ec:Arq_Intercept_2` con el eje :math:`N`?
   #. ¿En que parte del modelo propuesto se esta haciendo uso del principio de acción y reacción (tercera ley de Newton)?
   #. Calcule el valor de la densidad del líquido utilizado y exprese el resultado en la forma :math:`\rho=\rho_0\pm\Delta \rho` y compare este valor con el reportado en la literatura.

