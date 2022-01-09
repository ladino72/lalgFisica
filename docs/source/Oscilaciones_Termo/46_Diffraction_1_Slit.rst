+Difracción de la luz
=====================

**Objetivo**

El propósito de esta práctica es estudiar el patrón de difracción producido por una rendija.


**Recursos**

   #. Simulaciones disponibles en:

      `https://www.walter-fendt.de/html5/phen/singleslit_en.htm <https://www.walter-fendt.de/html5/phen/singleslit_en.htm>`_.

      `https://demonstrations.wolfram.com/MultipleSlitDiffractionPattern/ <https://demonstrations.wolfram.com/MultipleSlitDiffractionPattern/>`_.

**Resumen teórico**

Interferencia y difracción son fenómenos característicos de todas las ondas, tanto mecánicas como electromagnéticas. Interferencia se refiere al fenómeno donde dos o más de la misma naturaleza se superponen para producir una onda resultante de mayor, menor, o la misma amplitud. La interferencia es utilizada en muchas aplicaciones técnicas, como por ejemplo en la medición precisa de longitudes (espesores), en la protección de anteojos, en la obtención de aviones ``invisibles``, en la recepción de señales provenientes de estrellas, etc. La difracción tiene lugar cuando las ondas inciden interaccionan con objetos de dimensiones del mismo orden de magnitud que la longitud de onda de la onda incidente. Así, cuando luz visible incide por la izquierda sobre un objeto pequeño se produce un patrón de difracción sobre una pantalla colocada a la derecha de éste. El patrón de difracción consiste de una serie de franjas brillantes u oscuras y las particularidades de este patrón dependen de la geometría del objeto y las distancias entre la fuente y pantalla al objeto. Cuando la pantalla se encuentra a una distancia corta del objeto se tiene difracción de Fresnel y cuando la distancia entre el objeto y la pantalla es grande se tiene difracción de Fraunhofer. La distinción surge debido a que no solo las aproximaciones que se hacen en cada uno de los casos son diferentes sino a que los cálculos se hacen más complicados en el caso de la difracción de Fresnel.
El principio de Babinet establece que una abertura y un obstáculo, de la misma forma geométrica y las mismas dimensiones e igualmente iluminados, producen el mismo patrón de difracción.\newline Para el caso cuando luz de longitud de onda :math:`\lambda` e intensidad :math:`I_0` incide sobre un arreglo de :math:`N` rendijas idénticas rectangulares de ancho :math:`d` y distancia de separación :math:`b`, (:numref:`fig:Interf_dpfig20`), la intensidad del patrón de difracción sobre una pantalla ubicada a la derecha del arreglo está dado por

.. math::
   :label: Ec:Diff-01

   \begin{equation}
    I(\alpha)=I_0\Bigg(\frac{\sin\frac{1}{2}N\phi}{\sin\frac{1}{2}\phi}\Bigg)^{2}\Big(\frac{\sin u}{u}\Big)^{2}
   \end{equation}

donde :math:`\phi=\frac{2\pi}{\lambda}d\sin\alpha` y :math:`u=\frac{\pi}{\lambda}b\sin\alpha` y :math:`\alpha` es la posición angular del punto donde se quiere medir la intensidad.


.. figure:: /images/Oscilaciones_Termo/Diffraction_1_Slit/Diffaction_01.png
   :scale: 85
   :align: center
   :name: fig:Interf_dpfig20

   Frente de onda incidiendo sobre un arreglo de :math:`N` rejillas rectangulares idénticas de ancho :math:`d` y distancia de separación :math:`b`.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Diff_01` muestra la interfaz gráfica del usuario que permite estudiar la difracción de la luz por una rendija. Esta permite seleccionar la longitud de onda :math:`\lambda` de la luz incidente y el ancho de la rendija mediante las barras deslizables rotuladas como **Wavelength** y **Width of slit** ubicadas en la parte superior derecha de la interfaz. La forma del patrón de difracción recogido en la pantalla y la intensidad relativa del mismo se observa al seleccionar las opciones rotuladas como **Diffraction pattern** e **Intensity profile** respectivamente. Las posiciones angulares de los máximos y mínimos del patrón de intensidad se pueden leer y visualizar con las opciones rotuladas como **Maxima** y **Minima** respectivamente. La intensidad relativa del patrón de difracción para un ángulo determinado se puede leer y visualizar mediante la barra de desplazamiento rotulada como **Angle**.

.. figure:: /images/Oscilaciones_Termo/Diffraction_1_Slit/Diff_Gui_01.png
   :scale: 65
   :align: center
   :name: fig:Diff_01

   Interfaz gráfica del usuario para estudiar la difracción de la luz por una rendija.


**Mediciones y procedimientos**

**Máximos**

   #. Fije el valor de la longitud de onda, al igual que el ancho de la rendija, los valores que desee. Tome mediciones de posiciones angulares y verifique que los máximos de la intensidad relativa satisfacen la relación :math:`b\sin\alpha\approx(k+\frac{1}{2})\lambda`, donde :math:`k=1,2,3...`
   #. Verifique que la intensidad relativa siempre es maxima para :math:`\alpha=0` independiente de los valores de :math:`\lambda` y :math:`b`.

**Mínimos**

   #. Fije el valor de la longitud de onda, al igual que el ancho de la rendija, los valores que desee. Tome mediciones de posiciones angulares y verifique que los mínimos de la intensidad relativa satisfacen la relación :math:`b\sin\alpha=k\lambda`, donde :math:`k=1,2,3...`.

**Ancho rendija** :math:`b` constante

   #. Fije ancho de la rendija. ¿Cuál es el efecto en la forma del patrón de difracción al variar la longitud de onda?

**Longitud de onda** :math:`\lambda` constante

   #. Fije la longitud de onda. ¿Cuál es el efecto en la forma del patrón de difracción al variar el ancho de la rendija?

**Múltiple rendijas**

   #. Examine el efecto en la forma del patrón de difracción cuando la luz incide sobre un arreglo de rendijas (1,2,3,4...) Para ello utilice la simulación disponible en el segundo link de la sección de Recursos.
   #. Demuestre que los máximos y mínimos del patrón de difracción están dados respectivamente por las expresiones :math:`d\sin\alpha=m\lambda`, donde :math:`m=0,1,2,3...` y :math:`b\sin\alpha=n\lambda`, donde :math:`n=1,2,3...`.

.. note::

   **Problema**

   Verifique que la respuesta al siguiente problema es la opción B).

   .. figure:: /images/Oscilaciones_Termo/Diffraction_1_Slit/Diff_Problem_01.png
      :scale: 70
      :align: center
      :name: fig:Interf_prob

      Ejercicio.

