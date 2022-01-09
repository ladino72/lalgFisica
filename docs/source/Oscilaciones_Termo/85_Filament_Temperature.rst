+Temperatura del filamento de una bombilla
===========================================

**Objetivo**

El propósito de esta práctica es determinar la temperatura del filamento de una bombilla cuando ésta se encuentra encendida. Para ello, se mide la caída de potencial en la bombilla como función de la corriente :math:`i` que circula por su filamento. Asumiendo una dependencia entre la resistenica eléctrica  :math:`R` y su temperatura :math:`T` es de la forma :math:`R\sim T^{\beta}`, donde :math:`\beta` es una constante, la potencia :math:`P` disipada por la bombilla toma la forma :math:`P\sim R^{\frac{4}{\beta}}`. El valor de :math:`\beta` se determina al linealizar la relación entre la :math:`i` y :math:`R`.


**Recursos**


   #. Un variac :math:`60` Hz, :math:`110` V.
   #. Una bombilla de :math:`60` W, :math:`110` V.
   #. Dos Multímetros.
   #. Un termómetro.
   #. Cables de conexión.


**Resumen Teórico**

La resistencia eléctrica de la mayoría de los materiales depende de la temperatura.  La relación  entre  la resistencia y la temperatura  depende del rango de temperaturas considerado. Así, en un metal (a altas temperaturas) entre mayor es su temperatura mayor es su resistencia eléctrica y la relación entre  :math:`R` y :math:`T` es lineal. Sin embargo, a temperaturas muy bajas la resistencia del metal se hace prácticamente constante y su valor depende de la naturaleza del material y otros factores como su pureza. Otros materiales a temperaturas extremadamente bajas se convierten en *superconductores*, es decir su resistencia eléctrica se hace cero.  En materiales tal como semiconductores puros, la resistencia eléctrica decrece exponencialmente con la temperatura.

En el caso particular del filamento de una bombilla hecho de volframio o tungsteno la relación entre su resistencia eléctrica y temperatura no es lineal. Experimentos demuestran que la relación entre :math:`R` y :math:`T` es de la forma

.. math::
   :label: Ec:filatemp1

   \begin{equation}
    R=cT^{\beta}
   \end{equation}

donde :math:`c` y :math:`\beta` son cosntantes y :math:`T` es la temperatura absoluta (medida en grados Kelvin) del material. Así, determinado el valor de estas constantes, el valor de la temperatura del filamento se puede medir indirectamente a partir de su resistencia, la cual es una cantidad que se puede medir fácilmente en este caso. Por otro lado, la potencia :math:`P` disipada por la bombilla es proporcional a la cuarta potencia de su temperatura absoluta, es decir

.. math::
   :label: Ec:filatemp2

   \begin{equation}
    P=a T^{4}
   \end{equation}

donde :math:`a` es una constante.

**Descripción del Problema**

El arreglo experimental para determinar la temperatura del filamento de la bombilla se muestra en la :numref:`fig:Filament_Temperature2` y  consiste esencialmente de una bombilla de :math:`60` W, :math:`110` V conectada a un variac cuyo voltaje AC se puede variar entre :math:`0` y :math:`110` V, y dos multímetros en los modos de amperímetro y voltímetro. La potencia eléctrica disipada por la bombilla es dada por  :math:`P=Vi=Ri^{2}`, donde :math:`V`, :math:`R` e :math:`i` representan la caída de potencial entre sus terminales, la resistencia y  corriente eléctrica respectivamente. Teniendo en cuenta la ecuaciones :eq:`Ec:filatemp1` y :eq:`Ec:filatemp2` podemos escribir

.. math::
   :label: Ec:filatemp3

   \begin{equation}
    P=Ri^{2}=aT^{4}=a(\frac{R}{c})^{\frac{4}{\beta}}=q R^{\frac{4}{\beta}}
   \end{equation}

donde :math:`q=a\frac{1}{c}^{\frac{4}{\beta}}=constante`. De esta última expresión se sigue que :math:`i=q^{1/2}\times R^{\frac{4-\beta}{2\beta}}` y por tanto el valor de :math:`\beta ` se puede determinar del
valor de la pendiente :math:`m` de la gráfica de :math:`\log i` en función de :math:`\log R` (ver
:numref:`fig:Filament_Temperature1`). Conocido el valor de :math:`\beta=\frac{4}{2m+1}` se desprende que

.. figure:: /images/Oscilaciones_Termo/Filament_Temperature/Filament_Temperature1.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Filament_Temperature1

   Lienalización de la relación :math:`i=q^{1/2}\times R^{\frac{4-\beta}{2\beta}}`

.. math::
   :label: Ec:filatemp4

   \begin{equation}
    T=\left( \frac{R}{R_{0}}\right) ^{\frac{1}{\beta}}T_{0}
   \end{equation}

donde :math:`R_{0}` es la resistencia del filamento a la temperatura de referencia :math:`T_{0}`, que puede ser la temperatura ambiente.


.. figure:: /images/Oscilaciones_Termo/Filament_Temperature/Filament_Temperature2.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Filament_Temperature2

   Arreglo experimental para determinar la relación entre la resistencia y temperatura del filamento de la bombilla.


**Mediciones y procedimientos**

   #. Realice el montaje que se describe en la :numref:`fig:Filament_Temperature2`.
   #. Determine el exponente :math:`\beta` de la relación entre la resistencia :math:`R` y la temperatura :math:`T` del filamento. Para ello, mida la corriente :math:`i` y el voltage :math:`V` en la bombilla.
   #. Construya la :numref:`tab:filatemp1`. A partir de los datos obtenidos complete las columnas 3 y 4 de la tabla.
   #. Encuentre el valor de :math:`\beta` de la ecuación :eq:`Ec:filatemp3` como se explica arriba. Encontrado :math:`\beta`, mida el valor de la resistencia :math:`R_0` de la bombilla a temperatura ambiente :math:`T_0` cuando no hay corriente por el filamento. Utilice la ecuación :eq:`Ec:filatemp4` para hallar la temperatura del filamento.


      .. csv-table:: Mediciones para determinar la relación entre la resistencia y temperatura del filamento de la bombilla.
         :header: ":math:`V\\,\\text{(V)}`", ":math:`i\\,\\text{(A)}`",":math:`P(\\text{W})=V\\times i`",":math:`R(\\Omega) =\\frac{V}{i}`"
         :widths: 1,1,1,1
         :width: 10 cm
         :name: tab:filatemp1
         :align: center

         5.0 ,.,.,.
         10.0 ,.,.,.
         15.0 ,.,.,.
         20.0 ,.,.,.
         25.0 ,.,.,.
         30.0 ,.,.,.
         35.0 ,.,.,.
         40.0 ,.,.,.
         45.0 ,.,.,.
         50.0 ,.,.,.
         55.0 ,.,.,.
         60.0 ,.,.,.
         65.0 ,.,.,.
         70.0 ,.,.,.
         75.0 ,.,.,.
         80.0 ,.,.,.
         85.0 ,.,.,.
         90.0 ,.,.,.
         95.0 ,.,.,.
         100.0 ,.,.,.
         105.0 ,.,.,.
         110.0 ,.,.,.

   #. Construya una gráfica de la temperatura del filamento en función de la corriente.
   #. Construya una gráfica de la potencia disipada en el filamento como función de su temperatura.
   #. ¿Está de acuerdo con la afirmación que hacen algunos autores cuando dicen que el punto mas caliente de una casa es el filamento de una bombilla encendida?
