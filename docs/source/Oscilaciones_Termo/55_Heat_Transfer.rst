Transferencia de calor: conductividad térmica, calor específico, calorimetria
==============================================================================

**Objetivo**

El propósito de esta práctica es estudiar la dinámica del proceso de transferencia de calor entre dos recipientes (calorímetros) que contienen líquidos a temperaturas diferentes y que se encuentran conectados mediante una barra conductora. Los dos recipientes y la barra se encuentran térmicamente aislados para evitar pérdidas de calor con el entorno.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://www.geogebra.org/m/gxyx4b3z <https://www.geogebra.org/m/gxyx4b3z>`_.


**Resumen teórico**

El calor o energía térmica fluye de los cuerpos más calientes a los más fríos. La energía térmica (calor) se transfiere de tres maneras básicas: conducción, convección y radiación. Así, cuando un recipiente de aluminio y lleno de agua caliente se coloca en un cuarto, el agua pierde
calor: a) por conducción a través de la paredes de aluminio del recipiente ( por contacto directo con moléculas más frías); b) por
convección cuando las moléculas que forman el vapor y dejan el recipiente chocan con moléculas del aire, haciendo que estas aumenten su
energía cinética y c) por radiación debido a que se emiten ondas electromagnéticas por el hecho de que el agua se encuentra a una temperatura absoluta diferente de cero.

Ahora, si los extremos de una barra conductora (por ejemplo hecha de Cu, Al, etc) de longitud :math:`L` y sección transversal :math:`A` se mantienen a a temperaturas fijas :math:`T_{2}` y :math:`T_{1}` (:math:`T_{2}>T_{1}`) (ver :numref:`fig:Heat_Transfer_barra`), entonces fluye  calor :math:`q`  a lo largo de la barra con rapidez dada por:

.. math::
   :label: Ec:Heat_Transfer_10

   \begin{equation}
    \frac{dq}{dt}=kA\frac{T_{2}-T_{1}}{L}
   \end{equation}

donde :math:`k` es la conductividad térmica de la barra dada en :math:`W/m\cdot K`. La ecuación :eq:`Ec:Heat_Transfer_10` es válida cuando los extremos de la barra
se han mantenido a temperaturas fijas :math:`T_{2}` y :math:`T_{1}` por un tiempo suficientemente largo de modo que se haya alcanzado el *equilibrio térmico* y la barra se encuentre aislada térmicamente de su alrededor de modo que el calor solo fluya a lo largo de esta, del extremo más caliente al más frío.

.. figure:: /images/Oscilaciones_Termo/Heat_Transfer/Heat_Transfer_barra.png
   :scale: 50
   :align: center
   :name: fig:Heat_Transfer_barra

   Distribución estacionaria de temperatura a lo largo de la barra aislada térmicamente. Los extremos de la barra de mantienen a temperaturas fijas :math:`T_2` y :math:`T_1`, (:math:`T_2` > :math:`T_1`).

Por otra parte, la cantidad de calor :math:`Q` suministrado a un cuerpo de masa :math:`m` (sin ocasionar un cambio de fase) genera un cambio de temperatura :math:`\Delta T` en el mismo dado por

.. math::
   :label: Ec:Heat_Transfer_20

   \begin{equation}
   Q=mc\Delta T
   \end{equation}

la constante de proporcionalidad :math:`c` se denomina el calor específico y depende de la naturaleza de la sustancia. Las unidades de :math:`c` son :math:`J/kg\cdot K`.

Considere el sistema mostrado en la :numref:`fig:Heat_Trans_cal`. El sistema consta de dos calorímetros 1 y 2 térmicamente aislados, los cuales contienen líquidos cuyas masas, calores escpecíficos y temperaturas iniciales son :math:`m_{1}`, :math:`c_{1}`, :math:`T_{10}` y :math:`m_{2}`, :math:`c_{2}`, :math:`T_{20}` respectivamente. Los dos recipientes se encuentran conectados mediante una barra conductora aislada. La longitud, sección transversal y conductividad térmica son :math:`L`, :math:`A` y :math:`k` respectivamente. Los recipientes
intercambian energía térmica solo a través de la barra.

Supongamos que en el instante de tiempo :math:`t` las temperaturas de los recipientes 1 y 2 son :math:`T_{1}(t)` y :math:`T_{2}(t)` y que :math:`T_{2}(t)>T_{1}(t)`. En un tiempo :math:`%
t+dt` las temperaturas cambian a :math:`T_{2}+dT_{2}` y :math:`T_{1}+dT_{1}` debido al intercambio de calor. Al disminuir la temperatura del recipiente 2 en :math:`dT_{2}` este cede una cantidad
de calor igual a :math:`dq=-m_{2}c_{2}dT_{2}` al recipiente 1 a través de la barra. Luego por conservación de la energía se cumple:

.. math::
   :label: Ec:Heat_Transfer_1

   \begin{equation}
    -m_{2}c_{2}\frac{dT_{2}}{dt}=\frac{kA}{L}(T_{2}-T_{1})
   \end{equation}

.. math::
   :label: Ec:Heat_Transfer_2

   \begin{equation}
    m_{1}c_{1}\frac{dT_{1}}{dt}=\frac{kA}{L}(T_{2}-T_{1})
   \end{equation}

reescribiendo las anteriores ecuaciones  resulta

.. math::
   :label: Ec:Heat_Transfer_1a

   \begin{equation}
    \frac{dT_{1}}{dt}=-\frac{kA}{m_{1}c_{1}L}T_{1}+\frac{kA}{m_{1}c_{1}L}T_{2}
   \end{equation}

.. math::
   :label: Ec:Heat_Transfer_2a

   \begin{equation}
    \frac{dT_{2}}{dt}=\frac{kA}{m_{2}c_{2}L}T_{1}-\frac{kA}{m_{2}c_{2}L}T_{2}
   \end{equation}

.. figure:: /images/Oscilaciones_Termo/Heat_Transfer/calorimetro.png
   :scale: 50
   :align: center
   :name: fig:Heat_Trans_cal

   Los calorímetros 1 y 2 contienen líquidos a temperaturas iniciales :math:`T_{10}` y :math:`T_{20}` respectivamente y se  encuentran conectados mediante una barra conductora aislada térmicamente, la cual permite el flujo de energía térmica o calor entre los líquidos. Así, a medida que pasa el tiempo :math:`T_2(t)` disminuye mientras que :math:`T_1(t)` aumenta hasta alcanzarse el equilibrio térmico

Las ecuaciones :eq:`Ec:Heat_Transfer_1a` y :eq:`Ec:Heat_Transfer_2a` representan un sistema de ecuaciones diferenciales lineales de primer orden y acopladas. Este sistema debe ser solucionado sujeto a las condiciones iniciales

.. math::
   :label: Ec:Heat_Transfer_3

   \begin{equation}
    T_{1}(t=0)=T_{10}\mbox{,}\hspace{1cm}T_{2}(t=0)=T_{20}
   \end{equation}


La solución de este sistema de ecuaciones es [#f2]_ :

.. math::
   :label: Ec:Heat_Transfer_4

   \begin{equation}
    T_{1}(t) =\frac{PT_{20}+QT_{10}}{P+Q}+\frac{T_{10}-T_{20}}{P+Q}Pe^{-(P+Q)t}
   \end{equation}

.. math::
   :label: Ec:Heat_Transfer_5

   \begin{equation}
      T_{2}(t) =\frac{PT_{20}+QT_{10}}{P+Q}-\frac{T_{10}-T_{20}}{P+Q}Qe^{-(P+Q)t}
   \end{equation}

donde

.. math::
   :label: c.1

   \begin{equation}
      P=\frac{kA}{m_{1}c_{1}L}\mbox{,}\hspace{1cm}Q=\frac{kA}{m_{2}c_{2}L}
   \end{equation}

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Heat_Transf_setup_01` muestra la interfaz gráfica del usuario para estudiar la transferencia de calor entre recipientes a diferentes temperaturas a través de una barra conductora. Se tienen tres columnas de barras de desplazamiento. La columna 1 (verde) permite seleccionar la conductividad térmica :math:`\kappa` de la barra cilíndrica, su longitud :math:`L` y su radio :math:`r`. La columna 2: (azul) permite seleccionar la masa :math:`m_2`, el calor específico :math:`c_2` y temperatura inicial :math:`T_{20}` del líquido del recipiente 1 y la columna 3: (rojo) permite seleccionar la masa :math:`m_1`, el calor específico :math:`c_1` y la temperatura inicial :math:`T_{10}` del líquido del recipiente 2. Al seleccionar los parámetros anteriores la aplicación traza las temperaturas :math:`T_1` y :math:`T_2` de los líquidos en función del tiempo. La aplicación también muestra la temperatura de equilibrio de los líquidos.

.. figure:: /images/Oscilaciones_Termo/Heat_Transfer/Heat_Transfer_gui.png
   :scale: 45
   :align: center
   :name: fig:Heat_Transf_setup_01

   Interfaz gráfica del usuario para estudiar la transferencia de calor entre recipientes a diferentes temperaturas a través de una barra conductora.


**Mediciones y procedimientos**

**Efecto de la conductividad térmica de la barra**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`m_1=m_2=2.0\,\text{kg}`, :math:`c_1=c_2=2030\,\text{J/kg}\cdot \text{K}` y temperaturas iniciales :math:`T_1=10\,^{o}\text{C}` y :math:`T_2=90\,^{o}\text{C}`. Seleccione la longitud :math:`L` y radio :math:`r` de la barra por ejemplo :math:`L=0.02\,\text{m}` y :math:`r=0.02\,\text{m}`. Varíe la conductividad :math:`\kappa` de la barra y observe el comportamiento de las temperaturas de los líquidos. ¿Cómo afecta la conductividad de la barra en que tan rápido se alcanza la temperatura de equilibrio?


**Efecto de la longitud de la barra**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`m_1=m_2=2.0\,\text{kg}`, :math:`c_1=c_2=2030\,\text{J/kg}\cdot K` y temperaturas iniciales :math:`T_1=10\,^{o}\text{C}` y :math:`T_2=90\,^{o}\text{C}`. Seleccione la conductividad :math:`\kappa` y radio :math:`r` de la barra, por ejemplo :math:`\kappa=290.1\,\text{W/m}\cdot \text{K}` y :math:`r=0.02\,\text{m}`. Varíe la longitud :math:`L` de la barra y observe el comportamiento de las temperaturas de los líquidos. ¿Cómo afecta la longitud de la barra en que tan rápido se alcanza la temperatura de equilibrio?

**Efecto del radio de la barra**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`m_1=m_2=2.0\,\text{kg}`, :math:`c_1=c_2=2030\,\text{J/kg}\cdot \text{K}` y temperaturas iniciales :math:`T_1=10\,^{o}\text{C}` y :math:`T_2=90\,^{o}\text{C}`. Seleccione la conductividad :math:`\kappa` y longitud :math:`L` de la barra, por ejemplo :math:`\kappa=290.1\,\text{W/m}\cdot \text{K}` y :math:`L=0.02\,\text{m}`. Varíe el radio :math:`r` de la barra y observe el comportamiento de las temperaturas de los líquidos. ¿Cómo afecta el radio de la barra en que tan rápido se alcanza la temperatura de equilibrio?

**Efecto de las cantidades de las sustancias en los recipientes**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`c_1=c_2=2030\,\text{J/kg}\cdot \text{K}` y temperaturas iniciales :math:`T_1=10\,^{o}\text{C}` y :math:`T_2=90\,^{o}\text{C}`. Seleccione la conductividad :math:`\kappa`, longitud :math:`L`  y radio de la barra, por ejemplo :math:`\kappa=290.1\,\text{W/m}\cdot \text{K}`, :math:`L=0.02\,\text{m}` y :math:`L=0.02\,\text{m}` . Fije :math:`m_1=1\,\text{kg}`  y varíe :math:`m_2`. ¿Cómo afecta que :math:`m_2>m_1` en que tan rápido se alcanza la temperatura de equilibrio?


**Efecto de los calores específicos de las sustancias en los recipientes**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`m_1=m_2=2.0\,\text{kg}` y temperaturas iniciales :math:`T_1=10\,^{o}\text{C}` y :math:`T_2=90\,^{o}\text{C}`. Seleccione la conductividad :math:`\kappa`, longitud :math:`L`  y radio de la barra, por ejemplo :math:`\kappa=290.1\,\text{W/m}\cdot \text{K}`, :math:`L=0.02\,\text{m}` y :math:`L=0.02\,\text{m}` . Fije :math:`c_1=2030\,\text{J/kg}\cdot \text{K}`  y varíe :math:`c_2`. ¿Cómo afecta que :math:`c_2>c_1` en que tan rápido alcanza la temperatura de equilibrio?


**Efecto de las temperaturas iniciales de los líquidos en los recipientes**

   #. Seleccione un líquido en cada recipiente al fijar por ejemplo: :math:`m_1=m_2=2.0\,\text{kg}`, :math:`c_1=c_2=2030\,\text{J/kg}\cdot \text{K}`. Seleccione la conductividad :math:`\kappa` y longitud :math:`L` de la barra, por ejemplo :math:`\kappa=290.1\,\text{W/m}\cdot \text{K}` y :math:`L=0.02\,\text{m}`. Fije :math:`T_1=10\,^{o}\text{C}`, temperatura del líquido de la derecha. Varíe la temperatura :math:`T_2` y observe el comportamiento de las temperaturas de los líquidos. ¿Cómo afecta que :math:`T_2-T_1` sea muy grande en que tan rápido se alcance la temperatura de equilibrio?

**Consideraciones analíticas**


Examine las expresiones :eq:`Ec:Heat_Transfer_4` y :eq:`Ec:Heat_Transfer_5`. Verifique que las temperaturas se hacen iguales después de un tiempo muy grande (:math:`t \rightarrow \infty`), es decir, se alcanza el equilibrio térmico y que el valor de esta temperatura :math:`T_{e}` es:

.. math::
   :label: Ec:Heat_Transfer_te

   \begin{equation}
    T_{e}=T_{1}(t\rightarrow \infty )=T_{2}(t\rightarrow \infty )=\frac{PT_{20}+QT_{10}}{P+Q}=\frac{m_{1}c_{1}T_{10}+m_{2}c_{2}T_{20}}{m_{1}c_{1}+m_{2}c_{2}}
   \end{equation}

Nótese que la temperatura dada por la ecuación :eq:`Ec:Heat_Transfer_te` es la misma que se obtendría si tuviéramos inicialmente dos líquidos con masas, calores específicos  y temperaturas iniciales :math:`m_{1}`, :math:`c_{1}`, :math:`T_{10}` y :math:`m_{2}`, :math:`c_{2}`, :math:`T_{20}` respectivamente y los mezcláramos directamente. Esta temperatura es la temperatura de equilibrio de la mezcla.

**Discusión y Conclusiones**

Realice un análisis de sus observaciones e indique como debería modificarse el modelo para tener en cuenta el caso donde los recipientes y la barra no se encontraran térmicamente aislados y escriba sus conclusiones.

.. [#f2] Solucionar el sistema de ecuaciones diferenciales :eq:`Ec:Heat_Transfer_1a` y :eq:`Ec:Heat_Transfer_2a` significa que debemos encontrar funciones :math:`T_{1}` y :math:`T_{2}` como funciones del tiempo :math:`t` que satisfagan estas ecuaciones junto con las condiciones iniciales dadas por :eq:`Ec:Heat_Transfer_3`. Existen varias técnicas para solucionar sistemas de ecuaciones de esta naturaleza. Ver por ejemplo [#f1]_

.. [#f1] Dennis G. Zill, *Ecuaciones deiferenciales con aplicaciones de modelado*, Thompson Learning, Loyola Marymout University, séptima edición, 2001.






