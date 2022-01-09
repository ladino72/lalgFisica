+Circuito RC
============

**Objetivo**

 El propósito de esta práctica es estudiar el proceso de carga y descarga de un capacitor.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://physics.bu.edu/~duffy/HTML5/RC_circuit.html <http://physics.bu.edu/~duffy/HTML5/RC_circuit.html>`_.

**Resumen teórico**


**Carga del Capacitor**

Consideremos el circuito mostrado en la :numref:`fig:RC_circuit_01`, el cual consta de una fuente de voltaje :math:`\varepsilon`, un resistor de resistencia :math:`R`, un capacitor de capacitancia :math:`C` y un interruptor :math:`S`. Inicialmente, el capacitor tiene una carga :math:`q_0`.  Al cerrar :math:`S`, la carga :math:`q`  en el capacitor crece en el tiempo :math:`t`. La corriente eléctrica en el circuito es :math:`i=\frac{dq}{dt}`. Aplicando la segunda ley de Kirchhoff al lazo cerrado resulta


.. math::
   :label: RC1

   \begin{equation}
    \frac{dq}{dt}+\frac{1}{RC}q=\frac{\varepsilon }{R}
   \end{equation}

.. figure:: /images/Electromagnetismo/RC_Circuit/RC_circuit_01.png
   :scale: 100
   :align: center
   :name: fig:RC_circuit_01

   Circuito RC: Carga del capacitor

La solución de la ecuación :eq:`RC1` sujeta a la condición inicial :math:`q=q_0` en :math:`t=0` es

.. math::
   :label: RC2

   \begin{equation}
    q(t)=C\varepsilon -(C\varepsilon-q_0)e^{-\frac{t}{\tau }}
   \end{equation}

donde :math:`\tau =RC` es la constante de tiempo o tiempo de relajación del circuito. Obsérvese que la carga final del capacitor es :math:`C\varepsilon`, independiente de la carga inicial que tenía en :math:`t=0`. Los voltajes en el capacitor y el resistor son :math:`V_{c}=\frac{q}{C}` y :math:`V_R=Ri` respectivamente.

**Descarga del Capacitor**

Inicialmente la carga del capacitor es :math:`Q_0`, ver :numref:`fig:RC_circuit_02`. Al cerrar el interruptor :math:`S`, el capacitor se descarga a través del resistor, es decir su carga decrece en el tiempo :math:`t`. La corriente eléctrica en el circuito es :math:`i=-\frac{dq}{dt}`. Aplicando la segunda ley de Kirchhoff al lazo cerrado, resulta

.. figure:: /images/Electromagnetismo/RC_Circuit/RC_circuit_02.png
   :scale: 100
   :align: center
   :name: fig:RC_circuit_02

   Circuito RC: descarga del capacitor

.. math::
   :label: RC3

   \begin{equation}
    \frac{dq}{dt}=-\frac{1}{RC}q
   \end{equation}

La solución de la ecuación :eq:`RC3` sujeta a la condición inicial :math:`q=Q_0 ` en :math:`t=0` es

.. math::
   :label: RC4

   \begin{equation}
    q(t)=Q_0 e^{-\frac{t}{\tau _{c}}}
   \end{equation}

donde :math:`\tau _{c}=RC` es la constante de tiempo o tiempo de relajación del circuito. Los voltajes en el capacitor y el resistor son :math:`V_{c}=\frac{q}{C}` y :math:`Ri` respectivamente.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:RC_gui_01` muestra la interfaz gráfica del usuario, esta permite estudiar los procesos de carga y descarga de un capacitor a través de un resistor. La interfaz permite seleccionar los valores de la resistencia y capacitancia mediante las barras deslizables rotuladas **Resistance** y **Capacitance** entre los rangos comprendidos entre :math:`1\,\Omega` - :math:`5\,\Omega` y :math:`1\,\text{F}` - :math:`5\,\text{F}` respectivamente. La interfaz muestra en una misma gráfica los valores de los volatajes en el resistor (curva roja) y capacitor (curva azul) en función del tiempo. Al presionar los botones **Battery in the circuit** y **Battery removed** en cualquier momento el capacitor se carga y descarga sin importar la carga del capacitor. Al presionar el botón **Reset**, el proceso de carga se reinicia. El movimiento de los electrones de los conductores del circuito se observa al presionar el botón **Actual charge flow** y el de la corriente al presionar el botón **Conventional current**.

.. figure:: /images/Electromagnetismo/RC_Circuit/gui_01.png
   :scale: 65
   :align: center
   :name: fig:RC_gui_01

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

**Carga del capacitor**


   #. Fije los valores de :math:`R` y :math:`C` de modo que :math:`R=1\,\Omega` y :math:`C=2\,\text{F}`. A partir de las dos curvas de voltaje en función del tiempo verifique que el tiempo que transcurre para que el voltaje en el capacitor alcance al 63\% del voltaje máximo y el voltaje en el resistor se reduzca el 37\% de su valor inicial es :math:`\tau=RC`.  Obsérvese que :math:`V_c\propto q` y :math:`V_R\propto i`.
   #. Repita el procedimiento anterior para otros valores de :math:`R` y :math:`C` que usted fije de manera arbitraria. ¿Qué se puede concluir?
   #. Fije los valores de :math:`R` y :math:`C` con valores que usted desee. A partir de las dos curvas de voltaje en función del tiempo verifique que los instantes de tiempo para los cuales los voltajes en el capacitor y el resistor son iguales, ocurre para el instante de tiempo :math:`t=\tau \ln(2)=RC\ln(2)`.
   #. En el proceso de carga del capacitor, ¿por qué razón se considera que para un tiempo igual a :math:`5RC` el capacitor ya se encuentra completamente cargado?


**Descarga del capacitor**

   #. Fije los valores de :math:`R` y :math:`C` de modo que :math:`R=1\,\Omega` y :math:`C=1\,\text{F}`. Espere a que el capacitor se cargue al 100\%. Descárguelo y a partir de las dos curvas de voltaje en función del tiempo verifique que el tiempo que transcurre para que los voltajes en el capacitor y resistor se reduzcan al 37\% de valores iniciales es :math:`\tau=RC`.
   #. Repita el procedimiento anterior para otros valores de :math:`R` y :math:`C` que usted fije de manera arbitraria. ¿Qué se puede concluir?
   #. ¿Por qué razón, los signos de los voltajes en el capacitor y resistor son siempre opuestos?
   #. De las expresiones para carga y descarga del capacitor, demuestre que la rapidez con la cual el capacitor se carga es la misma rapidez con la cual se descarga. Verifique la anterior proposición con el simulador.


**Carga-Descarga del capacitor**

   #. Fije los valores de :math:`R` y :math:`C` de modo que :math:`R=1\,\Omega` y :math:`C=1\,\text{F}`. Aplique una señal de voltaje periódica cuadrada tal como muestra la :numref:`fig:RC_exerc_01b`, para ello utilice los botones **Battery in the circuit**, **Step:** :math:`>>` **Battery removed** alternadamente;  demuestre que las curvas de voltaje en el capacitor y resistor son como las mostradas en la :numref:`fig:RC_exerc_01`.

      .. figure:: /images/Electromagnetismo/RC_Circuit/exercise_01b.png
         :scale: 65
         :align: center
         :name: fig:RC_exerc_01b

         Señal periódica aplicada al capacitor inicialmente descargado

      .. figure:: /images/Electromagnetismo/RC_Circuit/exercise_01.png
         :scale: 65
         :align: center
         :name: fig:RC_exerc_01

         Carga-descarga del capacitor


   #. En un circuito RC, las señales de voltaje en el capacitor y resistor son como las mostradas en la :numref:`fig:RC_exerc_02`, si el capacitor se encontraba inicialmente descargado, dibuje la señal aproximada que fue aplicada al sistema RC en el diagrama de la :numref:`fig:RC_exerc_01a`.

      .. figure:: /images/Electromagnetismo/RC_Circuit/exercise_02.png
         :scale: 65
         :align: center
         :name: fig:RC_exerc_02

         Voltajes en :math:`R` y :math:`C` en función del tiempo.

      .. figure:: /images/Electromagnetismo/RC_Circuit/exercise_01a.png
         :scale: 65
         :align: center
         :name: fig:RC_exerc_01a

         Señal aplicada al circuito RC cuyas curvas de voltaje en :math:`C` y :math:`R` se muestran en la :numref:`fig:RC_exerc_02`.

   #. Realice una gráfica de energía almacenada en el capacitor en función del tiempo para la situación descrita en el inciso 2.
   #. Realice una gráfica de energía disipada en el resistor en función del tiempo para la situación descrita en el inciso 2.

