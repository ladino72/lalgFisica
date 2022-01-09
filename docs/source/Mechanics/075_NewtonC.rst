+Segunda ley de Newton
======================================

**Objetivo**

El propósito de esta práctica de determinar el valor de la fuerza de fricción :math:`f` sobre un carrito al moverse a lo largo de un riel rectilíneo. Para ello, se considera un sistema compuesto por el carrito y una masa conectados mediante una cuerda ligera, la cual pasa por una polea. A partir de las mediciones de aceleración del sistema (determinadas al usar una cebra y un foto interruptor) para diferentes masas del cuerpo que pende de la cuerda y manteniendo la masa del sistema constante se obtiene el valor de :math:`f`. Adicionalmente se obtiene el momento de inercia de la polea.

**Recursos**


   #. Un riel con carrito.
   #. Un juego de pesas (masa :math:`m_{2}`).
   #. Una balanza.
   #. Una cebra.
   #. Un fotointerruptor conectado al computador mediante una interfase.
   #. Una regla graduada en mm.


**Resumen teórico**

La segunda ley de Newton establece que la rata de cambio de momentum de un sistema es igual a la fuerza neta :math:`\overrightarrow{F}` que actua sobre el
sistema. Explicitamente, :math:`\overrightarrow{F}=\frac{d\overrightarrow{p}}{dt}`, donde :math:`\overrightarrow{p}` es el momentum del sistema. Si la masa :math:`m` del
sistema es constante entonces :math:`\overrightarrow{F}=\frac{d(m\overrightarrow{v}%
)}{dt}=m\overrightarrow{a}` donde :math:`\overrightarrow{a}=\frac{d\overrightarrow{v}}{dt}` es la aceleración del cuerpo. En otras palabras la
aceleración del sistema es proporcional a la fuerza aplicada al mismo.

Cuando un cuerpo se mueve en línea recta con aceleración constante :math:`a`, las ecuaciones cinemáticas que describen su posición y velocidad son

.. math::
   :label: Ec:pos_01

   \begin{equation}
    x =x_0+v_0t+\frac{1}{2}at^{2}
   \end{equation}

.. math::
   :label: Ec:pos_02

   \begin{equation}\label{Ec:pos_02}
    v =v_0+at
   \end{equation}

donde :math:`v_0`  y :math:`x_0` representan la velocidad y posición a la que se encuentra el cuerpo en :math:`t=0`.

**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:newCfig4`. Supongamos que el sistema esta en movimiento y
que existe una fuerza de rozamiento :math:`f` sobre el carrito de masa :math:`m_{1}`. Además, consideremos que la polea tiene masa no despreciable. La :numref:`fig:newCfig3` muestra las fuerzas que actúan sobre el carrito, la masa colgante y la polea. Usando la segunda ley de Newton al carrito y masa colgante resulta

.. math::
   :label: Ec:newC.1

   \begin{equation}
    T_{1}-f=m_{1}a
   \end{equation}

.. math::
   :label: Ec:newC.2

   \begin{equation}
    m_{2}g-T_{2}=m_{2}a
   \end{equation}

.. figure:: /images/Mecanica/NewtonC/newCfig4.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:newCfig4

   Sistema compuesto por carrito y masa colgante de masas :math:`m_1` y :math:`m_2` respectivamente.


.. figure:: /images/Mecanica/NewtonC/newCfig3.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:newCfig3

   Fuezas sobre el carrito, masa colgante y la polea de masa :math:`m`.

donde :math:`a`  representa la aceleración del sistema carrito y masa colgante. Obsérvese, que la tensión de la cuerda no es la misma en todos sus puntos. Si esta fuera igual, la polea no rotaría. Similarmente, aplicando la segunda ley de Newton a la polea resulta

.. math::
   :label: Ec:newC.3

   \begin{equation}
    (T_{2}-T_{1})R=I\alpha =I\frac{a}{R}
   \end{equation}

donde :math:`I` es el momento de inercia de la polea y :math:`\alpha` es su aceleración angular. La relación entre la aceleración lineal :math:`a` y angular :math:`\alpha` es dada por la expresión :math:`a=\alpha R`.

De las expresiones :eq:`Ec:newC.1`, :eq:`Ec:newC.2`, :eq:`Ec:newC.3` se obtiene

.. math::
   :label: Ec:newC.4

   \begin{equation}
   (m_{1}+m_{2}+\frac{I}{R^{2}})a=m_{2}g-f
   \end{equation}

Imponiendo la condición

.. math::
   :label: Ec:newC.5

   \begin{equation}
    m_{1}+m_{2}=M = constante
   \end{equation}

junto con la expresión :eq:`Ec:newC.4` se obtiene

.. math::
   :label: Ec:newC.6

   \begin{equation}
    a=\frac{m_2g}{M+\frac{I}{R^2}}-\frac{f}{M+\frac{I}{R^2}}
   \end{equation}

El valor de la aceleración :math:`a` se mide experimentalmente para cada valor de la masa :math:`m_{2}` teniendo cuidado en todo momento de mantener la condición dada por :eq:`Ec:newC.5`. Diferentes valores de :math:`m_{2}` producen diferentes valores aceleración del sistema. Para ello, se usa el foto interruptor y la cebra instalada sobre el carrito como se describe más adelante.

Al analizar la expresión :eq:`Ec:newC.6` vemos que la relación entre :math:`a` y :math:`m_{2}` es lineal. Por tanto, de la gráfica de :math:`a` en función de :math:`m_{2}` (ver :numref:`fig:newCfig5`) obtenemos la pendiente

.. math::
   :label: Ec:newC.6a

   \begin{equation}
    p=\frac{g}{M+\frac{I}{R^2}}
   \end{equation}

y el punto de intercepción :math:`b` de la recta con el eje vertical,

.. math::
   :label: Ec:newC.6b

   \begin{equation}
    b=-\frac{f}{M+\frac{I}{R^2}}
   \end{equation}


De los valores de :math:`p` y :math:`b` obtenemos

.. math::
   :label: Ec:newC.6c

   \begin{equation}
    f=-\frac{b}{p}g
   \end{equation}

Así, el valor de :math:`f` lo determinan los valores de :math:`p` y :math:`b`, los cuales se obtienen indirectamente a partir de mediciones de aceleración. Nótese que no se requiere conocer el valor del momento de inercia :math:`I` de la polea para hallar :math:`f`. De las expresiones anteriores para :math:`p` y :math:`b` se sigue que:

.. math::
   :label: Ec:newC.7

   \begin{equation}
   I=(\frac{g}{p}-M)R^{2}
   \end{equation}

.. figure:: /images/Mecanica/NewtonC/newCfig5.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:newCfig5

   Aceleración del sistema en función de la masa :math:`m_2` para el sistema mostrado en la :numref:`fig:newCfig4`.


**Medición de la aceleración**

Para medir la aceleración utilizamos el montaje que se muestra en la :numref:`fig:newCfig2`. Sobre el carrito se instala una lámina de acrílico transparente con franjas oscuras y claras dispuestas de manera alterna y paralela (denominada cebra, ver :numref:`fig:grfig10`). Al pasar las franjas oscuras por el fotointerruptor este es interrumpido; las interrupciones suceden justamente al comienzo de la franja oscura y el hardware registra estos instantes de tiempo. Sean :math:`x_0`, :math:`x_1`, :math:`x_2`, :math:`x_3` ... :math:`x_n` las distancias medidas directamente sobre la cebra, y :math:`t_0`, :math:`t_1`, :math:`t_2`, :math:`t_3` ... :math:`t_n` los instantes de tiempo que el reloj registra para estas posiciones. Con esta información construimos la :numref:`tab:Ctabla1`.

.. figure:: /images/Mecanica/NewtonC/newCfig2.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:newCfig2

   Sistema para medir la aceleración.


.. figure:: /images/Mecanica/NewtonC/newtoncgrfig1.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:grfig10

   Posiciones de las :math:`N+1` franjas oscuras de la cebra con respecto a un punto de referencia (un extremo de la cebra), la elección de este punto es arbitraria y en la práctica se toma de modo que coincida con el comienzo de la primera franja oscura, es decir, se toma de modo que :math:`x_0=0`


Para determinar el valor de la aceleración de caída de la cebra usaremos el siguiente resultado,

.. note::

   Cuando una partícula se mueve en línea recta con aceleración constante, el valor medio o promedio de su velocidad en el intervalo de tiempo comprendido entre} :math:`t_i` y :math:`t_j` \emph{es igual a su velocidad instantánea en} :math:`t=t_i+\frac{\Delta t_{ij}}{2}`, donde :math:`\Delta t_{ij} =t_j-t_i` . Ver demostración [#f1]_


Al ser la aceleración constante, la relación entre la velocidad y el tiempo es lineal. Ahora bien, consideremos las velocidades para los tres instantes de tiempo :math:`t_{n-1}`, :math:`t_{n}` y :math:`t_{n+1}`, ver :numref:`fig:newCgrfig4`. Apliquemos el resultado enunciado arriba a los intervalos de tiempo comprendidos entre :math:`t_{n-1}`  y :math:`t_n` y :math:`t_{n}`  y :math:`t_{n+1}`, las velocidades en los instantes de tiempo :math:`t_{n-1}+\frac{t_n-t_{n-1}}{2}` y :math:`t_{n}+\frac{t_{n+1}-t_{n}}{2}` vienen dadas :math:`\overline{v}_{n-1,n}` y :math:`\overline{v}_{n,n+1}` respectivamente. Estas velocidades satisfacen la ecuación :eq:`Ec:pos_02`,

.. math::
   :label: Ec:pos_03

   \begin{equation}
    \overline{v}_{n-1,n} = a(t_{n-1}+\frac{\Delta t_{n-1,n}}{2})+v_0
   \end{equation}

.. math::
   :label: Ec:pos_04

   \begin{equation}
    \overline{v}_{n,n+1}= a(t_{n}+\frac{\Delta t_{n,n+1}}{2})+v_0
   \end{equation}

donde por definición :math:`\overline{v}_{n-1,n}=\frac{\Delta x_{n-1,n}}{\Delta t_{n-1,n}}=\frac{x_n-x_{n-1}}{t_n-t_{n-1}}` y :math:`\overline{v}_{n,n+1}=\frac{\Delta x_{n,n+1}}{\Delta t_{n,n+1}}=\frac{x_{n+1}-x_n}{t_{n+1}-t_n}`

Al despejar :math:`a` y :math:`v_0` del sistema de ecuaciones dado por :eq:`Ec:pos_03` y :eq:`Ec:pos_04` resulta:

.. math::
   :label: Ec:pos_05

   \begin{equation}
    a =\frac{2(\overline{v}_{n,n+1}-\overline{v}_{n-1,n})}{t_{n+1}-t_{n-1}}
   \end{equation}

.. math::
   :label: Ec:pos_06

   \begin{equation}
   v_0= \frac{\overline{v}_{n-1,n}(2\Delta t_{n-1,n}+\Delta t_{n,n+1})-2t_{n-1}\overline{v}_{n,n+1}}{\Delta t_{n-1,n}+\Delta t_{n,n+1}}
   \end{equation}

Así, la ecuación :eq:`Ec:pos_02` se convierte explícitamente en:

.. math::
   :label: Ec:pos_07

   \begin{equation}
    v=\frac{\overline{v}_{n-1,n}(2\Delta t_{n-1,n}+\Delta t_{n,n+1})-2t_{n-1}\overline{v}_{n,n+1}}{\Delta t_{n-1,n}+\Delta t_{n,n+1}}+\frac{2(\overline{v}_{n,n+1}-\overline{v}_{n-1,n})}{t_{n+1}-t_{n-1}}t
   \end{equation}

La ecuación :eq:`Ec:pos_07` es muy importante, pues permite calcular la velocidad instantánea del carrito para cualquier tiempo en términos de las posiciones e instantes de tiempo registrados en la :numref:`tab:Ctabla1`. En particular, la velocidad para el instante de tiempo :math:`t=t_n` después de realizar algo de algebra elemental, es dada por

.. math::
   :label: Ec:pos_08

   \begin{equation}
    v_{n}=\frac{\overline{v}_{n,n+1}\Delta t_{n-1,n}+\overline{v}_{n-1,n}\Delta t_{n,n+1}}{\Delta t_{n-1,n+1}}
   \end{equation}

Obsérvese que la expresión :eq:`Ec:pos_08`, es una ecuación recursiva y que los valores del subíndice :math:`N` son dados por :math:`n=1,2,3,...,N-1`, donde :math:`N+1` es el número de parejas :math:`(x_n,t_n)` conisideradas. Además, con los valores de las velocidades instantáneas :math:`v_1, v_2, v_3,...,v_{N-1}` para los correspondientes instantes de tiempo  :math:`t_1, t_2, t_3,...,t_{N-1}` se construye la gráfica de velocidad en función del tiempo (ver :numref:`fig:newCgrfig4`), cuya pendiente corresponde a la aceleración de la cebra (aceleración del carrito).

A modo de ejemplo, supongamos que deseamos calcular el valor de la velocidad del carrito para el instante de tiempo :math:`t=t_5`. De la ecuación :eq:`Ec:pos_08` resulta

.. math::
   :label: Ec:pos_09

   \begin{equation}
    v_{5}=\frac{\overline{v}_{5,6}\Delta t_{4,5}+\overline{v}_{4,5}\Delta t_{5,6}}{\Delta t_{4,6}}
   \end{equation}

donde :math:`\overline{v}_{5,6}=\frac{x_6-x_5}{t_6-t_5}`, :math:`\Delta t_{4,5}=t_5-t_4` y :math:`\overline{v}_{4,5}=\frac{x_5-x_4}{t_5-t_4}` y :math:`\Delta t_{5,6}=t_6-t_5`.\\


   .. csv-table:: Tabla de datos para medir la aceleración.
      :header: "Posición", "Tiempo"
      :widths: 1,1
      :width: 12 cm
      :name: tab:Ctabla1
      :align: center

      :math:`x_0` , :math:`t_0`
      :math:`x_{1}` , :math:`t_{1}`
      :math:`x_{2}` , :math:`t_{2}`
      :math:`x_{3}` , :math:`t_{3}`
      :math:`x_{4}` , :math:`t_4`
      :math:`x_{5}` , :math:`t_{5}`
      :math:`\vdots` , :math:`\vdots`
      :math:`x_{N}` , :math:`t_{n}`



.. figure:: /images/Mecanica/NewtonC/newCgrfig4.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:newCgrfig4

   Velocidad en función del tiempo.


**Mediciones**

Ahora que ya sabemos determinar el valor de la aceleración construya la tabla :numref:`tab:Ccoef`. A partir de los datos, construya la gráfica de :math:`a` como función de :math:`m_2`. Varíe :math:`m_2` asegurándose de mantener :math:`M=m_1+m_2` constante! en todo momento. Nota: el valor de :math:`m_1` es la masa total del carrito incluida la masa de la cebra y demás accesorios.
De la pendiente :math:`p` de la recta dada por :eq:`Ec:newC.6a` y de su punto de corte :math:`b` dado por :eq:`Ec:newC.6b` determine los valores de :math:`f` e :math:`I`. Aplique la teoría de errores apropiada para expresar los valores de :math:`f` y :math:`I` junto con las correspondientes incertidumbres.


   .. csv-table:: Datos para determinar :math:`\mu`.
      :header: ":math:`m_{2}(g)`", ":math:`a(m/s^{2})`"
      :widths: 1,1
      :width: 12 cm
      :name: tab:Ccoef
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


.. [#f1] Cuando un cuerpo se mueve en línea recta con aceleración constante :math:`a`, su velocidad en función del tiempo es dada por  :math:`v=v_0+at`, ver figura de abajo. La velocidad media entre los instantes de tiempo :math:`t_i` y :math:`t_j` es dada por  :math:`\overline{v}_{i,j}=\frac{v_i+v_j}{2}=\frac{v_0+at_i+v_0+at_j}{2}=v_0+a\frac{t_i+t_j}{2}`. Por otra parte, la velocidad instantánea del cuerpo para el instante de tiempo :math:`t_{ij}=t_i+\frac{t_j-t_i}{2}=t_i+\frac{\Delta t_{i,j}}{2}` es dada por :math:`v=v_0+a(t_i+\frac{t_j-t_i}{2})=v_0+a(\frac{t_i+t_j}{2})`. Así, las dos velocidades son iguales :math:`\blacksquare`.

         .. figure:: /images/Mecanica/NewtonC/newCgrfig5.png
            :alt:
            :scale: 110
            :align: center
            :name: fig:newCgrfig5

