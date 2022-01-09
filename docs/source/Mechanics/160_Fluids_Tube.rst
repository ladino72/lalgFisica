Fluidos en un tubo en forma de U
====================================

**Objetivo**

El propósito de esta práctica es determinar la densidad de diferentes líquidos usando un tubo en forma de :math:`\Cup`.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `{http://www.thephysicsaviary.com/Physics/Programs/Labs/YouTubeLab/index.html <http://www.thephysicsaviary.com/Physics/Programs/Labs/YouTubeLab/index.html>`_.

**Resumen teórico**

En la mecánica de los fluidos, la presión hidrostática es aquella que un fluido en reposo genera por su propio peso. La presión hidrostática no depende de la masa, del peso o del volumen total del fluido, sino de la densidad del fluido :math:`\rho`, la aceleración de la gravedad :math:`g` y la profundidad del fluido :math:`h`. La presión hidrostática, por lo tanto, se calcula con la siguiente fórmula:

.. math::
   :label: FTU_01

   \begin{equation}
     p=\rho g h
   \end{equation}

La :numref:`fig:FTU_gui_03` muestra un tubo en forma de :math:`\Cup`, abierto por ambos extremos, por cada extremo del tubo (rama) se han vertido  líquidos inmiscibles de densidades :math:`\rho_1` y :math:`\rho_2`  respectivamente. El pistón móvil en el fondo del tubo separa los dos líquidos y se encuentra en equilibrio (suma de fuerzas igual a cero, en este caso la diferencia de presión hidrostática actuando por cada cara del pistón es cero), luego se cumple que

.. figure:: /images/Mecanica/Fluids_Tube/Tube_U_gui_03.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:FTU_gui_03

   Tubo en :math:`\Cup` con dos líquidos de diferentes densidades.

.. math::
   :label: FTU_02

   \begin{equation}
    \rho_1 g h_1=\rho_2 g h_2
   \end{equation}

**Descripción de la interfaz de la aplicación**

La figura :numref:`fig:FTU_gui_01` muestra la interfaz gráfica del usuario que permite determinar la densidad de un líquido mediante el uso de un tubo en forma de :math:`\Cup` abierto en ambos extremos.
El radio de cada una de la ramas del tubo se fija al hacer clic sobre las flechas verticales rotuladas **Tube 1 radius** y **Tube 2 radius**; el rango de los radios está comprendido entre 5 mm y 30 mm. El tipo de fluido en cada rama del tubo se selecciona al hacer clic sobre los nombres de las sustancias que aparecen debajo de los rótulos **Fluid 1** o **Fluid 2**; entre las sustancias a escoger se tienen: Maple Syrup, Ethanol, Crude oil, Gasoline, Brine, Glycerin, Fresh water. El nivel de cada líquido en el tubo se fija con el par de flechas verticales ubicadas en la parte inferior y a lado y lado de la interfaz. El nivel de la altura de los líquidos en cada tubo se mide con la ayuda de la grilla graduada en milímetros (mm). Al hacer clic sobre el pasador (pin) de color negro ubicado por encima del pistón que separa los líquidos, libera el pistón y permite su movimiento en sentido horizontal. Si se quiere cambiar algún parámetro asegúrese primero de hacer clic sobre el pasador.

.. figure:: /images/Mecanica/Fluids_Tube/Tube_U_gui_01.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:FTU_gui_01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

Asumiremos que la densidad del agua es :math:`1.0\,\text{g/cm}^{3}`.

**Nivel constante, radios cambian, ambas ramas del tubo con agua**


   #. Fije los radios de las ramas de modo que tengan el mismo radio (25 mm) y los niveles de agua en ellas sean de 300 mm.
   #. Tire del pasador que sujeta el pistón
   #. ¿Cómo se movió el pistón cuando tiró del pasador? ¿Por qué pasó esto?
   #. Cambie el radio de la rama del tubo 1 a 15 mm. Tire del pasador y observe cómo se mueve el pistón.
   #. Pruebe con algunos radios más para las ramas 1 y 2. Haga que sean muy diferentes entre sí. Discuta sus observaciones.
   #. ¿Influye el radio de las ramas en el movimiento del pistón?

**Radios cambian, ambas ramas del tubo con agua**

   #. Fije los radios de las ramas de modo que tengan el mismo radio (25 mm) y contengan agua.
   #. Eleve el nivel del agua en la rama 1 a 400 mm y mantenga la rama 2 a 300 mm.
   #. Tire del pasador que sostiene el pistón.
   #. ¿Cómo se movió el pistón cuando se tiró del pasador? ¿Cuál fue el nivel final de agua en cada rama?
   #. Cambie el radio de la rama 1 a 15 mm. Mantenga el nivel del agua en la rama 1 a 400 mm y mantenga la rama 2 a 300 mm.
   #. Tire del pasador que sostiene el pistón.
   #. ¿De qué manera los niveles finales de agua son diferentes difieren de los del inciso 4?
   #. Cambie el radio de la rama del 1 a 5 mm. Mantenga el nivel del agua de la rama 1 a 400 mm y mantenga la rama 2 a 300 mm.
   #. Tire del pasador.
   #. Describa lo que sucede con el nivel del agua en cada rama del tubo. ¿Qué se cumple cuando el pistón deja de moverse?
   #. ¿Qué puede concluir sobre los niveles de líquido cuando el pistón deja de moverse?




**Diferentes líquidos en las ramas**

   #. Fije los radios de las ramas de modo que tengan el mismo radio, 25 mm.
   #. Asegúrese de que la rama de la izquierda contenga Maple Syrup, la rama de la derecha sea agua y que sus niveles iniciales sean 200 mm y 300 mm respectivamente.
   #. Remueva el pasador y registre las alturas finales :math:`h_1` y :math:`h_2`. Registre sus mediciones en la :numref:`tab:FTU_h2_vs_h1`.

      .. csv-table:: Datos simulados para determinar la ralación entre :math:`h_2` y :math:`h_1`
         :header: ":math:`h_1` (mm)", ":math:`h_2` (mm)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:FTU_h2_vs_h1
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.

   #. A partir de la tabla de datos del inciso 3 construya una gráfica de :math:`h_2` en función de :math:`h_1`
   #. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`h_2` y :math:`h_1` y determine la densidad del Maple Syrup.
   #. Repita los pasos de los incisos anteriores y encuentre la densidad del Ethanol y Crude oil.




**Información:** si el tubo en :math:`\Cup` se llenase con un único líquido, la consecuencia es que el nivel superior en ambas ramas -por distantes que estuvieran- sería el mismo. Los albañiles suelen valerse de este fenómeno para ubicar posiciones de igual altura, pero distantes. En lugar de un tubo de vidrio usan una manguera larga y transparente.\newline

**Pregunta:** cuando lo que el albañil debe dejar horizontal es abarcable por el largo de una regla, usa una -llamada nivel- que también tiene un tubo en :math:`\Cup`, pero invertido. El tubo está cerrado en ambas ramas, por supuesto, y -además de agua- tiene en su interior una burbuja de aire. ¿Cómo funciona?
