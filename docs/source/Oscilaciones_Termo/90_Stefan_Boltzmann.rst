+Determinación de la constante de Stefan-Boltzmann
===================================================

**Objetivo**

El propóito de esta práctica es determinar el valor de la constante de Stefan-Boltzmann, :math:`\sigma`. Para ello, se utiliza una bombilla pequeña, por cuyo filamento de tungsteno se hace pasar una corriente eléctrica. Se asume que el filamento se comporta en una buena aproximación como un cuerpo negro y que su resistencia óhmica :math:`R` depende de la temperatura absoluta :math:`T` siguiendo la ley :math:`R\propto T^{\eta^{-1}}`, donde :math:`\eta` es una constante a determinar.  De las mediciones de la corriente y voltaje en el filamento junto con el modelo propuesto abajo se determina el valor de :math:`\sigma`.


**Recursos**

   #. Una fuente de voltaje.
   #. Dos multímetros digitales
   #. Cables de conexión
   #. Una bombilla pequeña


**Resumen Teórico**

Todos los cuerpos a una temperatura absoluta diferente de cero emiten radiación. La naturaleza de la radiación emitida depende de la temperatura
del cuerpo. Se denomina *cuerpo negro* aquel que es capaz de absorber cien por ciento  toda la radiación  que incide sobre él; de este modo el cuerpo negro no refleja la radiación. Un cuerpo negro también es un buen emisor de radiación.  Las estrellas, un horno a alta temperatura y el filamento de una
bombilla incandescente  son cuerpos cuya radiación se asemeja a la emitida por un cuerpo negro.

La potencia de la radiación emitida por un cuerpo negro cuya superficie tiene un área :math:`A` y que se encuentra a una temperatura  :math:`T`, es dada por

.. math::
   :label: Ec:SB_01

   \begin{equation}
   P=A\sigma T^{4}
   \end{equation}

donde :math:`\sigma=5.67\times 10^{-8} \,Wm^{-2}K^{-4}` representa la constante de Stefan-Boltzmann.

La potencia consumida por el filamento es

.. math::
   :label: Ec:SB_02

   \begin{equation}
    P=Ri^{2}
   \end{equation}

Si se asume que la radiación proveniente de una bombilla incandescente se asemeja a la radiación de un cuerpo negro y que la potencia
eléctrica que consume la bombilla se convierte completamente en radiación entonces

.. math::
   :label: Ec:SB_03

   \begin{equation}
    P=Ri^{2}=A\sigma T^{4}
   \end{equation}

donde :math:`R` e :math:`i` representan la resistencia  y corriente eléctrica. La relación entre la corriente y el voltaje en el filamento de la bombilla no es lineal y por otra parte su resistencia eléctrica depende de la temperatura. Evidencia experimental demuestra que :math:`T\propto R^{\eta }`, donde :math:`\eta ` es una constante. Combinando esta expresión con :eq:`Ec:SB_03` resulta

.. math::
   :label: Ec:SB_04

   \begin{equation}
   P=Ri^{2}=A\sigma T^{4}=\text{const}\times R^{4\eta }
   \end{equation}

De  esta última expresión se sigue que

.. math::
   :label: Ec:SB_020

   \begin{equation}
    i=\text{const}\times R^{\frac{4\eta -1}{2}}
   \end{equation}

y el valor de :math:`\eta ` se puede determinar en terminos del valor de la pendiente :math:`m` de la gráfica de :math:`\log i` en función de :math:`\log R` (ver :numref:`fig:SB_01`).  El valor de :math:`\eta` es dado por

.. math::
   :label: Ec:SB_021

   \begin{equation}
   \frac{2m+1}{4}
   \end{equation}

Conocido el valor de :math:`\eta` se desprende que

.. figure:: /images/Oscilaciones_Termo/Stefan_Boltzmann/Stefan_Boltzmann_00.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:SB_01

   Linalización de la relación :math:`i=\text{const}\times R^{\frac{4\eta -1}{2}}`.


.. math::
   :label: Ec:SB_05

   \begin{equation}
   T=\left( \frac{R}{R_{0}}\right) ^{\eta }T_{0}
   \end{equation}

donde :math:`R_{0}` es la resistencia de la bombilla a la temperatura de referencia :math:`T_{0}`, que puede ser la temperatura ambiente.
Reemplazando el valor de :math:`T` de la ecuación :eq:`Ec:SB_05` en la ecuación :eq:`Ec:SB_04` se sigue que

.. math::
   :label: Ec:SB_06

   \begin{equation}
   P=A\sigma \left( \frac{T_{0}}{R_{0}^{\eta}}\right)^{4}R^{4\eta}
   \end{equation}

Ahora al realizar una gráfica de :math:`P` en función de :math:`R^{4\eta}`, se obtiene una línea recta con pendiente

.. math::
   :label: Ec:SB_07

   \begin{equation}
   p=A\sigma\left( \frac{T_{0}}{R_{0}^{\eta}}\right)^{4}
   \end{equation}

Por otra parte, el filamento de la bombilla se puede considerar como un alambre cilíndrico de radio :math:`r_o` y longitud :math:`\ell_o`. Su resistencia óhmica a temperaura :math:`T_o` es dada por :math:`R_o=\rho \frac{\ell}{\pi r_o^{2}}`, donde :math:`\rho` es la resistividad del tungsteno; y el área de su superficie emisora de radiación del filamento es :math:`A=2\pi r_0\ell_o`. De estas dos expresiones se sigue que

.. math::
   :label: Ec:SB_08

   \begin{equation}
   A=\frac{2\pi^{2}r_o^{3}R_o}{\rho}
   \end{equation}

De las ecuaciones :eq:`Ec:SB_07` y :eq:`Ec:SB_08` se sigue finalmente que

.. math::
   :label: Ec:SB_09

   \begin{equation}
    \sigma=\frac{p\rho}{2\pi^{2}r_o^{3}}\frac{R_o^{4\eta-1}}{T_o^{4}}
   \end{equation}

De esta manera, el valor de la constante de Stefan-Boltzmann se puede determinar a partir de las mediciones de la resistencia óhmica :math:`R_o`  del filamento a temperatura ambiente :math:`T_o` y el valor del radio :math:`r_o` del filamento de la bombilla; el valor de la resistividad del tungsteno  a temperatura :math:`T_o` el cual es dado por  :math:`\rho=5.5\times 10^{-8}\,\Omega \cdot \text{m}` y el valor de :math:`p` dado por el valor de la pendiente de :math:`P` en función de :math:`R^{4\eta}`.


**Descripción del Problema**

El arreglo experimental para determinar la constante de Stefan-Boltzmann (ver :numref:`fig:SB_02`) consiste esencialmente de una bombilla incandescente de :math:`12` V, conectada a una fuente de voltaje DC variable. El amperímetro mide la corriente eléctrica por el filamento de la bombilla y el voltímetro su diferencia de potencial eléctrico.

.. figure:: /images/Oscilaciones_Termo/Stefan_Boltzmann/Stefan_Boltzmann_01.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:SB_02

   Arreglo experimental para determinar :math:`\sigma`.


**Mediciones y Procedimientos**

   #. Realice el montaje que se describe en la :numref:`fig:SB_02`.
   #. Antes de conectar el bomillo al circuito, mida el valor de su resistencia eléctrica a temperatura ambiente con el óhmetro.
   #. Antes de aplicar cualquier diferencia de potencial a la bombilla asegúrese de que el dial de la fuente de voltaje se encuentre completamente girado en el sentido anti horario, esto se hace con el fin de garantizar que la diferencia de potencial suministrada por la fuente sea cero voltios.
   #. Determine el exponente :math:`\eta` de la relación entre la corriente :math:`i` y la  resistencia :math:`R` del filamento de la bombilla. Para ello, mida la corriente :math:`i` y el voltage :math:`V` en la bombilla con un rango de voltaje comprendido entre 0 y 12 V máximo. Si aplica un voltaje mayor a 12 V, el filamento de la bombilla se quema!
   #. Construya la :numref:`tab:SB_01`. A partir de los datos obtenidos encuentre el valor de :math:`\eta` de la ecuación :eq:`Ec:SB_020` como se explica más arriba.
   #. Encuentre el valor de :math:`p` de la pendiente de la línea recta obtenida al graficar :math:`P` en función de :math:`R^{4\eta}`. Utilice la información del radio :math:`r_o` del filamento de la bombilla [#f1]_ suministrado y calcule el valor de :math:`\sigma`.

   Compare el valor obtenido con el valor teórico y discuta las posibles discrepancias en los resultados.

   .. csv-table:: Mediciones para determinar el valor de :math:`\sigma`
      :header: ":math:`V\\,\\text{(V)}`", ":math:`i\\,\\text{(A)}`",":math:`R(\\Omega)=\\frac{V}{i}`", ":math:`P(\\text{W})=Ri^{2}`",":math:`R^{4\\eta}`"
      :widths: 1,1,1,1,1
      :width: 12 cm
      :name: tab:SB_01
      :align: center

      0.0 ,.,.,.,.-
      0.5 ,.,.,.,.
      1.0 ,.,.,.,.
      1.5 ,.,.,.,.
      2.0 ,.,.,.,.
      2.5 ,.,.,.,.
      3.0 ,.,.,.,.
      3.5 ,.,.,.,.
      4.0 ,.,.,.,.
      4.5 ,.,.,.,.
      5.0 ,.,.,.,.
      5.5 ,.,.,.,.
      6.0 ,.,.,.,.
      6.5 ,.,.,.,.
      7.0 ,.,.,.,.
      7.5 ,.,.,.,.
      8.0 ,.,.,.,.
      8.5 ,.,.,.,.
      9.0 ,.,.,.,.
      9.5 ,.,.,.,.
      10.0 ,.,.,.,.
      10.5 ,.,.,.,.
      11.0 ,.,.,.,.
      11.5 ,.,.,.,.
       12.0 ,.,.,.,.

.. [#f1] El radio :math:`r_o` del filamento fue medido con un microscopio de luz.