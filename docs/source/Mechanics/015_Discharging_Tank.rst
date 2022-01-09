Tiempo de vaciado de un recipiente
====================================
**Objetivo**

Esta actividad tiene como finalidad estudiar de manera cuantitativa la forma en que los factores geométricos de un
recipiente que contiene agua determinan el tiempo de vaciado  del mismo.

**Recursos**


   #. Computador o tablet o cualquier otro dispositivo con conexión a internet.
   #. Simulación disponible en `https://www.geogebra.org/m/zyv5evad <https://www.geogebra.org/m/zyv5evad>`_.


**Situación**


Cuando se tiene un recipiente cilíndrico con un líquido, :numref:`Figure 7`, al cual previamente le hemos practicado un orificio en el fondo y permitimos que el líquido salga por este orificio, el nivel del líquido en el recipiente desciende a medida que pasa el tiempo y eventualmente se hace cero. Cuanto tiempo gasta el recipiente en desocuparse completamente depende de ciertos factores como son el radio :math:`R` del recipiente, la altura :math:`H_0` inicial del nivel del líquido en el recipiente, el radio :math:`r` del orifico y la naturaleza del líquido. Esta actividad tiene como finalidad encontrar la relación  matemática que existe entre el tiempo :math:`T` de vaciado de un recipiente cilíndrico que contiene agua con :math:`r`, :math:`H_0` y :math:`R`. Asumiremos que la relación entre :math:`T`, :math:`r`, :math:`R ` y :math:`H_0` es de la forma :math:`T=AR^{m}r^{n}H_0^{p}`, donde :math:`A`, :math:`m`, :math:`n` y :math:`p` son números reales. Así, el objetivo es determinar los valores de :math:`m`, :math:`n`, :math:`p` y :math:`A`.

.. figure:: /images/Mecanica/Discharging_Tank/Discharging_tank_01.jpg
   :alt: Discharging
   :scale: 40%
   :align: center
   :name: Figure 7

   Recipiente cilíndrico con orificio en el fondo


**Descripción de la interfaz de la aplicación**


La :numref:`Figure 8` muestra la interfaz gráfica del usuario que permite estudiar la dependencia
del tiempo :math:`T` de vaciado de un recipiente cilíndrico que contiene agua, de la altura del nivel inicial
:math:`H_0` de agua, del radio :math:`R` del recipiente y el radio :math:`r`  del orificio por donde se evacua
el agua. La interfaz permite establecer los valores de estas cantidades mediante las barras de desplazamiento rotuladas
*Initial height*, *Tank radius* y *Hole* radius respectivamente. Una vez seleccionados los valores de estas cantidades, el usuario puede llenar el tanque al presionar
el botón *Fill* y medir el tiempo de descarga del recipiente al presionar el botón *Empty*.
A medida que el tanque se descarga aparece la señal *Discharging tank* y una vez completado el proceso aparece la señal *Empty tank*. Ahora se está listo
para hacer cambios en los parámetros y tomar medidas de nuevo.

.. figure:: /images/Mecanica/Discharging_Tank/Gui_Discharging_tank.png
   :alt: Discharging
   :scale: 45%
   :align: center
   :name: Figure 8

   Interfaz del usuario.


**Mediciones y procedimientos**


**Relación entre** :math:`T` y :math:`H_0`

   #. Para determinar la relación entre :math:`T` y :math:`H_0` mantenga :math:`r` y :math:`R` fijos. Se sugiere por ejemplo tomar :math:`r=0.2\,\text{cm}` y :math:`R=3,0\,\text{cm}`. Realice la toma de datos y para ello complete la Tabla :numref:`Discharg_T_v_H`
       .. csv-table:: Relación entre :math:`T` y :math:`H_0`
          :header: "Tiempo :math:`T` (s)", "Altura :math:`H_0` (cm)"
          :widths: 1,1
          :width: 10 cm
          :name: Discharg_T_v_H
          :align: center
          :stub-columns: 0
          :header-rows: 0

          1.0,
          2.0,
          3.0,
          4.0,
          5.0,
          6.0,
          7.0,
          8.0,
          9.0,
          10.0,

   #. Realice una gráfica de :math:`T` en función de :math:`H_0`.
   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`T` y :math:`H_0`. Determine el valor de :math:`p`.

**Relación entre** :math:`T` y :math:`r`

   #. Para determinar la relación entre :math:`T` y :math:`r` mantenga :math:`H_0` y :math:`R` fijos. Se sugiere por ejemplo tomar :math:`H_0=6.0\,\text{cm}` y :math:`R=3.0\,\text{cm}` . Realice la toma de datos y para ello complete la Tabla :numref:`Discharg_T_v_r`
       .. csv-table:: Relación entre :math:`T` y :math:`r`
          :header: "Tiempo :math:`T` (s)", "Altura :math:`r` (cm)"
          :widths: 1,1
          :width: 10 cm
          :name: Discharg_T_v_r
          :align: center

          0.1,
          0.2,
          0.3,
          0.4,
          0.5,
          0.6,
          0.7,
          0.8,

   #. Realice una gráfica de :math:`T` en función de :math:`r`.
   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`T` y :math:`r`. Determine el valor de :math:`n`.

**Relación entre** :math:`T` y :math:`R`


   #. Para determinar la relación entre :math:`T` y :math:`R` mantenga :math:`r` y :math:`H_0` fijos. Se sugiere por ejemplo tomar :math:`r=0.2\,\text{cm}` y :math:`H=5.0\,\text{cm}`. Realice la toma de datos y para ello complete la Tabla :numref:`Discharg_TvR`
       .. csv-table:: Relación entre :math:`T` y :math:`R`
          :header: "Tiempo :math:`T` (s)", "Radio :math:`R` (cm)"
          :widths: 1,1
          :width: 10 cm
          :name: Discharg_TvR
          :align: center

          1.0,
          1.5,
          2.0,
          2.5,
          3.0,
          3.5,
          4.0,
          4.5,
          5.0,

   #. Realice una gráfica de :math:`T` en función de :math:`R`.
   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`T` y :math:`R`. Determine el valor de :math:`m`.

**Análisis y preguntas**


   #. Determine el valor de la constante :math:`A` propuesto en el modelo :math:`T=AR^{m}r^{n}H_0^{p}`, y explique detalladamente el procedimiento que conduce a la determinación de su valor.
   #. Use la relación matemática encontrada para calcular el tiempo de vaciado de un recipiente con :math:`R=5.0\,\text{cm}`, :math:`r=0.5\,\text{cm}` y :math:`H_0=10\,\text{cm}`. Compare el valor obtenido con el tiempo 14.29 s, el cual es el valor que predice la simulación.
   #. Establezca las posibles limitaciones del fenómeno estudiado en la simulación.
   #. ¿Qué sucede con el tiempo de vaciado del recipiente si el radio del orificio se duplica?
   #. ¿Qué sucede con el tiempo de vaciado del recipiente si el radio del recipiente se triplica?
   #. ¿Qué sucede con el tiempo de vaciado del recipiente si la altura inicial del agua en el recipiente se reduce a la mitad?


