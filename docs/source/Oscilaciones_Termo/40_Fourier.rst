Teorema de Fourier
===================

**Objetivo**

El propósito de esta práctica es entender y aprender como mediante la superposición de ondas elementales armónicas de diferentes frecuencias y pesos es posible construir una onda periódica de cualquier perfil.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://kforinas.pages.iu.edu/WJS/SuperpositionJS.html <https://kforinas.pages.iu.edu/WJS/SuperpositionJS.html>`_.

**Resumen teórico**
Teorema de Fourier: toda función periódica (espacial o temporal) de período :math:`\lambda` puede escribirse como la suma de funciones seno y coseno, de amplitudes
y fases adecuadas. Así, para la función :math:`f(x)` mostrada en la :numref:`fig:Fourier_01`, de periodo :math:`\lambda`, de acuerdo al teorema de Fourier:

.. figure:: /images/Oscilaciones_Termo/Fourier/Fourier_01.png
   :scale: 80
   :align: center
   :name: fig:Fourier_01

   Función periódica

.. math::
   :label: Ec:fourier_01

   \begin{equation}\label{Ec:fourier_01}
     f(x)=a_0+\sum_{n=0}^{\infty}(a_n\cos\frac{2\pi n}{\lambda}x+b_n\sin\frac{2\pi n}{\lambda}x)
   \end{equation}

donde

.. math::
   :label: Ec:fourier_02a

   \begin{equation}
     a_0 = \frac{1}{\lambda}\int_{-\lambda/2}^{\lambda/2}f(x)dx
   \end{equation}

.. math::
   :label: Ec:fourier_02b

   \begin{equation}
     a_n = \frac{2}{\lambda}\int_{-\lambda/2}^{\lambda/2}f(x)\cos(\frac{2\pi nx}{\lambda})dx
   \end{equation}

.. math::
   :label: Ec:fourier_02c

   \begin{equation}
     b_n = \frac{2}{\lambda}\int_{-\lambda/2}^{\lambda/2}f(x)\sin(\frac{2\pi nx}{\lambda})dx
   \end{equation}



Obsérvese que los periodos de las funciones :math:`\cos(\frac{2\pi nx}{\lambda})` y :math:`\sin(\frac{2\pi nx}{\lambda})` son iguales y sus valores son :math:`\frac{2\pi}{\frac{2\pi n}{\lambda}}=\frac{\lambda}{n}`. Así, la función :math:`f(x)` es la suma de funciones seno y coseno de periodos :math:`\lambda, \frac{\lambda}{2},\frac{\lambda}{3}...` y los pesos o contribuciones de estas funciones son determinados por los coeficientes :math:`a_n` y :math:`b_n`.
A modo de ejemplo, la función periódica de la :numref:`fig:Fourier_square_wave` tiene periodo :math:`\lambda=4.0\,\text{cm}` y altura :math:`k`. De las ecuaciones :eq:`Ec:fourier_02a`, :eq:`Ec:fourier_02b` y :eq:`Ec:fourier_02c` resulta:

.. figure:: /images/Oscilaciones_Termo/Fourier/square_wave.png
   :scale: 60
   :align: center
   :name: fig:Fourier_square_wave

   Función periódica

.. math::
   :label: Ec:fourier_03a

   \begin{equation}
    a_0 =\frac{k}{2}
   \end{equation}

.. math::
   :label: Ec:fourier_03b

   \begin{equation}
     a_n =\frac{2k}{n\pi}\sin\frac{n\pi}{2}
   \end{equation}

.. math::
   :label: Ec:fourier_03c

   \begin{equation}
     b_n =0
   \end{equation}


De donde :math:`a_n=0` cuando :math:`n` es par, :math:`a_n=\frac{2k}{n\pi}` cuando :math:`n=1,5,9,...` y :math:`a_n=-\frac{2k}{n\pi}` cuando :math:`n=3,7,11,...`. De aquí que el resultado final es:

.. math::
   :label: Ec:fourier_04

   \begin{equation}
    f(x)=\frac{k}{2}+\frac{2k}{\pi}\left(\cos\frac{\pi}{2}x-\frac{1}{3}\cos\frac{3\pi}{2}x+\frac{1}{5}\cos\frac{5\pi}{2}x-\frac{1}{7}\cos\frac{7\pi}{2}x+\ldots\right)
   \end{equation}

Nótese que la función :math:`f(x)` queda escrita solamente en términos de funciones coseno, no hay términos tipo seno. Nota: :math:`\cos\frac{\pi}{2}x` significa :math:`\cos(\frac{\pi}{2}x)` e igual para el resto de términos.

**Construcción de una onda**

La función periódica descrita por la ecuación :eq:`Ec:fourier_04` es una función de la variable :math:`x` y tiene perfil igual al mostrado en la :numref:`fig:Fourier_square_wave`. Construyamos ahora una onda viajera que tenga este mismo perfil. Para ello, hacemos el cambio de variable :math:`x\rightarrow x-vt` en la ecuación :eq:`Ec:fourier_04` y *voila*! tenemos una onda propagándose a lo largo del eje :math:`x` con velocidad :math:`v`. La onda resultante es representada por la ecuación:

.. math::
   :label: Ec:fourier_05

   \begin{equation}
   \begin{aligned}
      F(x,t) = \frac{k}{2}+\frac{2k}{\pi}\left(\cos\frac{\pi}{2}(x-vt) \\
             -\frac{1}{3}\cos\frac{3\pi}{2}(x-vt)+\frac{1}{5}\cos\frac{5\pi}{2}(x-vt)\\
             -\frac{1}{7}\cos\frac{7\pi}{2}(x-vt)+\ldots\right)
   \end{aligned}
   \end{equation}

**Descripción de interfaz de la aplicación**

La :numref:`fig:Fourier_gui_01` muestra la interfaz gráfica del usuario, que permite ver la propagación de las ondas cuyas ecuaciones escribamos en los campos ubicados en la parte superior de la interfaz y que dicen :math:`f(x,t)` y :math:`g(x,t)`. A modo de ejemplo, hemos escrito :math:`f(x,t)=2.0\sin(x-t)` y :math:`g(x,t)=2.0\sin(x+t)` que corresponden a dos ondas armónicas viajeras que se mueven a lo largo del eje :math:`x` en direcciones contrarias (signo :math:`-` hacia la derecha y :math:`+` hacia la izquierda) con igual velocidad (:math:`v=1\,\text{cm/s}`), número de onda :math:`k=1\,\text{rad/cm}`, frecuencia angular :math:`\omega=1\,\text{rad/s}`, longitud de onda :math:`\lambda=\frac{2\pi}{k}=2\pi\,\text{cm}`, frecuencia :math:`f=\frac{\omega}{2\pi}=\frac{1}{2\pi}\,\text{Hz}` y periodo :math:`T=\frac{2\pi}{\omega}=2\pi\,\text{s}`. Los tres botones ubicados en la parte inferior de la interfaz permiten ocultar o mostrar las ondas al igual que la resultante (suma) de las ondas :math:`f(x,t)` y :math:`g(x,t)`. Los botones \textbf{play/pause} permiten correr y detener la aplicación.

.. figure:: /images/Oscilaciones_Termo/Fourier/Fourier_gui_01.png
   :scale: 70
   :align: center
   :name: fig:Fourier_gui_01

   Interfaz gráfica del usuario

**Mediciones y procedimientos**

   #. Cosidere los tres primeros términos de la expresión :eq:`Ec:fourier_05` con :math:`k=4` y :math:`v=1\,\text{cm/s}`, es decir,

      .. math::
         :label: Ec:fourier_06

         \begin{equation}
         \begin{split}
            F(x,t)=\frac{4}{2}+\frac{2\times4}{\pi}\left(\cos\frac{\pi}{2}(x-t)-\frac{1}{3}\cos\frac{3\pi}{2}(x-t)\right)\\ =2+\frac{8}{\pi}\cos\frac{\pi}{2}(x-t)-\frac{8}{3\pi}\cos\frac{3\pi}{2}(x-t)
         \end{split}
         \end{equation}

      Introduzca estos términos en el simulador. La pregunta es, ¿qué términos escribimos en la casilla :math:`f(x,t)`? y  ¿qué términos escribimos en :math:`g(x,t)`? La respuesta es: no importa, pues finalmente lo que estamos calculando es la suma :math:`u(x,t)=f(x,t)+g(x,t)`. Así, a modo de ejemplo podemos hacer :math:`f(x,t)=2+\frac{8}{\pi}\cos\frac{\pi}{2}(x-t)` y :math:`g(x,t)=-\frac{8}{3\pi}\cos\frac{3\pi}{2}(x-t)`. La onda generada resultante (suma) se visualiza en la :numref:`fig:fourier_02`. ¿La forma de la gráfica mostrada en la :numref:`fig:fourier_02` se parece a la mostrada en la :numref:`fig:Fourier_square_wave` ?

      .. figure:: /images/Oscilaciones_Termo/Fourier/Fourier_02.png
         :scale: 70
         :align: center
         :name: fig:fourier_02

         Perfil de la onda viajera cuando se consideran solamente los 3 primeros términos en la expresión :eq:`Ec:fourier_05`

   #. Repita el paso anterior pero esta vez considere los 10 primeros términos de la expresión :eq:`Ec:fourier_05`. Responda la misma pregunta del inciso anterior.
   #. Basado en los resultados anteriores ¿qué puede predecir acerca de la forma de la onda cuando se consideran más y más términos de la expresión :eq:`Ec:fourier_05` ?
   #. ¿Qué sucede si en la expresión :eq:`Ec:fourier_05` reemplazamos en cada uno de los términos :math:`x-vt` por :math:`x+2t` ? ¡Verifique su respuesta con el simulador!
   #. ¿Qué sucede si la velocidad de propagación dada por el quinto término en la expresión :eq:`Ec:fourier_05`: :math:`-\frac{8}{3\pi}\cos\frac{3\pi}{2}(x-t)` se reemplaza por :math:`v=1.5\,\text{cm/s}`, es decir, :math:`-\frac{8}{3\pi}\cos\frac{3\pi}{2}(x-1.5t)`? Analice su efecto en el simulador. Escriba sus conclusiones.
   #. Demuestre en detalle los pasos que conducen a la expresión :eq:`Ec:fourier_04`.
   #. Suponga ahora que se tienen las siguientes ondas



   #.
      .. math::
         :label: Ec:fourier_07

         \begin{equation}
            H(x,t)=\frac{4}{\pi}\sin(x-t)+\frac{4}{3\pi}\sin(3(x-t))+\frac{4}{5\pi}\sin(5(x-t))+ \frac{4}{7\pi}\sin(7(x-t))+\ldots
         \end{equation}

      ¿Qué forma tiene esta onda?, ¿cuál es su dirección y velocidad de propagación?

   #.
      .. math::
         :label: Ec:fourier_08

         \begin{equation}
          U(x,t)=\frac{2}{\pi}\sin(x-t)-\frac{2}{2\pi}\sin(2(x-t))+\frac{2}{3\pi}\sin(3(x-t))-\frac{2}{4\pi}\sin(4(x-t))+\ldots
         \end{equation}

      ¿Qué forma tiene esta onda?, ¿cuál es su dirección y velocidad de propagación?



   #. Una onda de radio AM (amplitud modulada) tiene la forma

      .. math::
         :label: Ec:fourier_09

         \begin{equation}\label{Ec:fourier_09}
          K(x,t)=[A+B\sin(2\pi ft)]\times \sin[2\pi f_c(t-\frac{x}{v})]
         \end{equation}

      el factor :math:`\sin[2\pi f_c(t-\frac{x}{v})]` se llama la onda transportadora, la cual tiene una frecuencia muy alta :math:`f_c`, llamada la frecuencia de radio y es del orden de 1 MHz. La amplitud de la onda transportadora es :math:`[A+B\sin(2\pi ft)]`, la cual varía con el tiempo de manera armónica (de ahí que se llame amplitud modulada), :math:`f` es del orden de 100 Hz y se llama la frecuencia de audio. Para poder visualizar esta onda en el simulador use los siguientes datos ficticios :math:`A=2`, :math:`B=0.5`, :math:`f=0.1`, :math:`f_c=1.0` y :math:`1.0`. Describa el comportamiento de esta onda de radio a medida que se propaga. Use relaciones trigonométricas para demostrar que :math:`K(x,t)` se puede escribir como la suma de tres ondas de frecuencias :math:`f_c`, :math:`f_c+f` y :math:`f_c-f`, la primera es la onda transportadora y las otras dos son llamadas ondas de banda laterales.


