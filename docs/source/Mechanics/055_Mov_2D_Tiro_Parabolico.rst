Movimiento en 2d: Tiro parabólico
==================================

**Objetivo**

El propósito de esta práctica es estudiar el movimiento de un cuerpo pequeño (partícula) en dos dimensiones cuando sobre éste actúa una única fuerza constante y demostrar que bajo estas circunstancias la trayectoria que describe es una parábola.


**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.walter-fendt.de/html5/phen/projectile_en.htm <https://www.walter-fendt.de/html5/phen/projectile_en.htm>`_.

**Resumen teórico**

Cuando la fuerza que actúa sobre un cuerpo es constante, el movimiento resultante se puede descomponer en dos componentes independientes. Para el caso de la fuerza de la gravedad y con un sistema de coordenadas cartesianos donde la fuerza es paralela al eje :math:`y`, el movimiento resultante se puede descomponer en dos movimientos independientes: uno con velocidad constante y otro con aceleración constante.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Mov_2D_gui_03` muestra la interfaz gráfica del usuario. La aplicación simula el lanzamiento de un cuerpo pequeño cerca de la superficie donde la fuerza es constante, además ésta permite fijar los valores de la altura inicial, velocidad inicial, ángulo de lanzamiento, masa y aceleración de la gravedad del sitio desde donde se hace el lanzamiento. También permite visualizar la trayectoria descrita por el cuerpo y otras cantidades como su velocidad, aceleración, fuerza y energía cinética.

.. figure:: /images/Mecanica/Mov_2D_Tiro_Parabolico/GUI_03.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:Mov_2D_gui_03

   Interfaz gráfica del usuario

**Mediciones y procedimientos**

   #. Fije los valores de altura inicial, velocidad inicial, ángulo, masa y aceleración de la gravedad indicados en la :numref:`fig:Mov_2D_gui_03`. Anote los valores de las coordenadas :math:`x` y :math:`y` en la :numref:`tab:parab_01`. Realice el lanzamiento del cuerpo presionando el botón *Start* (arrancar). Presione rápidamente y varias veces el botón *Pause* (detener) y *Resume* (reanudar), y anote los correspondientes valores de :math:`x` y :math:`y` en la tabla. A partir de la tabla de datos y el uso de Excel demuestre que la relación entre la altura (:math:`y`) y el desplazamiento horizontal (:math:`x`) es una ecuación cuadrática (parábola). (Nota: la ecuación de una cuadrática es de la forma :math:`y=ax^{2}+bx+c`, donde :math:`a`, :math:`b` y :math:`c` son constantes. Para el caso considerado, encuentre los valores de estas constantes.

      .. csv-table:: Datos posición :math:`x` y :math:`y`
         :header: ":math:`h`", ":math:`\\Delta t`` (s)"
         :widths: 1,1
         :width: 10 cm
         :name: tab:parab_01
         :align: center

         0,50.
         .,.
         .,.
         .,.
         .,.
         :math:`\vdots`,:math:`\vdots`
         .,.
         .,.
         .,.
         .,.
         .,.
         5.6,0.0


   #. Con los mismos valores de altura inicial, velocidad inicial, ángulo, masa y aceleración de la gravedad del caso anterior seleccione el radio botón *velocity*, ver :numref:`fig:Mov_2D_gui_04`. La aplicación despliega los valores de las componentes del vector velocidad del cuerpo.  Presione rápidamente y varias veces el botón *Pause* (detener) y *Resume* (reanudar), y anote los correspondientes valores de las componentes de la velocidad :math:`v_x` y :math:`v_y`  en función del tiempo en la :numref:`tab:parab_02`. A partir de la tabla de datos demuestre que la relación entre :math:`v_y` y :math:`t` es lineal, es decir, es una relación de la forma :math:`v_y=a+bt`; encuentre los valores de estas constantes, sus unidades y su relación con las condiciones iniciales de movimiento y la aceleración de la gravedad.

      .. figure:: /images/Mecanica/Mov_2D_Tiro_Parabolico/GUI_04.png
         :alt:
         :scale: 68
         :align: center
         :name: fig:Mov_2D_gui_04

         Interfaz para captura de componentes de la velocidad

   #. Verifique con el simulador que el movimiento del cuerpo es independiente de su masa.
   #. Repita el experimento del inciso 1 con los mismos valores de altura inicial, velocidad inicial, ángulo, masa, pero esta vez cambie el valor de la aceleración a 1.62 :math:`\text{m/s}^{2}` (valor de la aceleración de la gravedad en la superficie de la Luna). ¿Qué puede concluir acerca del movimiento del cuerpo si este se moviera en la Tierra y la Luna?
   #. Interprete sus resultados y escriba sus conclusiones

      .. csv-table:: Datos velocidad :math:`v_x`, :math:`v_y` y tiempo
         :header: "Comp. velocidad, :math:`v_x` (m/s)", "Comp. velocidad, :math:`v_y` (m/s)", "Tiempo :math:`t` (s)"
         :widths: 1,1,1
         :width: 17 cm
         :name: tab:parab_02
         :align: center

         4.33, 0, 0
          .,.,.
          .,.,.
          .,.,.
          .,.,.
         :math:`\vdots`, :math:`\vdots`, :math:`\vdots`
          .,.,.
          .,.,
          .,.,.
          .,.,.
          .,.,.
          .,.,.
          .,.,.
         4.33, -10.2, 1.296



