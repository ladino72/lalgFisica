+Oscilaciones forzadas en el circuito RLC
================================================

**Objetivo**

El propósito de esta práctica es estudiar el fenómeno de la resonancia en un circuito RLC cuando este es alimentado con una fuente de voltaje alterno. En particular se analiza efecto de la resistencia en el estado de resonancia del circuito.


**Recursos**

   #. Un osciloscopio de doble canal.
   #. Un Un generador de funciones.
   #. Un Un protoboard
   #. Un  Caja de resistores.
   #. Un Caja de capacitores.
   #. Un Una bobina
   #. Un Cables de conexión

**Resumen teórico**

Sistemas tanto mecánicos como eléctricos manifiestan un fenómeno interesante cuando estos son perturbados por fuerzas o señales periódicas respectivamente. La respuesta de estos sistemas crece notablemente cuando la frecuencia de excitación aplicada es próxima a la frecuencia natural de ellos. La frecuencia para la cual la respuesta es máxima se denomina frecuencia de resonancia. Entre menos rozamiento tengan estos sistemas, la frecuencia de resonancia tiende a coincidir con la frecuencia natural. Sistemas eléctricos simples tales como el circuito RLC poseen una frecuencia de resonancia que depende de la de la capacitancia y la auto inductancia. Sistemas complejos  pueden tener varias frecuencias de resonancia.


**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:Forced_oscilations_00`, el cual consta de un condensador de capacitancia :math:`C`, un resistor de resistencia :math:`R` y una bobina de auto inductancia :math:`L` conectados en serie a una fuente de voltaje alterno, cuya dependencia con el tiempo es de la forma  :math:`V(t)=V_0\sin \omega t`, siendo :math:`V_0` y :math:`\omega=2\pi f` la amplitud y la frecuencia angular.

La corriente y voltaje en cada uno de los elementos es gobernada por las leyes de Kirchhoff [#f1]_, [#f2]_. Si en cierto instante de tiempo :math:`t`, la corriente es :math:`I` y la carga del condensador es :math:`q`, de la segunda ley de Kirchhoff (ver :numref:`fig:Forced_oscilations_01`) resulta:

.. figure:: /images/Oscilaciones_Termo/Forced_Oscillations_RLC/Forced_oscilations_00.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Forced_oscilations_00

   Circuito RLC forzado armónicamente


.. figure:: /images/Oscilaciones_Termo/Forced_Oscillations_RLC/Forced_oscilations_01.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Forced_oscilations_01

   Corriente :math:`I` y carga  :math:`q` en cierto instante de tiempo :math:`t`


.. math::
   :label: Ec:forced_Osc_01

   \begin{equation}
    V_0\sin\omega t-Ri-L\frac{di}{dt}-\frac{q}{C}=0
   \end{equation}

donde :math:`i=+\frac{dq}{dt}`. Al definir :math:`\omega_0^{2}=\frac{1}{LC}`, :math:`\lambda=\frac{R}{2L}` y reemplazar el valor de :math:`I`, la anterior ecuación se convierte en:

.. math::
   :label: Ec:forced_Osc_02

   \begin{equation}
    \frac{d^{2}i}{dt^{2}}+2\lambda\frac{di}{dt}+\omega_0^{2}i=\frac{\omega V_0}{L}\cos\omega t
   \end{equation}

la solución de la ecuación :eq:`Ec:forced_Osc_02` en el régimen estacionario es dada por:

.. math::
   :label: Ec:forced_Osc_03

   \begin{equation}
    i(t)=I_0(\omega)\cos(\omega t-\phi)
   \end{equation}

donde

.. math::
   :label: Ec:forced_Osc_04

   \begin{equation}
    I_0(\omega)=\frac{V_0}{\sqrt{R^{2}+(\omega L-\frac{1}{\omega C})^{2}}}
   \end{equation}

y

.. math::
   :label: Ec:forced_Osc_05

   \begin{equation}
   \tan\phi=\frac{\omega L-\frac{1}{\omega C}}{R}
   \end{equation}

Obsérvese que tanto la amplitud :math:`I_0` de las oscilaciones en la corriente como la fase :math:`\phi` dependen de la frecuencia angular :math:`\omega=2\pi f` de la fuente de voltaje alterna.
Se puede demostrar que la amplitud :math:`I_0` presenta un máximo cuando :math:`\omega_r = \sqrt{\omega_0^{2}-2\lambda^{2}}=\sqrt{\frac{1}{LC}-\frac{R^{2}}{2L^{2}}}`. Es decir, la frecuencia en Hertz para la cual la amplitud es máxima es dada por:

.. math::
   :label: Ec:forced_Osc_06

   \begin{equation}
   f_r=\frac{1}{2\pi}\sqrt{\frac{1}{LC}-\frac{R^{2}}{2L^{2}}}
   \end{equation}

la cual se denomina frecuencia de resonancia del sistema.

En las anteriores expresiones se suponen elementos ideales, es decir que la resistencia de la bobina es cero y que la fuente de voltaje no presenta resistencia óhmica alguna. Así, si se tienen en cuenta que en general estos valores son no nulos, el valor de :math:`R` se debe reemplazar por :math:`R=R_1+R_g+R_b`, donde :math:`R_1` es la resistencia del resistor físico que se conecta en serie con :math:`C` y :math:`L`, :math:`R_g` es la resistencia del generador de funciones que es de 50 :math:`\Omega` y :math:`R_b` es la resistencia de la bobina con auto inductancia :math:`L`.

El voltaje en el resistor :math:`R_1`  como función del tiempo es dado por

.. math::

    V_{1}(t)=R_1I_0\sin(\omega t-\phi)=V_{10}\sin(\omega t-\phi)

donde :math:`V_{10}` es la amplitud del voltaje en la resistencia física y es dado por

.. math::
   :label: Ec:forced_Osc_07

   \begin{equation}
   V_{10}=R_1I_0= \frac{R_1V_0}{\sqrt{R^{2}+(\omega L-\frac{1}{\omega C})^{2}}}
   \end{equation}


**Montaje experimental**

*Valores sugeridos:* :math:`C=0.0047\,\mu\text{F}`, :math:`L=47\,\text{mF}`, :math:`R_1=1\,k\Omega` ó :math:`R_1=2\, k\Omega`.

Realice el montaje que se muestra en la :numref:`fig:forced_Setup_01`, el cual consiste de un capacitor de capacitancia :math:`C`, una bobina con auto inductancia :math:`L` un resistor de resistencia :math:`R_1` conectados en serie a un generador de funciones que suministra una onda senoidal de frecuencia :math:`f`. En el osciloscopio de doble canal se observan: la señal senoidal de frecuencia :math:`f` y el voltaje en el elemento :math:`R_1`. Las tierras del osciloscopio y el generador de funciones están conectadas entre sí.

.. figure:: /images/Oscilaciones_Termo/Forced_Oscillations_RLC/Experimental_Setup.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:forced_Setup_01

   Arreglo experimental para determinar el valor total de :math:`R`.

**Mediciones**

   #. Mida el valor de la capacitancia :math:`C` con el multímetro digital.
   #. Mida el valor de la auto inductancia  :math:`L`  de la bobina con el multímetro digital.
   #. Mida el valor de la resistencia :math:`R_b` de la bobina con el multímetro digital.
   #. Mida el valor de la resistencia  :math:`R_1` del resistor con multímetro digital.
   #. Fije el valor de la amplitud de la señal senoidal en :math:`V_0= 5\,\text{V}`. *Atención:* a pesar de que el voltaje :math:`V_0` se fija, al variar la frecuencia del generador de funciones su valor puede variar. De esta manera verifique y ajuste su valor (manteniéndolo constante) si es necesario cada vez que cambie la frecuencia del generador. Sin tomar datos: varíe el valor de :math:`f` y observe como cambia el valor de la amplitud :math:`V_{10}` en el osciloscopio. Si todo está bien, debería observar que al aumentar :math:`f`, :math:`V_{10}` crece y luego disminuye sustancialmente. Tenga en cuenta el rango de frecuencias para el cual se presenta esta situación.
   #. Mida la amplitud :math:`V_{10}` de las oscilaciones del voltaje en :math:`R_1` como función de la frecuencia  :math:`f`, variando ésta última dentro del rango observado en el inciso 5. Registre el valor de la frecuencia :math:`f` y el correspondiente valor de :math:`V_{10}` en la :numref:`tab:forced_osc`. Repita el procedimiento anterior para diferentes frecuencias (por lo menos 15).
   #. A partir de los datos de la :numref:`tab:forced_osc` grafique :math:`V_{10}` en función de :math:`\gamma=2\pi f`. Describa el comportamiento de la gráfica y a partir de ésta determine el valor de la frecuencia :math:`\omega_r` para el cual la amplitud de las oscilaciones es máxima. ¿Cómo se compara el valor obtenido de esta frecuencia angular con el dado por la expresión :math:`\omega_r =\sqrt{\frac{1}{LC}-\frac{R^{2}}{2L^{2}}}`?
   #. Grafique :math:`V_{10}` en función de :math:`\gamma=2\pi f`, ecuación :eq:`Ec:forced_Osc_07`, usando los valores de :math:`C`, :math:`L`, :math:`R_b` y :math:`R_1`  medidos en los incisos 1, 2, 3 y 4 respectivamente. Recuerde que :math:`R=R_g+R_b+R_1`. Superponga ésta gráfica con la obtenida en el inciso 5. ¿La gráfica obtenida se ajusta o se superpone perfectamente a la obtenida en el inciso 7? Explique las discrepancias.
   #. El factor de calidad :math:`Q` del circuito RLC se define como :math:`Q=\frac{\omega_0}{\Delta \omega}`, donde :math:`\Omega` es el rango de frecuencias para la cual la potencia promedio :math:`<P(t)>` transferida del generador de funciones al circuito es mayor que un medio de la potencia promedio máxima (ver :numref:`fig:Forced_oscilations_03`). Ahora bien, nosotros no medimos potencia directamente, luego no podemos generar la curva mostrada en la :numref:`fig:Forced_oscilations_03`. No obstante, se puede demostrar teóricamente que el valor de :math:`\Delta \omega`  se puede obtener a partir de la curva de  :math:`V_{10}` como función de :math:`\omega=2\pi f` tal como indica la :numref:`fig:Forced_oscilations_04`; este es dado por :math:`\omega=\omega_{+}-\omega_{-}`. Halle el valor de :math:`Q` para el circuito usado.  En qué afecta el valor de :math:`Q` medido si :math:`R_b\sim R_g\sim R_1`?; y si :math:`R_g<< R_1` y :math:`R_b<<R_1`? Discuta sus resultados.
   #. Ahora duplique el valor :math:`R_1`  y repita los pasos anteriores. Compare las curvas de :math:`V_{10}` como función de la frecuencia y los factores de calidad :math:`Q`. Discuta sus resultados.


      .. figure:: /images/Oscilaciones_Termo/Forced_Oscillations_RLC/Forced_oscilations_03.png
         :alt:
         :scale: 100
         :align: center
         :name: fig:Forced_oscilations_03

         Ancho de banda del pico.

      .. figure:: /images/Oscilaciones_Termo/Forced_Oscillations_RLC/Forced_oscilations_04.png
         :alt:
         :scale: 100
         :align: center
         :name: fig:Forced_oscilations_04

         Ancho de banda del pico.

      .. csv-table:: Datos experimentales para determinar :math:`R` y :math:`R_1`
         :header: "Frecuencia :math:`f` (Hz)", ":math:`V_{10}` (V)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:forced_osc
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
         .,.
         .,.
         .,.
         .,.


.. [#f1] Serway, R., *FISICA para ciencias e ingeniería*, McGraw-Hill, Tomo 2, México, 2000.
.. [#f2] Sanny Sanny, J.,Moebs, W., *University Physics*, Wm. C. Brown Publishers}, Vol 2, Loyola Marymount University, 1996.
