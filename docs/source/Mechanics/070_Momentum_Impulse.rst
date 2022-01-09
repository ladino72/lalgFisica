Impulso-Momentum
===================

**Objetivo**

El propósito de esta práctica es estudiar el efecto de una fuerza aplicada a un cuerpo sobre su cantidad de movimiento lineal.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://physics.bu.edu/~duffy/HTML5/impulse.html <http://physics.bu.edu/~duffy/HTML5/impulse.html>`_.

**Resumen teórico**

La cantidad de movimiento lineal o momentum de un cuerpo de masa :math:`m` y velocidad :math:`v` es una cantidad vectorial y se define como

.. math::
   :label: mom_imp_Ec_00

   \begin{equation}\label{mom_imp_Ec_00}
    \overrightarrow{p}=m\overrightarrow{v}
   \end{equation}

de la definición se sigue que una bala en movimiento presenta un momentum grande debido a su gran velocidad y que un camión grande a baja velocidad presenta un momentum grande debido a su gran masa.

El impulso :math:`\overrightarrow{I}` de una fuerza :math:`\overrightarrow{F}` actuando sobre un cuerpo durante un tiempo :math:`\Delta t` es una cantidad que describe su efecto sobre este y se define como

.. math::
   :label: mom_imp_Ec_01

   \begin{equation}
     \overrightarrow{I}=\int_{t_i}^{t_f}\overrightarrow{F}(t)dt
   \end{equation}

De lo anterior se sigue que de un diagrama de fuerza :math:`F` neta en función del tiempo, el área bajo la curva entre :math:`t_i` y :math:`t_f` representa el impulso aplicado al cuerpo por la fuerza  durante el intervalo de tiempo :math:`t_f-t_i`. En el caso que la fuerza sea constante la anterior expresión se reduce a

.. math::
   :label: mom_imp_Ec_011

   \begin{equation}
    \overrightarrow{I}=\overrightarrow{F}\Delta t
   \end{equation}

donde :math:`\Delta t =t_f-t_i`. En el Sistema Internacional (S.I.) las unidades del impulso son newton por segundo ( N·s ). El teorema del impulso mecánico establece que el impulso mecánico de la fuerza resultante que actúa sobre un cuerpo es igual a la variación de su cantidad de movimiento lineal o momentum:

.. math::
   :label: mom_imp_Ec_02

   \begin{equation}
    \overrightarrow{I}= \Delta \overrightarrow{p}= \overrightarrow{p}_{f}-\overrightarrow{p}_{i}
   \end{equation}

donde :math:`\overrightarrow{p}=m\overrightarrow{v}`. Obsérvese que la expresión anterior significa que para conferir una determinada velocidad a un cuerpo (aumentar su cantidad de movimiento lineal) podemos actuar de dos formas: actuar sobre la fuerza o sobre el tiempo durante el cual actúa. Así, en los transbordadores espaciales la nave alcanza la velocidad deseada debido al efecto continuado de la fuerza que proporcionan los propulsores.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:mom_imp_01` muestra la interfaz gráfica del usuario para estudiar el efecto de una fuerza sobre la cantidad de movimiento de un cuerpo. Para ello, un cuerpo de masa :math:`m` se mueve a lo largo del eje :math:`x` con velocidad inicial constante :math:`v_0=8.0\,\text{m/s}`, y justamente en :math:`t=2.0\,\text{s}` se le aplica una fuerza constante dirigida a lo largo del eje :math:`x` durante un intervalo de tiempo :math:`\Delta t`. El movimiento dura hasta que el cuerpo recorre una distancia total de 100 m. La magnitud de la fuerza se puede controlar con la barra de desplazamiento rotulada **Set applied forced** en el rango comprendido entre -10 N y +10 N, el signo negativo significa que la fuerza está dirigida hacia la izquierda y el signo positivo hacia la derecha. El intervalo de tiempo  :math:`\Delta t` que la fuerza dura aplicada se fija con la barra de desplazamiento rotulada **Set the amount of time the force is applied, starting at t = 2 s** en el rango comprendido entre 0 y 5 s. Una vez fijados los anteriores parámetros, el movimiento del cuerpo se inicia al presionar el botón **Play**, se puede detener el moviniento con el botón **Pause**, a igual que avanzar o retroceder paso a paso con los botones **Step** :math:`>>` :math:`<<` **Step** respectivamente. Al presionar el botón **Reset**, la posición del cuerpo se hace :math:`x=0` y se prepara para iniciar de nuevo. A medida que el cuerpo avanza, su coordenada de posición :math:`x`, velocidad instantánea :math:`v` se muestran para diferentes instantes de tiempo :math:`t`, a igual que la gráfica de momentum :math:`p` del cuerpo en función del tiempo :math:`t`.

.. figure:: /images/Mecanica/Momentum_Impulse/IM_gui_01.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:mom_imp_01

   Interfaz gráfica del usuario para estudiar el efecto de una fuerza sobre la cantidad de movimiento de un cuerpo.

**Mediciones y procedimientos**

   #. A partir de la definición de momentum y de la información mostrada en la interfaz gráfica del usuario determine la masa del cuerpo.
   #. Fije la duración de la fuerza en :math:`\Delta t=2\,\text{s}` y registre la posición :math:`x` en función del tiempo :math:`t` (cada 0.5 s) para las fuerzas de valor -10 N, 0 N y +10 N. Complete la :numref:`tab:mom_imp_01`, :numref:`tab:mom_imp_03` y :numref:`tab:mom_imp_05`.
   #. A partir de la información de la :numref:`tab:mom_imp_01`, :numref:`tab:mom_imp_03` y :numref:`tab:mom_imp_05` construya las gráficas de posición en función del tiempo. Con la ayuda de las gráficas anteriores, construya las gráficas de velocidad en función del tiempo, para ello utilice sus conocimiento de linealización de funciones con la ayuda de Excel. Verifique, a partir de la ecuación :eq:`mom_imp_Ec_02` que :math:`v_f=v_i+\frac{F}{m}\Delta t`, donde :math:`v_i=8,\text{m/s}` y :math:`\Delta t=2\,\text{s}` en todos los tres casos.
   #. A partir de la información de los anteriores incisos construya las gráficas de momentum en función del tiempo para uno de los tres casos. Compare sus resultados con los obtenidos directamente de la gráfica que muestra la interfaz gráfica.

      .. csv-table:: :math:`F=-10\,\text{N}`, Duración de la fuerza :math:`t=2\,\text{s}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_01
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,

      .. csv-table:: :math:`F=0\,\text{N}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_03
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,

      .. csv-table:: :math:`F=+10\,\text{N}` Duración de la fuerza :math:`t=2\,\text{s}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_05
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,

   #. Repita los procedimientos de los incisos 2, 3 y 4, pero esta vez fije la duración de la fuerza en :math:`\Delta t=4\,\text{s}`. Complete la :numref:`tab:mom_imp_06`, :numref:`tab:mom_imp_08` y :numref:`tab:mom_imp_10`.

      .. csv-table:: :math:`F=-10\,\text{N}`, Duración de la fuerza :math:`t=4\,\text{s}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_06
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,


      .. csv-table:: :math:`F=0\,\text{N}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_08
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,

      .. csv-table:: :math:`F=+10\,\text{N}` Duración de la fuerza :math:`t=4\,\text{s}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:mom_imp_10
         :align: center

         0.0,	0.0
         0.5,
         1.0,
         1.5,
         2.0,
         2.5,
         3.0,
         3.5,
         4.0,
         4.5,
         5.0,
         5.5,
         6.0,
         6.5,
         7.0,
         7.5,
         8.0,
         8.5,
         9.0,
         9.5,
         10.0,

   #. Discuta sus resultados y escriba sus conclusiones.
