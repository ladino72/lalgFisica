+Péndulo físico o compuesto
=============================

**Objetivo**

El propósito de esta práctica es doble: se estudia la variación del periodo de oscilación de una barra homogénea como función de la distancia desde el punto de oscilación de la misma y su centro de masa; y se determinan los valores de la aceleración de la gravedad y radio de giro de la barra homogénea a partir de los datos experimentales.

**Recursos**

   #. Soporte
   #. Barra metálica
   #. Cronómetro
   #. Regla

**Resumen teórico**

Se denomina  péndulo físico o compuesto a cualquier sólido rígido que pueda oscilar, bajo la acción de
la gravedad, alrededor de un eje horizontal que no pase por su centro de gravedad, ver :numref:`Fig:pendulum00`. El periodo :math:`T` de oscilaciones pequeñas de este péndulo viene dado por

.. figure:: /images/Oscilaciones_Termo/Physical_Pendulum/pendulum00.png
   :alt:
   :scale: 70
   :align: center
   :name: Fig:pendulum00

   Péndulo físico


.. math::
   :label: Ec:Pendulum-01

   \begin{equation}
    T=2\pi\sqrt{\frac{I_0}{mgh}}
   \end{equation}

donde :math:`I_0` es el momento de inercia del sólido con respecto al eje de rotación :math:`o`, :math:`m` la masa, :math:`h` la distancia desde el centro de masa del sólido y el eje de rotación; y :math:`g` representa el valor de la aceleración de la gravedad.

**Descripción del problema**

Consideremos el sistema representado en la :numref:`Fig:pendulum01`, el cual consiste de una barra metálica homogénea plana  de masa :math:`m` y longitud :math:`L`. Esta presenta una serie de oficios pequeños igualmente espaciados y ubicados a lo largo de uno de sus ejes principales. La barra puede oscilar alrededor de un eje que pasa por uno cualquiera de sus orificios.

.. figure:: /images/Oscilaciones_Termo/Physical_Pendulum/pendulum01.png
   :alt:
   :scale: 70
   :align: center
   :name: Fig:pendulum01

   Péndulo a estudiar: barra plana homogénea


El periodo de oscilación de la barra con respecto al punto :math:`o` viene dado por la ecuación :eq:`Ec:Pendulum-01` con  :math:`h=x`.  El valor del momento de inercia :math:`I_0` de la barra con respecto al punto :math:`o` se encuentra a partir del teorema de ejes paralelos  :math:`I_0=mx^{2}+I_{cm}`, donde :math:`I_{cm}=mK^{2}` es el momento de inercia de la barra con respecto a su centro de masa :math:`cm` y :math:`K` su radio de giro. Al reemplazar estas cantidades en la ecuación :eq:`Ec:Pendulum-01` resulta

.. math::
   :label: Ec:Pendulum-02

   \begin{equation}
    T=2\pi\sqrt{\frac{x^{2}+K^{2}}{gx}}
   \end{equation}


La ecuación :eq:`Ec:Pendulum-02` se puede reescribir como

.. math::
   :nowrap:

   \begin{eqnarray}
    xT^{2} &=& \frac{4\pi^{2}}{g}(x^{2}+K^{2})\\
    xT^{2} &=& \frac{4\pi^{2}}{g}x^{2}+\frac{4\pi^{2}}{g}K^{2}
   \end{eqnarray}


Al definir :math:`Y=xT^{2}` y :math:`X=x^{2}`, la ecuación anterior se convierte en

.. math::
   :label: Ec:Pendulum-03

   \begin{equation}
    Y=mx+b
   \end{equation}


donde :math:`m=\frac{4\pi^{2}}{g}` y :math:`b=\frac{4\pi^{2}}{g}K^{2}`.  Al realizar una gráfica de :math:`Y` como función de :math:`X` se obtiene una línea recta con pendiente :math:`m` y punto de intersección con el eje vertical igual a :math:`b`, ver :numref:`Fig:pendulum02`. De estas expresiones se sigue que

.. math::
   :label: Ec:Pendulum-05

   \begin{equation}
    g=\frac{4\pi^{2}}{m}
   \end{equation}


.. math::
   :label: Ec:Pendulum-04

   \begin{equation}
    K=\sqrt{\frac{b}{m}}
   \end{equation}


.. figure:: /images/Oscilaciones_Termo/Physical_Pendulum/pendulum02.png
   :alt:
   :scale: 80
   :align: center
   :name: Fig:pendulum02

   Linealización del periodo de oscilación :math:`T` como función de la distancia :math:`x` entre el eje de oscilación y el centro de masa


**Mediciones**

Antes de empezar a tomar mediciones, determine el centro de masa de la barra. Para ello, suspenda la barra de un punto hasta que ésta quede horizontal. El punto de suspensión se debe encontrar aproximadamente en la mitad de la longitud de la barra (Justifique este hecho). Marque el punto sobre la barra con un lápiz para indicar su ubicación.
Determine el periodo :math:`T` de oscilación de la barra con respecto a la distancia :math:`x` de  cada uno de estos huecos al centro de masa, donde :math:`-\frac{L}{2}\leq x\leq\frac{L}{2}`. Complete las dos primeras columnas de la :numref:`tab:Pendulum01`.


.. csv-table:: Datos experimentales para determinar :math:`K` y :math:`g`
         :header: ":math:`T\\,(\\text{s})`", ":math:`x\\,(\\text{m})`", ":math:`Y=xT\^{2}`",":math:`X=x^{2}`"
         :widths: 1,1,1,1
         :width: 12 cm
         :name: tab:Pendulum01
         :align: center

         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.
         .,.,.,.

A partir de los datos de las dos primeras columnas de la :numref:`tab:Pendulum01`, complete las columnas 3 y 4 de la misma tabla. Grafique :math:`Y` como función de :math:`X` y determine los valores  :math:`m` y :math:`b` como se indica arriba en la teoría. (Ayuda: la gráfica obtenida debería tener el perfil de la :numref:`Fig:pendulum03`). Con este par de valores encuentre el valor de la aceleración de la gravedad y el radio de giro :math:`K` de la barra a partir de las ecuaciones :eq:`Ec:Pendulum-05` y :eq:`Ec:Pendulum-04`. Recuerde que para la barra homogénea delgada de masa :math:`m`, longitud :math:`L` y ancho :math:`b`, :math:`I_{cm}=m\frac{L^{2}+h^{2}}{12}=mK^{2}`, donde :math:`K=\sqrt{\frac{L^{2}+h^{2}}{12}}`. Compare los valores de :math:`g` y :math:`K` obtenidos experimentalmente con los valores teóricos. Discuta sus resultados.

.. figure:: /images/Oscilaciones_Termo/Physical_Pendulum/pendulum03.png
   :alt:
   :scale: 90
   :align: center
   :name: Fig:pendulum03

   Periodo :math:`T` como función de la distancia :math:`x`

