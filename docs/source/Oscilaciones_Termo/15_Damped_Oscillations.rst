Oscilaciones eléctricas amortiguadas
======================================

**Objetivo**

El propósito de esta práctica es estudiar el efecto de la resistencia eléctrica :math:`R` en el caso de las oscilaciones amortiguadas libres en el circuito :math:`RLC`. En particular se examinan las oscilaciones sobreamortiguadas, cr\'{\i}ticamente amortiguadas y  subamortiguadas. Para ello se carga un condensador con una batería y luego se descarga a través del resistor e inductor conectados en serie. A partir de los voltajes dependientes del tiempo en :math:`R`, :math:`L` y :math:`C` medidos  mediante un osciloscopio se determina el efecto de :math:`R` en el decaimiento de las oscilaciones eléctricas.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.walter-fendt.de/html5/phen/oscillatingcircuit_en.htm <https://www.walter-fendt.de/html5/phen/oscillatingcircuit_en.htm>`_.

**Resumen teórico**

Oscilaciones libres amortiguadas se presentan tanto en sistemas mecánicos como eléctricos. Las primeras fueron estudiadas en la práctica \emph{Oscilaciones mecánicas Libres}. En esta práctica nos ocuparemos de las eléctricas. Para ello, consideremos el circuito de la :numref:`fig:RCL_setup`, el cual consiste de un condensador con capacitancia :math:`C` conectado en serie con un resistor e inductor de valores :math:`R` y :math:`L` y un interruptor :math:`S` de dos posiciones. Cuando el interruptor se encuentra en la posición 1, el condensador se carga. Cuando el interruptor pasa a la posición 2, el condensador se descarga. Veamos como depende la carga del condensador en función del tiempo en los casos de carga y descarga.

**Descarga del condensador**

Sea :math:`q` es la carga del capacitor en el instante de tiempo :math:`t` e :math:`i` la corriente en el circuito. La relación entre estas dos cantidades es :math:`i=-\frac{dq}{dt}`. Aplicando la segunda ley de Kirchhoff al circuito cerrado (lazo) de la derecha resulta

.. figure:: /images/Oscilaciones_Termo/Damped_Oscillations/DO_setup.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:RCL_setup

   Cicuito para estudiar las oscilaciones amortiguadas


.. math::
   :label: DO:RLC_1

   \begin{equation}
     \frac{d^{2}q}{dt^{2}}+\frac{R}{L}\frac{dq}{dt}+\frac{q}{LC}=0
   \end{equation}

La solución general de la ecuación diferencial de segundo orden :eq:`DO:RLC_1` admite tres posibles soluciones que dependen de los valores :math:`R`, :math:`L` y :math:`C`. Si se toma como condiciones iniciales :math:`q=q_0` y :math:`i=i_0` en :math:`t=0`, y si definimos :math:`\lambda=\frac{R}{2L}` y :math:`\omega^{2}=\frac{1}{LC}`, entonces se tiene:


   #. Oscilaciones subamortiguadas (:math:`\lambda ^{2}` :math:`<` :math:`\omega ^{2}`)

      .. math::
        :label: DO_SobreAmortiguado

        \begin{equation}
         q=e^{-\lambda t}[c_{1}e^{\Omega t}+c_{2}e^{-\Omega t}]
        \end{equation}

      donde :math:`\Omega =\sqrt{\lambda ^{2}-\omega ^{2}}`, :math:`c_{1}=\frac{1}{2\Omega}\left[i_{0}+(\Omega +\lambda) q_{0}\right]` y :math:`c_{2}=-\frac{1}{2\Omega}\left[i_{0}-(\Omega-\lambda)q_{0}\right]`

   #. Oscilaciones cr\'{\i}ticamente amortiguadas (:math:`\lambda ^{2}` :math:`=` :math:`\omega ^{2}`).

      .. math::
        :label: DO_Criticamente_Amortiguado

        \begin{equation}
         q=e^{-\lambda t}(c_{1}+c_{2}t)
        \end{equation}

      donde :math:`c_{1}=q_{0}` y :math:`c_{2}=i_{0}+\lambda q_{0}`


   #. Oscilaciones sobreamortiguadas (:math:`\lambda ^{2}` :math:`>` :math:`\omega ^{2}`).


      .. math::
        :label: DO_Subamortiguado

        \begin{equation}
         q=Ae^{-\lambda t}\sin (\Omega t+\phi )
        \end{equation}

      donde :math:`\Omega =\sqrt{\omega ^{2}-\lambda ^{2}}`, :math:`A=\sqrt{q_{0}^{2}+\frac{1}{\Omega ^{2}}\left( i_{0}+\lambda q_{0}\right)^{2}}` y :math:`\phi = \arcsin \frac{q_{0}}{\sqrt{q_{0}^{2}+\frac{1}{\Omega ^{2}}\left( i_{0}+\lambda q_{0}\right) ^{2}}}`


**Mediciones**

La :numref:`fig:RCL_Gui` muestra la consola de comandos que permite estudiar las oscilaciones amortiguadas de la carga :math:`q` en el capacitor en función del tiempo. Fije los valores de la capacitancia, la resistencia y autoinductancia tal como indica la figura. :math:`\varepsilon` representa la diferencia de potencial o voltaje máximo de la bateria. Las gráficas muestran las variaciones del voltaje en el capacitor y la corriente por el resistor e inductor. El medidor de tiempo mide el tiempo desde que el capacitor comienza a descargarse.

.. figure:: /images/Oscilaciones_Termo/Damped_Oscillations/DO_GUI.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:RCL_Gui

   Interfaz gráfica del usuario


**Procedimiento**

   #. Seleccione el valor de la resistencia de modo que se generen oscilaciones criticamente amortiguadas. Escriba la ecuación del voltaje en el capacitor :math:`V=\frac{q}{C}` como función del tiempo. Ayuda: :math:`i_0=0` y :math:`q_0=C\varepsilon`.
   #. Seleccione un valor para la resistencia de modo que se generen oscilaciones sobre amortiguadas. Escriba la ecuación del voltaje en el capacitor :math:`V=\frac{q}{C}` como función del tiempo.
   #. Seleccione el valor para la resistencia de modo que se generen oscilaciones subamortiguadas. Escriba la ecuación del voltaje en el capacitor :math:`V=\frac{q}{C}` como función del tiempo.
   #. Para el caso subamortiguado, tome datos que permitan ver gráficamente que la amplitud de las oscilaciones decrece exponencialmente con el tiempo. Linealice la curva obtenida y compruebe que la pendiente de la recta está relacionada con la resistencia :math:`R`.
   #. Para un sistema masa-resorte que oscila libremente sobre una superficie horizontal, donde la fuerza de rozamiento se asume toma la forma :math:`f=-bv=-\frac{dx}{dt}`, donde :math:`b` es la constante de amortiguamiento y :math:`x` es la posición de la masa, la ecuación que rige el movimiento del sistema es

.. math::
   :label: DO:RCL_3

    \begin{equation}
      \frac{d^{2}x}{dt^{2}}+\frac{b}{m}\frac{dq}{dt}+\frac{k}{m}x=0
    \end{equation}

Si se compara la ecuación :eq:`DO:RCL_3` con la ecuación :eq:`DO:RLC_1`, se oberva que las ecuaciones son matemáticamente idénticas si :math:`q\longrightarrow x`, :math:`R\longrightarrow b`, :math:`L\longrightarrow m` y :math:`\frac{1}{C}\longrightarrow k`. Lo anterior significa que para el sistema masa-resorte, también se presentarian oscilaciones criticamente amortiguadas, sobreamortiguadas y subamortiguadas. Describa para cada caso como seria el movimiento del cuerpo oscilante. ¿Qué ventaja tiene que un sistema mecánico tenga un equivalente eléctrico?

