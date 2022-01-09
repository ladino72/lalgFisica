+Aceleración de la gravedad
============================

**Objetivo**

En esta práctica se calcula el valor de la aceleración de la gravedad. Para ello se suelta una lámina rectangular de acrílico con franjas oscuras y claras dispuestas de manera alterna e igualmente espaciadas, las cuales  obstruyen el paso de luz en un fotointerruptor a medida que la lámina desciende. Los instantes de tiempo en que ocurre la interrupción son medidos por un circuito conectado a la computadora. A partir de las  poisiones de las franjas y los tiempos de interrupción medidos se determina el valor de *g*.

**Recursos**

   #. Una lámina de transparente de acrílico con franjas oscuras y claras dispuestas alternamente. (Dimensiones aproximadas 30 cm x 5 cm  y espesor entre 2 y 4 mm.)
   #. Un fotointerruptor conectado a la computadora.
   #. Una regla graduada en mm.

**Resumen teórico**

Cuando un cuerpo se mueve en línea recta con aceleración constante :math:`a`, las ecuaciones cinemáticas que describen su posición y velocidad son

.. math::
   :label: Ec:gv_01

   \begin{equation}
    x =x_0+v_0t+\frac{1}{2}at^{2}
   \end{equation}

.. math::
   :label: Ec:gv_02

   \begin{equation}
    v =v_0+at
   \end{equation}

donde :math:`v_{0}`  y :math:`x_0` representan la velocidad y posición a la que se encuentra el cuerpo en :math:`t=0`.

**Descripción del problema**

Consideremos el sistema que se muestra en la :numref:`fig:grfig1`, el cual consta de una lámina de acrílico transparente con franjas oscuras y claras dispuestas de manera alterna y paralela (denominada cebra) la cual atraviesa el fotointerruptor en caída libre. Al pasar las franjas oscuras por el fotointerruptor este es interrumpido; las interrupciones suceden justamente al comienzo de la franja oscura y el hardware registra estos instantes de tiempo. Sean :math:`x_0`, :math:`x_1`, :math:`x_2`, :math:`x_3` ... :math:`x_n` las distancias medidas directamente sobre la cebra,  y :math:`t_0`, :math:`t_1`, :math:`t_2`, :math:`t_3` ... :math:`t_n` los instantes de tiempo que el reloj registra para estas posiciones. Con esta información construimos la :numref:`tab:tabla1`.



  .. figure:: /images/Mecanica/Gravity/grfig1.png
      :alt:
      :scale: 80
      :align: center
      :name: fig:grfig1

      Posiciones de las :math:`N+1` franjas oscuras de la cebra con respecto a un punto de referencia (un extremo de la cebra), la elección de este punto es arbitraria y en la práctica se toma de modo que coincida con el comienzo de la primera franja oscura, es decir, se toma de modo que :math:`x_0=0`


Para determinar el valor de la aceleración de caída de la cebra usaremos el siguiente resultado,

.. note::

   Cuando una partícula se mueve en línea recta con aceleración constante, el valor medio o promedio de su velocidad en el intervalo de tiempo comprendido entre :math:`t_i` y :math:`t_j` *es igual a su velocidad instantánea en* :math:`t=t_i+\frac{\Delta t_{ij}}{2}`, *donde* :math:`\Delta t_{ij} =t_j-t_i`. Ver demostración [#f1]_


Al ser la aceleración constante, la relación entre la velocidad y el tiempo es lineal. Ahora bien, consideremos las velocidades para los tres instantes de tiempo :math:`t_{n-1}`, :math:`t_{n}` y :math:`t_{n+1}`, ver :numref:`fig:grfig4`. Apliquemos el resultado enunciado de arriba a los intervalos de tiempo comprendidos entre :math:`t_{n-1}`  y :math:`t_n` y :math:`t_{n}`  y :math:`t_{n+1}`, las velocidades en los instantes de tiempo :math:`t_{n-1}+\frac{t_n-t_{n-1}}{2}` y :math:`t_{n}+\frac{t_{n+1}-t_{n}}{2}` vienen dadas :math:`\overline{v}_{n-1,n}` y :math:`\overline{v}_{n,n+1}` respectivamente. Estas velocidades satisfacen la ecuación :eq:`Ec:gv_02`,

.. math::
   :label: Ec:gv_03

   \begin{equation}
    \overline{v}_{n-1,n} = a(t_{n-1}+\frac{\Delta t_{n-1,n}}{2})+v_0
   \end{equation}

.. math::
   :label: Ec:gv_04

   \begin{equation}
    \overline{v}_{n,n+1}= a(t_{n}+\frac{\Delta t_{n,n+1}}{2})+v_0
   \end{equation}

donde por definición :math:`\overline{v}_{n-1,n}=\frac{\Delta x_{n-1,n}}{\Delta t_{n-1,n}}=\frac{x_n-x_{n-1}}{t_n-t_{n-1}}` y :math:`\overline{v}_{n,n+1}=\frac{\Delta x_{n,n+1}}{\Delta t_{n,n+1}}=\frac{x_{n+1}-x_n}{t_{n+1}-t_n}`

Al despejar :math:`a` y :math:`v_0`  del sistema de ecuaciones dado por :eq:`Ec:gv_03` y :eq:`Ec:gv_04` resulta

.. math::
   :label: Ec:gv_05

   \begin{equation}
    a =\frac{2(\overline{v}_{n,n+1}-\overline{v}_{n-1,n})}{t_{n+1}-t_{n-1}}
   \end{equation}

.. math::
   :label: Ec:gv_06

   \begin{equation}
    v_0= \frac{\overline{v}_{n-1,n}[t_{n+1}+t_{n}]-\overline{v}_{n,n+1}[t_{n-1}+t_n]}{ t_{n+1}- t_{n-1}}
   \end{equation}

Así, la ecuación :eq:`Ec:gv_02` se convierte explícitamente en:

.. math::
   :label: Ec:gv_07

   \begin{equation}
    v=\frac{\overline{v}_{n-1,n}[t_{n+1}+t_{n}]-\overline{v}_{n,n+1}[t_{n-1}+t_n]}{ t_{n+1}- t_{n-1}}+\frac{2(\overline{v}_{n,n+1}-\overline{v}_{n-1,n})}{t_{n+1}-t_{n-1}}t
   \end{equation}


La ecuación :eq:`Ec:gv_07` es muy importante, pues permite calcular la velocidad instantánea de caída de la cebra para cualquier tiempo en términos de las posiciones e instantes de tiempo registrados en la :numref:`tab:tabla1`. En particular, la velocidad para el instante de tiempo :math:`t=t_n` después de realizar algo de algebra elemental, es dada por

.. math::
   :label: Ec:gv_08

   \begin{equation}
    v_{n}=\frac{\overline{v}_{n,n+1}\Delta t_{n-1,n}+\overline{v}_{n-1,n}\Delta t_{n,n+1}}{\Delta t_{n-1,n+1}}
   \end{equation}

donde :math:`\Delta t_{n-1,n+1}=t_{n+1}- t_{n-1}`. Obsérvese que la expresión :eq:`Ec:gv_08` es una ecuación recursiva y que los valores del subíndice :math:`N` son dados por :math:`n=1,2,3,...,N-1`, donde :math:`N+1` es el número de parejas :math:`(x_n,t_n)` conisideradas. Además, con los valores de las velocidades instantáneas :math:`v_1, v_2, v_3,...,v_{N-1}` para los correspondientes instantes de tiempo  :math:`t_1, t_2, t_3,...,t_{N-1}` se construye la gráfica de velocidad en función del tiempo, ver :numref:`fig:grfig4`, cuya pendiente corresponde a la aceleración de caída de la cebra (aceleración de la gravedad).


.. csv-table:: Tabla de datos para medir la aceleración.
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 10 cm
      :name: tab:tabla1
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`\vdots` , :math:`\vdots`
      :math:`x_{N}` , :math:`t_{n}`


.. figure:: /images/Mecanica/Gravity/grfig4.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:grfig4

   Velocidad en función del tiempo.


**Mediciones**

Realice el montaje experimental que se muestra en la  :numref:`fig:grfig3`. Verifique que el modo de operación del reloj sea el Modo 1. Suelte la cebra desde diferentes alturas con respecto al fotointerruptor y con las mediciones de tiempo y distancia construya la tabla :numref:`tab:tabla3`, :numref:`tab:tabla4`, :numref:`tab:tabla5`, :numref:`tab:tabla6` y la :numref:`tab:tabla7`  para cada valor de altura señalado.

.. figure:: /images/Mecanica/Gravity/grfig3.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:grfig3

   Arreglo experimental para determinar :math:`g`.


.. csv-table:: Posición en función del tiempo para :math:`h=2\,\text{cm}`
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla3
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`x_{6}` , :math:`t_{6}`
      :math:`x_{7}` , :math:`t_{7}`


.. csv-table:: Posición en función del tiempo para :math:`h=4\,\text{cm}`
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla4
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`x_{6}` , :math:`t_{6}`
      :math:`x_{7}` , :math:`t_{7}`

.. csv-table:: Posición en función del tiempo para :math:`h=6\,\text{cm}`
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla5
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`x_{6}` , :math:`t_{6}`
      :math:`x_{7}` , :math:`t_{7}`

.. csv-table:: Posición en función del tiempo para :math:`h=8\,\text{cm}`
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla6
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`x_{6}` , :math:`t_{6}`
      :math:`x_{7}` , :math:`t_{7}`

.. csv-table:: Posición en función del tiempo para :math:`h=10\,\text{cm}`
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla7
      :align: center

      :math:`x_{0}` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`x_{6}` , :math:`t_{6}`
      :math:`x_{7}` , :math:`t_{7}`



A partir de los datos en la :numref:`tab:tabla3`, :numref:`tab:tabla4`, :numref:`tab:tabla5`, :numref:`tab:tabla6` y la :numref:`tab:tabla7` construya la tab:tabla :numref:`tab:tabla8`, :numref:`tab:tabla9`, :numref:`tab:tabla10`, :numref:`tab:tabla11` y la :numref:`tab:tabla12` de velocidad instantánea en función del tiempo.

A modo de ejemplo, supongamos que deseamos calcular el valor de la velocidad del cuerpo para el instante de tiempo :math:`t=t_5`. De la ecuación :eq:`Ec:gv_08` resulta

.. math::
   :label: Ec:gv_09

   \begin{equation}
    v_{5}=\frac{\overline{v}_{5,6}\Delta t_{4,5}+\overline{v}_{4,5}\Delta t_{5,6}}{\Delta t_{4,6}}
   \end{equation}


donde :math:`\overline{v}_{5,6}=\frac{x_6-x_5}{t_6-t_5}`, :math:`\Delta t_{4,5}=t_5-t_4` y :math:`\overline{v}_{4,5}=\frac{x_5-x_4}{t_5-t_4}` y :math:`\Delta t_{5,6}=t_6-t_5`.

En una misma gráfica represente la velocidad en función del tiempo para cada una de las alturas consideradas. Linealice sus datos usando el método de los mínimos cuadrados y obtenga el valor de las pendientes. ¿Cuál es el  valor de la aceleración de la gravedad a partir de las pendientes  obtenidas? \textquestiondown Depende la aceleración de caída de la cebra del valor de la altura inicial desde donde se soltó? Discuta sus resultados.
Grafique los datos de posición en función del tiempo para cada una de las alturas establecidas en una hoja de cálculo, por ejemplo Excel. Ajuste la curva a una función polinómica de grado 2 similar a la dada por la relación :eq:`Ec:gv_01`. El valor de la aceleración se obtiene directamente del coeficiente que acompaña al término de grado 2 multiplicado por 2. Compare el valor de  la aceleración de la gravedad obtenida de esta manera con la obtenida en el inciso previo. Discuta sus resultados. ¿Cuál método es mejor?



.. csv-table:: Tabla de datos de velocidad en función del tiempo para :math:`h=2\,\text{cm}`
      :header: "Velocidad", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla8
      :align: center

      :math:`v_{1}` , :math:`t_{1}`
      :math:`v_{2}` , :math:`t_{2}`
      :math:`v_{3}` , :math:`t_{3}`
      :math:`v_{4}` , :math:`t_4`
      :math:`v_{5}` , :math:`t_{5}`
      :math:`v_{6}` , :math:`t_{6}`
      :math:`v_{7}` , :math:`t_{7}`


.. csv-table:: Tabla de datos de velocidad en función del tiempo para :math:`h=4\,\text{cm}`
      :header: "Velocidad", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla9
      :align: center

      :math:`v_{1}` , :math:`t_{1}`
      :math:`v_{2}` , :math:`t_{2}`
      :math:`v_{3}` , :math:`t_{3}`
      :math:`v_{4}` , :math:`t_4`
      :math:`v_{5}` , :math:`t_{5}`
      :math:`v_{6}` , :math:`t_{6}`
      :math:`v_{7}` , :math:`t_{7}`

.. csv-table:: Tabla de datos de velocidad en función del tiempo para :math:`h=6\,\text{cm}`
      :header: "Velocidad", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla10
      :align: center

      :math:`v_{1}` , :math:`t_{1}`
      :math:`v_{2}` , :math:`t_{2}`
      :math:`v_{3}` , :math:`t_{3}`
      :math:`v_{4}` , :math:`t_4`
      :math:`v_{5}` , :math:`t_{5}`
      :math:`v_{6}` , :math:`t_{6}`
      :math:`v_{7}` , :math:`t_{7}`


.. csv-table:: Tabla de datos de velocidad en función del tiempo para :math:`h=8\,\text{cm}`
      :header: "Velocidad", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla11
      :align: center

      :math:`v_{1}` , :math:`t_{1}`
      :math:`v_{2}` , :math:`t_{2}`
      :math:`v_{3}` , :math:`t_{3}`
      :math:`v_{4}` , :math:`t_4`
      :math:`v_{5}` , :math:`t_{5}`
      :math:`v_{6}` , :math:`t_{6}`
      :math:`v_{7}` , :math:`t_{7}`


.. csv-table:: Tabla de datos de velocidad en función del tiempo para :math:`h=10\,\text{cm}`
      :header: "Velocidad", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:tabla12
      :align: center

      :math:`v_{1}` , :math:`t_{1}`
      :math:`v_{2}` , :math:`t_{2}`
      :math:`v_{3}` , :math:`t_{3}`
      :math:`v_{4}` , :math:`t_4`
      :math:`v_{5}` , :math:`t_{5}`
      :math:`v_{6}` , :math:`t_{6}`
      :math:`v_{7}` , :math:`t_{7}`

.. [#f1] Cuando un cuerpo se mueve en línea recta con aceleración constante :math:`a`, su velocidad en función del tiempo es dada por  :math:`v=v_0+at`, ver figura de abajo. La velocidad media entre los instantes de tiempo :math:`t_i` y :math:`t_j` es dada por  :math:`\overline{v}_{i,j}=\frac{v_i+v_j}{2}=\frac{v_0+at_i+v_0+at_j}{2}=v_0+a\frac{t_i+t_j}{2}`. Por otra parte, la velocidad instantánea del cuerpo para el instante de tiempo :math:`t_{ij}=t_i+\frac{t_j-t_i}{2}=t_i+\frac{\Delta t_{i,j}}{2}` es dada por :math:`v=v_0+a(t_i+\frac{t_j-t_i}{2})=v_0+a(\frac{t_i+t_j}{2})`. Así, las dos velocidades son iguales :math:`\blacksquare`.

         .. figure:: /images/Mecanica/Gravity/grfig5.png
            :alt:
            :scale: 110
            :align: center
            :name: fig:grfig5

