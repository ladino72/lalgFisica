+Motor de corriente continua y dinamo
=======================================

**Objetivo**

El propósito de esta práctica es estudiar el comportamiento de un motor DC pequeño cuando opera directamente y en reversa como generador o dinamo. En el primer caso al motor se la aplica un voltaje constante y se mide la corriente de operación como función de la frecuencia de rotación de su eje. La rotación del motor se controla mediante un freno magnético. A partir de las mediciones se encuentra el voltaje inducido en el rotor y la potencia desarrollada por el motor como función de su frecuencia de rotación. En el segundo caso, el eje del motor se hace girar mediante la ayuda de otro motor y se mide el voltaje o corriente inducida como función de la frecuencia de rotación de su eje.

**Recursos**


   #. Dos motores DC pequeños conectados mediante una correa de transmisión de movimiento.
   #. Una fotointerruptor.
   #. Un osciloscopio
   #. Un multímetro.
   #. Cables de conexión.


**Resumen teórico**

La ley de Faraday (establecida en 1831)  establece que el voltaje inducido en un circuito cerrado es directamente proporcional a la rapidez con que cambia en el tiempo el flujo magnético que atraviesa una superficie cualquiera con el circuito como borde. En el caso de un inductor con :math:`N` vueltas de alambre, la ley anterior se transforma en:

.. math::
   :label: Ec:motorDC0

   \begin{equation}
    \varepsilon_i=-N\frac{d\Phi}{dt}
   \end{equation}

donde :math:`\varepsilon_i` es el voltaje inducido y :math:`\frac{d\Phi}{dt}` es la rapidez con la cual cambia el flujo magnético :math:`\Phi`. La dirección voltaje inducido (el signo negativo en la fórmula) se debe a la ley de Lenz.
El transformador, el motor y el dinamo son ejemplos de dispositivos cuyo principio de funcionamiento se basa en la ley de Faraday.


Para el caso de un motor pequeño de corriente continua (motor DC, :numref:`fig:motorDC0`) este tiene dos componentes básicos a saber, el estator (o inductor) y el rotor (o inducido). El estator genera un campo magnético en el cual gira el rotor. Este campo magnético es generado por un magneto permanente. El rotor es una pieza giratoria formada por un núcleo magnético alrededor del cual va el devanado de alambre de cobre, y sobre el que actúa el campo magnético. Al pasar corriente por el devanado, el rotor experimenta un torque magnético  y como consecuencia se produce su giro.

.. figure:: /images/Electromagnetismo/Motor_DC/motorDC0.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:motorDC0

   Esquema de un motor DC, con dos posiciones diferentes de su rotor.


**Descripción del problema**

**Motor**

Consideremos el caso de un motor DC pequeño (ver :numref:`fig:motorDC0`) cuyo devanado tiene una resistencia eléctrica igual a :math:`R`. A dicho devanado le aplicamos un  voltaje :math:`V`. Luego, por ley de Ohm una vez que el motor se encuentra girando con velocidad angular constante se cumple

.. math::
   :label: Ec:motorDC1

   \begin{equation}
   V-\varepsilon _{i}=RI
   \end{equation}

donde :math:`\varepsilon _{i}` es el voltaje inducido en el devanado, el cual por ley de Lenz es opuesto en signo al voltaje :math:`V` suministrado por la batería e :math:`I` es la corriente eléctrica en el devanado.


De la conservación de la energía se sigue que la potencia :math:`P_{b}=VI` suministrada por la batería (o fuente de voltaje) debe ser igual a la potencia disipada en :math:`R` más la rapidez con la cual el motor realiza trabajo, la cual denotamos por :math:`P`. Luego,

.. math::
   :label: Ec:motorDC2

   \begin{equation}
    VI=RI^{2}+P
   \end{equation}

multiplicando ambos lados de la ecuación :eq:`Ec:motorDC1` por :math:`I` resulta

.. math::
   :label: Ec:motorDC2.2

   \begin{equation}
    VI-\varepsilon _{i}I=RI^{2} \quad \quad \text{o} \quad \quad VI=RI^{2}+\varepsilon _{i}I
   \end{equation}

Al comparar esta expresión con la ecuación :eq:`Ec:motorDC2` se sigue que

.. math::
   :label: Ec:motorDC2.5

   \begin{equation}
    P=\varepsilon _{i}I
   \end{equation}

Esta resultado significa que la potencia útil del motor es igual al producto de la fuerza electromotriz inducida (f.e.m) y la corriente. Por otra parte, de :eq:`Ec:motorDC1` se sigue que :math:`I=\frac{V-\varepsilon _{i}}{R}`, es decir la magnitud de la corriente en el inducido depende del valor de la f.e.m, :math:`\varepsilon _{i}`. De la ley inducción de Faraday, el valor de la f.e.m inducida es proporcional a la rapidez de cambio del flujo magnético en el inducido, es decir, :math:`\varepsilon _{i}\sim \Delta \Phi / \Delta t`. Además, la rapidez de cambio del flujo magnético es a su vez proporcional a la velocidad angular :math:`\omega` del rotor. Así,

.. math::
   :label: Ec:motorDC3

   \begin{equation}
    \varepsilon _{i}\sim \Delta \Phi /\Delta t\sim \omega =k\omega
   \end{equation}

donde :math:`k` es una constante de proporcionalidad que depende de las características de diseño del motor. Así, la gráfica de la dependencia de :math:`\varepsilon _{i}` en función de :math:`\omega` es una línea recta.

Veamos ahora la dependencia de la potencia útil del motor con su velocidad angular. De las ecuaciones :eq:`Ec:motorDC1` y :eq:`Ec:motorDC3` resulta

.. math::
   :label: Ec:motorDC4

   \begin{equation}
    I=\frac{V-k\omega }{R}
   \end{equation}

reemplazando este valor de la corriente en la ecuación :eq:`Ec:motorDC2.5` se
obtiene

.. math::
   :label: Ec:motorDC5

   \begin{equation}
    P=\frac{kV\omega -k^{2}\omega ^{2}}{R}
   \end{equation}

Las dependencias de la f.e.m inducida, corriente :math:`I` y potencia útil :math:`P` como función de la
velocidad angular del inducido se muestran en la :numref:`fig:motorDC1`. De la figura se sigue que existen dos valores de velocidades angulares diferentes para los
cuales la potencia útil es la misma. Además, entre mayor es la velocidad angular del motor menor es el valor de la corriente que circula por su devanado.

¿Cómo depende la velocidad angular :math:`\omega`  del torque producido por la corriente sobre el devanado debido al campo
magnético? La fuerza magnética  sobre el inducido es proporcional a su corriente :math:`I`, y por tanto el torque :math:`M_{e}` producido por esta fuerza también es proporcional  a  :math:`I`.

.. figure:: /images/Electromagnetismo/Motor_DC/motorDC1.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:motorDC1

   Relación entre la f.e.m :math:`\varepsilon_{i}`, corriente :math:`I` y potencia :math:`p` útil como función de la velocidad angular :math:`\omega`.

.. math::

   M_{e}=k_{1}I

combinando este resultado con la expresión :eq:`Ec:motorDC4` resulta

.. math::
   :label: Ec:motorDC7

   \begin{equation}
    M_{e}=k_{1}\frac{V-k\omega }{R}
   \end{equation}

ésta expresión indica que el torque eléctrico depende linealmente de la velocidad angular del inducido. El torque es grande cuando la velocidad
angular es baja; cuando la velocidad aumenta el torque disminuye y se hace cero cuando

.. math::
   :label: Ec:motorDC15

   \begin{equation}
   \omega =\frac{V}{k}
   \end{equation}


Por otra parte, un torque mecánico actúa sobre el eje del motor (pues los motores se usan para transmitir movimiento). Si el motor levanta por ejemplo
una carga de peso :math:`mg` mediante una cuerda ligera con velocidad constante, entonces el torque mecánico es :math:`M=mgr`, donde :math:`r` es el radio del eje del
motor. En este caso, el torque eléctrico :math:`M_{e}` se hace igual al torque mecánico :math:`M`, es decir :math:`M_{e}=M`  y la velocidad angular de la ecuación :eq:`Ec:motorDC7` es

.. math::
   :label: Ec:motorDC8

   \begin{equation}
   \omega _{0}=\frac{k_{1}V-MR}{k_{1}k}
   \end{equation}

Así, el torque mecánico determina la velocidad angular del inducido al igual que su corriente.

**Dinamo**

El motor DC es una máquina eléctrica reversible. Esto significa que si hacemos rotar su devanado con la ayuda de algún dispositivo (por ejemplo con otro motor) esta máquina genera corriente eléctrica y se denominada dinamo o generador.  Así, el dinamo de una bicicleta transforma la energía mecánica del movimiento de las ruedas en la energía eléctrica que necesita el faro para alumbrar.
Dado que la f.e.m inducida en el motor depende solamente del diseño del motor y de la velocidad angular :math:`\omega` de su rotor, se sigue entonces que cuando este opera como dinamo la f.e.m que se induce debe ser la misma. Por tanto, si las velocidades de rotación de motor y dinamo son :math:`\omega_m` y :math:`\omega_d` entonces la relación entre los voltajes inducidos en el motor y dinamo es

.. math::
   :label: Ec:motorDC9

   \begin{equation}
    \frac{\varepsilon_d}{\varepsilon_m}=\frac{ \omega_d}{ \omega_m}
   \end{equation}

La ley de Ohm aplicada al dinamo se reduce a

.. math::
   :label: Ec:motorDC9.5

   \begin{equation}
   \varepsilon _{d}=RI_{d}
   \end{equation}

donde :math:`\varepsilon _{d}` , :math:`R` y :math:`I_{d}` representan el voltage inducido, la resistencia y la corriente en el dinamo. La ecuación equivalente a la :eq:`Ec:motorDC2` es

.. math::
   :label: Ec:motorDC10

   \begin{equation}
   P_{m}=\varepsilon _{d}I_{d}
   \end{equation}

donde :math:`P_{m}` es la potencia mecánica que se emplea para hacer girar el rotor y :math:`\varepsilon _{d}I_{d}` es la potencia eléctrica producida por el generador.


**Montaje Experimental**

Considere el esquema de la :numref:`fig:motorDC2`, el cual consta de dos motores DC pequeños (motor :math:`A` y motor :math:`B`) conectados mediante una correa ligera, con lo cual la velocidad de los motores es igual.
Si al motor :math:`A` se le aplica una diferencia de potencial :math:`V`, este gira y transmite su movimiento al motor :math:`B`, convirtiéndolo en dinamo. El motor :math:`A` tiene conectado en su eje un disco delgado de aluminio, el cual posee 4 ranuras dispuestas de manera radial. El propósito de este disco es doble: a) permite determinar la velocidad angular :math:`\omega` del eje del motor al obstruir el fotointerruptor repetidamente y b) permite mediante su interación con el imán cambiar la velocidad de rotación :math:`\omega=2\pi f` del motor; las corrientes parásitas que se inducen en el disco se traducen en un torque sobre el eje del motor. El valor de este torque es mayor entre menor es la distancia imán-disco. Este sistema de frenado del disco constituye un freno magnético.
Si ahora, solamente al motor :math:`B` se la aplica una diferencia de potencial :math:`V`, este gira y transmite su movimiento al motor :math:`A`, convirtiéndolo en dinamo.

.. figure:: /images/Electromagnetismo/Motor_DC/motorDC2.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:motorDC2

   Esquema que se utiliza para estudiar el motor y la dinamo. Izquierda: vista lateral. Derecha: vista superior.

.. figure:: /images/Electromagnetismo/Motor_DC/motorDC3.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:motorDC3

   Montaje experimental para estudiar el motor DC.

.. figure:: /images/Electromagnetismo/Motor_DC/motorDC4.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:motorDC4

   Montaje experimental para estudiar el dinamo.


**Mediciones**

**Motor**

Realice el montaje experimental que se indica en la :numref:`fig:motorDC3` y apliquemos un voltaje al motor :math:`A` de modo que  :math:`V=4\,\text{V}`. En esta parte a pesar de que el motor :math:`B` se encuentra rotando puede ser ignorado. El amperímetro conectado en serie como indica la figura registra el valor de la corriente que circula por el devanado del motor. La señal del fotointerruptor, la cual consiste de una serie de pulsos rectangulares es enviada al osciloscopio una vez que ha sido acondicionada por un circuito alojado en la caja negra adjunta al imán. Si la frecuencia de la señal medida en en osciloscopio es :math:`f_0`, la frecuencia del motor en Hertz es dada por :math:`f=\frac{f_0}{4}`. Una vez fijado el valor del voltaje :math:`V` aplicado al motor, la corriente en el motor es grande entre mayor sea la acción del freno magnético.


.. Note:: No mantenga frenado el motor por mucho tiempo, pues el devanado podría recalentarse y llegar al punto de quemarse causando daño permanente al motor.

Complete la :numref:`table:MotorDC_tab1`.

   #. Usando la ecuación :eq:`Ec:motorDC4` y a partir de las mediciones encuentre el valor de :math:`K` y la resistencia :math:`R` del devanado.
   #. Usando los resultados anteriores y la ecuación :eq:`Ec:motorDC1` construya la gráfica de voltaje inducido :math:`\varepsilon_i` en función de la frecuencia :math:`\omega`. Es la relación entre :math:`\varepsilon_i` y :math:`\omega=2\pi f` lineal? Discuta sus resultados.
   #. Usando los resultados anteriores construya la gráfica de la potencia desarrollada por el motor en función de :math:`\omega`. De la gráfica encuentre el valor de la frecuencia :math:`\omega` para el cual la potencia es máxima. Compare con la teoría.

.. csv-table:: Mediciones relacionadas con el motor. *No haga circular corriente por el motor mayores a 0.7 A*
      :header: "Corriente :math:`I` (A)", "Frecuencia :math:`f` (Hz)"
      :widths: 1,1
      :width: 10 cm
      :name: table:MotorDC_tab1
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
      0.70,.


**Dinamo**

Realice el montaje experimental que se indica en la :numref:`fig:motorDC4` y aplique un voltaje :math:`V=4\,\text{V}` al motor :math:`B`. De esta manera el motor :math:`A` se convierte en un dinamo o generador. El voltímetro se conecta directamente al motor :math:`B` o generador y su lectura corresponde al voltaje inducido :math:`\varepsilon_d`. Complete la :numref:`table:MotorDC_tab2`.


   #. Mida el voltaje inducido :math:`\varepsilon_d` en el dinamo como función de la frecuencia :math:`\omega=2\pi f`. Es la relación entre :math:`\varepsilon_d` y :math:`\omega` lineal? Discuta sus resultados.
   #. Realice una gráfica de la potencia obenida en el dinamo como función :math:`\omega`. Discuta sus resultados.


.. csv-table:: Mediciones relacionadas con el dinamo. *No haga circular corriente por el dinamo mayores a 0.7 A*.
      :header: "Voltaje inducido :math:`\\varepsilon_d` (V)", "Frecuencia :math:`f` (Hz)"
      :widths: 1,1
      :width: 10 cm
      :name: table:MotorDC_tab2
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
      0.70,.


**Pregunta**

¿Cómo verifica Usted la afirmación hecha arriba acerca de que el voltaje inducido en el motor es el mismo que cuando este opera como dinamo? Soporte su afirmación cuantitativamente.
