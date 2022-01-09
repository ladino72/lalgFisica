+Resistencia de un conductor como función de la temperatura
=================================================================


**Objetivo**

El propósito de esta práctica es determinar el coeficiente de temperatura :math:`\alpha` de la resistencia eléctrica del cobre. Para ello, se mide la resistencia de un pedazo de alambre de cobre como función de su temperatura y a partir de los datos obtenidos se determina :math:`\alpha`

**Recursos**

   #. Una fuente voltaje DC variable.
   #. Dos multímetros digitales.
   #. Un termómetro de mercurio con un enrrollado de alambre de cobre en su bulbo.
   #. Cubeta con hielo.
   #. Cables de conexion.

**Resumen teórico**

El coeficiente de temperatura :math:`\alpha` de la resistencia eléctrica es una propiedad que cuantifica la relación entre la variación de la resistencia eléctrica del material y el cambio de su temperatura. Para un conductor, este coeficiente es constante para determinados rangos de temperatura y se tiene que

.. math::
   :label: Ec:Rest_T0

   \begin{equation}
    R=R_{0}[1+\alpha (t-t_{0})]\qquad \Longleftrightarrow \qquad \frac{R}{R_{0}} =1+\alpha \cdot \Delta t
   \end{equation}

donde :math:`R_{0}` y :math:`R` representan las resistencias eléctricas (medidas en Ohmios) a las correspondientes temperaturas :math:`t_{0}` y :math:`t` medidas en grados centigrados y :math:`\Delta t=t-t_{0}`. Usualmente :math:`t_{0}` es la temperatura ambiente. Las unidades de :math:`\alpha` son :math:`^{o}C^{-1}`.

**Descripción del problema**

Considere el circuito mostrado en la :numref:`fig:ResTemp_01`, el cual consta de una funte de voltaje variable y un alambre de cobre de longitud aproximada 5 m enrollado en el bulbo de un termómetro de mercurio. El amperímetro y voltímetro están conectados de modo que miden la corriente y el voltaje por el conductor de cobre de resistencia :math:`R`. Al pasar corriente por el alambre, este se calienta debido al efecto Joule y su temperatura se incrementa. El valor de esta temperatura se determina directamente de la lectura del termómetro.

.. figure:: /images/Electromagnetismo/Resistance_Temperature/ResTemp_01.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:ResTemp_01

   Montaje experimental para determinar la dependencia de la resistencia con la temperatura.


**Mediciones**

Manipule con mucho cuidado el termómetro, pues este es muy frágil. En caso de romper el termómetro avise a su profesor y no toque el mercurio con ninguna parte de su cuerpo. El mercurio es altamente nocivo para la salud.
Realice el montaje que se indica en la :numref:`fig:ResTemp_01`. Mida el valor de la resistencia del conductor y su temperatura antes de prender la fuente de voltaje. Estos valores medidos corresponden a resistencia :math:`R_{0}` a temperatura ambiente :math:`t_{0}`. Para ello, coloque el termómetro sobre un soporte de modo que su bulbo no toque ninguna superficie. Complete la :numref:`tab:Res_temp00`. *Advertencia:* asegúrese de no usar voltajes mayores a 5.0 V, pues a estos voltajes la corriente en el enrrollado es alta a igual que su temperatura, haciendo que este se queme. La temperatura del enrollado no debe llevarse por encima de los :math:`180\, ^{o}\text{C}`.

.. csv-table:: Datos experimentales para determinar  la dependencia de :math:`R` con :math:`t`.
   :header: ":math:`V(V)`", ":math:`I(A)`", ":math:`t(^{o}C)`"
   :widths: 1,1,1
   :width: 11 cm
   :name: tab:Res_temp00
   :align: center

   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.


Para realizar las mediciones  a :math:`0\,^{o}\text{C}` inserte con cuidado el bulbo del termómetro junto con el enrollado en una cubeta con hielo. Fije el valor del voltaje en aproximadamente 1.0 V y mida la correspondiente corriente y temperatura. Cada vez que establezca un valor del voltaje,
espere aproximadamente 5 minutos antes de medir la correspondiente corriente y temperatura. Este tiempo de espera es necesario para que se establezca el equilibrio térmico del enrollado con el medio ambiente.

A partir de la tabla de mediciones contruya la :numref:`tab:Res_temp01` y realice una grafica de :math:`\frac{R}{R_{0}}` en función de :math:`\Delta t`. De la pendiente de la recta obtenida determine el valor de :math:`\alpha`. Compare este valor con 0.0039 :math:`^{o}\text{C}^{-1}`, que es el valor que se reporta en los manuales de ingeniería para el coeficiente de temperatura de la resistencia del cobre.

Discuta sus resultados.

.. csv-table:: Datos experimentales para determinar :math:`\alpha`
   :header: ":math:`R=\\frac{V}{I} (\\Omega)`", ":math:`\\Delta t=(t-t_{0})(^{o}\\text{C})`", ":math:`\\frac{R}{R_{0}}`"
   :widths: 1,1,1
   :width: 11 cm
   :name: tab:Res_temp01
   :align: center

   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.
   .,.,.

