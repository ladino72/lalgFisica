Equivalente mecánico del calor
================================


**Objetivo**

El propósito de esta práctica es determinar el equivalente mecánico del calor.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://www.thephysicsaviary.com/Physics/Programs/Labs/ElectricalDeterminationOfSpecificHeatLab/ <https://www.thephysicsaviary.com/Physics/Programs/Labs/ElectricalDeterminationOfSpecificHeatLab/>`_.

Los conceptos de calor y temperatura son conceptos que a la ciencia le costó mucho tiempo entender su verdadera naturaleza. Galileo Galilei fue el primero en proponer la teoría del calórico, la cual afirmaba que todo cuerpo estaba formado por dos tipos de sustancias: la primera del material en sí (cobre, aluminio, etc) y la segunda era llamada el calórico y es lo que intercambian los cuerpos cuando se ponen en contacto. Esta teoría vio su fin en 1756 con los trabajos de Joseph Black donde sus experimentos muestran la inexistencia del calórico. No es obvio que la energía que fluye hacia su dedo cuando toca un objeto caliente, sea del mismo tipo que la energía cinética de un ladrillo que cae; es decir, el calor es una forma de energía. El experimento de Joule realizado en 1840 demuestra que el calor no es más que una forma de energía, y que se podía obtener a partir de la energía mecánica. Dicho experimento se conoce como el equivalente mecánico del calor. Antes del experimento de Joule se pensaba que calor y energía eran dos magnitudes diferentes, por lo que las unidades en que se medían ambas eran también distintas. La unidad de calor que se empleaba era la caloría. Con su experimento, Joule se propuso demostrar que se podía elevar la temperatura del agua transfiriéndole energía mecánica. Es decir, que la temperatura de un sistema puede elevarse proporcionándole calor, pero también realizando un trabajo sobre él, ver :numref:`fig:Mec_Equiv_Heat_02` y :numref:`fig:Mec_Equiv_Heat_01`.

En la primera situación, ver :numref:`fig:Mec_Equiv_Heat_02`, la cantidad de calor requerida para producir un cambio de temperatura igual a  :math:`\Delta T=T-T_0` en una sustancia  de masa :math:`m` es :math:`Q=mc\Delta T`, donde :math:`c` es el calor específico de la sustancia y :math:`T_0`, :math:`T` son sus temperaturas inicial y final. De esta expresión se sigue que :math:`c=\frac{Q}{m\Delta T}`. Para el caso del agua :math:`c=\frac{1\,\text{cal}}{(1\,\text{g})(1\,^o \text{C})}=1\frac{\text{cal}}{\text{g}\, ^o \text{C}}`, lo que indica que se requiere 1 caloría (cal) para incrementar la temperatura de 1 gramo de agua en :math:`1\,^o\text{C}`. En la segunda situación, ver :numref:`fig:Mec_Equiv_Heat_01`, se tiene un líquido de masa :math:`m` en un recipiente a cierta temperatura :math:`T_0`.  Al recipiente se le acoplan unas paletas conectadas mediante una cuerda a un cuerpo de masa :math:`M`  que puede caer. Conforme el cuerpo cae a velocidad constante, las paletas giran, por lo que se convierte su energía potencial gravitatoria en energía para hacer girar las paletas. Debido a este giro, el agua aumenta su temperatura a un valor :math:`T` (el giro de las paletas se transforma en calor). Así, la energía :math:`Q` suministrada al líquido cuando el cuerpo ha descendido una distancia :math:`H` es :math:`Q=MgH`. Por conservación de la energía se tiene

.. math::
   :label: Mech_Equiv_Heat:Ec_01

   \begin{equation}
    mc\Delta T=MgH
   \end{equation}

.. figure:: /images/Oscilaciones_Termo/Heat_Mechanical_Equivalent/Mec_Equiv_Heat_02.png
   :scale: 60
   :align: center
   :name: fig:Mec_Equiv_Heat_02

   El agua se calienta mediante un mechero

.. figure:: /images/Oscilaciones_Termo/Heat_Mechanical_Equivalent/Mec_Equiv_Heat_01.png
   :scale: 60
   :align: center
   :name: fig:Mec_Equiv_Heat_01

   El agua se calienta al efectuar trabajo sobre ella mediante las aspas giratorias


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Mec_Equiv_Heat_Gui_01` muestra la interfaz gráfica del usuario que permite determinar el equivalente mecánico del calor. La aplicación muestra el recipiente al que se acoplan unas paletas conectadas mediante una cuerda a un cuerpo de masa :math:`M` que cae con velocidad constante. La masa del cuerpo se puede cambiar al hacer clic sobre la masa colgante, se pueden seleccionar hasta seis valores diferentes. De igual manera, la altura inicial desde la cual la masa comienza a descender se selecciona al hacer clic sobre la polea, se pueden seleccionar hasta seis valores diferentes y sus valores se leen con la ayuda de la regla graduada. La interfaz presenta un termómetro el cual registra la temperatura del agua cuyo volumen en mililitros se puede leer del recipiente. Al presionar el botón **Reset** la aplicación coloca la masa en el punto inicial de partida. Al presionar el botón **Start** la masa comienza a descender y la temperatura del agua comienza a aumentar.

.. figure:: /images/Oscilaciones_Termo/Heat_Mechanical_Equivalent/Gui_Mec_Equiv_Heat_01.png
   :scale: 80
   :align: center
   :name: fig:Mec_Equiv_Heat_Gui_01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

   #. Registre los valores de la cantidad de agua y su temperatura inicial.
   #. Fije el valor de una masa cualquiera y déjela caer desde alturas diferentes. Registre la correspondiente temperatura una vez que esta llega al piso en la :numref:`tab:Mech_Equiv_Heat_01`.
   #. Construya una gráfica de valor absoluto de energía potencial gravitacional :math:`Q` perdida por la masa en función del cambio de temperatura :math:`\Delta T` del agua. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`Q` y :math:`\Delta T`.
   #. Repita los pasos de los incisos 2 y 3 pero con un valor de masa diferente. Registre sus mediciones en la :numref:`tab:Mech_Equiv_Heat_02`.
   #. De los resultados obtenidos en los incisos anteriores compruebe que :math:`1\,\text{cal}\approx 4.186\,\text{J}`.

      .. csv-table:: masa :math:`m_1`.
         :header: "Altura, :math:`H` (m)", "Temperatura, :math:`T\\,^o \\text{C}`"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Mech_Equiv_Heat_01
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.

      .. csv-table:: masa :math:`m_2`.
         :header: "Altura, :math:`H` (m)", "Temperatura, :math:`T\\,^o \\text{C}`"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Mech_Equiv_Heat_02
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.

