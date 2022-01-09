+Pulsaciones en ondas sonoras
==============================

**Objetivo**

El propósito de esta práctica es estudiar las pulsaciones (o batidos) generados cuando se superponen dos ondas
sonoras audibles.

**Recursos**

   #. Un computador con tarjeta de sonido y parlantes; y acceso a la internet.
   #. Simulación disponible en `https://www.compadre.org/osp/EJSS/4370/203.htm <https://www.compadre.org/osp/EJSS/4370/203.htm>`_.


**Resumen teórico**

Consideremos las ondas senoidales descritas por las expresiones :eq:`Ec:Beats_1` y :eq:`Ec:Beats_2`, las cuales tienen igual amplitud :math:`\varepsilon _{0}`, frecuencias muy similares :math:`f_{A}` , :math:`f_{B}` y que viajan a lo largo del eje :math:`x`.

.. math::
   :label: Ec:Beats_1

   \begin{equation}
    \varepsilon _{1}(x,t)=\varepsilon _{0}\sin (k_{1}x-\omega _{1}t+\phi _{1})
   \end{equation}

.. math::
   :label: Ec:Beats_2

   \begin{equation}
     \varepsilon _{2}(x,t)=\varepsilon _{0}\sin (k_{2}x-\omega _{2}t+\phi _{2})
   \end{equation}

:math:`\phi _{1}` y :math:`\phi _{2}` representan las fases que se mantienen constantes en el tiempo. La velocidad de propagación de estas ondas es

.. math::
   :label: Ec:Beats_3

   \begin{equation}
    v=\frac{\omega _{1}}{k_{1}}=\frac{2\pi f_{A}}{k_{1}}=\frac{\omega _{2}}{k_{2}}=\frac{2\pi f_{B}}{k_{1}}
   \end{equation}

La superposición de :math:`\varepsilon _{1}(x,t)` y :math:`\varepsilon _{2}(x,t)` es :math:`\varepsilon (x,t)=\varepsilon _{1}(x,t)+\varepsilon _{2}(x,t)`  ó

.. math::
   :label: Ec:Beats_4

   \begin{equation}
   \begin{split}
    \varepsilon (x,t)=-2\varepsilon _{0}\cos \left[ \pi (f_{A}-f_{B})t-\frac{\pi }{v}(f_{A}-f_{B})x-\Phi _{1}\right] \\  \times \sin \left[ \pi (f_{A}+f_{B})t-\frac{\pi }{v} (f_{A}+f_{B})x-\Phi _{2}\right]
   \end{split}
   \end{equation}

donde hemos definido :math:`\Phi _{1}=\frac{\phi _{1}+\phi _{2}}{2}` y :math:`\Phi _{2}=\frac{\phi _{1}-\phi _{2}}{2}.`

Los periodos de los términos cosenoidal y senoidal son :math:`T_c=\frac{2\pi}{f_A-f_B}` y :math:`T_s=\frac{2\pi}{f_A+f_B}` respectivamente, con :math:`T_c>T_s`. Así, el término cosenoidal oscila más lentamente en el tiempo que
el termino senoidal y por tanto podemos considerarlo como el factor
modulante del termino senoidal y tomarlo como la amplitud. La ecuación :eq:`Ec:Beats_4` puede interpretarse como una oscilación armónica de frecuencia :math:`\frac{%
f_{A}+f_{B}}{2}` y con amplitud  varía armónicamente  en cada punto en el tiempo con frecuencia :math:`\frac{f_{A}-f_{B}}{2}`.

La intensidad de una onda es proporcional al cuadrado de su amplitud y por
tanto la intensidad de la onda descrita por la expresión :eq:`Ec:Beats_4` es

.. math::
   :label: Ec:Beats_5

   \begin{equation}
    I(t,x)=4I_{0}\cos ^{2}\left[ \pi (f_{A}-f_{B})t-\frac{\pi }{v}(f_{A}-f_{B})x-\Phi _{1}\right]
   \end{equation}

donde :math:`I_{0}\sim \varepsilon _{0}^{2}` . Ahora bien, si nos ubicamos en un
punto particular del espacio :math:`x=x_{0}`, entonces la expresión :eq:`Ec:Beats_5`
se convierte en

.. math::
   :label: Ec:Beats_6

   \begin{eqnarray}
    I(t,x_{0}) &=&4I_{0}\cos ^{2}\left[ \pi (f_{A}-f_{B})t-\frac{\pi }{v}(f_{A}-f_{B})x_{0}-\Phi _{1}\right]  \nonumber \\
    &=&4I_{0}\cos ^{2}\left[ \pi (f_{A}-f_{B})t-\Psi \right]
   \end{eqnarray}


donde :math:`\Psi =\frac{\pi }{v}(f_{A}-f_{B})x_{0}+\Phi _{1}=`constante. Así, la
intensidad en el punto :math:`x=x_{0}` oscila entre cero y :math:`4I_{0}` con una frecuencia :math:`f_b` llamada frecuencia de batidos igual a

.. math::
   :label: Ec:Beats_7

   \begin{equation}\label{Ec:Beats_7}
    f_b=|f_A-f_B|
   \end{equation}

La :numref:`fig:Beats_beatsfig1` muestra la gráfica de la variación de la intensidad de la señal resultante en función del tiempo.


.. figure:: /images/Oscilaciones_Termo/Beats/beatsfig11.png
   :scale: 60
   :align: center
   :name: fig:Beats_beatsfig1

   Intensidad relativa (:math:`\frac{I}{I_0}`) de la superposición de dos ondas armónicas de igual amplitud y frecuencias :math:`f_A` y :math:`f_B`  que se propagan en la misma dirección, en un punto :math:`x_0` en función del tiempo



**Descripción de la interfaz de la aplicación**

Para la generación de las señales sonoras utilizaremos la aplicación cuyo enlace se cita arriba en la sección de Recursos y cuya interfaz se muestra en la :numref:`fig:Beats_setup_00`.

.. figure:: /images/Oscilaciones_Termo/Beats/Beats_setup_00.png
   :scale: 80
   :align: center
   :name: fig:Beats_setup_00

   Interfaz gráfica del usuario para estudiar las pulsaciones o batidos

La aplicación permite seleccionar las frecuencias :math:`f_A` y :math:`f_B` de las dos ondas armónicas en el rango de 0 a 1000 Hz. Para ello simplemente digite sus valores en cada una de las casillas de entrada ubicadas en la parte superior de la consola. La amplitud :math:`\varepsilon_0` de las ondas se fija mediante la barra deslizante rotulada \textbf{balance} ubicada en la parte inferior izquierda de la consola. La diferencia de fase entre las ondas se fija mediante la barra deslizante rotulada \textbf{delay} ubicada en la parte inferior derecha de la consola. La escala horizontal del tiempo se fija con el menú desplegable rotulado \textbf{scope :math:`\Delta t`} ubicado en la parte inferior central de la consola. La forma de las ondas y su resultante (suma) se pueden observar en la gráfica de amplitud en función del tiempo al seleccionar las opciones :math:`f_A` , :math:`f_B` y sum. Las ondas de frecuencias :math:`f_A` y :math:`f_B` se muestran en color rojo y verde respectivamente mientras que la onda resultante se muestra en color azul.


**Mediciones y procedimientos**

   #. Configure el sistema tal como se muestra en la :numref:`fig:Beats_setup_01`. Presione el icono de sonido para escuchar las pulsaciones sonoras.  Analice los casos para las frecuencias que se indican en la :numref:`tab:Beats_Pulse`.

      .. figure:: /images/Oscilaciones_Termo/Beats/Beats_setup_01.png
         :scale: 90
         :align: center
         :name: fig:Beats_setup_01

         Configuración para estudiar las pulsaciones o batidos


   #. Mida la frecuencia de las pulsaciones que escucha en cada caso (recuerde que :math:`f=\frac{1}{T}`) y compárelas con las que predice la ecuación :eq:`Ec:Beats_7`. ¿Qué relación existe entre la curva de la señal resultante mostrada en la aplicación con la gráfica mostrada en la :numref:`fig:Beats_beatsfig1` ? Reporte el resultado de sus discusiones.


   .. csv-table::  Datos para determinar la frecuencia de las pulsaciones
         :header: ":math:`f_{A}` (Hz)", ":math:`f_{B}` (Hz)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Beats_Pulse
         :align: center

         300 , 300.1
         400 , 400.3
         400 , 400.1
         400 , 401.0
         800 , 800.1
         800 , 800.05

   #. Si la superposición de ondas con frecuencias similares se realizara con ondas electromagnéticas pertenecientes al espectro visible, ¿qué se observaría? ¿qué posible aplicación tendría la situación planteada?
   #. Discuta sus resultados y escriba sus conclusiones.

