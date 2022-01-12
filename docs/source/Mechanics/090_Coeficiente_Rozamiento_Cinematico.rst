+Coeficiente de rozamiento cinemático
=====================================

**Objetivo**

El propósito de esta práctica determinar el coeficiente de rozamiento cinético :math:`\mu` entre un bloque de madera con superficies diferentes y una superficie de aluminio. Para ello, se conectan los dos bloques mediante una cuerda ligera. Uno de los bloques yace sobre la mesa y el otro se suspende de la cuerda, la cual pasa por una polea. El bloque que pende de la cuerda se suelta desde diferentes alturas :math:`h` con respecto al piso y se miden las correspondientes distancias :math:`\lambda` que recorre el bloque sobe la mesa. Luego, el papel de los bloques se intercambia. Con la información de las alturas y distancias recorridas, y usando las leyes de Newton se desarrolla un método que permite hallar :math:`\mu`.


**Recursos**

   #. Dos bloques de madera de masas diferentes pero desconocidas.
   #. Una polea y cuerda para conectar los bloques.
   #. Una regla graduada.

**Resumen teórico**

Cuando un cuerpo se lanza sobre una superficie horizontal, de modo que este se deslice sobre ésta, se observa que el cuerpo se detiene en el transcurso del tiempo. Decimos entonces que el cuerpo se detiene debido a la fuerza de rozamiento cienética o dinámica. La dirección de la fuerza de rozamiento es opuesta a la del movimiento del cuerpo y su magnitud es

.. math::
   :label: Ec:kroz1

   \begin{equation}
    F=\mu N
   \end{equation}

donde :math:`N` es la fuerza normal entre los cuerpos y :math:`\mu` es una constante denominada coeficiente de rozamiento cinético, el cual depende de la naturaleza de las superficies en contacto. Esta constituye la segunda ley de fricción de Amonton. El hecho de que la fuerza de rozamiento sea independiente del área de contacto constituye la primera ley de fricción de Amonton. El hecho de que la fuerza de rozamiento sea independiente de la velocidad de deslizamiento constituye la primera ley de fricción de Coulomb.

**Descripción del problema**

Consideremos el sistema mecánico  mostrado en la :numref:`fig:kfdyn1` *Izq.*. Este consta de dos bloques de masas :math:`M` y :math:`m` conectados mediante una cuerda ligera que pasa por una polea de masa despreciable. Se ignora el rozamiento entre la cuerda y la polea, pero entre el bloque que yace sobre la mesa y la superficie de ésta existe un coeficiente de rozomiento cinético igual a :math:`\mu`.
Si inicialmente, la cuerda se encuentra lo mas estirada posible y el bloque de masa :math:`M` se libera desde una altura :math:`h_{1}` medida desde el piso,  el bloque :math:`m` que inicialmente se encontraba en reposo, recorre una distancia :math:`\lambda _{1}` sobre la mesa antes de detenerse. Notese que :math:`\lambda_1>h_1`.

Analicemos ahora la dinámica de este sistema usando las leyes de Newton. Las fuerzas que actuan sobre cada uno de los bloques se muestran la :numref:`fig:kfdyn1` *Der.*

.. figure:: /images/Mecanica/Coeficiente_Rozamiento_Cinematico/kfdyn1.png
   :scale: 120
   :align: center
   :name: fig:kfdyn1

   *Izq.* Bloque de masa :math:`M` se libera desde una altura :math:`h_1`. *Der.* Diagramas de cuerpo libre.

.. math::
   :label: Ec:kfdyn1

   \begin{equation}
   Mg-T_{1}=Ma_{1}
   \end{equation}

.. math::
   :label: Ec:kfdyn2

   \begin{equation}
   T_{1}-\mu mg=ma_{1}
   \end{equation}

De estas ecuaciones se sigue que la aceleración del sistema es

.. math::
   :label: Ec:kfdyn3

   \begin{equation}
   a_{1}=\frac{M-\mu m}{M+m}g
   \end{equation}

Cuando el bloque :math:`M` llega al piso se cumple que :math:`v^2=v_{0}^2+2a_1h_1=2a_1h_1`, donde :math:`v_{0}=0` y :math:`a_1`  es dada por la ecuación :eq:`Ec:kfdyn3`. Note que la magnitud de la aceración de los dos curpos es igual. Explícitamente

.. math::
   :label: Ec:kfdyn4

   \begin{equation}
    v^{2}=\frac{2(M-\mu m)}{M+m}gh_{1}
   \end{equation}

Esta rapidez es la misma que la del bloque :math:`m` ya que la cuerda es inextensible. Después de que :math:`M` llega al piso, el cuerpo :math:`m` continúa su movimiento con una aceleración igual a :math:`a=-\mu g` ya que la única fuerza horizontal sobre este es la fuerza de rozamiento :math:`f_1=-\mu mg`. La distancia recorrida por :math:`m` una vez que :math:`M` llega al piso es por tanto :math:`0=v^2+2a (\lambda _1-h_1)`. Reemplazando los valores de :math:`a=-\mu g` y la rapidez dada por :eq:`Ec:kfdyn4` obtenemos

.. math::
   :label: Ec:kfdyn5

   \begin{equation}
   \lambda _{1} =\frac{M}{(M+m)}\frac{(1+\mu)}{\mu}h_{1}=n_{1}h_{1}
   \end{equation}

donde hemos definido

.. math::
   :label: Ec:kfdyn6

   \begin{equation}
    n_{1} =\frac{M}{(M+m)}\frac{(1+\mu)}{\mu}
   \end{equation}

De igual manera se puede mostrar que si intercambiamos las posiciones de los bloques tal como se indica en la :numref:`fig:kfdyn2` *Izq.* y la :numref:`fig:kfdyn2` *Der.*, la distancia que :math:`M` avanza sobre la superficie horizontal es [#f1]_

.. figure:: /images/Mecanica/Coeficiente_Rozamiento_Cinematico/kfdyn2.png
   :scale: 120
   :align: center
   :name: fig:kfdyn2

   *Izq.* Bloque de masa :math:`m` se libera desde una altura :math:`h_2`. *Der.* Diagramas de cuerpo libre.

.. math::
   :label: Ec:kfdyn7

   \begin{equation}
     \lambda _{2} =\frac{m}{(M+m)}\frac{(1+\mu)}{\mu}h_{2}=n_{2}h_{2}
   \end{equation}

donde hemos definido

.. math::
   :label: Ec:kfdyn8

   \begin{equation}
    n_{2} =\frac{m}{(M+m)}\frac{(1+\mu)}{\mu}
   \end{equation}

los valores de :math:`n_{1}` y :math:`n_{2}`  dados por :eq:`Ec:kfdyn6` y :eq:`Ec:kfdyn8` se determinan experimentalmente. Una vez conocidos sus valores, de estas mismas ecuaciones el coeficiente rozamiento en cada caso es

.. math::
   :label: Ec:kfdyn8a

   \begin{equation}
    \mu  =\frac{1}{n_{1}\left( 1+\frac{m}{M}\right) -1}
   \end{equation}

.. math::
   :label: Ec:kfdyn8b

   \begin{equation}
    \mu =\frac{1}{n_{2}\left( 1+\frac{M}{m}\right) -1}
   \end{equation}


Para obtener el valor de :math:`n_{1}`, el bloque de masa :math:`M` se libera desde diferentes alturas :math:`h_{1}` y se miden las distancias :math:`\lambda _{1}` recorridas por :math:`m` sobre la superficie horizontal. Los diferentes valores de puntos (:math:`h_{1},\lambda_1)` determinan una recta (ver :numref:`fig:kcgraph` *Izq.*, cuya pendiente :math:`n_1`  se determina realizando una regresión lineal. Similarmente, después de intercambiar las posiciones de los bloques,  el bloque de masa :math:`m` se libera desde diferentes alturas :math:`h_{2}` y se miden las distancias :math:`\lambda _{2}` recorridas por :math:`M` sobre la superficie horizontal. Los diferentes valores de puntos (:math:`h_{2},\lambda _{2})` determinan una recta (ver :numref:`fig:kcgraph` *Der.*), cuya pendiente :math:`n_2`  se determina realizando una regresión lineal.


Recordemos que los valores de las masas :math:`m` y :math:`M` son desconocidos. No obstante, de las ecuaciones :eq:`Ec:kfdyn8a` y :eq:`Ec:kfdyn8b` se sigue que

.. figure:: /images/Mecanica/Coeficiente_Rozamiento_Cinematico/kfgraph.png
   :scale: 120
   :align: center
   :name: fig:kcgraph

   *Izq.* Linealización de :math:`\lambda_1` en función de :math:`h_1`. *Der.*  Linealización de :math:`\lambda_2` en función de :math:`h_2`

.. math::
   :label: Ec:kc.90

   \begin{equation}
    \frac{m}{M}=\frac{n_{2}}{n_{1}}
   \end{equation}

Así, esta expresión nos proporciona una relación entre las masas en términos de las pendientes determinadas a partir de los datos experimentales. Reemplazando este valor de :math:`m/M` en cualquiera de las ecuaciones :eq:`Ec:kfdyn8a` o :eq:`Ec:kfdyn8b` se obtiene

.. math::
   :label: Ec:kc.9

   \begin{equation}
   \mu =\frac{1}{n_{1}+n_{2}-1}
   \end{equation}

Nótese que esta última expresión permite calcular :math:`\mu` en términos de :math:`n_1` y :math:`n_2` sin tener que conocer los valores de las masas.



**Mediciones**

   #. Realice el montaje que se muestra en la :numref:`fig:kfdyn1`. Ponga en contacto la cara del bloque con lija sobre la superficie de aluminio. Mida los valores de :math:`\lambda_1` para diferentes valores de :math:`h_1`. Invierta las posiciones de los bloques de modo que la superficie del bloque en contacto con el aluminio sea también de lija. Mida los correspondientes valores de :math:`\lambda_2` para diferentes valores de :math:`h_2`, :numref:`fig:kfdyn2` *Izq.*. Complete la :numref:`tab:kfriction_la`. Con los datos obtenidos determine los valores :math:`n_1` y :math:`n_2` que conducen a determinar :math:`\mu` a partir de la ecuación :eq:`Ec:kc.9`.

      .. csv-table:: Mediciones para determinar el coeficiente de rozamiento cinético entre lija y aluminio.
         :header: ":math:`h_{1}\\,\\text{(cm)}`", ":math:`\\lambda _{1}\\,\\text{(cm)}`",":math:`h_{2}\\,\\text{(cm)}`",":math:`\\lambda_{2}\\,\\text{(cm)}`"
         :widths: 1,1,1,1
         :width: 15 cm
         :name: tab:kfriction_la
         :align: center
         :stub-columns: 0
         :header-rows: 0

         1,,1
         2,,2
         3,,3
         4,,4
         5,,5
         6,,6
         7,,7
         8,,8
         9,,9
         10,,10
         11,,11
         12,,12

   #. Realice el montaje que se muestra en la :numref:`fig:kfdyn1`. Ponga en contacto la cara del bloque con corcho sobre la superficie de aluminio. Mida los valores de :math:`\lambda_1` para diferentes valores de :math:`h_1`. Invierta las posiciones de los bloques de modo que la superficie del bloque en contacto con el aluminio sea también de corcho. Mida los correspondientes valores de :math:`\lambda_2` para diferentes valores de :math:`h_2`, :numref:`fig:kfdyn2` *Izq.*. Complete la :numref:`tab:kfriction_ca`. Con los datos obtenidos determine los valores :math:`n_1` y :math:`n_2` que conducen a determinar :math:`\mu` a partir de la ecuación :eq:`Ec:kc.9`.

      .. csv-table:: Mediciones para determinar el coeficiente de rozamiento cinético entre corcho y aluminio.
         :header: ":math:`h_{1}\\,\\text{(cm)}`", ":math:`\\lambda _{1}\\,\\text{(cm)}`",":math:`h_{2}\\,\\text{(cm)}`",":math:`\\lambda_{2}\\,\\text{(cm)}`"
         :widths: 1,1,1,1
         :width: 15 cm
         :name: tab:kfriction_ca
         :align: center
         :stub-columns: 0
         :header-rows: 0

         1,,1
         2,,2
         3,,3
         4,,4
         5,,5
         6,,6
         7,,7
         8,,8
         9,,9
         10,,10
         11,,11
         12,,12


      Halle el valor de :math:`m/M` a partir de la ecuación :eq:`Ec:kc.90` para las situaciones de los dos incisos de arriba y compárelos con el valor obtenido a partir de las mediciones directas de :math:`m` y :math:`M` con una balanza. Discuta sus resultados.


.. [#f1] La acelaración de los bloques cuando :math:`M` pende de la cuerda es :math:`a_{1}=\frac{M-\mu m}{M+m}g` y cuando :math:`m` pende de la cuerda es :math:`a_{2}=\frac{m-\mu M}{M+m}g`. En ambos casos se debe cumplir que :math:`a_1>0` y :math:`a_2>0` para que los cuerpos desciendan. Esto implica que :math:`M-\mu m>0` y :math:`m-\mu M>0`. De este par de condiciones se sigue que :math:`\frac{m}{M}<1`. En otras palabras, para poder realizar el experimento se debe cumplir que :math:`M\neq m` y que los coeficientes de rozamiento estático sean tales que el sistema siempre se pone en movimiento independiente de cual de los dos bloques pende de la cuerda.