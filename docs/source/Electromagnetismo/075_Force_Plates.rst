Fuerza entre placas de un condensador de placas paralelas
===========================================================

**Objetivo**

El propósito de esta práctica es determinar la capacitancia :math:`C` de un condensador de placas paralelas a partir de la medición de la fuerza de atraccción entre las placas  cuando la diferencia de potencial entre éstas cambia.

**Resumen teorico**

Consideremos los sistemas mostrados en la figura :numref:`fig:Fplates1` y la :numref:`fig:Fplates2`. Estos constan de un par de placas conductoras de área :math:`A` y separadas una distnancia :math:`x`. La placa de la izquierda se encuentra fija y la placa de la derecha es móvil. En el primer sistema las placas tienen cargas :math:`+Q` y :math:`-Q`  constantes. En el segundo sistema las placas se mantienen a una diferencia de potencial constante :math:`V`. En ambas situaciones a la placa de la derecha se le debe aplicar una fuerza :math:`F` para mantener la distancia de separación :math:`x` constante. Hallemos el valor de :math:`F`.


.. figure:: /images/Electromagnetismo/Force_Plates/Fplates1.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:Fplates1

   Las placas se separan manteniendo la carga de las placas :math:`+Q` y :math:`-Q` constante.

.. figure:: /images/Electromagnetismo/Force_Plates/Fplates2.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:Fplates2

   Las placas se separan manteniendo la diferencia de potencial :math:`V` entre las placas constante.


Denotemos por :math:`C_0` y :math:`C` las capacitancias del sistema cuando la distancia de separación ente las plcas es :math:`x` y :math:`x+\Delta x` respectivamente.

   #. :math:`Q` = constante. El cambio de energía del condensador es

      .. math::

         \Delta U=\frac{Q^{2}}{2C}-\frac{Q^{2}}{2C_{0}}=\frac{Q^{2}}{2}[\frac{1}{C}-\frac{1}{C_{0}}]=\frac{Q^{2}}{2}[\frac{1}{\frac{\varepsilon _{0}A}{x+\Delta x}}-\frac{1}{\frac{\varepsilon _{0}A}{x}}]=\frac{Q^{2}}{2\varepsilon _{0}A}\Delta x

      Por otra parte, el trabajo hecho por la fuerza :math:`F` es :math:`\Delta W=F\Delta x`. Usando la conservación de la energía:

      .. math::

         \begin{eqnarray*}
          \Delta W &=&\Delta U \\
          F\Delta x &=&\frac{Q^{2}}{2\varepsilon_{0}A}\Delta x
         \end{eqnarray*}

      Despejando el valor de :math:`F` en esta ultima expresión se sigue que

      .. math::
         :label: Ec:Fplacas1

         \begin{equation}
             F=\frac{Q^2}{2\varepsilon_0A}=\frac{1}{2}\frac{C^2V^2}{\varepsilon_0A}
         \end{equation}


   #. :math:`V` = constante El cambio de energía del condensador es

      .. math::

         \Delta U=\frac{1}{2}CV^{2}-\frac{1}{2}C_{0}V^{2}=\frac{1}{2}[C-C_{0}]V^{2}=\frac{1}{2}\Delta C\cdot V^{2},


      donde la variación en la capacitancia :math:`\Delta C` es


      .. math::

         \Delta C=\frac{\varepsilon _{0}A}{x+\Delta x}-\frac{\varepsilon _{0}A}{x}=\varepsilon _{0}A\left[ \frac{1}{x+\Delta x}-\frac{1}{x}\right]=-\varepsilon _{0}A\left[ \frac{\Delta x}{x(x+\Delta x)}\right] \simeq-\varepsilon _{0}A\frac{\Delta x}{x^{2}}

      Así,

      .. math::

         \Delta U=\frac{1}{2}\Delta C\cdot V^{2}\simeq -\frac{1}{2}\varepsilon_{0}AV^{2}\frac{\Delta x}{x^{2}}


      hemos hecho la aproximaxion :math:`x+\Delta x\simeq x` ya que :math:`\Delta x<<x.` Por otra parte, dado que la bateria se encuentra conectada a las placas y la capacitancia disminuye al aumentar la distancia entre las placas, la batería realiza un trabajo, el cual es dado por

      .. math::

         \Delta W_{b}=\Delta qV=\Delta C\cdot V\cdot V\simeq -\varepsilon_{0}AV^{2}\frac{\Delta x}{x^{2}}

      Por otra parte, el trabajo hecho por la fuerza :math:`F` es :math:`\Delta W=F\Delta x.` Usando la conservacion de la energía:

      .. math::
         :nowrap:

         \begin{eqnarray*}
          \Delta W+\Delta W_{b}&=&\Delta U \\
          F\Delta x-\varepsilon_{0}AV^{2}\frac{\Delta x}{x^{2}} &=&-\frac{1}{2}\varepsilon_{0}AV^{2}\frac{\Delta x}{x^{2}}
         \end{eqnarray*}

      Despejando el valor de :math:`F` es esta ultima expresión se sigue que

      .. math::
         :label: Ec:Fplacas2

         \begin{equation}
          F=\frac{1}{2}\varepsilon_{0}AV^{2}\frac{1}{x^{2}}=\frac{1}{2}\frac{\varepsilon_{0}A}{x^{2}}V^{2}=\frac{1}{2}\frac{C^{2}}{\varepsilon_{0}A}V^{2}
         \end{equation}

      .. note::
         La fuerza que se requiere para mantener las placas separadas una distancia :math:`x` cuando estas tienen carga :math:`+Q` y :math:`-Q` es la misma que cuando las placas se mantienen a una diferencia de potencial :math:`V` constante.

De la ecuación :eq:`Ec:Fplacas1` se sigue que la relación entre la fuerza :math: y la diferencia de potencial :math:`V` entre las placas es cuadrática. Dicho de otra manera, la fuerza :math:`F` depende linealmente de :math:`V^{2}` y el coeficiente de proporcionalidad es :math:`\eta =\frac{1}{2}\frac{C^{2}}{\varepsilon _{0}A}`. Esto significa que si realizamos una gráfica de :math:`F` vs :math:`V^{2}`, la pendiente de la recta es

.. math::
   :label: Ec:Fplacas3

   \begin{equation}
    \eta =\frac{1}{2}\frac{C^{2}}{\varepsilon _{0}A}
   \end{equation}

De la expresión :eq:`Ec:Fplacas3` se sigue que determinado el valor de :math:`\eta` el valor de la capacitancia del sistema es dado por

.. math::
   :label: Ec:Fplacas4

   \begin{equation}
    C=\sqrt{2\varepsilon _{0}A\eta }
   \end{equation}

**Descripción del Problema**

El arreglo experimental para determinar la capacitancia (ver :numref:`fig:Fplates3`) consiste esencialmente de un par de placas paralelas, una fuente de alto voltaje (0-20 kV), una balanza electrónica y una placa dieléctrica. La placa :math:`2` reposa sobre un bloque ligero de madera y este a su vez reposa sobre el platillo de la balanza. El propósito del bloque es permitir la lectura registrada por la balanza. La placa :math:`1` se encuentra suspendida de un soporte de modo que las placas queden paralelas, con una distancia de separación :math:`x` en el rango :math:`1.0<x<3.0` cm y aisladas eléctricamente. A las placas :math:`1` y :math:`2` se les aplica una diferencia de potencial :math:`V`. Dado que la fuerza :math:`F` entre las placas es atractiva, la placa :math:`2` experimenta una fuerza hacia arriba y por tanto la lectura de la balanza disminuye. Esta disminución en la lectura de la balanza  corresponde a la fuerza dada por la expresión :eq:`Ec:Fplacas1` ó :eq:`Ec:Fplacas2`. Entre las placas :math:`1` y :math:`2` también se puede colocar una lamina dieléctrica de modo que repose directamente sobre la placa :math:`2` y el efecto de atracción entre las placas se va observar también.

.. figure:: /images/Electromagnetismo/Force_Plates/Fplates3.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:Fplates3

   Arreglo experimental para determinar la capacitancia.


**Mediciones**

*PELIGRO ALTO VOLTAJE*

Realice el montaje que se describe en la :numref:`fig:Fplates3`. Asegúrese de hacer las conexiones con la fuente apagada. *NO encienda la fuente de alto voltaje sin el visto bueno del instructor*. Establezca la distancia de separción entre las placas en el rango sugerido arriba. Complete la :numref:`tab:fplates` de mediciones. Grafique :math:`mg` en función de :math:`V`, luego linealice los datos al graficar :math:`mg` en función de :math:`V^2` y utilice la ecuación :eq:`Ec:Fplacas4` para determinar :math:`C`.

.. csv-table:: Datos para determinar la capacitancia de las placas :math:`1` y :math:`2`.
   :header: "Masa (g)", "Voltaje (kV)"
   :widths: 1,1
   :width: 10 cm
   :name: tab:fplates
   :align: center

   0.0 , 0.00
   , 0.5
   , 1.0
   , 1.5
   , 2.0
   , 2.5
   , 3.0
   , 3.5
   , 4.0
   , 5.0
   , 6.0
   , 7.0
   .,.
   .,.
   .,.

