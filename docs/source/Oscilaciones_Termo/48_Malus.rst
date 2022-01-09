Ley de Malus
==============

**Objetivo**

El propósito de esta práctica es estudiar la polarización de la luz a través de la ley de Malus.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://www.educaplus.org/luz/polarizacion.html <http://www.educaplus.org/luz/polarizacion.html>`_

**Resumen teórico**

La luz natural es, en general, no polarizada, pero cuando esta incide sobre una lámina polarizante o polarizador se obtiene luz polarizada, es decir, luz donde la dirección de oscilación del campo eléctrico se encuentra a lo largo de la dirección del eje del polarizador, ver :numref:`fig:Malus_01`. Si ahora se coloca un segundo polarizador llamado analizador después del primero y se gira para tener un ángulo :math:`\theta` entre los ejes de los dos polarizadores, la intensidad transmitida :math:`I` está relacionada con la intensidad de la luz incidente :math:`I_0` mediante la expresión [#f1]_

.. figure:: /images/Oscilaciones_Termo/Malus/Malus_01.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:Malus_01

   Ley de Malus.

.. math::
   :label: Ec:Malus_01

   \begin{equation}
    I=I_0\cos^2(\theta)
   \end{equation}



**Montaje experimental**

La :numref:`fig:Malus_Setup` muestra la interfaz del usuario que permite la toma de datos para estudiar la ley de Malus. En la parte inferior derecha se sencuentra un  botón deslizador el cual permite variar el ángulo entre los ejes de los polarizadores en el rango comprendido entre 0 y :math:`360\,^o`; el eje del primer polarizador permanece fijo. En la parte inferior izquierda se muestran los dos polarizadores junto con el porcentaje de la intensidad de la luz que emerge del analizador. Note también que, en el esquema de la parte  superior de  la  ventana  del  simulador,  las  líneas  en  forma  de  diámetros  que representan  las  direcciones  de  los  ejes  de  transmisión  de  los  polarizadores  se  muestran perpendiculares entre sí, en este caso.

.. figure:: /images/Oscilaciones_Termo/Malus/Malus_Setup.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Malus_Setup

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

   #. Coloque el ángulo entre los polarizadores en cero.
   #. Incremente :math:`\theta` en intervalos de  :math:`5\,^o` y registre  en  cada paso la 'Intensidad relativa de la luz recibida' :math:`\frac{𝐼(\theta)}{𝐼(0)}`, que proporciona el simulador en forma porcentual en la :numref:`tab:Malus_01`.

      .. csv-table:: Datos medidos de :math:`\\theta` e Intensidad relativa
         :header: "Angulo, :math:`\\theta\\,(^o)`", ":math:`\\frac{𝐼(\\theta)}{𝐼(0)}`",":math:`\\frac{𝐼(\\theta)}{𝐼(0)}\\times\\frac{1}{100}`"
         :widths: 1,1,1
         :width: 10 cm
         :name: tab:Malus_01
         :align: center

         0,100,1
         5,99.2,0.992
         10,.,.
         15,.,.
         20,.,.
         25,.,.
         30,.,.
         35,.,.
         40,.,.
         45,.,.
         50,.,.
         55,.,.
         60,.,.
         65,.,.
         70,.,.
         75,.,.
         80,.,.
         85,.,.
         90,.,.

   #. Realice una gráfica de :math:`\frac{𝐼(\theta)}{𝐼(0)}\times\frac{1}{100}` en función de :math:`\theta` con los datos de la :numref:`tab:Malus_01`.
   #. Utilice sus conocimientos de linealización para demostrar que los datos de las columnas 1 y 3 de la :numref:`tab:Malus_01` satisfacen la ecuación :eq:`Ec:Malus_01`.

**Preguntas**

   #. ¿Qué demuestra la ley de malus?
   #. ¿Qué tipo de polarización tiene la luz que emerge del primer polarizador?
   #. Desde el punto de vista miscroscópico que sucede en el polarizador cuando la luz incide sobre este?
   #. ¿Qué aplicaciones tiene la luz polarizada?



.. [#f1] Jenkins F.A., White H.E., (1950) *Fundamentals of Optics*, McGraw-Hill, Nueva York