Trabajo y energía cinética
=====================================
**Objetivo**

El propósito de esta práctica es estudiar el efecto de una fuerza aplicada a un cuerpo sobre su energía cinética.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `{http://physics.bu.edu/~duffy/HTML5/work_energy.html <{http://physics.bu.edu/~duffy/HTML5/work_energy.html>`_.

**Resumen teórico**

El trabajo realizado por una fuerza :math:`\overrightarrow{F}` para llevar un cuerpo de un punto :math:`A` a un punto :math:`B` se define \ como

.. math::
   :label: Ec:Work_Energy_01

   \begin{equation}
   W=\int \overrightarrow{F}\cdot d\overrightarrow{r}
   \end{equation}

donde la integral que aparece en la expresión :eq:`Ec:Work_Energy_01` es una integral especial
denominada integral de l\'{\i}nea ya que la integral se realiza sobre un camino que conecta los puntos :math:`A` y :math:`B`. En general el valor de la integral depende de la trayectoria que conecta los puntos :math:`A` y :math:`B`.
La expresión :eq:`Ec:Work_Energy_01` se reduce a la dada por :eq:`Ec:Work_Energy_02` cuando el movimiento es rectilíneo (eje :math:`x` por ejemplo) y la fuerza es constante y también va dirigida a lo largo del eje :math:`x`.

.. math::
   :label: Ec:Work_Energy_02

   \begin{equation}
    W=F\Delta x
   \end{equation}



donde :math:`\Delta x` es el desplazamiento realizado por el cuerpo.

Se define energía cinética de un cuerpo con masa :math:`m` y velocidad :math:`v` como :math:`E_J=\frac{1}{2}mv^{2}` y se mide  en julios.

El teorema del trabajo y energia afirma que si como resultado de aplicar :math:`N` fuerzas :math:`\overrightarrow{F}_{1},\overrightarrow{F}_{2},\ldots \overrightarrow{F}_{N}` \ a un cuerpo, su energia cinética cambia de :math:`E_{k_{A}}` a :math:`E_{k_{B}}`, entonces el trabajo neto :math:`W` hecho por estas fuerzas es igual al cambio de su energia cinética :math:`\Delta E_{k}`, es decir

.. math::
   :label: tab:Work_Energy_03

   \begin{equation}
    W=W_{\overrightarrow{F}_{1}}+W_{\overrightarrow{F}_{2}}+W_{\overrightarrow{F}_{3}}+\ldots W_{\overrightarrow{F}_{N}}=\Delta E_{k}=E_{k_{B}}-E_{k_{A}}
   \end{equation}

Este teorema es de gran validez y la naturaleza de las fuerzas no importa; es decir, que las fuerzas pueden ser de origen mecánico, eléctrico,
magnético, gravitacional, etc y el teorema aplica.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Work_Energy_01` muestra la interfaz gráfica del usuario para estudiar el efecto del trabajo hecho por una fuerza aplicada a un cuerpo sobre su energía cinética. Para ello, un cuerpo de masa :math:`m` se mueve a lo largo del eje :math:`x` con velocidad inicial constante :math:`v_0=10.0\,\text{m/s}`, y  justamente cuando el cuerpo ha recorrido una distancia de :math:`20.0\,\text{m}`  se le aplica una fuerza constante dirigida a lo largo del eje :math:`x`, la cual permanece aplicada durante cierta distancia recorrida por el cuerpo. El movimiento dura hasta que el cuerpo recorre una distancia total de 100 m. La magnitud de la fuerza se puede controlar con la barra de desplazamiento rotulada **{Set applied forced** en el rango comprendido entre -10 N y +10 N, el signo negativo significa que la fuerza está dirigida hacia la izquierda y el signo positivo hacia la derecha. La distancia que permanece aplicada la fuerza se fija con la barra de desplazamiento rotulada **Set the distance through which the force is applied, starting at x = 20 m** en el rango comprendido entre 0 y 50 m. Una vez fijados los anteriores parámetros, el movimiento del cuerpo se inicia al presionar el botón **Play**, se puede detener el movimiento con el botón **Pause**, a igual que avanzar o retroceder paso a paso con los botones **Step** :math:`>>` :math:`<<` **Step** respectivamente. Al presionar el botón **Reset**, la posición del cuerpo se hace :math:`x=0` y se prepara para iniciar de nuevo. A medida que el cuerpo avanza, su coordenada de posición :math:`x`, velocidad instantánea :math:`v` se muestran para diferentes instantes de tiempo :math:`t`, a igual que la gráfica de energía cinética :math:`E_J` del cuerpo en función de la distancia :math:`x`.


.. figure:: /images/Mecanica/Trabajo_Energia/gui_01.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Work_Energy_01

   Interfaz gráfica del usuario para estudiar el efecto del trabajo hecho por una fuerza aplicada a un cuerpo sobre el cambio en su energía cinética.


**Mediciones y procedimientos**

   #. A partir de la definición de energía cinética y de la información mostrada en la interfaz gráfica del usuario determine la masa del cuerpo.
   #. Fije la distancia en la que actúa la fuerza en :math:`\Delta x=15\,\text{m}` y registre la posición :math:`x` en función del tiempo :math:`t` (cada 0.5 s) para las fuerzas de valor -10 N, 0 N y +10 N. Complete la :numref:`tab:Work_Energy_01`, la :numref:`tab:Work_Energy_03` y la :numref:`tab:Work_Energy_05`.
   #. A partir de la información de la :numref:`tab:Work_Energy_01`, la :numref:`tab:Work_Energy_03` y la :numref:`tab:Work_Energy_05` construya las gráficas de posición en función del tiempo. Con la ayuda de las gráficas anteriores, construya las gráficas de velocidad en función del tiempo, para ello utilice sus conocimientos de linealización de funciones con la ayuda de Excel. Verifique, a partir de la ecuaciones :eq:`Ec:Work_Energy_01` y :eq:`tab:Work_Energy_03` que :math:`v_f=\sqrt{v_i^{2}+\frac{2F}{m}\Delta x}`, donde :math:`v_i=10,\text{m/s}`  y :math:`\Delta x=15\,\text{m}` en todos los tres casos.
   #. A partir de la información de los anteriores incisos construya las gráficas de energía cinética en función de la posición :math:`x` para uno de los tres casos. Compare sus resultados con los obtenidos directamente de la gráfica que muestra la interfaz gráfica.
   #. Repita los procedimientos de los incisos 2, 3 y 4, pero esta vez fije la distancia en la que actúa la fuerza en :math:`\Delta x=40\,\text{m}` y registre la información en la :numref:`tab:Work_Energy_06`, la :numref:`tab:Work_Energy_08` y la :numref:`tab:Work_Energy_10`.
   #. Discuta sus resultados y escriba sus conclusiones.

      .. csv-table:: :math:`F=-10\,\text{N}`, Distancia :math:`\Delta x=15\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_01
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

      .. csv-table:: :math:`F=0\,\text{N}`, Distancia :math:`\Delta x=15\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_03
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

      .. csv-table:: :math:`F=+10\,\text{N}`, Distancia :math:`\Delta x=15\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_05
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

   #. Repita los procedimientos de los incisos 2, 3 y 4, pero esta vez fije la distancia en la que actúa la fuerza en :math:`\Delta x=40\,\text{m}` y registre la información en la :numref:`tab:Work_Energy_06`, la :numref:`tab:Work_Energy_08` y la :numref:`tab:Work_Energy_10`.
   #. Discuta sus resultados y escriba sus conclusiones.

      .. csv-table:: :math:`F=-10\,\text{N}`, Distancia :math:`\Delta x=40\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_06
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

      .. csv-table:: :math:`F=0\,\text{N}`, Distancia :math:`\Delta x=40\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_08
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

      .. csv-table:: :math:`F=+10\,\text{N}`, Distancia :math:`\Delta x=40\,\text{m}`
         :header: ":math:`t` (s)", ":math:`x` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Work_Energy_10
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



