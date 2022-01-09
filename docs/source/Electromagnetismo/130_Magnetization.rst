Magnetización de un imán
==========================

**Objetivo**

El propósito de esta práctica es calcular la magnetización de un imán en forma de barra a partir de las mediciones de campo magnético.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/es/simulation/legacy/magnets-and-electromagnets <https://phet.colorado.edu/es/simulation/legacy/magnets-and-electromagnets>`_.

**Resumen teórico**

Se denomina momento dipolar magnético (o simplemente momento magnético) a la cantidad vectorial definida como :math:`\overrightarrow{\mu}=IA\hat{u}`, donde :math:`I` es la corriente eléctrica que circula por una espira de área :math:`A` y :math:`\hat{u}` en un vector unitario perpendicular al plano de la espira y que sigue la regla de la mano derecha. La :numref:`Magnetic_dipole` muestra la similitud entre las líneas de campo magnético de un imán pequeño y un dipolo magnético. El momento magnético :math:`\overrightarrow{\mu}` mide la tendencia de un objeto a interactuar con un campo magnético externo. En RMN (resonancia magnética nuclear), el objeto de interés es típicamente una molécula, átomo, núcleo o partícula subatómica. \newline

.. figure:: /images/Electromagnetismo/Magnetization/MagneticDipole_01.png
   :scale: 70
   :align: center
   :name: Magnetic_dipole

   Similitud entre las líneas de campo magnético de un imán y un dipolo magnético.



Cada electrón en un átomo gira alrededor del núcleo generando corrientes muy pequeñas, y cada uno de estos dipolos genera un campo magnético y por tanto el campo magnético total en un punto del espacio es la suma de los campos de cada uno de los dipolos magnéticos. Los átomos pueden o no presentar un momento dipolar magnético neto, dependiendo de la simetría o de la orientación relativa de las órbitas. Como la mayoría de las moléculas no presentan simetría esférica, pueden tener un momento dipolar magnético permanente, debido a la orientación especial de las órbitas electrónicas. Una porción de materia, con la excepción de los materiales ferromagnéticos, no presenta momento magnético neto, debido a la orientación al azar de las moléculas.
Se denomina magnetización :math:`\overrightarrow{M}` de un material como el momento magnético del medio por unidad de volumen. Si :math:`\overrightarrow{\mu}` es el momento dipolar magnético de cada átomo o molécula y :math:`m` es el número de átomos o moléculas por unidad de volumen la magnetización es igual a :math:`\overrightarrow{M}=m\overrightarrow{\mu}`, y sus unidades son amperio/metro, es decir, A/m. Ejemplo de cuerpos con una magnetización muy grande lo constituyen los imanes.\newline
Se puede demostrar que la componente :math:`x` del campo magnético generado por un imán en forma de prisma con dimensiones :math:`2a`, :math:`2b` y :math:`2c` (ver :numref:`magnet_bar`) en puntos que se encuentran sobre el eje :math:`x`, para :math:`|x|>a` es

.. math::
   :label: Ec:Magnetiz_01

   \begin{equation}
    B(x)=\frac{\mu_0M}{\pi}\bigg( \arctan\frac{bc}{(x-a)\sqrt{b^{2}+c^{2}+(x-a)^{2}}}-\arctan\frac{bc}{(x+a)\sqrt{b^{2}+c^{2}+(x+a)^{2}}}\bigg)
   \end{equation}

donde :math:`\mu _{0}=4\pi \times 10^{-7}\text{L}\cdot \text{m/A}` es la permeabilidad del vacío, :math:`M` es la magnetización que está dirigida a lo largo del eje :math:`+x`.

.. figure:: /images/Electromagnetismo/Magnetization/magnet_bar_prisma.png
   :scale: 80
   :align: center
   :name: magnet_bar

   Barra magnética de dimensiones :math:`2a`, :math:`2b` y :math:`2c`

**Descripción de interfaz de la aplicación**

La :numref:`fig:Magnetiz_gui_02` muestra la interfaz gráfica del usuario que permite determinar la magnetización de una barra imantada. La simulación presenta un imán en forma de prisma el cual se puede localizar en cualquier parte de la pantalla. Se cuenta con un medidor de campo magnético el cual da la lectura de las componentes :math:`x` y :math:`y` de sus componentes en Gauss (1 Gauss, G = 0.0001 Tesla, T) en puntos cercanos al imán. También, se cuenta con una brújula móvil que da la orientación del campo magnético generado por el imán y la zona de trabajo está poblada por pequeñas agujas imantadas espaciadas de manera \texttt{equidistante}. La magnetización del imán controla con la barra de desplazamiento rotulada **Fuerza**.

.. figure:: /images/Electromagnetismo/Magnetization/gui_01.png
   :scale: 50
   :align: center
   :name: fig:Magnetiz_gui_02

   Interfaz gráfica del usuario


**Mediciones y procedimientos**

Asuma las siguientes dimensiones para el prisma :math:`2c=6.0\,\text{u.l}`, :math:`2a=2b=1.0\,\text{u.l}`, donde u.l es una unidad de longitud arbitraria.

   #. Fije la fuerza del imán en un valor igual al 75\% u otro valor que desee. Entre mayor mejor, para efecto de las mediciones de campo magnético
   #. Coloque el imán a la izquierda de la zona de trabajo como indica la :numref:`fig:Magnetiz_gui_01`. Realice mediciones de campo magnético a lo largo del eje de simetría del imán (línea de color azul). Se toma el centro del imán como origen de coordenadas. Complete la :numref:`Tab:readings_01`.
   #. Realice una gráfica de :math:`B` en función de :math:`x`
   #. A la gráfica obtenida en el inciso anterior superponga la curva teórica dada por la ecuación :eq:`Ec:Magnetiz_01`. Ajuste el valor de :math:`M` de modo que la curva coincida con la experimental.
   #. Ayuda: si sus procedimientos son correctos, el valor obtenido para :math:`M` debería estar en el rango comprendido entre 30 y 40 kA/m. Discuta sus resultados.


      .. figure:: /images/Electromagnetismo/Magnetization/gui_02.png
         :scale: 50
         :align: center
         :name: fig:Magnetiz_gui_01

         Ubicación del imán y su eje de simetría


      .. csv-table:: Datos de posición e intensidad del campo magnético a lo largo del eje de simetría del imán
         :header: "Posición, :math:`x` (u.l)", "Intensidad, :math:`B` (T)"
         :widths: 1,1
         :width: 15 cm
         :name: Tab:readings_01
         :align: center
         :stub-columns: 0
         :header-rows: 0

         3.5,.
         4.0,.
         5.0,.
         6.0,.
         7.0,.
         8.0,.
         9.0,.
         10.0,.
         11.0,.
         12.0,.
         13.0,.

**Análisis y preguntas**

   #. ¿Qué tiene que ver la magnetización con los materiales ferromagnéticos, paramagnéticos y diamagéticos?
   #. ¿Qué es la temperatura de Curie?
   #. Cite ejemplos tecnológicos de aplicación de la magnetización.




