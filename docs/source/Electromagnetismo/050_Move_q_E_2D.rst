Moviemiento den 2D de una carga eléctrica en un campo eléctrico constante
===========================================================================

**Objetivo**
El propósito de esta práctica es determinar el efecto del campo eléctrico en el movimiento de una partícula cargada.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://ophysics.com/em6.html <https://ophysics.com/em6.html>`_.

**Resumen teórico**

Cuando una partícula con carga eléctrica :math:`q`, se encuentra ya sea en reposo o en movimiento en una zona del espacio donde existe un campo eléctrico :math:`\overrightarrow{E}`, ésta experimenta una fuerza eléctrica dada por

.. math::
   :label: Ec:Mov_q_E_2D_01

   \begin{equation}
    \overrightarrow{F}=q \overrightarrow{E}
   \end{equation}

La fuerza eléctrica posee las siguientes características:

   #. es nula si la partícula es neutra, tiene la misma dirección de :math:`\overrightarrow{E}` es :math:`q>0` y dirección opuesta si :math:`q<0`.
   #. en general realiza trabajo sobre la carga eléctrica, lo que implica que su rapidez y en consecuencia su energía cinética se altera.
   #. para el caso particular cuando el campo eléctrico :math:`\overrightarrow{E}` es uniforme y la velocidad inicial :math:`\overrightarrow{v_0}` de la partícula es perpendicular a :math:`\overrightarrow{E}`, ésta describe una trayectoria parabólica.  Para la situación mostrada en la :numref:`q_In_E_plates-2D`, las ecuaciones paramétricas para la posición en :math:`x` y :math:`y` son:


.. figure:: /images/Electromagnetismo/Move_q_E_2D/plates-2D.png
   :scale: 100
   :align: center
   :name: q_In_E_plates-2D

   Partícula con carga :math:`q` y masa :math:`m` en un campo eléctrico uniforme

.. math::
   :label: Ec:mov_q_in_E-2D_ec_01

   \begin{equation}
        x = v_0t
   \end{equation}

.. math::
   :label: Ec:mov_q_in_E-2D_ec_02

   \begin{equation}
        y = \frac{1}{2}a_yt^{2}=\frac{1}{2}\frac{qE}{m}t^{2} =\frac{1}{2}\frac{qV}{dm}t^{2}
   \end{equation}


donde :math:`E` es el campo eléctrico, :math:`V` es la diferencia de potencial entre las placas.



**Descripción de la interfaz de la aplicación**

La :numref:`Fig:gui_mov_q_in_E-2D` muestra la interfaz gráfica del usuario que permite estudiar los factores que afectan la dinámica de una partícula cargada cuando ingresa de manera perpendicular a una zona donde existe un campo eléctrico uniforme generado por un par de placas paralelas a las cuales se les aplica una diferencia de potencial eléctrico. La distancia de separación y la diferencia de potencial eléctrico se pueden fijar con las barras deslizables rotuladas **Distance between plates** (cm) y **Voltage** (V) respectivamente. Tanto la carga como la masa y velocidad de la partícula se pueden fijar con las barras de desplazamiento rotuladas **Charge of particle** (:math:`\mu C`), **Particle mass** (:math:`\times 10^{-16}\,\text{kg}`) y **Initial velocity** (:math:`\times 10^{5}\,\text{m/s}`).

**Nota:** las anteriores cantidades también se pueden fijar manualmente al escribir directamente el valor deseado en la casilla correspondiente.

.. figure:: /images/Electromagnetismo/Move_q_E_2D/gui_01_mov_q_in_E-2D.png
   :scale: 55
   :align: center
   :name: Fig:gui_mov_q_in_E-2D

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

   #. Antes de iniciar explore la aplicación y examine el efecto de cada uno de los parámetros: carga (:math:`q`), masa (m), velocidad (:math:`v_0`) inicial de la partícula, distancia de separación :math:`d` entre las placas y diferencia de potencial :math:`V` entre las placas sobre la trayectoria de la partícula.
   #. ¿Qué sucede si :math:`V=0`?
   #. ¿Qué sucede si :math:`q=0`?, ¿qué sucede si :math:`q>0`? , ¿qué sucede si :math:`q<0`?
   #. Demuestre a partir de las ecuaciones :eq:`Ec:mov_q_in_E-2D_ec_01` y :eq:`Ec:mov_q_in_E-2D_ec_02` que la ecuación de la trayectoria de la partícula es una parábola, cóncava hacia arriba si :math:`q>0` y la dirección de :math:`E` es :math:`\uparrow` o :math:`q<0` y la dirección de :math:`E` es :math:`\downarrow`, y es cóncava hacia abajo si :math:`q>0` y dirección de :math:`E` es :math:`\downarrow` o :math:`q<0` y dirección de :math:`E` es :math:`\uparrow`.
   #. Fije :math:`q=0.1\,\mu\text{C}`, :math:`v_0=1\times10^{5}\,\text{m/s}`, :math:`V=100\,\text{V}` y :math:`d=5\,\text{cm}`. Se disparan partículas de masas diferentes y estas golpean los puntos rojos señalados en la :numref:`field_problem_01-2D` como 1, 2, 3, 4, 5, 6, 7, 8, 9 y 10, determine los valores de las masas de las partículas. Verifique su respuesta con el simulador.
   #. Fije :math:`q=1.0\,\mu\text{C}`, :math:`v_0=10\times10^{5}\,\text{m/s}`, :math:`V=7.2\,\text{V}`, :math:`m=0.3\,\text{kg}` y :math:`d=5\,\text{cm}`. Observe que la partícula sale de las placas justamente rozando la placa superior (ver :numref:`field_problem_02-2D`). Manteniendo fijos los parámetros anteriores excepto :math:`V` y :math:`d`, demuestre que si se quiere que la partícula pase rozando de nuevo la placa superior al variar la :math:`d` entonces debemos variar :math:`V` de modo que :math:`V=0.288d^{2}`. Verifique su respuesta con el simulador.


.. figure:: /images/Electromagnetismo/Move_q_E_2D/field_problem_01.png
   :scale: 85
   :align: center
   :name: field_problem_01-2D

   Partículas con diferentes masas llegando a diferentes puntos bajo la acción del mismo campo eléctrico.

.. figure:: /images/Electromagnetismo/Move_q_E_2D/field_problem_02.png
   :scale: 55
   :align: center
   :name: field_problem_02-2D

   Partícula sale rozando la placa superior.

