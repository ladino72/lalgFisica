+El termistor
=============

**Objetivo**

El propósito de esta práctica es aprender a calibrar un termistor y saber usarlo como instrumento de trabajo para medir temperaturas en otras situaciones que lo requieran. Para ello, se insertan el termistor y una termocupla en un recipiente con agua; a medida que la temperatura del termistor cambia su resistencia eléctrica también cambia. El agua se va calentando gradualmente mediante una fuente de calor. A partir de las lecturas de la resistencia eléctrica medida con un óhmetro y la temperatura registrada con la termocupla, se
construye la curva de resistencia en función de la temperatura absoluta. Al linealizar la curva usando el modelo propuesto abajo se obtiene la constante
que caracteriza al termistor.

**Recursos**


  #. Un termistor.
  #. Una termocupla con milivoltiímetro
  #. Un multímetro.
  #. Un recipiente con agua.
  #. Una fuente de calor (calentador eléctrico).
  #. Un par de guantes.


**Medidas de seguridad**

En esta práctica usted hará uso de una  fuente de calor (plancha eléctrica) para calentar el agua. El agua se calentará hasta una temperatura menor a la temperatura de ebullición.  Aunque usted NO necesita remover el recipiente con el agua de la superficie caliente en ningún momento, en caso de hacerlo, por favor proceda con cuidado, use guantes de protección para evitar cualquier tipo de quemaduras ya se con el agua o la superficie de la plancha caliente. En caso de necesitar ayuda puede solicitarla al profesor o al personal técnico del laboratorio.

**Resumen teórico**

Un termistor (:numref:`fig:terfig2`) es un dispositivo cuya resistencia eléctrica varía de manera significativa con la temperatura. Los termistores se clasifican en dos clases. Si su resistencia aumenta con la temperatura entonces este se denomina termistor con coeficiente de temperatura positivo o PTC. Por el contrario, si la resistencia disminuye con la temperatura entonces este se denomina termistor con coeficiente de temperatura negativo o NTC.

.. figure:: /images/Electromagnetismo/Thermistor/terfig2.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:terfig2

   Termistor tipo NTC.


La dependencia de la resistencia :math:`r` con la temperatura :math:`t` absoluta  para un termistor de tipo NTC se puede modelar bastante bien por la siguiente expresión

.. math::
   :label: Ec:ter.1

   \begin{equation}
    R=R_{0}e^{\beta\left( \frac{1}{T}-\frac{1}{T_{0}}\right) }
   \end{equation}

donde :math:`R_{0}` es la resistencia eléctrica medida en ohms a temperatura :math:`T_{0}=298.15` :math:`K` (o 25 :math:`^{o}`C) y :math:`\beta\` es una constante propia del termistor
cuyas unidades son grado Kelvin.

La ecuación :eq:`Ec:ter.1` puede ser reescrita de la siguiente manera

.. math::
   :label: Ec:ter.2

   \begin{equation}
    R=R_{\infty }e^{\frac{\beta}{T}}
   \end{equation}

donde :math:`R_{\infty }=R_{0}e^{-\frac{\beta}{T_{0}}}=` constante. Tomando logaritmo natural a ambos lados de la ecuación :eq:`Ec:ter.2` resulta

.. math::
   :label: Ec:ter.3

   \begin{equation}
    \ln R=\ln R_{\infty }+\frac{\beta}{T}
   \end{equation}

Ahora bien, si llamanos :math:`y=\ln R`, :math:`x=\frac{1}{T}`, :math:`a=\ln R_{\infty }` y :math:`m=\beta`, entonces la anterior ecuación es de la forma :math:`y=a+mx`, la cual corresponde a una relación lineal como se observa en la :numref:`fig:terfig1`.

.. figure:: /images/Electromagnetismo/Thermistor/terfig1.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:terfig1

   Linealizacion de la curva de resistencia en función de la temperatura de un termistor tipo NTC.


De esta manera, el valor de la constante :math:`\beta` que caracteriza el termistor representa la pendiente de la gráfica de :math:`\ln(R)` como función de :math:`\frac{1}{T}`. El valor de la la constante :math:`R_{\infty }` es dado por el punto de corte de la recta experimental con el eje de las ordenadas. Adviértase que las temperaturas que se usan para la construcción de la gráfica y las usadas en el modelo dado por la ecuación :eq:`Ec:ter.1` son temperaturas absolutas, es decir, se deben expresar en grados Kelvin. La relación entre temperatura absoluta medida en grados kelvin, K y la temperatura expresada en grados Celsius :math:`\text{C}` es :math:`K=273,15+^{\circ}\,\text{C}`

Una vez encontrado el valor de :math:`\beta` y :math:`R_0`, podemos medir temperaturas simplemente midiendo la resistencia del termistor en contacto con el cuerpo al que queremos determinarle la temperatura mediante la expresión

.. math::
   :label: Ec:ter.4

   \begin{equation}
    T=\frac{1}{\frac{1}{T_0}+\frac{1}{B}\ln\frac{R}{R_0}}
   \end{equation}

la cual se obtiene de la ecuación :eq:`Ec:ter.1`.


**Montaje experimental**

Realice el montaje que se indica en la :numref:`Fig:Term_Setup_01`. Este consta esencialmente de un termistor, una termocupla sumergida en un beaker con agua, una estufa con regulador de temperatura y un multímetro digital. El cable de la  termocupla va conectado directamente a un milivoltímetro, el cual muestra la temperatura de la punta de la termocupla en grados Celsius o Fahrenheit. La punta de la termocupla se encuentra muy cerca al termistor. Encienda el calentador eléctrcio y coloque la perilla de control de temperatura en 240 C y el valor del agitador en 120 (favor no exceda el valor del agitador al sugerido). Estos valores garantizan que el agua comienza a calentarse lenta y uniformemente, y nos da tiempo para hacer las lecturas de temperatura y resistencia registradas por el milivoltímetro y multímetro (en escala de ohmios) digitales respectivamente. Lea estos valores inmediatamente después que la temperatura cambia a un nuevo valor y consígnelos en la tabla :numref:`tab:termistor`. Cuando la la lectura de la termocupla indique 60 :math:`^{\circ} C` apague el calentador eléctrico. *Peligro:* No toque la superficie plana del calentador  eléctrico ni el recipiente con agua sin protección, pues estos se encuentran a alta temperatura y pueden causar serias quemaduras en la piel.

.. figure:: /images/Electromagnetismo/Thermistor/termistor_Setup.png
   :alt:
   :scale: 120
   :align: center
   :name: Fig:Term_Setup_01

   Arreglo experimental para determinar :math:`\beta` del termistor.


**Mediciones**

   #. Grafique la resistencia del termistor como función de la temperatura en grados kelvin, K.
   #. Grafique :math:`y=\ln R` como función de :math:`x=\frac{1}{T}`
   #. De la gráfica obtenida encuentre los valores de la pendiente y punto de intersección. A partir de estos valores calcule el valor de :math:`\beta`.
   #. Encuentre el valor de :math:`R_0`.
   #. *Problema de desafío*: Steinhart-Hart [#1]_ proponen una ecuación más elaborada que la dada por la ecuación :eq:`Ec:ter.1` para la relación entre la resistencia :math:`r` del termistor con su temperatura :math:`t`: :math:`\frac{1}{T}=A+B[\ln(R)]^{2}+C[\ln(R)]^{3}`. Determine los valores de :math:`A`, :math:`B` y :math:`C` para el termistor usado en la práctica.
   #. El coeficiente de temperatura de resistencia del termistor define la sensibilidad del sensor a los cambios de temperatura. Si este se define como :math:`\alpha=\frac{1}{R}\frac{dR}{dT}`. Halle el valor :math:`\alpha`.
   #. Insvestigue los diferentes tipos de termistores y sus posibles usos.
   #. ¿Entre qué rangos de temperatura funcionan los termistores?
   #. ¿Cuáles son las ventajas y desventajas de los termistores?


.. csv-table:: Datos experimentales para determinar :math:`\beta`
   :header: "Temperatura (:math:`\\,^{\\circ}` C)", "Resistencia (:math:`\\Omega`)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:termistor
   :align: center

   15,.
   16,.
   17,.
   18,.
   19,.
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
   35,.
   36,.
   37,.
   38,.
   39,.
   40,.
   41,.
   42,.
   43,.
   44,.
   45,.
   46,.
   47,.
   48,.
   49,.
   50,.
   51,.
   52,.
   53,.
   54,.
   55,.
   56,.
   57,.
   58,.
   59,.
   60,.


.. [#1] Fraiden,J, *Handbook of Modern Sensors*, Springer Verlag, York, 2004.
