Choques en una dimensión
==========================

**Objetivo**
El propósito de esta práctica es estudiar la conservación de la cantidad de movimiento lineal y la energía.


**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://ophysics.com/e2.html <https://ophysics.com/e2.html>`_.


**Resumen teórico**

Cuando dos o más cuerpos chocan entre sí, el momentum total del sistema se conserva sin importar el tipo de choque siempre y cuando el sistema se
encuentre aislado. Existen varios tipos de choques: elásticos, inelásticos y  completamente inelásticos. En un choque elástico tanto la
energía cinética como el momentum del sistema permanecen constantes. En un choque inelástico o completamente inelástico solo el momentum del sistema
permanece constante. La mayoría de los choques que suceden en la naturaleza son inelásticos. Un choque es completamente inelástico cuando
los cuerpos quedan pegados después del choque.
Para el choque en una dimensión de la :numref:`fig:Collis-1D_cmefig1`, la conservación del momentum y la energía se escriben como:

.. figure:: /images/Mecanica/Choques_1D/cmefig1.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Collis-1D_cmefig1

   Choque elástico


.. math::
   :label: Ec:Collision_1

   \begin{equation}
        m_{1}v_{1}+m_{2}v_{2}=m_{1}v_{1}^{\prime }+m_{2}v_{2}^{\prime }
    \end{equation}


.. math::
   :label: Ec:Collision_2

   \begin{equation}
        \frac{1}{2}m_{1}v_{1}^{2}+\frac{1}{2}m_{2}v_{2}^{2}=\frac{1}{2}m_{1}v_{1}^{\prime 2}+\frac{1}{2}m_{2}v_{2}^{\prime 2}  +Q
    \end{equation}

donde :math:`v_{1}`, :math:`v_{1}^{\prime}` y :math:`v_{2}`, :math:`v_{2}^{\prime}` representan las velocidades iniciales y finales de los cuerpos con masas :math:`m_{1}` y :math:`m_{2}` respectivamente. :math:`Q` representa la energía cinética ganada o perdida en el choque, de tal manera que si:

.. math::
   \begin{eqnarray*}
        Q &=& 0,\,\text{Colisión elástica} \\
        Q &>& 0,\,\text{Colisión inelástica} \\
        Q &<& 0,\,\text{Colisión super elástica}
   \end{eqnarray*}

Como los choques ocurren en una dimensión (eje :math:`x`), por simplicidad se omite la notación vectorial. El signo de :math:`v` denota la dirección, si :math:`v` es positiva entonces
su dirección es :math:`+x` y si :math:`v` negativa su dirección es :math:`-x`.


Si el choque es elástico (:math:`Q = 0`) y se conocen las masas y las velocidades iniciales, al combinar las ecuaciones :eq:`Ec:Collision_1`, :eq:`Ec:Collision_2`  y resolver para :math:`v_{1}^{\prime }`, :math:`v_{2}^{\prime }` resulta

.. math::
   :label: Ec:Collision_25

   \begin{equation}
    v_{1}^{\prime } =\frac{(m_{1}-m_{2})v_{1}+2m_{2}v_{2}}{m_{1}+m_{2}}
   \end{equation}

.. math::
   :label: Ec:Collision_26

   \begin{equation}
     v_{2}^{\prime }=\frac{(m_{2}-m_{1})v_{2}+2m_{1}v_{1}}{m_{1}+m_{2}}
   \end{equation}

Para un choque completamente inelástico (ver :numref:`fig:Collis-1D_cmefig2`) la conservación del momentum y la energía son

.. figure:: /images/Mecanica/Choques_1D/cmefig2.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Collis-1D_cmefig2

   Choque inelástico

.. math::
   :label: Ec:Collision_3

    \begin{equation}
     m_{1}v_{1}+m_{2}v_{2}=(m_{1}+m_{2})V
    \end{equation}

.. math::
   :label: Ec:Collision_4

   \begin{equation}
   \frac{1}{2}m_{1}v_{1}^{2}+\frac{1}{2}m_{2}v_{2}^{2}=\frac{1}{2}%
    (m_{1}+m_{2})V^{2}+Q
   \end{equation}

donde :math:`v_{1}` y :math:`v_{2}`  representan las velocidades iniciales de los cuerpos con masas :math:`m_{1}\ `y :math:`m_{2}` antes del choque y :math:`V` es la
velocidad del cuerpo de masa total  :math:`m_{1}+m_{2}` después del choque. :math:`Q` es la energía que se gasta para deformar los objetos y que se pierde en forma de calor. Al solucionar :math:`Q` de las expresiones :eq:`Ec:Collision_3` y :eq:`Ec:Collision_4` resulta

.. math::
   :label: Ec:Collision_5

   \begin{equation}
   Q= \frac{1}{2}m_{1}m_{2}\frac{\left( v_{1}-v_{2}\right) ^{2}}{m_{1}+m_{2}}
   \end{equation}

**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:Collis-1D_cmefig1` y asumamos que los
cuerpos de masas :math:`m_{1}` y :math:`m_{2}` tienen velocidades :math:`v_{1}=v` y :math:`v_{2}=0` antes
del choque. Si la colisión es elástica, las ecuaciones :eq:`Ec:Collision_25` y :eq:`Ec:Collision_26` se reducen a:

.. math::
   :label: Ec:Collision_55

   \begin{equation}
    v_{1}^{\prime } =\frac{(m_{1}-m_{2})v}{m_{1}+m_{2}} =u_1v
   \end{equation}

.. math::
   :label: Ec:Collision_56

   \begin{equation}
      v_{2}^{\prime } =\frac{2m_{1}v}{m_{1}+m_{2}}=u_2v
   \end{equation}

donde :math:`u_{1}=\frac{(m_{1}-m_{2})}{m_{1}+m_{2}}` y :math:`u_{2}=\frac{2m_{1}}{m_{1}+m_{2}}` respectivamente.
Si el choque es completamente inelástico, las ecuaciones  :eq:`Ec:Collision_3` y :eq:`Ec:Collision_5`  se reducen a:

.. math::
   :label: Ec:Collision_58

   \begin{equation}
     V=\frac{m_1v}{m_1+m_2}=u_3v
   \end{equation}

donde :math:`u_3=\frac{m_1}{m_1+m_2}`

.. math::
   :label: Ec:Collision_6

   \begin{equation}
     Q=\frac{1}{2}m_{1}m_{2}\frac{v^{2}}{m_{1}+m_{2}}
   \end{equation}

Note que al verificar la dependencia \emph{lineal} entre :math:`v_{1}^{\prime }` y :math:`v`; :math:`v_{2}^{\prime }` y :math:`v`; y :math:`V` y :math:`v` hemos comprobado la conservación del momentum y la energía. ?`Por qué?

**Descripción de la interfaz de la aplicación**

La :numref:`Collisions-1D-Gui-01` muestra la interfaz gráfica del usuario que permite estudiar la conservación de la
cantidad de movimiento lineal y la conservación de la energía. Desde la interfaz se pueden seleccionar las velocidades iniciales
y los valores de las masas de los cuerpos que interactúan a través de la barras deslizables de colores rojo y azul
rotuladas *Initial velocity of red box*, *mass of red box* y *Initial velocity of blue box*, *mass of blue box* respectivamente.
Mediante la barra de desplazamiento rotulada *elasticity* se selecciona el tipo de colisión: 1 elástica, 0 totalmente inelástica y
:math:`(0-1)` inelástica. Una vez que ocurre la colisión, la aplicación muestra de manera numérica tanto la energía cinética
:math:`KE` y cantidad de movimiento :math:`p` inicial y final para cada cuerpo. Las gráficas muestran las velocidades y cantidad
de movimiento lineal de cada cuerpo y del centro de masa en función del tiempo. De igual manera de despliega la posición
y centro de masa (COM) de los dos cuerpos. Los botones *Run*, *Pause* y *Set* permiten iniciar, pausar y comenzar
de nuevo la animación respectivamente.


.. figure:: /images/Mecanica/Choques_1D/Gui-Collisions-1D.png
   :alt:
   :scale: 50
   :align: center
   :name: Collisions-1D-Gui-01

   Interfaz gráfica del usuario.


**Mediciones y procedimientos**

**Colisión elástica**

   #. Fije valores de masas, ajuste la velocidad inicial de la masa 2 (:math:`v_2`) en 0 y valor de la elasticidad en 1. Para diferentes valores de la velocidad inicial de la masa 1 (:math:`v`), registre las correspondientes velocidades finales y complete la :numref:`tab:Collis-1D_01`.

      .. csv-table:: Datos colisión eelástica
         :header: ":math:`v` (m/s)", ":math:`v_1^{'}` (m/s)", ":math:`v_2^{'}` (m/s)"
         :widths: 1,1,1
         :width: 12 cm
         :name: tab:Collis-1D_01
         :align: center

         .,.,
         .,.,
         .,.,
         .,.,
         .,.,
         .,.,
         .,.,
         .,.,
         .,.,
         .,.,


   #. Elabore las gráficas de :math:`v_1'` vs :math:`v`, :math:`v_2'` vs :math:`v` para comprobar la linealidad de las ecuaciones :eq:`Ec:Collision_55` y :eq:`Ec:Collision_56` mediante el análisis estadístico de los datos. Nota: para esto considere a :math:`v` como la variable independiente y las pendientes, en cada caso, estarán relacionadas con los valores :math:`u_1` y :math:`u_2`, que se deben utilizar para comparar resultados.


**Colisión completamente inelástica**

   #. Fije valores de masas, ajuste la velocidad inicial de la masa 2 (:math:`v_2`) en 0 y valor de la elasticidad en 0. Para diferentes valores de la velocidad inicial de la masa 1 (:math:`v`), registre la correspondiente velocidad final :math:`V` y complete la  :numref:`tab:Collis-1D_02`.

      .. csv-table:: Datos colisión inelástica
         :header: ":math:`v` (m/s)", ":math:`V` (m/s)"
         :widths: 1,1
         :width: 10 cm
         :name: tab:Collis-1D_02
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

   #. Elabore la gráfica de :math:`V` vs :math:`v` para comprobar la linealidad de la ecuación :eq:`Ec:Collision_58`, mediante el análisis estadístico de los datos. Compare el valor de la pendiente con el resultado de calcular :math:`u_3`.


**Análisis y preguntas**

   #. Establezca las posibles limitaciones del fenómeno estudiado a través de la simulación.
   #. Discuta con sus compañeros acerca de la energía perdida en el segundo experimento, para cada valor de velocidad inicial :math:`v`. ¿Es posible cuantificarla? De ser así, ¿cuál es su valor?
   #. Averigüe que es una colisión super elástica y utilice el simulador para revisar su comportamiento. Identifique al menos dos casos de este tipo de colisión.
   #. Para colisiones el\'asticas en una dimensi\'on y haciendo uso del simulador, revise los siguientes casos: a) Masas iguales, b) :math:`m_1 \gg m_2` y c) :math:`m_1 \ll m_2`. Encuentre ejemplos cotidianos donde sea posible estos casos especiales.


   #. ¿Qué significa un :math:`Q` grande?
   #. ¿Qué tipo de colisi\'on ocurre cuando un asteroide choca con un planeta?
   #. Consulte qué es el CERN y qué tipos de experimento hacen.
   #. Enumere al menos dos tipos de colisiones el\'asticas.
   #. Idee un experimento mecánico simple que permita medir la velocidad de un bal\'on de fútbol.



