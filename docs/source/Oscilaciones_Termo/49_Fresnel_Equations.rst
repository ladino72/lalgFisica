Ecuaciones de Fresnel
=======================

**Objetivo**

El propósito de esta práctica es determinar la dirección de polarización de una onda a partir de mediciones y las ecuaciones de Fresnel.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html <https://phet.colorado.edu/sims/html/bending-light/latest/bending-light_en.html>`_. *Bending Light: More Tools*

**Resumen teórico**

Las ecuaciones de Fresnel son un conjunto de relaciones matemáticas que relacionan las amplitudes de las ondas reflejadas y refractadas (o transmitidas) en función de la amplitud de la onda incidente [#f1]_, [#f2]_.
Cuando una onda electromagnética que se desplaza por un medio con índice de refracción :math:`n_1`, incide sobre la interfaz con otro medio que posee un índice de refracción :math:`n_2`, una parte de la onda se refleja y otra porción se transmite al otro medio, ver :numref:`fig:Fresnel_01`.  Dicho esto mismo en términos energéticos, si la intensidad de la onda incidente la asumimos como 100%, entonces :math:`T+R = 100\%`, donde :math:`T` y :math:`R` representan los porcentajes de las intensidades de las ondas refractadas y reflejadas. Se suele llamar a estos porcentajes los coeficientes de transmisión y reflexión respectivamente.

.. figure:: /images/Oscilaciones_Termo/Fresnel_Equations/Fresnel_01.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Fresnel_01

   Rayos incidente, reflejado y refractado (transmitido).

El cálculo de :math:`T` y :math:`R` depende de la polarización de la onda incidente, es decir, depende de la dirección del campo eléctrico. En general, el campo eléctrico de la onda electromagnética incidente se puede descomponer en dos componentes: una componente paralela :math:`E_{\parallel}` y otra perpendicular :math:`E_{\bot}` al plano de incidencia.

.. figure:: /images/Oscilaciones_Termo/Fresnel_Equations/Fresnel_02n.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:Fresnel_02

   :math:`E_{r\,\bot}`, :math:`E_{r\,\parallel}` representan las componentes reflejadas de :math:`\vec{E}`, y :math:`E_{t\,\bot}`, :math:`E_{t\,\parallel}` representan las componentes refractadas de :math:`\vec{E}` perpendiculares y paralelas al plano de incidencia.


A partir de las ecuaciones de Fresnel se puede demostrar que los coeficientes de refracción y reflexión para las componentes paralelas y perpendiculares son diferentes.  Los valores de estos coeficientes en términos del ángulo de incidencia :math:`\theta_i` vienen dados por las siguientes expresiones:

.. math::
   :label: Ec:Fresnel_01

   \begin{equation}
    R_{\bot}=R_s=\Bigg|\frac{n_1\cos(\theta_i)-n_2\sqrt{1-\Big(\frac{n_1}{n_2}\sin(\theta_i)\Big)^2}}{ n_1\cos(\theta_i)+n_2\sqrt{1-\Big(\frac{n_1}{n_2}\sin(\theta_i)\Big)^2}} \Bigg|^2
   \end{equation}

.. math::
   :label: Ec:Fresnel_02

   \begin{equation}
    R_{ \parallel} =R_p=\Bigg|\frac{ n_1\sqrt{1-\Big(\frac{n_1}{n_2}\sin(\theta_i)\Big)^2}-n_2\cos(\theta_i) }{ n_1\sqrt{1-\Big(\frac{n_1}{n_2}\sin(\theta_i)\Big)^2}+n_2\cos(\theta_i) }\Bigg|^2
   \end{equation}

.. math::
   :label: Ec:Fresnel_03

   \begin{equation}
    T_{\bot} =T_s=1-R_{\bot}
   \end{equation}

.. math::
   :label: Ec:Fresnel_04

   \begin{equation}
    T_{\parallel} =T_p=1-R_{\parallel}
   \end{equation}


Es de anotar que las anteriores ecuaciones se dedujeron con el supuesto que la ley de Snell se satisface, es decir,

.. math::
   :label: Ec:Fresnel_05

   \begin{equation}
    n_1\sin(\theta_i)=n_2\sin(\theta_t)
   \end{equation}


**Montaje experimental**

La :numref:`fig:Fresnel_Setup_01` muestra la interfaz del usuario que permite la toma de datos para la determinación de la polarización de la onda incidente. En la parte superior izquierda se puede seleccionar la longitud de onda de la luz emitida por la fuente de luz al desplazar el botón de color rojo. El rango de longitudes de onda va desde 380 a 700 nm, que corresponde al visible.  El ángulo de incidencia del rayo de luz con respecto a la normal se puede variar al girar la fuente de luz.  En la interfaz también se encuentran un medidor de intensidad de la luz, uno de velocidad, un transportador (uno digital y otro mecánico) y un osciloscopio rudimentario. Además, en la parte derecha central se dispone de dos cajas consolas idénticas, con un par de botones que permiten seleccionar el tipo de material y el correspondiente índice de refracción. En esta práctica solo utilizaremos el medidor de intensidad de luz y el transportador digital.

.. figure:: /images/Oscilaciones_Termo/Fresnel_Equations/Fresnel_Setup_01.png
   :alt:
   :scale: 110
   :align: center
   :name: fig:Fresnel_Setup_01

   Interfaz gráfica del usuario.



**Mediciones y procedimientos**

.. _aire_vidrio:

**Paso de la luz del aire a vidrio**


   #. Encienda la fuente de luz laser.
   #. Coloque el medidor de intensidad de luz tal como indica la :numref:`fig:Fresnel_Setup_02`, de esta manera se medirá el coeficiente de reflexión cuando el haz de luz pasa del aire (:math:`n_1=1`) al vidrio (:math:`n_2=1.5`).

      .. figure:: /images/Oscilaciones_Termo/Fresnel_Equations/Fresnel_Setup_02.png
         :alt:
         :scale: 35
         :align: center
         :name: fig:Fresnel_Setup_02

         El haz de luz pasa del aire al vidrio reflejándose y refractándose.

   #. Incremente :math:`\theta` en intervalos de :math:`5\,^o` partiendo desde :math:`5\,^o` y registre  en  cada paso la Intensidad reflejada :math:`R`, que proporciona el simulador en forma porcentual en la :numref:`tab:Reflectance_01`.

      .. csv-table:: Datos medidos de :math:`\theta_i` e Intensidad reflejada :math:`R`
         :header: "Angulo, :math:`\\theta_i\\,(^o)`", ":math:`R` \\%",":math:`\\frac{R}{100}`"
         :widths: 1,1,1
         :width: 10 cm
         :name: tab:Reflectance_01
         :align: center

         5,.,.
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

   #. Realice una gráfica de :math:`\frac{R}{100}` en función de :math:`\theta_i` con los datos de la :numref:`tab:Reflectance_01`.
   #. Para los mismos valores de ángulos de la tabla :numref:`tab:Reflectance_01`, a la anterior gráfica superponga las gráficas de las funciones dadas por las ecuaciones :eq:`Ec:Fresnel_01` y :eq:`Ec:Fresnel_02`.
   #. Para los mismos valores de ángulos de la tabla :numref:`tab:Reflectance_01` realice la gráfica de la función dada por la ecuación :eq:`Ec:Fresnel_03`.


.. _vidrio_aire:

**Paso de la luz del vidrio al aire**

   #. Encienda la fuente de luz laser.
   #. Coloque el medidor de intensidad de luz tal como indica la :numref:`fig:Fresnel_Setup_03`, de esta manera se medirá el coeficiente de reflexión cuando el haz de luz pasa del vidrio (:math:`n_2=1.5`) al aire (:math:`n_1=1`).

      .. figure:: /images/Oscilaciones_Termo/Fresnel_Equations/Fresnel_Setup_03.png
         :alt:
         :scale: 35
         :align: center
         :name: fig:Fresnel_Setup_03

         El haz de luz pasa del vidrio  al aire  reflejándose y refractándose.

   #. Incremente :math:`\theta` en intervalos de :math:`5\,^o` partiendo desde :math:`5\,^o` y registre  en  cada paso la Intensidad reflejada :math:`R`, que proporciona el simulador en forma porcentual en la :numref:`tab:Reflectance_02`.

      .. csv-table:: Datos medidos de :math:`\theta_i` e Intensidad reflejada :math:`R`
         :header: "Angulo, :math:`\\theta_i\\,(^o)`", ":math:`R` \\%",":math:`\\frac{R}{100}`"
         :widths: 1,1,1
         :width: 10 cm
         :name: tab:Reflectance_02
         :align: center

         5,.,.
         10,.,.
         15,.,.
         20,.,.
         25,.,.
         30,.,.
         35,.,.
         40,.,.
         :math:`\vdots`, :math:`\vdots`, :math:`\vdots`


   #. Realice una gráfica de :math:`\frac{R}{100}` en función de :math:`\theta_i` con los datos de la :numref:`tab:Reflectance_02`.
   #. Para los mismos valores de ángulos de la tabla :numref:`tab:Reflectance_02`, a la anterior gráfica superponga las gráficas de las funciones dadas por las ecuaciones :eq:`Ec:Fresnel_01` y :eq:`Ec:Fresnel_02`.
   #. Para los mismos valores de ángulos de la tabla :numref:`tab:Reflectance_02` realice la gráfica de la función dada por la ecuación :eq:`Ec:Fresnel_03`.
   #. Mida el valor de la intensidad refractada para :math:`\theta_i=0`.

**Análisis y Preguntas**

   #. Basado en las gráficas realizadas en el inciso :ref:`Paso de luz del aire al vidrio <aire_vidrio>`, ¿qué puede concluir acerca del estado de polzarización del haz de luz utilizado en la simulación?
   #. Basado en las gráficas realizadas en el inciso :ref:`Paso de luz del vidrio al aire <vidrio_aire>`, ¿qué puede concluir acerca del estado de polzarización del haz de luz utilizado en la simulación?
   #. Para el caso del paso de luz del vidrio al aire, verifique que el punto de corte de la gráfica :math:`T_s` en función de :math:`\theta_i` con el eje horizontal coincide con el ángulo crítico, es decir, el valor del ángulo de incidencia para el cual se obtiene reflexión total interna y que su valor es :math:`\theta_c=\sin^{-1}\Big(\frac{1}{n_2}\Big)=\sin^{-1}\Big(\frac{1}{1.5}\Big)=48.2^o`.
   #. Verifique que para incidencia perpendicular del haz de luz, es decir :math:`\theta_i=0`, se cumple que :math:`R_s=\Big(\frac{n_1-n_2}{n_1+n_2}\Big)^2=0.04` y :math:`T_s=\Big(\frac{4n_1n_2}{n_1+n_2} \Big)^2=5.76`. Compare estos valores con los medidos con el simulador.
   #. ¿Qué aplicaciones tiene la reflexión interna en el principio de funcionamiento de la fibra óptica?
   #. ¿Qué aplicaciones tiene el saber la polarización de la luz?

.. [#f1] Jenkins F.A., White H.E., (1950) *Fundamentals of Optics*, McGraw-Hill, Nueva York
.. [#f2] ‎Eugene Hecht, *Optics*, Addison-Wesley; 4a edición (1 Agosto 2001)