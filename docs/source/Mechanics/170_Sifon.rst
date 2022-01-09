Sifón
==============

**Objetivo**

El propósito de esta práctica es estudiar el principio de funcionamiento del sifón mediante la ecuación de Bernoulli, en particular se calcula la velocidad de salida de un liquido en la manguera de un sifón.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.thephysicsaviary.com/Physics/Programs/Labs/SiphonLab/index.html <https://www.thephysicsaviary.com/Physics/Programs/Labs/SiphonLab/index.html>`_.

**Resumen teórico**

El sifón es un dispositivo que se utiliza para extraer liquidos de un recipiente sin inclinarlo. Funciona como lo muestra la :numref:`Fig:Gui_Siphon_01`. Si el tubo está inicialmente lleno, el liquido comienza a fluir. El movimiento del liquido se describe por la ecuación de Bernoulli:

.. math::
   :label: Ec:siphon_01

   \begin{equation}
    P+\rho gh+\frac{1}{2}\rho v^{2} = \text{Constante}
   \end{equation}

.. figure:: /images/Mecanica/Sifon/Gui_Siphon_01.png
   :scale: 80
   :align: center
   :name: Fig:Gui_Siphon_01

   Sifón


Aplicando la ecuación :eq:`Ec:siphon_01` a los puntos :math:`A` y :math:`C`

.. math::
   :label: Ec:siphon_02

   \begin{equation}
     P_A+\rho gh_A+\frac{1}{2}\rho v_A^{2} = P_C+\rho gh_C+\frac{1}{2}\rho v_C^{2}
   \end{equation}

teniendo en cuenta que :math:`P_A=P_C=P_{atm}`, :math:`h_A=h_1`, :math:`h_C=0` y :math:`v_A=0` (el recipiente es grande y la variación de altura del liquido es despreciable) resulta :math:`v_C=\sqrt{2gh_1}`.\newline Aplicando la ecuación :eq:`Ec:siphon_01` a los puntos :math:`B` y :math:`C`

.. math::
   :label: Ec:siphon_03

   \begin{equation}
    P_B+\rho gh_B+\frac{1}{2}\rho v_B^{2} = P_C+\rho gh_C+\frac{1}{2}\rho v_C^{2}
   \end{equation}

teniendo en cuenta que :math:`P_C=P_{atm}`, :math:`h_B=h_1+h_2`, :math:`h_C=0` y :math:`v_B=v_C`, resulta :math:`P_B=P_{atm}-\rho g(h_1+h_2)`.\newline Aplicando la ecuación :eq:`Ec:siphon_01` a los puntos :math:`D` y :math:`C`

.. math::
   :label: Ec:siphon_04

   \begin{equation}
    P_D+\rho gh_D+\frac{1}{2}\rho v_D^{2} = P_C+\rho gh_C+\frac{1}{2}\rho v_C^{2}
   \end{equation}

teniendo en cuenta que :math:`P_C=P_{atm}`, :math:`h_D=h_1`, :math:`h_C=0` y :math:`v_D=v_C`, resulta :math:`P_D=P_{atm}-\rho gh_1`.


**Descripción de la interfaz de la aplicación**


La :numref:`Fig:Gui_Siphon_03` muestra la interfaz gráfica del usuario que permite estudiar el funcionamiento del sifón. La interfaz permite establecer el nivel de agua en el recipiente, la altura del doblez de la manguera, la profundidad de la manguera en el recipiente de arriba y la profundidad de la misma en el recipiente de abajo mediante los  pares de flechas indicadas con las letras mayusculas rotuladas como **A**, **B**, **C** y **D** respectivamente. Al hacer clic sobre el botón **Start** el recipiente inferior comienza a llenarse, el cronómetro registra el tiempo que dura este proceso. El recipiente inferior tiene forma cilindrica de radio 60 mm. La manguera tiene un diámetro interior igual a 9.5 mm. En cualquier momento el proceso de llenado puede detenerse al presionar el botón **Pause**, si se desea continuar con el llenado haga clic en el botón **Resume**.

.. figure:: /images/Mecanica/Sifon/Gui_Siphon_03.png
   :scale: 80
   :align: center
   :name: Fig:Gui_Siphon_03

   Interfaz para estudiar el sifón


**Mediciones y procedimientos**

La velocidad de salida del liquido por la manguera se puede determinar a partir de la relación :math:`v_C=\frac{R^{2}H}{r^{2}\Delta T}`, donde :math:`R` y :math:`r` son los radios del recipiente inferior y el radio interno de la manguera respectivamente y :math:`\Delta T` es el tiempo que gasta el liquido en ascender una altura :math:`H` en el recipiente, ver figura :numref:`Fig:Gui_Siphon_04`.

   #. Para determinar la relación entre la velocidad de salida :math:`v_C` del liquido en función :math:`h_1`, es decir, de la distancia de la boca de la manguera al nivel del agua en el recipiente de arriba, fije el nivel del agua con respecto al piso igual a :math:`d=1.8\,\text{m}`, varie la distancia de la boca de la manguera al piso :math:`h` y mida el tiempo :math:`\Delta T` que gasta el nivel de agua en ascender una distancia :math:`H=0.5\,\text{m}`. Complete la :numref:`tab:Siphon_VC_v_h`.

      .. csv-table:: Datos simulados para determinar la ralación entre :math:`v_C` y :math:`h_1`
         :header: ":math:`h` (m)", ":math:`\\Delta T` (m)", ":math:`h_1=d-h`, (m)"
         :widths: 1,1,1
         :width: 15 cm
         :name: tab:Siphon_VC_v_h
         :align: center

         0.1,.,.
         0.3,.,.
         0.5,.,.
         0.7,.,.
         0.9,.,.
         1.1,.,.
         1.3,.,.
         1.5,.,.

   #. A partir de la tabla de datos obtenidos en el anterior inciso, realice una gráfica de :math:`v_C` en función de :math:`h_1`.  Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`v_C` y :math:`h_1`. Asuma una relación de la forma :math:`v_C=ah_1^{m}`. Determine los valores de :math:`a` y :math:`m` y relaciónelos con el coeficiente y exponente de :math:`h_1` en la expresión :math:`v_C=\sqrt{2gh_1}` encontrada arriba en el resumen teórico. Encuentre el valor de la aceleración de la gravedad. Discuta la validez de sus resultados.


.. figure:: /images/Mecanica/Sifon/Gui_Siphon_04.png
   :scale: 70
   :align: center
   :name: Fig:Gui_Siphon_04

   Configuración para medir la velocidad de salida del liquido por la manguera.


**Análisis**

   #. Analizando el sifón y basándose en la ecuación de Bernoulli, demuestre que si se quiere que el liquido ascienda por la parte izquierda de la manguera (ver :numref:`Fig:Gui_Siphon_01`) se debe cumplir que la presión en el punto :math:`D` debe ser mayor que la presión en el punto :math:`B` y que la diferencia debe satisfacer :math:`P_D-P_B=\rho gh_2`.
   #. De la ecuación :eq:`Ec:siphon_03` se encontró que :math:`P_B=P_{atm}-\rho g(h_1+h_2)=P_{C}-\rho g(h_1+h_2)`, lo que significa que :math:`P_B < P_C`. A la luz del resultado del inciso anterior, esto significaria que el líquido ascenderia por la parte derecha de la manguera, pero en realidad desciende. Explique esta contradicción.


