+Energía cinética rotacional
=============================


**Objetivo**

El propósito de esta práctica es estudiar la dependencia de la velocidad tanto traslacional como rotacional de una esfera de su radio de giro. Para ello, la esfera se deja rodar a lo largo de un par de rieles paralelos e inclinados y cuya distancia de separación entre ellos se puede variar. La velocidad de la esfera en la base del riel es una función de la distancia de separación entre los rieles, el radio de la esfera y la altura desde donde se suelta; y su valor se determina de manera indirecta usando las ecuaciones cinemática de caída libre.


**Recursos**

   #. Un riel acanalado metálico de ancho variable.
   #. Un calibrador digital.
   #. Una esfera metálica de diámetro aproximadamente igual a 10 mm.
   #. Una regla graduada en mm.
   #. Un transportador.
   #. Un soporte.


**Resumen teórico**

Cuando un cuerpo gira sus partículas describen circunferencias centradas en el eje de rotación con una velocidad que es proporcional al radio de la circunferencia que describen :math:`v_i=\omega \cdot R_i`. La energía cinética total es la suma de las energías cinéticas de cada una de las partículas. Esta suma se puede expresar de forma simple en términos del momento de inercia y la velocidad angular de rotación.

.. math::

   \begin{equation}
    E_k=\sum\frac{1}{2}m_iv_i^2=\sum\frac{1}{2}m_i\omega^2 R_i^2=\frac{1}{2}(\sum m_i R_i^2) \omega^2 =\frac{1}{2}I \omega^2
   \end{equation}

donde :math:`I=\sum m_i R_i^2` se denomina momento de inercia del sólido con respecto a su eje de rotación. Así, para una esfera homogénea de masa :math:`m` y radio :math:`R` que rota con respecto a un eje que pasa por su centro :math:`I=\frac{2}{5}mR^2`.


**Descripción del Problema**

Consideremos el sistema representado en la :numref:`fig:rssetup0`, el cual consiste de un plano inclinado  cuyo ángulo de inclinación con respecto al horizonte es :math:`\theta`. Si una partícula *puntual* de masa :math:`m` se liberara desde una altura :math:`H`, su velocidad :math:`v` en la base del plano según el principio de conservación de la energía :math:`mgH =\frac{1}{2}mv^2`, es

.. math::
   :label: Ec:rs.1

   \begin{equation}
    v=\sqrt{2gH}
   \end{equation}

.. figure:: /images/Mecanica/Rotational_Energy/rssetup0.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:rssetup0

   Partícula puntual moviéndose a  lo largo de un plano inclinado


Ahora bien, si reemplazamos el plano por un riel acanalado de ancho :math:`W` (:numref:`fig:rssetup`) y la partícula es ahora una esfera radio :math:`R`, donde :math:`W<2R`, entonces la ecuación anterior se debe modificar para tener en cuenta la energía cinética rotacional de la esfera: :math:`mgH =\frac{1}{2}mv^2 + \frac{1}{2}I \omega ^2`, donde :math:`\omega` e :math:`I=\frac{2}{5}mR^2` representan la velocidad angular y momento de
inercia de la esfera con respecto a un eje que pasa por su centro de masa. Si la esfera rueda (no se desliza) entonces las
relación entre :math:`v` y :math:`R` es :math:`v=\omega R`. Usando éstas tres últimas expresiones obtenemos

.. figure:: /images/Mecanica/Rotational_Energy/rssetup.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:rssetup

   Arreglo usado para estudiar la velocidad de llegada de una esfera a la base de un riel inclinado. La esfera se libera desde una altura :math:`H` y al llegar a la base del riel esta cae libremente bajo la acción de la gravedad.


.. math::
   :label: Ec:rs.2

   \begin{equation}
    v=\sqrt{\frac{10}{7}gH}
   \end{equation}

La ecuación :eq:`Ec:rs.2` es válida cuando la esfera rueda y hace contacto solo con un punto de la superficie. No obstante,
cuando la esfera rueda por el riel acanalado como se muestra en la :numref:`fig:rswedge`, ésta hace contacto con dos puntos y como
consecuencia el radio efectivo es

.. figure:: /images/Mecanica/Rotational_Energy/rswedge.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:rswedge

   Vista frontal de la esfera en contacto con el riel acanalado.


.. math::
   :label: Ec:rs.3

   \begin{equation}
    r=\sqrt{R^{2}-\frac{W^{2}}{4}}=R\sqrt{1-\frac{W^{2}}{4R^{2}}}
   \end{equation}

Para hallar la velocidad :math:`v` de la esfera en la base de la rampa, basta con utilizar la condición
de rodadura :math:`v=\omega r` (con :math:`r` dado por la ecuación :eq:`Ec:rs.3`) en la ecuación de la conservación de la energía mecáncia anterior


.. math::
   :label: Ec:rs.4

   \begin{equation}
    v=\sqrt{\frac{10}{7}gH}\times \sqrt{\frac{1-\frac{W^{2}}{4R^{2}}}{1-\frac{5W^{2}}{28R^{2}}}}  \label{rs.4}
   \end{equation}

Observe que la anterior ecuación  en el límite cuando :math:`W/R\rightarrow 0` se reduce a la ecuación :eq:`Ec:rs.2`. Además, en el límite cuando :math:`W/R \rightarrow 2`, la velocidad tiende a cero.

La ecuación :eq:`Ec:rs.4` se puede reescribir como

.. math::
   :label: Ec:rs.4.5

   \begin{equation}
    v^{2}\big(1-\frac{5}{28}\frac{W^2}{R^2}\big)= \frac{10}{7}gH \times \big(1-\frac{1}{4}\frac{W^2}{R^2}\big)
   \end{equation}

Al definir

.. math::
   :label: Ec:rs.5

   \begin{equation}
    Y=v^{2}(1-\frac{5}{28}\frac{W^{2}}{R^{2}})
   \end{equation}

.. math::
   :label: Ec:rs.6

   \begin{equation}
   X=1-\frac{1}{4}\frac{W^{2}}{R^{2}}
   \end{equation}

la ecuación anterior se convierte en

.. math::
   :label: Ec:rs.7

   \begin{equation}
    Y=pX
   \end{equation}

donde :math:`p=\frac{10}{7}gH`. Al realizar una gráfica de :math:`Y` como función de :math:`X` se obtiene una línea recta con pendiente :math:`p` y punto de intersección con el eje vertical igual a cero, ver  (:numref:`fig:rswedge2`).


.. figure:: /images/Mecanica/Rotational_Energy/rswedge2.png
   :alt:
   :scale: 120
   :align: center
   :name: Fig:rswedge2

   Linealización de la rapidez :math:`v` de la esfera como función de la distancia :math:`W` de separación entre los rieles.


Por completez, el problema de la condición de rodadura se analiza en el pie de nota [#f1]_.


**Determinación de la velocidad de la esfera en la base del riel**

La velocidad de la esfera en el extremo del riel puede ser medida
indirectamente usando las ecuaciones cinemáticas de caída libre
(tiro parabólico). Tomando nuestro origen de coordenadas en el
extremo inferior del riel, las posiciones horizontal y vertical como
función del tiempo son

.. math::
   :label: Ec:rs.11

   \begin{equation}
    x_1=v\cos \theta t \qquad y_1 =-vsen\theta t -\frac{1}{2}gt^2
   \end{equation}

cuando la esfera llega al piso :math:`x_1=x` y :math:`y_1=-y`. Luego, las anteriores ecuaciones se convierten en

.. math::
   :label: Ec:rs.12

   \begin{equation}
    x=v\cos \theta t \qquad -y =-v \sin \theta t -\frac{1}{2}gt^2
   \end{equation}

Eliminando el tiempo de las ecuaciones :eq:`Ec:rs.8` y despejando la velocidad :math:`v` de la ecuación resultante obtenemos

.. math::
   :label: Ec:rs.13

   \begin{equation}
    v=\sqrt{\frac{gx^{2}}{2\cos ^{2}\theta (y-x\tan \theta )}}
   \end{equation}

Así, midiendo los valores de :math:`x`, :math:`y` y :math:`\theta` podemos determinar el valor de la velocidad :math:`v` de la esfera en el extremo del riel para un valor de :math:`H` determinado.


**Mediciones**

Realice el montaje que se indica en la :numref:`fig:rssetup`. La distancia de separación :math:`W` entre los rieles se puede variar en el rango comprendido entre 0 y 10 mm en pasos de 1 mm mediante un par de tornillos micrométricos instalados en el sistema rieles. Los tornillos micrométricos sirven como sistema de guía para posicionar los rieles de manera paralela; el verdadero paralelismo se logra ajustando cuidadosamente los calibradores y midiendo la distancia entre los rieles con  el calibrador digital en diferentes puntos a lo largo de estos.

Antes de tomar mediciones fije un valor del ángulo :math:`\theta` de inclinación del riel acanalado de modo que la esfera siempre ruede. Recuerde siempre soltar la esfera desde la misma altura :math:`H` y el mismo punto. Complete la :numref:`tab:Rot_Energy_01`. Los valores de la columna :math:`v` se deben calcular a partir de las columnas de distancias :math:`x` e :math:`y` y el uso de la ecuación :eq:`Ec:rs.13`.

A partir de los datos obtenidos grafique la rapidez de la bola :math:`v\,\text{(m/s)}` en la base de los rieles como función de la distancia de separación :math:`W(m)` entre los rieles.  ¿Para qué valor de :math:`W`, la rapidez :math:`v` se hace cero?  Para responder a la pregunta planteada. Analice la gráfica obtenida.

Demostremos ahora que la relación entre :math:`v` y :math:`W` obedece la ecuación :eq:`Ec:rs.7`. Para ello, graficaremos :math:`Y` como función de :math:`X`  a partir de los datos experimentales de :math:`v`, :math:`W` y :math:`R`. Las definiciones de  :math:`Y` y :math:`X` vienen dadas por las expresiones :eq:`Ec:rs.5` y :eq:`Ec:rs.6` respectivamente.  A partir de la gráfica obtenga el valor de la pendiente :math:`b` de la línea recta. Si nuestro modelo es correcto se debe cumplir que :math:`b=p=\frac{10}{7}gH`. ¿Se cumple lo anterior? Para esto, debe usar un tratamiento adecuado de los datos (regresión lineal y  teoría de errores)


**Preguntas:**


   #. Si la distancia de separación :math:`W` entre los rieles aumenta ¿qué le pasa a la velocidad angular y traslacional del centro de masa de la esfera?
   #. Si la distancia de separación :math:`W` entre los rieles aumenta ¿qué le pasa a la fuerza de fricción ejercida por los rieles sobre la esfera?
   #. Si la distancia de separación :math:`W` entre los rieles aumenta ¿qué le pasa a la energía cinética rotacional y traslacional de la esfera a medida que desciende por los rieles?


.. csv-table:: Datos para determinar :math:`v` como función de :math:`W`. Los valores de :math:`\theta` y :math:`H` deben permanecer constantes.
   :header: ":math:`W\\,\\text{(mm)}`", ":math:`v\\,\\text{(m/s)}`",":math:`x\\,\\text{(m)}`",":math:`y\\,\\text{(m)}`"
   :widths: 1,1,1,1
   :width: 12 cm
   :name: tab:Rot_Energy_01
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
   .,.,.,.
   .,.,.,.

.. [#f1] Condición de rodadura de la esfera sobre el riel: Para que la esfera ruede sin deslizarse debe existir un mínimo coeficiente de fricción entre la esfera y la superficie. Calculemos este valor a partir de la segunda ley de Newton

        .. math::
           :label: Ec:rs.8

           \begin{equation}
            mg\sin \theta - f = ma \qquad fr=I\alpha=\frac{2}{5}mR^2
           \end{equation}

        donde hemos usado la condición de rodadura :math:`a=\alpha r`. Solucionando :math:`f` de las ecuaciones :eq:`Ec:rs.8` se obtiene

        .. math::
           :label: Ec:rs.9

           \begin{equation}
            f=  \frac{mg\sin \theta}{1+\frac{5r^2}{2R^2}}
           \end{equation}

        Usando la relación :math:`f\leq \mu N= \mu mg\cos \theta` y el valor de :math:`r` dado por :eq:`Ec:rs.3` obtenemos para :math:`\mu`

        .. math::
           :label: Ec:rs.10

           \begin{equation}
            \mu \geq  \frac{2}{7}\frac{\tan \theta}{1- \frac{5W^2}{28R^2}}
           \end{equation}

        Así, el mínimo valor de :math:`\mu` es una función del cociente :math:`W/R`, y aumenta cuando :math:`W/R` aumenta. Observe también que cuando :math:`W/R \rightarrow 0` entonces :math:`\mu \geq \frac{2}{7}\tan\theta`, el cual es un resultado conocido para la esfera que rueda
        sobre una superficie plana. Ahora, cuando :math:`W/R \rightarrow 2` entonces  :math:`\mu \geq \tan \theta` y de la ecuación :eq:`Ec:rs.4` :math:`v=0`; este último resultado se debe a que el radio efectivo se hace cero y por tanto el torque debido a la fricción también se hace cero.