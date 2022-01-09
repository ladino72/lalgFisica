Choques en dos dimensiones
===========================

**Objetivo**

El propósito de esta práctica es estudiar la conservación de la cantidad de movimiento lineal o momentum en dos dimensiones de dos discos que colisionan.

**Recursos**

   #.  Conjunto de fotografías de la colisión de dos discos de igual masa.
   #.  Tabla de las posiciones :math:`x` y :math:`y` en función del tiempo de cada uno de los discos.

**Resumen teórico**

Cuando dos o más cuerpos chocan entre sí, la cantidad de movimiento lineal total del sistema
se conserva sin importar el tipo de choque siempre y cuando el sistema se encuentre aislado. Existen varios tipos de choques: elásticos,
inelásticos y completamente inelásticos. En un choque elástico tanto la energía cinética como el momentum del sistema permanecen constantes. En un choque inelástico o completamente inelástico solo el momentum del sistema permanece constante. La mayoria de los choques que suceden en la naturaleza son inelásticos. Un choque es completamente inelástico cuando los cuerpos quedan pegados después del choque. La ley de conservación del momentun es una ley de validez universal. La idea de «conservación» es tan poderosa en ciencia que los científicos creen que siempre estará justificada. Cualquier aparente excepción a la ley se entenderá tarde o temprano de una manera tal que no nos obligue a renunciar a la ley.

Para un choque elástico en dos dimensiones (ver :numref:`fig:cmefig1`) la conservación del momentum es:

.. figure:: /images/Mecanica/Choques_2D/Choques_2D.png
   :alt:
   :scale: 55
   :align: center
   :name: fig:cmefig1

   Choque elástico

.. math::
   :label: mom.0

   \begin{equation}
    m_1\overrightarrow{v}_1+m_2\overrightarrow{v}_2=m_1\overrightarrow{v}^{{\prime}}_1+m_2\overrightarrow{v}^{{\prime}}_2
   \end{equation}

donde :math:`\overrightarrow{v}_{1}`, :math:`\overrightarrow{v}_{1}^{\prime }` y :math:`\overrightarrow{v}_{2}`, :math:`\overrightarrow{v}_{2}^{\prime }` representan las velocidades iniciales y finales de los cuerpos con masas :math:`m_{1} ` y :math:`m_{2}` respectivamente. La ecuación :eq:`mom.0` en componentes cartesianas :math:`x` y :math:`y` es:

.. math::
   :label: mom.10

   \begin{equation}
    m_{1}v_{x1}+m_{2}v_{x2}=m_{1}v\prime _{x1}+m_{2}v\prime _{x2}
   \end{equation}

.. math::
   :label: mom.20

   \begin{equation}
    m_{1}v_{y1}+m_{2}v_{y2}=m_{1}v\prime _{y1}+m_{2}v\prime _{y2}
   \end{equation}

Las ecuaciones anteriores en términos de los ángulos son

.. math::
   :label: mom.1

   \begin{equation}
   m_{1}v_{1}\cos\theta_1+m_{2}v_{2}\cos\theta_2=m_{1}v_{1}\cos\theta^{{\prime}}_1+m_{2}v_{2}\cos\theta{\prime}_2
   \end{equation}

.. math::
   :label: mom.2

   \begin{equation}
    -m_{1}v_{1}\sin\theta_1+m_{2}v_{2}\sin\theta_2=m_{1}v_{1}\sin\theta^{{\prime}}_1-m_{2}v_{2}\sin\theta{\prime}_2
   \end{equation}

Para un sistema de los dos cuerpos mostrados en la :numref:`fig:cmefig1` el vector posición de su centro de masa está dado por

.. math::
   :label: mom.3

   \begin{equation}
    \overrightarrow{r}_{cm}=\frac{m_1\overrightarrow{r}_1+m_2\overrightarrow{r}_2}{m_1+m_2}
   \end{equation}

donde :math:`m_1`, :math:`\overrightarrow{r}_1` y :math:`m_2`, :math:`\overrightarrow{r}_2` representan las masas y vectores posición de las mismas medidos con respecto a un sistema de coordenadas determinado. Las coordenadas cartesianas del vector posición son

.. math::
   :label: mom.41

   \begin{equation}
    x_{cm}=\frac{m_1x_1+m_2x_2}{m_1+m_2}
   \end{equation}


.. math::
   :label: mom.42

   \begin{equation}
    y_{cm}=\frac{m_1y_1+m_2y_2}{m_1+m_2}
   \end{equation}

Las componentes cartesianas de la velocidad del centro de masa son

.. math::
   :label: mom.51

   \begin{equation}
    {v_x}_{,cm}=\frac{m_1{v_x}_{1}+m_2{v_x}_{2}}{m_1+m_2}
   \end{equation}

.. math::
   :label: mom.52

   \begin{equation}
    {v_y}_{,cm}=\frac{m_1{v_y}_{1}+m_2{v_y}_{1}}{m_1+m_2}
   \end{equation}

**Descripción del problema**

La :numref:`fig:collision_sequence` muestra una secuencia de 8 fotografías correspondientes a la colisión de dos discos de igual masa que se desplazan sobre una superficie sin fricción. Las fotografías fueron tomadas cada 2/25 de segundo. La :numref:`tab:Collision-2d_01` y la :numref:`tab:Collision-2d_02` muestran las coordenadas cartesianas :math:`x` y :math:`y` de los discos rojo y azul para los instantes de tiempo que fueron tomadas. Nótese que la primera fotografía fue tomada en :math:`t=0` s.

.. figure:: /images/Mecanica/Choques_2D/collision_sequence.png
   :alt:
   :scale: 60
   :align: center
   :name: fig:collision_sequence

   Secuencia de fotografías de la colisión de dos discos de igual masa que se deslizan sobre una superficie sin fricción. Fotografías tomadas cada 2/15 s. En rojo se muestra el sistema de coordenadas cartesianas. Los pequeños rombos de colores representan las trayectorias de los centros de los discos.

Las siguientes dos tablas muestran las coordenadas cartesianas de los centros de los discos en función del tiempo.

.. csv-table:: Disco rojo
   :header: ":math:`t` (s)", ":math:`x` (m)", ":math:`y` (m)"
   :widths: 1,1,1
   :width: 12 cm
   :name: tab:Collision-2d_01
   :align: center

   0.000 , 16.880 , -13.950
   0.133 , 16.230 , -7.178
   0.267 , 15.690 , -0.465
   0.400 , 15.200 , 6.204
   0.534 , 20.080 , 7.084
   0.667 , 25.450 , 7.434
   0.801 , 30.720 , 7.854
   0.934 , 36.020 , 8.203


.. csv-table:: Disco azul
   :header: ":math:`t` (s)", ":math:`x` (m)", ":math:`y` (m)"
   :widths: 1,1,1
   :width: 12 cm
   :name: tab:Collision-2d_02
   :align: center

   0.000, -16.610, 13.930
   0.133, -8.195, 13.780
   0.267, 0.184, 13.710
   0.400, 8.456, 13.450
   0.534, 11.250, 19.110
   0.667, 13.660, 25.120
   0.801, 15.990, 31.100
   0.934, 18.370, 36.990


**Mediciones y procedimientos**

   #. A partir de la  :numref:`tab:Collision-2d_01` y :numref:`tab:Collision-2d_02` identifique las coordenadas cartesianas de los discos rojo y azul que corresponden a sus posiciones antes y después de la colisión. Construya las gráficas de la :math:`x` y :math:`y` en función del tiempo para cada disco antes y después de la colisión. De las gráficas obtenidas encuentre las componentes cartesianas :math:`v_x` y :math:`v_y` de la velocidad para cada disco antes y después de la colisión. Verifique que el momentum del sistema compuesto por los dos discos se conserva al usar las ecuaciones :eq:`mom.10` y :eq:`mom.20`. Discuta sus resultados
   #. A partir de la tablas :numref:`tab:Collision-2d_01` y :numref:`tab:Collision-2d_02` construya una tabla que muestre las  coordenadas cartesianas :math:`x_{cm}` y :math:`y_{cm}` del centro del sistema compuesto por los dos discos para cada instante de tiempo, para ellos utilice las ecuaciones :eq:`mom.41` y :eq:`mom.42`. Demuestre que la trayectoria que describe el centro de masa es una línea recta.
   #. Con la tabla construida en el inciso anterior construya gráficas para :math:`x_{cm}` y :math:`y_{cm}` en función del tiempo. De las gráficas obtenidas encuentre las componentes cartesianas :math:`{v_x}_{,cm}` y :math:`{v_y}_{,cm}` el vector velocidad del centro de masa del sistema. Verifique sus resultados con las ecuaciones :eq:`mom.51` y :eq:`mom.52`
   #. Discuta sus resultados y escriba sus conclusiones.


