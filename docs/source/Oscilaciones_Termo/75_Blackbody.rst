Radiación del cuerpo negro: Ley de radiación de Planck
=======================================================

**Objetivo**

El propósito de esta práctica es estudiar la ley de radiación de Planck, sus implicaciones (ley de Wien y ley de Stefan) y aplicaciones.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_en.html <https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_en.html>`_.

**Resumen teórico**

Todo cuerpo a temperatura absoluta diferente de cero emite radiación y el tipo de radiación depende de su temperatura. Por otra parte, se sabe que la cantidad de energía radiada por una superficie a una longitud de onda dada depende del material del cuerpo y del estado de su superficie, así como de la temperatura de la superficie. Por lo tanto, varios materiales emiten diferentes cantidades de energía radiante incluso cuando están a la misma temperatura. Se denomina cuerpo negro a un cuerpo físico ideal que posee la característica de que toda la radiación que incide sobre éste (independiente de la frecuencia y ángulo de incidencia) es absorbida y a su vez reemitida completamente. Así, un cuerpo negro tiene absortividad 1 y emisividad igual a 1 (máximos valores posibles). En la práctica, todo cuerpo posee valores de absortividad y emisividad menores que 1. El problema de la determinación de la distribución de la intensidad :math:`I ` de la radiación (potencia por unidad de área y por unidad de longitud de onda) emitida  por un cuerpo negro a temperatura :math:`T` fue solucionado por Planck en 1900 y establece que

.. math::
   :label: Ec:Blackbody_01

   \begin{equation}
     I(\lambda,T)= \frac{2\pi h c^{2}}{\lambda ^{5}}\frac{1}{e^{\frac{hc}{\lambda kT}}-1}
   \end{equation}


donde :math:`k=1.38\times 10^{-23}\,\text{J/K}` es la contante de Boltzmann, :math:`c=3\times10^{8}\,\text{m/s}` es la velocidad de la luz.


**Descripción de la interfaz de la aplicación**


La :numref:`fig:gui_01_blackbody` muestra la interfaz gráfica del usuario que permite estudiar la ley de Planck. La interfaz permite seleccionar la temperatura del cuerpo negro al desplazar el cursor azul cerca al termómetro en el rango de temperaturas comprendido entre 3000 a 11000 K. Para cada valor de temperatura aparece la gráfica de distribución de intensidad de la radiación (**Spectral Power Density**) emitida. Sobre la gráfica aparecen los tres tipos de radiación emitida: ultravioleta, visible e infrarrojo al seleccionar la opción **Labels**. Al seleccionar la opción **Graph Values** se es posible leer con precisión el valor de la longitud de onda y la correspondiente intensidad para cada punto de la curva. La estrella mostrada en la parte superior de la interfaz toma un color diferente que depende del valor de la temperatura. Al seleccionar la opción **Intensity** aparece el valor del área bajo la curva de la distribución de la intensidad desde :math:`\lambda=0` hasta :math:`\lambda=\infty`, nótese que las unidades de esta área son :math:`\text{W/m}^{2}` que corresponde a la potencia total  por unidad de área emitida por el cuerpo para todas las longitudes de onda.

.. figure:: /images/Oscilaciones_Termo/Blackbody/Blackbody_gui_01.png
   :scale: 45
   :align: center
   :name: fig:gui_01_blackbody

   Interfaz gráfica del usuario


**Mediciones y procedimientos**

   #. Varíe la temperatura del cuerpo negro desde las temperaturas más bajas hasta las temperaturas mas altas. Describa el comportamiento del color de los cuerpos cuando la temperatura cambia. A la luz de sus observaciones explique la razón por la cual cuando un herrero trabaja el hierro y lo calienta este adquiere diferentes colores.
   #. ¿Por qué el cuerpo humano no lo podemos ver sin la ayuda de ningún instrumento en la oscuridad?
   #. Varíe la temperatura y registre los correspondientes valores de la longitud de onda :math:`\lambda` para la cual la intensidad toma el máximo valor y el valor del área bajo la curva. Registre sus datos en la :numref:`tab:Blackbody_01`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`\lambda` y :math:`T`, :math:`A` y :math:`T`; y demuestre que

      .. math::
         :label: Ec:Blackbody_02

         \begin{equation}
           \lambda =\frac{2.899\times10^{-3}\,m\cdot\text{K}}{T}
         \end{equation}

      .. math::
         :label: Ec:Blackbody_03

         \begin{equation}
            A=\sigma T^{4}
         \end{equation}


      donde :math:`\sigma=5.675\,\text{W}\cdot\text{m}^{-2}\cdot\text{K}^{-4}`. Estas relaciones reciben el nombre de ley de Wien y ley de Stefan respectivamente.

   #. ¿Cómo se determinaría la temperatura de una estrella lejana a partir de los resultados anteriores? Suministre un ejemplo.
   #. ¿Qué tiene que ver la ley de Wien y Stefan con la ley de Planck?

      .. csv-table:: Datos de la radiación del cuerpo negro para diferentes temperaturas
         :header: "Temperatura, :math:`T` (K)", "Longitud de onda, :math:`\\lambda,\\,(\\mu m)`","Area bajo la curva, :math:`A\\,(\\text{W/m}^2)`"
         :widths: 1,1,1
         :width: 15 cm
         :name: tab:Blackbody_01
         :align: center

         3000,
         3500,
         4000,
         4500,
         5000,
         5500,
         6000,
         6500,
         7000,
         7500,
         8000,
         8500,
         9000,
         9500,
         10000,
         10500,
         11000,

   #. La :numref:`fig:Blackbody_spect-dens` muestra la distribución de intensidad para cierto cuerpo estelar. Realice el mejor estimativo de su temperatura si se asume que este se comporta como un cuerpo negro.

      .. figure:: /images/Oscilaciones_Termo/Blackbody/spectral-density.png
         :scale: 85
         :align: center
         :name: fig:Blackbody_spect-dens

         Distribución de intensidad para cierto cuerpo estelar

