+Conservación de la energía Mecánica
=====================================

**Objetivo**

El propósito de esta práctica determinar el valor de la aceleración de la gravedad :math:`g` a partir del  principio de conservación de la energía mecánica. Para ello, se utiliza un péndulo cuya masa se suelta desde diferentes alturas :math:`H` medidas desde los puntos de supensión de las cuerdas y se mide la correspondiente rapidez :math:`v` de la masa
en su punto mas bajo. A partir de las mediciones de :math:`v` y :math:`H` y la conservación de la energía se determina :math:`g`.

**Recursos**

   #. Una esfera metálica con ojal de diámetro menor que 1 cm.
   #. Dos cuerdas delgadas.
   #. Un fotointerruptor con interfase conectada al computador.
   #. Una regla graduada en mm.
   #. Un transportador.

**Resumen teórico**

El trabajo realizado por una fuerza :math:`\overrightarrow{F}` para llevar una partícula de un punto :math:`A` a un punto :math:`B` se define  como

.. math::
   :label: Ec:EC_0

   \begin{equation}
    W=\int \overrightarrow{F}\cdot d\overrightarrow{r}
   \end{equation}


donde la integral que aparece en la expresión :eq:`Ec:EC_0` es una integral especial denominada integral de línea ya que ésta se realiza sobre una trayectoria y en general su valor depende de la trayectoria o camino que conecta los puntos :math:`A` y :math:`B`.

El teorema del trabajo y energía afirma que si como resultado de aplicar :math:`N` fuerzas :math:`\overrightarrow{F}_{1},\overrightarrow{F}_{2},\ldots \overrightarrow{F}_{N}` a un sistema, su energía cinética cambia de :math:`E_{k_A}` a :math:`E_{k_B}`, entonces el trabajo neto :math:`W` hecho por estas fuerzas es igual al cambio en la energía cinética :math:`\Delta E_{k}` del sistema, es decir

.. math::
   :label: Ec:EC_1

   \begin{equation}
    W=W_{\overrightarrow{F}_{1}}+W_{\overrightarrow{F}_{2}}+W_{\overrightarrow{F}_{3}}+\ldots W_{\overrightarrow{F}_{N}}=\Delta E_{k}=E_{k_{B}}-E_{k_{A}}
   \end{equation}

Este teorema es de gran validez y la naturaleza de las fuerzas no importa; es decir, que las fuerzas pueden ser de origen mecánico, eléctrico, magnético, gravitacional, etc y el teorema aplica. Por otra parte, cuando una fuerza :math:`\overrightarrow{F}` es conservativa entonces la fuerza tiene asociada una energía potencial :math:`U`, la cual es una función escalar y en este caso el trabajo hecho por :math:`\overrightarrow{F}` es dado por :math:`W=\int \overrightarrow{F}\cdot d\overrightarrow{r}=U_{A}-U_{B}`. La ventaja de una fuerza conservativa es que su trabajo :math:`W` se calcula directamente como
la diferencia de energía :math:`U` entre los puntos :math:`A` \ y :math:`B`; y por tanto no es necesario calcular la integral dada por la expresión :eq:`Ec:EC_0`. Así, si la única fuerza que actúa sobre el sistema es :math:`\overrightarrow{F}` y es conservativa, entonces la expresión :eq:`Ec:EC_1` se transforma en

.. math::
   :label: Ec:EC_2

   \begin{equation}
   W=W_{\overrightarrow{F}}=U_{A}-U_{B}=E_{k_{B}}-E_{k_{A}}
   \end{equation}

o

.. math::
   :label: Ec:EC_3

   \begin{equation}
    U_{A}+E_{k_{A}}=U_{B}+E_{k_{B}}
   \end{equation}

La expresión :eq:`Ec:EC_3` no es mas que la conservación de la energía mecánica.

**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:enfig1`, el cual consiste de cuerpo de masa :math:`m` suspendido de dos cuerdas iguales y de longitud :math:`L` de los puntos :math:`o` y :math:`o'`. Al usar la conservación de la energía entre los puntos :math:`A` y :math:`B` al cuerpo de masa :math:`m` resulta


.. figure:: /images/Mecanica/Energy_Conservation/enfig1.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:enfig1

   Cuerpo suspendido de dos cuerdas ligeras e inextensibles de igual longitud :math:`L`. Izquierda (vista frontal): el cuerpo se encuentra en su posición de equilibrio. Derecha (vista lateral): La masa se desplaza de su posición de equilibrio un ángulo :math:`\theta` (punto A) y se libera, llegando a su punto más bajo (punto :math:`B`) con rapidez :math:`v`.


.. math::
   :label: Ec:EC_4

   \begin{equation}
    -mgH=-mgL\cos\alpha+\frac{1}{2}mv^{2}
   \end{equation}

donde :math:`-mgH` y :math:`-mgL\cos\alpha` corresponden a las energías potencial gravitacional en los puntos :math:`A` y :math:`B` respectivamente y el segundo término de la derecha corresponde a la energía cinética del cuerpo en su punto más bajo (punto :math:`B`). Hemos definido energía potencial cero desde un nivel de referencia que pasa por la línea que une los puntos :math:`o` y :math:`o'`. La expresión :eq:`Ec:EC_4` se puede reescribir como

.. math::
   :label: Ec:EC_5

   \begin{equation}
    v^{2}=2gL\cos\alpha-2gH
   \end{equation}

donde el rango de la variable :math:`H` es :math:`0\leq H \leq L\cos\alpha`. Obsérvese que la relación entre :math:`v^{2}` y :math:`H` es lineal y que el valor de la pendiente viene dado por :math:`p = -2g` (ver :numref:`fig:enfig2`). Así, al variar :math:`\theta` y por tanto :math:`H` estamos variando el valor :math:`v` del cuerpo en el punto :math:`B`.

.. figure:: /images/Mecanica/Energy_Conservation/enfig2.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:enfig2

   Gráfica de :math:`v^2` como función de :math:`H` para el sistema mostrado en la :numref:`fig:enfig1`.


**Mediciones**

El valor de la velocidad del cuerpo en en el punto :math:`B` se determina con la ayuda del fotointerruptor operando en el Modo 2 y una pequeña placa opaca rectangular de masa despreciable,  ancho :math:`\Delta D` y longitud :math:`\ell` pegada al cuerpo de masa :math:`m` en su parte inferior, la cual bloquea el fotointerruptor. En el Modo 2, el fotointerruptor conectado al computador permite medir los intervalos de tiempo :math:`\Delta t` para los cuales el  fotointerruptor permanece bloqueado. Así, la velocidad :math:`v` de la masa en el punto :math:`B` es :math:`v=\frac{\Delta D}{\Delta t}\big( 1- \frac{\ell}{L\cos \alpha}\big)` [#f1]_.
Complete la tabla de datos :numref:`tab:EC_grav`. A partir de los datos, construya la gráfica de :math:`v^{2}` como función de :math:`H`. De la pendiente :math:`p` de la recta obtenida determine :math:`g` como se indica arriba. Aplique la teoría de errores apropiada para expresar el valor de :math:`g` junto con la correspondiente incertitumbre.


.. csv-table:: Datos para determinar :math:`g`
      :header: ":math:`H \\, (\\text{cm})`", ":math:`\\Delta t(ms)`"
      :widths: 1,1
      :width: 10 cm
      :name: tab:EC_grav
      :align: center

      0, 
      1, 
      2,  
      3,  
      4,  
      5,  
      :math:`\vdots`
      :math:`L\cos\alpha`

**Análisis y Preguntas**

En el método descrito arriba para determinar la velocidad del cuerpo de masa :math:`m`, no se tuvo en cuenta el tamaño de la esfera, es decir, su radio :math:`R`. Realice un análisis cuantitativo y detallado de como el tamaño de la esfera altera el valor del cálculo de su velocidad.

.. [#f1] Para cuaquier valor de :math:`\theta` se cumple que la rapidez :math:`v` de :math:`m` y la rapidez :math:`v_{\ell}=\frac{\Delta D}{\Delta t}` del extremo inferior de la placa de longitud :math:`\ell` están dadas por :math:`v=\omega L\cos \alpha` y :math:`v_{\ell}=\omega (L\cos \alpha+\ell)`, donde :math:`\omega` es la velocidad angular. De estas dos expresiones se encuentra que :math:`v=\frac{\frac{\Delta D}{\Delta t}}{1+\frac{\ell}{L\cos\alpha}}\approx \frac{\Delta D}{\Delta t}\big(1-\frac{\ell}{L\cos\alpha}\big)`. Hemos hecho uso de la aproximación :math:`(1+x)^n \approx 1+x`, la cual es válida para :math:`x<<1`.