Distribución de velocidades de Maxwell
=======================================
**Objetivo**

El propósito de esta práctica es encontrar el número de partículas y la temperatura a la cual se encuentra un gas ideal conocida su distribución de velocidades.

**Recursos**

   #. Simulación 1:

       * Opción a: [#f1]_
       * Opción b: [#f2]_

   #. Simulación 2: `https://www.falstad.com/gas/ <https://www.falstad.com/gas/>`_.

**Resumen teórico**

En un gas ideal encerrado en un recipiente el único tipo de energía que tienen las partículas es energía cinética (no existe ningún tipo de interacción entre las partículas, excepto los choques). En el gas ideal, el movimiento de las moléculas es completamente al azar, es decir, todas las direcciones del espacio son igualmente probables. De acuerdo al trabajo de Maxwell-Boltzmann, la distribución de las velocidades de las moléculas de un gas ideal con :math:`N`  moléculas idénticas de masa :math:`m`: a temperatura :math:`T`, viene dada por la expresión

.. math::
   :label: Ec:Max.Dist_01

   \begin{equation}
    \frac{dn}{dv}=4\pi N (\frac{m}{4\pi kT})^{3/2}v^{2}e^{\frac{-mv^{2}}{2kT}}
   \end{equation}

donde :math:`k=1.38\times10^{-23}\,\text{J/K}` es la constante de Boltzmann. La ecuación :eq:`Ec:Max.Dist_01` proporciona el número :math:`dn` de moléculas que se mueven con una velocidad comprendida entre :math:`v` y :math:`v+dv` independientemente de la dirección del movimiento. De esta expresión se sigue que no todas las partículas se mueven con la misma velocidad, existen partículas con velocidades comprendidas desde las más bajas hasta las más altas. De la ecuación anterior se puede demostrar que  las velocidades media, cuadrática media y velocidad más probable vienen dadas por

.. math::

   \begin{eqnarray}
    <v> &=& \frac{1}{N}\int_0^{\infty}v dn =\sqrt{\frac{8kT}{\pi m}}\\
    <v^{2}> &=& \frac{1}{N}\int_0^{\infty}v^{2} dn =\frac{3kT}{ m}\rightarrow v_{rms}= \sqrt{\frac{3kT}{ m}}\\
    v_{p}=\frac{d}{dv}(\frac{dn}{dE})=0 \rightarrow v_p&=& \sqrt{\frac{2kT}{ m}}
   \end{eqnarray}

el término :math:`v_{rms}` se denomina la velocidad cuadrática media y se utiliza para el cálculo de la energía cinética media de una partícula del gas, :math:`\overline{E}_k=\frac{1}{2}mv_{rms}^{2}=\frac{3}{2}kT`.

**Descripción de la interfaz de la aplicación (Simulación 1)**

La :numref:`fig:Max_Dist_01` muestra la interfaz gráfica del usuario que permite estudiar la distribución de velocidades de un gas ideal compuesto por átomos de He a determinada temperatura. Presione el botón **RUN** para comenzar la simulación.  La interfaz permite observar la formación del histograma de la distribución de velocidades de un gas formado por :math:`N` átomos de He. Inicialmente, todos los átomos tienen la misma velocidad, pero debido a las colisiones sus velocidades cambian. A medida que el tiempo pasa se logra el equilibrio (en el histograma, la distribución de las velocidades no cambia, espere unos minutos). La curva continua en color cian en la gráfica, muestra la distribución de velocidades de Maxwell-Boltzman dada por la :eq:`Ec:Max.Dist_01`. Una de las partículas en la simulación tiene un color diferente con el fin de poder seguir su trayectoria.

.. figure:: /images/Oscilaciones_Termo/Maxwell_Distribution/Mx_Dist_gui_01.png
   :scale: 40
   :align: center
   :name: fig:Max_Dist_01

   Distribución de velocidades de un gas ideal compuesto por átomos de He

**Descripción de la interfaz de la aplicación (Simulación 2)**

La :numref:`fig:Max_Dist_02` muestra la interfaz gráfica del usuario que permite estudiar la distribución de velocidades de un gas ideal. La simulación muestra el movimiento al azar de las partículas que componen el gas y su distribución de velocidades dada por la ecuación :eq:`Ec:Max.Dist_01`. Los colores azul, rojo, amarillo y blanco significan que las moléculas tienen velocidades cada vez más grandes. En la simulación se puede ver entre otras: a) el efecto de la fuerza de la gravedad en la distribución de velocidades (barra de desplazamiento rotulada **gravity**, b) el efecto de la temperatura en la distribución de la velocidades, para ello seleccione la opción **Heater**, fije el valor de la temperatura con la barra de desplazamiento **Heater temperature** y presione el botón **Reset**, c) el efecto del tamaño de las moléculas, para ello seleccione del menú desplegable la opción Setup: 1 Gas, Small, d) el efecto de las distribuciones cuando se tienen dos gases con partículas de diferentes masas y tamaños, para ello seleccione del menú desplegable la opción Setup: 2 Gases, Random Speeds e) la distribución de la energía de las partículas en el gas (opción **Energy Distribution**), etc.

.. figure:: /images/Oscilaciones_Termo/Maxwell_Distribution/Mx_Dist_gui_02.png
   :scale: 65
   :align: center
   :name: fig:Max_Dist_02

   Distribución de velocidades de un gas ideal

**Mediciones y procedimientos**

**Simulación 1**

   #. Una vez iniciada la simulación, espere a que se alcance el equilibrio.
   #. Del histograma mostrado en la interfaz determine el número :math:`N` de átomos de He que componen el gas.
   #. Determine la temperatura del gas.
   #. Determine la energía cinética media de un átomo de He.
   #. Determine la energía interna del gas.
   #. Determine el número de choques por segundo de los átomos contra la pared. (Para esta parte, investigue la expresión que permite el cálculo)
   #. Discuta sus resultados y escriba sus conclusiones.

**Simulación 2**

   #. Del menú desplegable seleccione la opción Setup: 1 Gases, Random Speeds. Varíe la temperatura del gas, desde la más baja hasta las más alta posible y observe el comportamiento de la curva de distribución de velocidades. ¿Qué se esperaría si el valor de la temperatura del gas tiende a cero? ¿Cuál sería el comportamiento de las velocidades de las partículas que componen el gas? ¿Qué le sucede a la energía interna del gas? Responda las mismas preguntas, pero esta vez cuando la temperatura del gas ideal se hace muy grande.
   #. Del menú desplegable seleccione: la opción Setup: 1 Gases, Random Speeds y la opción **Energy distribution**. Observe la forma de la curva de la distribución de energía de las partículas del gas. ¿Cuál es el significado de esta curva y por qué razón tiene que ser monótonamente decreciente?
   #. Responda las mismas preguntas anteriores pero esta vez cuando el gas está formado por dos gases diferentes.
   #. Discuta sus resultados y escriba sus conclusiones.


.. [#f1] Instrucciones para ejecutar la simulación 1. Haga click en el enlace <https://drive.google.com/file/d/16iahc__0xN-eJe7xCkvzQttlxqLAdwI4/view?usp=sharing. En seguida aparece una página con una gran cantidad de código. No se preocupe, todo está bien.  Abra un editor de texto plano como por ejemplo el *Notepad* y  coloque el código copiado en este archivo, luego salve el archivo con el nombre **gas.html**. Para ejecutar la aplicación haga doble clic en el archivo!
.. [#f2] Alternativa para ejecutar la simulación 1: Descarque el archivo y haga doble click sobre este. :download:`Gas.html <Downloadable/Maxwell_Distribution/gas.html>`.