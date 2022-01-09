Condensador de placas paralelas
=================================

**Objetivo**

El propósito de esta experiencia es: a) determinar de manera cuantitativa la dependencia de un condensador de placas paralelas de la distancia de separación entre las placas y el tamaño de las mismas y b) entender que el capacitor es un dispositivo que sirve para almacenar energia eléctrica.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/capacitor-lab-basics/latest/capacitor-lab-basics_es_MX.html <https://phet.colorado.edu/sims/html/capacitor-lab-basics/latest/capacitor-lab-basics_es_MX.html>`_.
   #. Hoja de cálculo de Excel.

**Resumen teórico**

Se denomina capacitor o condensador al sistema formado por dos conductores :math:`A` y :math:`B` no necesariamene iguales, los cuales tienen cargas generalmente de igual valor pero de signo opuesto :math:`+Q` y :math:`-Q`, tal como se indica en la :numref:`fig:capacitor_01`. Entre los conductores existe una diferencia de potencial :math:`\Delta V` la cual está relacionada con la carga :math:`+Q` mediante la relación :math:`\Delta V=\frac{+Q}{C}`, donde :math:`C` es una constante positiva denominada la capacitancia del capacitor y cuyo valor depende de factores geométricos como son el tamaño de los conductores, distancia de separación y su orientación relativa. Entre los conductores del capacitor se tiene un campo eléctrico cuyas líneas de campo eléctrico son perpendiculares a las superficies de los mismos.
El valor de la capacitancia también depende del tipo de sustancia que se tenga en medio de los conductores, sustancia que se llama material dieléctrico. Las unidades de la capacitancia son culombio/voltio=Faradio, representado por la letra mayúscula :math:`F`. Así, dependiendo de la geometría de los conductores se tienen diferentes tipos de capacitores: de placas paralelas, cilíndrico, esférico, etc. Los capacitores se utilizan para almacenar carga eléctrica y energía eléctrica. El campo eléctrico entre los conductores del capacitor almacena la energía eléctrica, la cual puede utilizarse como por ejemplo para encender un LED (light emitter diode). Los capacitores son elementos muy utilizados en los dispositivos electrónicos.

.. figure:: /images/Electromagnetismo/Capacitance/Capacitor_01.png
   :scale: 70
   :align: center
   :name: fig:capacitor_01

   Capacitor formado por dos conductores

**Descripción de la interfaz de la aplicación**

Para estudiar la dependencia de la capacitancia de factores geométricos utilizaremos la aplicación cuyo enlace se cita arriba en la sección de Recursos y cuya interfaz se muestra en la :numref:`Fig:Capacitance_Gui_00`. Esta consta de una batería que suministra una diferencia de potencial entre -1.5 V y +1.5 V, dos interruptores y un par de placas paralelas (condensador o capacitor) cuyo tamaño de placas y distancia de separación se puede variar. Mediante los interruptores es posible conectar o desconectar la batería del capacitor. Tanto la capacitancia, como la cantidad de carga y energía almacenada por el capacitor se pueden leer en la parte superior izquierda de la interfaz.

.. figure:: /images/Electromagnetismo/Capacitance/setup_00.png
   :scale: 40
   :align: center
   :name: Fig:Capacitance_Gui_00

   Interfaz gráfica del usuario para estudiar la dependencia de la capacitancia de factores geométricos


**Mediciones y procedimientos**


**Dependencia de la capacitancia de factores geométricos**

   #. Para encontrar la dependencia de la capacitancia :math:`C` de la distancia :math:`d` de separación  entre las placas del capacitor, fije el valor del área en un valor cualquiera entre :math:`100\, \text{mm}^2` y :math:`400\, \text{mm}^2`. Varíe el valor de la distancia :math:`d` en pasos de 0.5 mm desde 2.0 hasta 10 mm y para cada valor de :math:`d` establecido registre el valor de la correspondiente capacitancia :math:`C` en la :numref:`tab:cap_01`. Se asume que la relación entre :math:`C` y :math:`d` es de la forma :math:`C=ad^{n}`, siendo :math:`a` una constante de proporcionalidad y :math:`n` un real a determinar. Haga uso de sus conocimientos de linealaización de funciones para encontrar el valor de :math:`n`.

      .. csv-table:: Mediciones para determinar la dependencia de :math:`C` de :math:`d`, el valor de :math:`A` se mantiene fijo
         :header: ":math:`d \\,\\text{(mm)}`", ":math:`C` (pF)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:cap_01
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.


   #. Para encontrar la dependencia de la capacitancia :math:`C` del capacitor del área :math:`A` de las placas,  fije el valor de la distancia `d` en un valor cualquiera entre :math:`2\, \text{mm}` y :math:`10\,\text{mm}`. Varíe el valor del área en pasos de :math:`50\, \text{mm}^{2}` desde 10 hasta :math:`400\,\text{mm}^{2}` y para cada valor de :math:`A` establecido registre el valor de la correspondiente capacitancia :math:`C` en la :numref:`tab:cap_02`. Se asume que la relación entre :math:`C` y :math:`A` es de la forma :math:`C=bd^{m}`, siendo :math:`b` una constante de proporcionalidad y :math:`m` un real a determinar. Haga uso de sus conocimientos de linealización de funciones para encontrar el valor de :math:`m`.

      .. csv-table:: Mediciones para determinar la dependencia de :math:`C` de :math:`A`, el valor de :math:`d` se mantiene fijo
         :header: ":math:`A \\,\\text{(mm)}^2`", ":math:`C` (pF)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:cap_02
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.
         .,.

**Relación entre** :math:`\Delta V` y :math:`C`

Compruebe que si la carga del capacitor se mantiene constante entonces el producto :math:`C\times \Delta V` se mantiene constante, siendo :math:`\Delta V` diferencia de potencial (voltaje) entre las placas del capacitor y :math:`C` su capacitancia.

Sugerencia:

   #. Ajuste las placas del capacitor de modo que tengan la mayor superficie y estén a la menor distancia de separación.
   #. Cargue el condensador a +1.5 V con la batería.
   #. Desconecte el capacitor de la batería.
   #. Conecte los terminales del voltímetro, un terminal a cada terminal del capacitor.
   #. varíe la distancia entre las placas y registre la correspondiente lectura del voltímetro, para ello construya una tabla de por lo menos 8 entradas de la forma :math:`(C,\Delta V)` y f) realice una gráfica de :math:`\Delta V` en función de :math:`C`.

**Energía almacenada en el capacitor**

   #. Utilice el montaje  de la :numref:`Fig:Capacitance_Gui_01`.

      .. figure:: /images/Electromagnetismo/Capacitance/setup_01.png
         :scale: 40
         :align: center
         :name: Fig:Capacitance_Gui_01

         Interfaz gráfica del usuario para estudiar la energía almacenada por un capacitor.

   #.
      a. Fije el área :math:`A` de las placas del capacitor a su máximo valor.
      b. Cargue el condensador a 1.5 V mediante la batería.
      c. Fije la distancia :math:`d` de separación entre las placas a su mínimo valor.
      d. Descargue el condensador a través de la bombilla y registre el tiempo que esta dura iluminada.
      e. Aumente el valor de la distancia :math:`d` y repita el procedimiento anterior.


   #. Repita el procedimiento anterior pero esta vez aplicando al capacitor una diferencia de potencial de 0.7 V.

¿Qué concluye respecto a la energí a almacenada en el capacitor con respecto al valor de la capacitancia? ¿Es correcto afirmar que entre mayor es la capacitancia mayor es la energía almacenada en el capacitor? Argumente con solidez.

