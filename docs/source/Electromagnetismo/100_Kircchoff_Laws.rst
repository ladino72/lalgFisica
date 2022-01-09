+Leyes de Kircchoff
===================

**Objetivo**

El propósito de esta práctica es estudiar la ley de Ohm y las leyes de Kirchhoff.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/circuit-construction-kit-dc/latest/circuit-construction-kit-dc_es.html <https://phet.colorado.edu/sims/html/circuit-construction-kit-dc/latest/circuit-construction-kit-dc_es.html>`_.

**Resumen teórico**

La ley de Ohm establece que el voltaje :math:`V` (medido en Voltios) entre los extremos de ciertos tipos de materiales conductores es directamente proporcional a la corriente eléctrica :math:`I` (medida en amperios) que fluye a través del material.

.. math::

   \begin{equation}
     V = RI
   \end{equation}

siendo :math:`R` el valor de la resistencia eléctrica del material, la cual depende de su naturaleza y de factores geométricos.
Por otro lado, las Leyes de Kirchhoff constituyen la base para el análisis de los circuitos eléctricos. Estas pueden aplicarse a cualquier circuito, desde el circuito más sencillo, hasta la red más compleja.

   #. Primera ley de Kirchhoff: la suma algebraica de las corrientes que entran (o salen de) a una unión de dos o más elementos es igual a cero. Esto significa que la suma de las corrientes que entran a la unión (nodo) es igual a la suma de las corrientes que salen de ella. Así, para el fragmento de circuito de la :numref:`fig:kirchhoff_1` se cumple: :math:`I_3=I_2+I_1`

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/kirchhoff_01.png
         :scale: 90
         :align: center
         :name: fig:kirchhoff_1

         Suma de corrientes que entran al nodo (punto rojo) es igual a la suma de las corrientes que salen del mismo nodo.


   #. Segunda ley de Kirchhoff: la suma algebraica de las diferencias de potencial alrededor de cualquier trayectoria cerrada (lazo) en un circuito es cero. Esto significa que, en un circuito cerrado, la suma de las elevaciones de tensión es igual a la suma de las caídas de tensión. Así, para los lazos 1, 2 y 3 del circuito de la :numref:`fig:kirchhoff_2` se cumple: :math:`\varepsilon-R_1I_1=0`, :math:`\varepsilon-R_2I_2=0` y :math:`+R_1I_1-R_2I_2=0` respectivamente.

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/kirchhoff_02.png
         :scale: 80
         :align: center
         :name: fig:kirchhoff_2

         Suma algebraica de las caidas de voltaje a lo largo de los lazos 1, 2 y 3 es cero.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Kirc_gui_01` muestra la interfaz gráfica del usuario, esta permite armar un sinnúmero de circuitos DC consistentes de baterías, fuentes de voltaje, resistencias, bombillas e interruptores. Estos elementos se seleccionan del panel ubicado en la parte izquierda de la interfaz. Las corrientes eléctricas y diferencias de potencial se pueden medir con los amperímetros y voltímetros en el panel de la derecha. Se pueden usar tantos elementos como se requieran. A cada resistor y cable se le puede asignar una resistencia, incluyendo al filamento de las bombillas y la resistencia interna de las fuentes de voltaje DC mediante la barra de desplazamiento que aparece cuando se presiona con el puntero del ratón sobre el elemento.  Para medir corriente se tienen dos tipos de amperímetros (ideales: resistencia interna nula), uno de ellos requiere interrumpir el circuito y conectarlo en serie, mientras que el otro basta con colocar el cursor en forma de mira sobre el conductor por el que circula corriente para medir su valor.

.. figure:: /images/Electromagnetismo/Kircchoff_Laws/Kirc_gui_01.png
         :scale: 70
         :align: center
         :name: fig:Kirc_gui_01

         Interfaz gráfica del usuario

**Mediciones y procedimientos**

**Ley de Ohm**


   #. Monte y simule el circuito de la :numref:`fig:Kirc_gui_03`. La :numref:`fig:Kirc_gui_02` muestra una manera de realizar las conexiones (No es necesario, pero se ha intercalado un interruptor, :math:`S`). Nótese que: el amperímetro se encuentra en serie con el resistor de :math:`120\,\Omega`, el voltímetro está conectado en paralelo con el resistor. Varíe el voltaje :math:`V` como indica la :numref:`tab:Ohm_law_01`, mida el valor de la corriente y regístrelo  en la tabla. Realice una gráfica de :math:`V` en función de :math:`I` y verifique que la relación entre estas variables es lineal. ¿Qué significa el valor de la pendiente obtenida y cuáles son sus unidades?

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/Kirc_gui_03.png
         :scale: 55
         :align: center
         :name: fig:Kirc_gui_03

         Circuito

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/Kirc_gui_02.png
         :scale: 90
         :align: center
         :name: fig:Kirc_gui_02

         Montaje del circuito para estudiar la ley de Ohm

      .. csv-table::  :math:`R=120\,\Omega`
         :header: "Voltaje, :math:`V` (V)", "Corriente, :math:`I` (A)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ohm_law_01
         :align: center

         0,.
         10,.
         20,.
         30,.
         40,.
         50,.
         60,.
         70,.
         80,.
         90,.
         100,.

      .. csv-table::  :math:`R=50\,\Omega`
         :header: "Voltaje, :math:`V` (V)", "Corriente, :math:`I` (A)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Ohm_law_02
         :align: center

         0,.
         10,.
         20,.
         30,.
         40,.
         50,.
         60,.
         70,.
         80,.
         90,.
         100,.

   #. Fije el valor de la resistencia en :math:`R=60\,\Omega` y repita las mismas mediciones anteriores. Registre sus datos en la :numref:`tab:Ohm_law_02`, mida el valor de la corriente y consígnelo en la tabla. Realice una gráfica de :math:`V` en función de :math:`I` y verifique que la relación entre estas variables es lineal. Si se tiene en cuenta los resultados del anterior inciso, ¿qué se puede concluir?
   #. Discuta sus resultados y escriba sus conclusiones.

**Leyes de Kirchhoff**


   #. Monte y simule el circuito de la :numref:`fig:Kirc_circ_01`. Como elementos resistivos escoja bombillas y fije las resistencias de sus filamentos en :math:`R_1=10.0\,\Omega`, :math:`R_2=1.0\,\Omega`, :math:`R_3=R_4=0.5\,\Omega`. Una versión de este circuito en simulador podría ser como la mostrada en la :numref:`fig:Kirc_gui_04`, usted es libre de realizar su propio montaje.

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/K_circuit_01.png
         :scale: 100
         :align: center
         :name: fig:Kirc_circ_01

         Circuito para estudiar las leyes de Kirchhoff


      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/Kirc_gui_04.png
         :scale: 80
         :align: center
         :name: fig:Kirc_gui_04

         Circuito para estudiar las leyes de Kirchhoff

   #. Fije el valor del voltaje de la batería en 3.0 V. Cierre los interruptores :math:`S_1`, :math:`S_2`, :math:`S_3` y haga las lecturas de las corrientes :math:`i_1`, :math:`i_2` e :math:`i_3` y escriba sus valores en la :numref:`tab:kirchhoff_law_1`. Varíe el valor del voltaje de la batería tal como sugiere la tabla y registre los correspondientes valores de corrientes. ¿Cómo están relacionados los valores de las corrientes entre sí? ¿En qué cambia su conclusión, si se cambia la polaridad de la batería?

      .. csv-table::  Corrientes en la unión de las amperímetros ideales
         :header: "Voltaje, :math:`V` (V)", "Corriente, :math:`i_1` (A)", "Corriente, :math:`i_2` (A)", "Corriente, :math:`i_3` (A)"
         :widths: 1,1,1,1
         :width: 16 cm
         :name: tab:kirchhoff_law_1
         :align: center

         5,,,   
         8,,,   
         10,,,    
         15,,,  
         20,,,  

   #. En el simulador, con la ayuda del voltímetro y fijando el voltaje de la batería en 10 V verifique la segunda ley de Kirchhoff para cada uno de los lazos que se indican en la :numref:`fig:K_Setup_02`.
   #. Repita el inciso anterior pera esta vez para un voltaje de batería diferente, el que desee. ¿Qué se puede concluir?
   #. Compruebe que las ecuaciones que se obtienen al aplicar las leyes de Kirchhoff al circuito de la :numref:`fig:Kirc_circ_01` son:

      .. math::

        \begin{eqnarray}
         -R_1i_1+V-(R_3+R_4)i_2 &=& 0  \\
         -R_2i_3+(R_3+R_4)i_2 &=& 0 \\
         i_1 &=& i_2+i_3
        \end{eqnarray}

      .. figure:: /images/Electromagnetismo/Kircchoff_Laws/K_circuit_02.png
         :scale: 100
         :align: center
         :name: fig:K_Setup_02

         Lazos para verificar la segunda ley de Kirchhoff

   #. Solucione el anterior sistema de ecuaciones para las corrientes :math:`i_1`, :math:`i_2` e :math:`i_3` con :math:`R_1=R_2=R_3=R_4=2\,\Omega`, V=5V. Verifique su respuesta con la obtenida directamente del simulador.
   #. Fije el voltaje de la batería en 10 V y las resistencias de los filamentos de las 4 bombillas en :math:`10\,\Omega` cada una. Explique la razón por la cual la intensidad de la bombilla izquierda es mayor que la del resto de bombillas. ¿Por qué razón, la intensidad de las bombillas conectadas en serie (bombillas centrales) es igual? Si se abre el interruptor de la derecha, :math:`S_3` ¿Por qué razón las intensidades de las tres bombillas izquierdas se hacen iguales?

