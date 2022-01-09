+Coeficientes de rozamiento cinético y estático
===============================================

**Objetivo**

El propósito de esta práctica es determinar los coeficientes de fricción estático :math:`\mu _{e}` y cinético :math:`\mu _{k}` de un cilindro que rueda deslizándose a lo largo de un plano inclinado. Para ello, se miden la distancias que avanza un punto sobre la periferia del cilindro a lo largo del plano para diferentes ángulos de inclinación. De estas mediciones y el modelo desarrollado  se determinan :math:`\mu _{e}` y :math:`\mu _{k}`.

**Recursos**

   #. Un cilindro metálico con marcador incorporado.
   #. Un plano inclinado con transportador.
   #. Tiras de papel blanco.
   #. Una regla graduada en mm.

**Resumen Teórico**

Cuando un cuerpo como por ejemplo una rueda o cilindro se mueven sobre una superficie, su movimiento rotacional y traslacional   dependen en gran medida de los coeficientes de rozamiento estático :math:`\mu_s` y cinético :math:`\mu_k` entre las superficies en contacto. Cuando uno de estos cuerpos de radio :math:`R`, rueda sin deslizarse sobre una superficie, se cumple que la distancia recorrida por su centro de masa es igual a la distancia recorrida por un punto de su periferia medida a lo largo del arco que describe. Esta condición de rodadura se escribe matemáticamente como :math:`v=\omega R`, donde :math:`v` y :math:`\omega` representan las velocidades lineal y angular respectivamente. En el caso de tener una superficie inclinada, la rotación con deslizamiento o sin deslizamiento depende no solamente de los coeficientes :math:`\mu_s` y :math:`\mu_k` sino también del ángulo de inclinación :math:`\theta` de la superficie.

**Descripción del Problema**

Consideremos el movimiento de un cilindro de radio :math:`R` y masa :math:`m` a lo largo del plano inclinado como se muestra en la :numref:`fig:Roll_Frict1`. Estudiaremos dos posibles casos: cuando el cilindro rueda sin deslizarse y cuando rueda deslizándose a lo largo del plano. En cualquier caso, las fuerzas que actúan sobre el cilindro se indican en la figura adjunta. Al aplicar la segunda ley de Newton tanto para la traslación del centro de masa y rotación del cilindro alrededor de su centro de masa resulta

.. figure:: /images/Mecanica/Rotation_Kinetic_Static_Coeff/Roll_Frict1.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Roll_Frict1

   Cilindro sobre un plano inclinado y diagrama de fuerzas sobre el cilindro.

.. math::
   :label: Ec:Rol_f1a

   \begin{equation}
   mg\sin \theta -f=ma
   \end{equation}

.. math::
   :label: Ec:Rol_f1b

   \begin{equation}
    mg\cos \theta =N
   \end{equation}

.. math::
   :label: Ec:Rol_f1c

   \begin{equation}
    fR=I_{0}\alpha
   \end{equation}

donde :math:`f` \ y :math:`N` son las fuerza de fricción y normal sobre el cilindro; :math:`I_{0}=\frac{mR^2}{2}` es el momento de inercia del cilindro con respecto a su centro de masa. :math:`a`  y :math:`\alpha` representan los valores de la aceleración lineal del centro de masa a lo largo del plano inclinado y aceleración angular del cilindro respectivamente.

**Rodamiento sin deslizamiento**

En el caso de rozamiento sin deslizamiento, a las anteriores ecuaciones debemos agregar la condición de rodadura dada por

.. math::
   :label: Ec:Rol_f01

   \begin{equation}
    a =\alpha R
   \end{equation}

De las ecuaciones :eq:`Ec:Rol_f1a`, :eq:`Ec:Rol_f1b`, :eq:`Ec:Rol_f1c` y :eq:`Ec:Rol_f01` resulta

.. math::
   :label: Ec:Rol_f02

   \begin{equation}
    a=\frac{2}{3}g\sin \theta
   \end{equation}

.. math::
   :label: Ec:Rol_f02b

   \begin{equation}
   \alpha =\frac{2g}{3R}\sin \alpha
   \end{equation}

.. math::
   :label: Ec:Rol_f03

   \begin{equation}
   f= \frac{1}{3}mg\sin \theta
   \end{equation}

La expresión :eq:`Ec:Rol_f03` determina el valor de la fuerza de rozamiento que debe actuar sobre el cilindro para que este ruede sin deslizarse. El máximo valor de esta fuerza es determinado por la condición :math:`f\leq \mu_s N=\mu_s \cos \theta`, donde :math:`\mu_s` es el coeficiente de rozamiento estático; es decir, que el cilindro rueda sin deslizarse si se cumple

.. math::
   :label: Ec:Rol_f04

   \begin{equation}
    \tan \theta \leq 3\mu _{s}
   \end{equation}


**Rodamiento con deslizamiento**

En el caso de rozamiento con deslizamiento, el ángulo del plano inclinado debe ser tal que cumpla la condición :math:`\tan \theta > 3\mu_s` como se determinó más arriba. La fuerza de fricción es dada por

.. math::
   :label: Ec:Rol_f2

   \begin{equation}
   f=\mu _{k}N=\mu _{k}mg\cos \theta
   \end{equation}

donde :math:`\mu_k` es el coeficiente de rozamiento cinético. De las ecuaciones :eq:`Ec:Rol_f1a`, :eq:`Ec:Rol_f1c` y :eq:`Ec:Rol_f2` resulta

.. math::
   :label: Ec:Rol_f3a

   \begin{equation}
   a=g(\sin \theta -\mu _{k}\cos \theta )
   \end{equation}

.. math::
   :label: Ec:Rol_f3b

   \begin{equation}
    \alpha =\frac{2\mu _{k}g\cos \theta }{R}
   \end{equation}

La distancia :math:`X_{d}` recorrida por el centro de masa  del cilindro y el ángulo :math:`\Phi _{d}` que el cilindro gira mientras este rueda deslizándose en función de tiempo vienen dados por

.. math::
   :label: Ec:Rol_f4a

   \begin{equation}
   X_{d}=x_{0}+v_{0}t+\frac{1}{2}at^{2}=\frac{1}{2}g(\sin \theta -\mu _{k}\cos\theta )t^{2}
   \end{equation}


.. math::
   :label: Ec:Rol_f4b

   \begin{equation}
    \Phi=\Phi _{0}+\omega _{0}t+\frac{1}{2}\alpha t^{2}=\frac{\mu _{k}g\cos \theta }{R}t^{2}
   \end{equation}


En estas ecuaciones hemos asumido que el cilindro parte del reposo y que inicialmente no gira, es decir, :math:`v_{0}=0` y :math:`\omega _{0}=0`; igualmente hemos tomado :math:`x_{0}=0` y :math:`\Phi _{0}=0`.

Al existir deslizamiento, se cumple que la diferencia :math:`\Delta x=X_{d}- x_{\Phi}\neq 0`, donde :math:`x_{\Phi}=\Phi R` es la longitud medida a lo largo del arco descrito por cualquier punto de la periferia del cilindro, ver :numref:`fig:Roll_Frict2`. El valor de :math:`\Delta x` es,


.. figure:: /images/Mecanica/Rotation_Kinetic_Static_Coeff/Roll_Frict2.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Roll_Frict2

   Marcas (circulos) dejadas por el cilindro que se desliza cada vez que completa una vuelta.


.. math::
   :label: Ec:Rol_f5

   \begin{equation}
    \Delta x=X_{d}-\Phi R=\frac{1}{2}g(\sin \theta -3\mu _{k}\cos \theta)t^{2}
   \end{equation}

En el caso cuando el cilindro rueda sin deslizarse por el plano :math:`\Delta x=X_{d}- x_{\Phi}=0` para cualquier instante de tiempo. De la ecuación :eq:`Ec:Rol_f4b` se deduce que el tiempo :math:`t_{N}` empleado por el cilindro para completar :math:`N` vueltas, (:math:`\Phi _{N}=2\pi N`) es

.. math::

   \begin{equation}
    t_{N}=\sqrt{\frac{2\pi NR}{g\mu _{k}\cos \theta }}
   \end{equation}

y por tanto la ecuación :eq:`Ec:Rol_f5` se convierte en

.. math::
   :label: Ec:Rol_f5.5

   \begin{equation*}
    \Delta x_{N}=\frac{1}{2}g(\sin \theta -3\mu _{k}\cos \theta )t_{N}^{2}=(\frac{\tan \theta }{\mu _{k}}-3)\pi NR
   \end{equation*}

Por otra parte, de la :numref:`fig:Roll_Frict2` es claro que

.. math::

   \begin{equation*}
   X_{dN}=\Delta x_{N}+x_{\Phi _{N}}
   \end{equation*}

donde :math:`x_{\Phi _{N}}=R\Phi _{N}`. Luego la distancia entre dos marcas consecutivas es

.. math::
   :label: Ec:Rol_f6

   \begin{align}
   D &= X_{d(N+1)}-X_{dN}=\Delta x_{N+1}+R\Phi _{(N+1)}-\Delta x_{N}-R\Phi_{N} \\
     &= \Delta x_{N+1}-\Delta x_{N}+R(\Phi _{(N+1)}-\Phi _{dN}) \nonumber  \\
     &= (\frac{\tan \theta }{\mu _{k}}-3)\pi R+2\pi R \nonumber
   \end{align}

Obsérvese que la distencia :math:`D` dejada por dos marcas consecutivas es independiente de :math:`N`. Así, si realizamos una gráfica de :math:`D` en función de :math:`\tan \theta` se obtiene la gráfica mostrada en la :numref:`fig:Roll_Frict3`, donde para ángulos mayores al ángulo crítico :math:`\theta_c` la relación es lineal y con pendiente :math:`p=\pi R/\mu_k`. Conocido el valor de :math:`p`, el valor del coeficiente de rozamiento cinético es dado por

.. math::
   :label: Ec:Rol_f7

   \begin{equation}
    \mu_k=\frac{\pi R}{p}
   \end{equation}

El valor del coeficiente de rozamiento estático es dado por

.. math::
   :label: Ec:Rol_f8

   \begin{equation}
    \mu_e=\frac{\tan \theta_c}{3}
   \end{equation}


.. figure:: /images/Mecanica/Rotation_Kinetic_Static_Coeff/Roll_Frict3.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Roll_Frict3

   Distancia :math:`D` entre dos marcas consecutivas dejadas or el cilindro como función :math:`\tan \theta`.

**Montaje experimental**

Considérese el esquema de la :numref:`fig:Roll_Frict4`, el cual consta de un plano cuyo ángulo de inclinación :math:`\theta` se puede variar. Un cilindro (de latón o aluminio) se suelta desde la parte superior del plano y dependiendo del ángulo de inclinación :math:`\theta`, el cilindro rueda sin deslizarse o rueda deslizándose a lo largo del plano inclinado. El cilindro tiene un marcador ligero incorporado  de modo que en cualquiera de los dos casos de rotación, cada vez que el cilindro completa una vuelta, este deja una marca sobre el plano.

.. figure:: /images/Mecanica/Rotation_Kinetic_Static_Coeff/Roll_Frict4.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Roll_Frict4

   Arreglo experimental para determinar :math:`\mu_s` y :math:`\mu_k`.


**Mediciones**

Halle los valores de :math:`\mu_s` y :math:`\mu_k` a partir de la ecuación :eq:`Ec:Rol_f6`. Para ello fije el valor del ángulo de inclinación :math:`\theta` del plano y libere el cilindro desde la parte alta del plano. Mida la distancia :math:`D` entre las marcas dejadas por el marcador sobre el papel para cada valor de :math:`\theta`. Registre los datos experimentales en la :numref:`tab:kfriction`. Determine los valors de :math:`\mu_k` y :math:`\mu_e`. Discuta sus resultados.


.. csv-table:: Mediciones para determinar :math:`\mu_s` y :math:`\mu_k`.
   :header: ":math:`\\theta \\,(^o)`", ":math:`D` (cm)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:kfriction
   :align: center
 
   20,.
   21,.
   22,.
   23,.
   24,.
   25,.
   26,.
   27,.
   28,.
   29,.
   30,.
   31,.
   32,.
   33,.
   34,.
   :math:`\vdots`, :math:`\vdots`
   62,.
   63,.
   64,.
   65,.
