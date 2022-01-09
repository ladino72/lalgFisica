Gas ideal
============

**Objetivo**

El propósito de esta práctica es estudiar algunas características de la ecuación de estado que gobierna el comportamiento de los gases ideales.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/gas-properties/latest/gas-properties_en.html <https://phet.colorado.edu/sims/html/gas-properties/latest/gas-properties_en.html>`_.

**Resumen teórico**

Recibe el nombre de gas ideal un conjunto de partículas puntuales (sin volumen) que se mueven al azar y donde no existen fuerzas de interacción molecular. La mayoría de los gases a baja presión obedecen esta condición [#f1]_. Para los gases ideales son válidas las siguientes leyes:

   #. *Ley de Boyle Mariotte:* a temperatura y masa constantes el producto de la presión por el volumen del gas es una cantidad también constante:

      .. math::
         :label: Ec:Ideal-Gas_1

          \begin{equation}
           pV=const.
          \end{equation}

   #. *Ley de Gay-Lussac:* a presión constante el volumen de una masa dada de gas es directamente proporcional a su temperatura absoluta

      .. math::
         :label: Ec:Ideal-Gas_2

         \begin{equation}
          V=\alpha V_{0}T=V_{0}\frac{T}{T_{0}}
         \end{equation}

      donde :math:`V_{0}` es el volumen del gas a la temperatura :math:`T_{0}=273.15` :math:`K` y :math:`\alpha =\frac{1}{T_{0}}` es el coeficiente de dilatación cúbica.

   #. *Ley de Charles:* a volumen constante la presión de una masa dada de gas es directamente proporcional a su temperatura absoluta:

      .. math::
         :label: Ec:Ideal-Gas_3

         \begin{equation}
          p=p_{0}\frac{T}{T_{0}}
         \end{equation}

      donde :math:`p_{0}` es la presión del gas a temperatura :math:`T_{0}=273.15` :math:`K`

Las anteriores expresiones pueden ser combinadas en una sola expresión y llegar a la denominada ecuación de estado para un gas ideal

.. math::
   :label: Ec:Ideal-Gas_4

   \begin{equation}
    pV=nRT=NkT
   \end{equation}

donde :math:`p`, :math:`V` y :math:`T` representan la presión, volumen y temperatura absoluta del gas;
:math:`n` es el numero de moles de gas, :math:`R=8.31` :math:`J/mol\cdot K` es la constante
universal de los gases, :math:`N` es el numero total de moléculas del gas, :math:`k=1.38\times 10^{-23}` :math:`\text{J/K}` es la constante de Boltzmann. Además, :math:`n=\frac{M}{\mu }` :math:`=\frac{N}{N_{A}},` donde :math:`M` es la
masa del gas, :math:`\mu ` es la masa molecular y  :math:`N_{A}=6.02\times 10^{23}` es el numero de Avogadro. De estas expresiones se sigue que , :math:`k=\frac{R}{N_{A}}`.
Por otra parte, de la teoría cinética de los  gases ideales se cumple:


   * La energía cinética media de una molécula de masa :math:`m` es  :math:`\overline{E}_k=\frac{1}{2}mv_{rms}^{2}=\frac{3}{2}kT`, donde el término :math:`v_{rms}` se denomina la velocidad cuadrática media.
   * La velocidad media de una molécula es :math:`<v>=\sqrt{\frac{8kT}{\pi m}}`
   * El número de moléculas que chocan contra las paredes del recipiente por unidad de área y tiempo está dado por :math:`\nu=\frac{1}{4}\frac{N}{V}<v>`.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Ideal-Gas_01` muestra la interfaz gráfica del usuario, que permite estudiar algunas características de la ecuación de estado para un gas ideal. La interfaz permite seleccionar el número de partículas mediante la bomba al subir y bajar el mango de la misma, el número exacto de partículas se fija con los botones que se encuentra a la derecha de la interfaz cuyo rótulo dice **Particles**. Se puede escoger entre partículas pesadas (color azul) y ligeras (color rojo). También se puede determinar el número de choques (\texttt{Wall collisions}) contra las paredes del recipiente durante tres periodos de tiempo (5, 10 y 20 ps), al seleccionar la opción **Collision counter**.
Para realizar un experimento a temperatura constante: se debe primero seleccionar cierto número de partículas,  la opción **Nothing** del panel rotulado **Hold constant** debe estar seleccionada; enseguida, caliente o enfríe el gas con la fuente de calor ubicada en la parte inferior de la interfaz rotulada (**Heat**-**Cool**) al mover el botón de la barra de desplazamiento. Una vez establecida la temperatura del gas seleccione la opción **Temperature** para mantenerla constante. En este estado se puede cambiar el número de partículas del gas o variar el volumen del gas al desplazar la agarradera (mango) ubicado en la parte izquierda del recipiente. La lectura de la presión del gas se puede realizar directamente del manómetro. Al seleccionar la opción **Width** :math:`<-->` aparece una cinta métrica que permite medir el ancho del recipiente.\newline
Para realizar un experimento a volumen constante: se debe primero seleccionar cierto número de partículas, varíe el ancho del recipiente (el cual es proporcional al volumen) con la opción **Width** :math:`<-->` y fije el volumen al seleccionar la opción **Volumen**. En este estado se puede cambiar el número de partículas del gas o variar la temperatura del gas. \newline
Para realizar un experimento a presión constante: se debe primero seleccionar cierto número de partículas; enseguida, caliente o enfríe el gas hasta alcanzar el valor de presión deseada. Para fijar el valor de la presión se tienen dos opiones: **Pressure** :math:`\updownarrow` V o **Pressure** :math:`\updownarrow` :math:`T`. Con la primera, la temperatura y volumen del gas cambian al suministrar energía térmica con la fuente de calor. Al seleccionar la opción **Width** :math:`<-->` aparece una cinta métrica que permite medir el ancho del recipiente, el cual es proporcional al volumen del mismo. Con la segunda opción, al desplazar la agarradera (mango) hacia la derecha o izquierda el gas libera o absorbe calor y por tanto este se enfría o calienta. La temperatura se mide directamente del termómetro. \newline

.. figure:: /images/Oscilaciones_Termo/Ideal_Gas/IG_gui_01.png
   :scale: 85
   :align: center
   :name: fig:Ideal-Gas_01

   Interfaz gráfica del usuario


**Mediciones y procedimientos**

**Ley de Boyle-Mariotte**

   #. Fije el número de partículas y su temperatura: :math:`N=500` (partículas pesadas) y :math:`T=400\,\text{K}`, ver :numref:`fig:Ideal-Gas_02`.  Si :math:`V` es el volumen ocupado por el gas, :math:`V=A\ell`, donde :math:`A` es el área de la superficie lateral del recipiente y :math:`\ell` es su ancho. Así, :math:`V\propto \ell`. Realice mediciones de :math:`p` y :math:`\ell` y registre sus mediciones en la :numref:`tab:Ideal-Gas_01`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`p` y :math:`\ell`.

      .. figure:: /images/Oscilaciones_Termo/Ideal_Gas/IG_gui_02.png
         :scale: 50
         :align: center
         :name: fig:Ideal-Gas_02

         Configuración para determinar la relación entre :math:`p` y :math:`V` a temperatura constante


   #. Repita el mismo procedimiento del inciso 1 pero esta vez con partículas ligeras y registre sus mediciones en la :numref:`tab:Ideal-Gas_02`. ¿Cómo afecta la masa de las partículas la relación entre :math:`p` y :math:`\ell`?

      .. csv-table:: Valores de :math:`\ell` (nm) y presión (atm) a temperatura constante: Partículas pesadas
         :header: "Ancho, :math:`\\ell` (nm)", "Presión, :math:`P` (atm)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_01
         :align: center

         5.0,155.7
         6.0,
         7.0,
         8.0,
         9.0,
         10.0,
         11.0,
         12.0,
         13.0,
         14.0,
         15.0,

      .. csv-table:: Valores de :math:`\ell` (nm) y presión (atm) a temperatura constante: Partículas ligeras
         :header: "Ancho, :math:`\\ell` (nm)", "Presión, :math:`P` (atm)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_02
         :align: center

         5.0,155.7
         6.0,
         7.0,
         8.0,
         9.0,
         10.0,
         11.0,
         12.0,
         13.0,
         14.0,
         15.0,

**Ley de Gay-Lussac**

   #. Fije el número de partículas y su volumen: :math:`N=500` (partículas pesadas) y :math:`\ell=10\,\text{nm}`, ver :numref:`fig:Ideal-Gas_03`. Realice mediciones de presión :math:`p` contra temperatura :math:`T` del gas y registre sus mediciones en la :numref:`tab:Ideal-Gas_03`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`p` y :math:`T`.

      .. figure:: /images/Oscilaciones_Termo/Ideal_Gas/IG_gui_03.png
         :scale: 50
         :align: center
         :name: fig:Ideal-Gas_03

         Configuración para determinar la relación entre :math:`p` y :math:`T` a volumen constante

   #. Repita el mismo procedimiento del inciso 1 pero esta vez con partículas ligeras y registre sus mediciones en la :numref:`tab:Ideal-Gas_04`. ¿Cómo afecta la masa de las partículas la relación entre :math:`p` y :math:`T`?

      .. csv-table:: Valores de presión y temperatura a volumen constante: Partículas pesadas
         :header: "Temperatura, :math:`T` (K)", "Presión, :math:`P` (atm)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_03
         :align: center

         100,19.5
         200,
         300,
         400,
         500,
         600,
         700,
         800,
         900,

      .. csv-table:: alores de presión y temperatura a volumen constante: Partículas ligeras
         :header: "Temperatura, :math:`T` (K)", "Presión, :math:`P` (atm)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_04
         :align: center

         100,19.5
         200,
         300,
         400,
         500,
         600,
         700,
         800,
         900,

**Ley de Charles**

   #. Fije el número de partículas y su volumen: :math:`N=500` (partículas pesadas) y :math:`p=120\,\text{atm}`, ver :numref:`fig:Ideal-Gas_04`. Realice mediciones de presión :math:`V` contra temperatura :math:`T` del gas y registre sus mediciones en la :numref:`tab:Ideal-Gas_05`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`V` y :math:`T`.

      .. figure:: /images/Oscilaciones_Termo/Ideal_Gas/IG_gui_04.png
         :scale: 50
         :align: center
         :name: fig:Ideal-Gas_04

         Configuración para determinar la relación entre :math:`V` y :math:`T` a presión constante

   #. Repita el mismo procedimiento del inciso 1 pero esta vez con partículas ligeras y registre sus mediciones en la :numref:`tab:Ideal-Gas_06`. ¿Cómo afecta la masa de las partículas la relación entre :math:`V` y :math:`T`?

      .. csv-table:: Valores de volumen (u.a = unidades arbitrarias) y temperatura a presión constante: Partículas pesadas
         :header: "Volumen V(u.a)", "Temperatura , :math:`T` (K)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_05
         :align: center

         5,307
         6,
         7,
         8,
         9,
         10,
         11,
         12,
         13,
         14,
         15,

      .. csv-table:: Valores de volumen (u.a = unidades arbitrarias) y temperatura a presión constante: Partículas ligeras
         :header: "Volumen V(u.a)", "Temperatura , :math:`T` (K)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ideal-Gas_06
         :align: center

         5,	307
         6,
         7,
         8,
         9,
         10,
         11,
         12,
         13,
         14,
         15,

**Relación entre** :math:`p`, :math:`N` y :math:`\nu`

   #. Para estudiar la relación de la presión :math:`p` del gas con el número de partículas :math:`N` y número de choques por unidad de área y tiempo contra las paredes del recipiente, fije su volumen y temperatura, ver :numref:`fig:Ideal-Gas_05`. Varíe el número :math:`N` de partículas en el recipiente y para cada valor tome por lo menos 10 mediciones del número de choques para obtener un promedio durante un periodo de muestreo de 20 ps y registre sus valores en la :numref:`tab:Ideal-Gas_choques` con la correspondiente presión. Obsérvese que :math:`\nu=\frac{\#\text{choques}}{A\Delta t}`, donde :math:`A` es el área de las paredes del recipiente (desconocido) y :math:`\Delta t=20\,\text{ps}`. Así, :math:`\nu\propto \#\text{choques}`. Grafique :math:`p` en función de :math:`N` y :math:`p` en función de :math:`\#\text{choques}`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`p` y :math:`N` y entre :math:`p` y :math:`\nu`. Discuta sus resultados y compárelos con los de la teoría del gas ideal.

      .. figure:: /images/Oscilaciones_Termo/Ideal_Gas/IG_gui_05.png
         :scale: 40
         :align: center
         :name: fig:Ideal-Gas_05

         Gas con volumen y temperatura constante

      .. csv-table:: Datos para determinar la relación ente :math:`p`, :math:`N` y :math:`\nu`
         :header: "#Partículas" , "I1" , "I2" , "I3" , "I4" , "I5" ,"I6" ,"I7" , "I8" ,"I9" , "I10" , "Promedio", "Presión(atm)"
         :widths: 1,1,1,1,1,1,1,1,1,1,1,1,1
         :width: 16 cm
         :name: tab:Ideal-Gas_choques
         :align: center

         100 ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         200,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         300,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         400,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         500,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         600,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         700,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         800,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         900,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,
         1000,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,  ,


      Teniendo en cuenta los resultados anteriores, ¿Cuál es la relación entre :math:`p`, :math:`V`, :math:`T` y :math:`N`?

.. [#f1] Cualquier gas se comporta como un gas ideal a alta temperatura y baja presión. El oxígeno atmosférico está a 25 :math:`\,^{o}\text{C}`, que es mayor que su temperatura crítica, la cual es -150 :math:`\,^{o}\text{C}` y su presión es de alrededor 159 mm de Hg (21.1 kPa). Por lo tanto, se dice que los gases atmosféricos se comportan como los de un gas ideal.