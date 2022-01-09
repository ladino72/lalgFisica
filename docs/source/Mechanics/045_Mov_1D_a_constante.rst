Movimiento rectilíneo con aceleración constante
================================================

**Objetivo**

El propósito de esta práctica es estudiar el movimiento de un auto que se mueve en una dimensión (eje :math:`x`). Durante su movimiento, sobre el auto actua  una fuerza constante (a lo largo del eje :math:`x`) causando que éste se mueva con aceleración constante. De los datos de la simulación se encontrarán las ecuaciones cinemáticas que describen el movimiento del auto.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.walter-fendt.de/html5/phen/acceleration_en.htm <https://www.walter-fendt.de/html5/phen/acceleration_en.htm>`_.

**Resumen teórico**

Para un cuerpo que se mueve en una dimensión en general se cumple:

   #. De la gráfica de velocidad en función del tiempo, el área bajo la curva entre los instantes de tiempo :math:`t_1` y :math:`t_2` representa el desplazamiento del cuerpo, es decir, :math:`\Delta x=\text{área bajo la curva}`
   #. De la gráfica de velocidad en función del tiempo, la pendiente de la recta tangente a la curva en un instante de tiempo :math:`t` representa la aceleración instantánea del cuerpo.
   #. De la gráfica de aceleración en función del tiempo, el área bajo la curva entre los instantes de tiempo :math:`t_1` y :math:`t_2` representa el cambio de velocidad del cuerpo, es decir, :math:`\Delta v=\text{área bajo la curva}`
   #. De la gráfica de posición en función del tiempo, la pendiente de la recta tangente a la curva en un instante de tiempo :math:`t` representa la velocidad instantánea del cuerpo.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:MUAR_GUI_01` muestra la interfaz gráfica del usuario, la cual presenta dos fotoceldas (1 y 2) que el usuario puede desplazar hacia la izquierda o derecha y sus ubicaciones se determinan por sus coordenadas :math:`x`; en el caso mostrado, sus ubicaciones son :math:`x=25\,\text{m}` y :math:`x=50\,\text{m}`. La posición inicial, velocidad inicial y aceleración  del auto se pueden establecer en el recuadro de la derecha al introducir valores directamente sobre los recuadros de entrada. Cuando el auto se pone en movimiento y pasa por las fotoceldas estas sensan su movimiento y activan los medidores de tiempo los cuales registran los tiempos que transcurrren desde que el auto se puso en marcha hasta que pasa por los fotoceldas.
A medida que el auto se desplaza sus gráficas de posición, velocidad y aceleración se van trazando.

.. figure:: /images/Mecanica/Mov_1D_a_constante/MUAR_GUI_01.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:MUAR_GUI_01

   Interfaz gráfica del usuario


**Mediciones y procedimientos**


   #. Fije las fotoceldas 1 y 2 en :math:`x=5\,\text{m}` y :math:`x=10\,\text{m}` y los valores de posición inicial, velocidad inicial y aceleración en 0 m,0 m/s y :math:`a=5\,\text{m/s}^{2}`. Ponga el auto en marcha (presione el botón start (arrancar)) y registre los tiempos en la :numref:`tab:MUAR_1`. Repita el paso anterior pero esta vez colocando las fotoceldas en las posiciones :math:`x=15\,\text{m}`, :math:`x=20\,\text{m}`, :math:`x=25\,\text{m}`, :math:`x=30\,\text{m}`, :math:`x=35\,\text{m}`, :math:`x=40\,\text{m}` y :math:`x=45\,\text{m}` y :math:`x=50\,\text{m}`. Obsérvese que con la ayuda de las fotoceldas estamos registrando la posición del auto como función del tiempo. Demuestre que la relación entre :math:`x` y :math:`t` obedece a una relación de la forma :math:`x=c_0+c_1t+c_2t^{2}`, donde :math:`c_0`, :math:`c_1` y :math:`c_2` son constantes. Utilice Excel para encontrar los valores de estas constantes. \textquestiondown Cuál es el significado y qué dimensiones tienen estas constantes? ¿Qué tienen que ver estas constantes con las condiciones iniciales fijadas inicialmente en el recuadro derecho de la interfaz gráfica? De la relación matemática encontrada deduzca la ecuación para la velocidad y aceleración en función del tiempo. Grafique estas ecuaciones.
   #. En esta parte no utilizaremos las fotoceldas, para ellos fije las fotoceldas 1 y 2 en :math:`x=50\,\text{m}`, ver :numref:`fig:MUAR_gui_02`. Fije los valores de posición inicial, velocidad inicial y aceleración en 0 m, 9.0 m/s y :math:`a=-1.0\,\text{m/s}^{2}`. Ponga el auto en marcha y registre los tiempos en la :numref:`tab:MUAR_2`, para ello presione el botón Pause (detener) y Resume (reanudar) rápidamente y tomar las mediciones. Demuestre que la relación entre :math:`x` y :math:`t` obedece la misma relación anterior, es decir, :math:`x=c_0+c_1t+c_2t^{2}`, donde :math:`c_0`, :math:`c_1` y :math:`c_2` son constantes. Utilice Excel para encontrar los valores de estas constantes. \textquestiondown Cuál es el significado y qué dimensiones tienen estas constantes? ¿Qué tienen que ver estas constantes con las condiciones iniciales fijadas inicialmente en el recuadro derecho de la interfaz gráfica? De la relación matemática encontrada deduzca la ecuación para la velocidad y aceleración en función del tiempo. Grafique estas ecuaciones.
   #. Interprete sus resultados y escriba sus conclusiones

.. figure:: /images/Mecanica/Mov_1D_a_constante/MUAR_GUI_02.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:MUAR_GUI_02

   Interfaz gráfica del usuario


.. csv-table:: Datos posición y tiempo
   :header: "Posición, :math:`x` (m)", "Tiempo, :math:`t` (s)"
   :widths: 1,1
   :width: 10 cm
   :name: tab:MUAR_1
   :align: center

   0, 0
   5.0,
   10.0,
   15.0,
   20.0,
   25.0,
   30.0,
   35.0,
   40.0,
   45.0,
   50.0,


.. csv-table:: Datos posición y tiempo
   :header: "Posición, :math:`x` (m)", "Tiempo, :math:`t` (s)"
   :widths: 1,1
   :width: 10 cm
   :name: tab:MUAR_2
   :align: center

   0, 0
   5.0,
   10.0,
   15.0,
   20.0,
   25.0,
   30.0,
   35.0,
   40.0,


