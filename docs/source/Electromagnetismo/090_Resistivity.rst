Resistividad: Ley de Ohm
============================

**Objetivo**

El propósito de esta práctica es determinar la resistividad de un conductor usando la ley de Ohm.


**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.thephysicsaviary.com/Physics/Programs/Labs/ResistanceOfWireChallengeLab/ <https://www.thephysicsaviary.com/Physics/Programs/Labs/ResistanceOfWireChallengeLab/>`_.

**Resumen teórico**

Todos los conductores eléctricos se oponen al paso de la corriente eléctrica en mayor o menor medida. Esto es debido a que los portadores de carga (electrones o iones) no se mueven libremente dentro del conductor, estos experimentan continuos choques con los núcleos de los átomos los cuales forman la estructura cristalina del conductor. Esta oposición se denomina resistencia eléctrica de un conductor. La resistencia eléctrica del conductor depende de:

   #. El material del que está compuesto.
   #. La temperatura a la que se encuentra, cuanto mayor es la temperatura, mayor es su resistencia eléctrica.
   #. Factores geométricos: longitud y sección transversal.

Matemáticamente, el valor de la resistencia :math:`R` está dado por

.. math::
   :label: Ec:Resistiv_01

   \begin{equation}
    R=\rho \frac{\ell}{A}
   \end{equation}

donde :math:`R` es la resistencia eléctrica, :math:`\rho` es la resistividad del material, :math:`\ell` es la longitud del conductor y :math:`S` es el área de la sección transversal del conductor. Sus unidades en el Sistema Internacional (S.I.) son el ohmio (:math:`\Omega`), ohmio por metro (:math:`\Omega \cdot m`), metro (:math:`m`) y metro cuadrado :math:`m^{2}` respectivamente.

La ley de Ohm establece que el voltaje :math:`V` (medido en Voltios) entre los extremos de ciertos tipos de materiales conductores es directamente proporcional a la corriente eléctrica :math:`I` (medida en amperios) que fluye a través del material.

.. math::
   :label: Ley_Ohm

   \begin{equation}
    V = RI
   \end{equation}

siendo :math:`R` el valor de la resistencia eléctrica del material.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Gui_Resistiv_Ohms_law_01` muestra la interfaz gráfica del usuario que permite determinar la resistividad de un conductor. La interfaz presenta un conductor de determinado material y sección transversal circular constante, el cual se encuentra conectado a una batería que suministra una determinada diferencia de potencial :math:`V` en dos puntos de contacto. El área de la sección transversal del alambre se determina al hacer clic sobre el botón rotulado **Show Area** (el lado de cada cuadradito es de 0.1 mm). Uno de los puntos se encuentra fijamente conectado al extremo izquierdo del conductor, mientras que el otro punto es movible a lo largo de éste. La posición de este punto se puede fijar en cinco diferentes puntos al hacer clic sobre los botones rotulados **1 2 3 4 5** ubicados en la parte superior de la interfaz. La distancia de separación entre los puntos de contacto se determina con una regla graduada en milímetros la cual se muestra u oculta al hacer clic sobre el botón rotulado como **Show Ruler** o **Hide Ruler**. Intercalado se encuentra un amperímetro ideal (A encerrada en un círculo) el cual mide la corriente que circula por el conductor, su valor se determina al hacer clic sobre este.

.. figure:: /images/Electromagnetismo/Resistivity/Gui_Resistivity_Ohms_law_01.png
   :scale: 70
   :align: center
   :name: fig:Gui_Resistiv_Ohms_law_01

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

Nota: Cada vez que cargue este programa obtendrá una resistividad generada aleatoriamente y una batería con diferencia de potencial diferente, así que no salga del programa una vez que comience.

   #. Determine el valor de la resistencia eléctrica :math:`R` del conductor como función de la distancia :math:`\ell` de separación de los puntos de contacto. Para ello tome mediciones de longitud :math:`\ell` y corriente :math:`I` y complete la :numref:`tab:Resistivity_01`.
   #. A partir de los datos obtenidos en el inciso 1 y la ley de Ohm construya la :numref:`tab:Resistivity_02`.
   #.  A partir de la tabla construida en el inciso 2 realice una gráfica de :math:`R` en función de :math:`\ell`.
   #. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`R` y :math:`\ell`. Asuma una relación de la forma :math:`R=a\ell^{m}`, determine :math:`a` y :math:`m`.
   #. Mida el área :math:`A` de la sección del conductor.
   #. Relacione el valor de :math:`a` encontrado en el inciso 4 con el coeficiente de :math:`\ell` de la ecuación :eq:`Ec:Resistiv_01`. Determine el valor de la resistividad del conductor y reporte su valor en la forma :math:`R=R_0 \pm \Delta R`. Para esto último aplique la teoría de errores.
   #. Discuta sus resultados y escriba sus conclusiones.


      .. csv-table::  Mediciones de longitud y corriente
         :header: "Longitud :math:`\\ell` (m)", "Corriente :math:`I` (A)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Resistivity_01
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.

      .. csv-table::  Longitud medida y Resistencia calculada
         :header: "Longitud :math:`\\ell` (m)", "Resistencia :math:`R\\,\\,(\\Omega)`"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Resistivity_02
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.


