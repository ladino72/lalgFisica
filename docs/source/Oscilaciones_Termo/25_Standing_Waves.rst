+Ondas estacionarias en una cuerda
=====================================

**Objetivo**

El propósito de esta práctica es estudiar las ondas estacionarias en una cuerda en dos casos: a) con ambos extremos fijos y b) un extremo fijo y el otro libre, mediante el uso de una simulación.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/wave-on-a-string/latest/wave-on-a-string_es.html <https://phet.colorado.edu/sims/html/wave-on-a-string/latest/wave-on-a-string_es.html>`_.


**Resumen teórico**

Las ondas estacionarias en una cuerda se forman como resultado de la superposición de dos ondas viajeras que tienen igual amplitud y frecuencia y que se propagan en direcciones opuestas, los extremos de la cuerda están fijos. Si se hace vibrar uno de los extremos de la cuerda de manera armónica y perpendicular a la cuerda, la perturbación se propaga en forma de onda armónica por ésta. Al llegar a los extremos fijos, la onda se refleja de forma que al final en la cuerda tendrá lugar la superposición de dos ondas que originan la onda estacionaria. Si tomamos el extremo izquierdo de la cuerda como origen de coordenadas, las ecuaciones que describen las ondas viajeras son

.. math::
   :label: sw_01

   \begin{equation}
     y_1(x,t) = A\cos(kx-\omega t)
   \end{equation}

.. math::
   :label: sw_02

   \begin{equation}
     y_2(x,t) = A\cos(kx+\omega t)
   \end{equation}


donde :math:`A` es la amplitud del movimiento armónico simple, :math:`f` es su frecuencia, :math:`k=\frac{2\pi}{\lambda}` y :math:`\omega=2\pi f`, :math:`\lambda` es la longitud de onda de las ondas. La relación entre :math:`k` y :math:`\omega` es :math:`\omega=kv`, la cual es equivalente a

.. math::
   :label: sw_03

   \begin{equation}
    v=\lambda f
   \end{equation}

.. math::
   :label: sw_04

   \begin{equation}
    v=\sqrt{\frac{T}{\rho}}
   \end{equation}

donde :math:`T` es la tensión a la cual se encuentra sometida la cuerda y :math:`\rho` es la masa por unidad de longitud de la misma. Al sumar las ecuaciones :eq:`sw_01` y :eq:`sw_02` resulta la onda cuya ecuación es

.. math::
   :label: sw_05

   \begin{equation}
     y(x,t)=2A\sin(\frac{2\pi}{\lambda}x)\cos(2\pi ft)
   \end{equation}

Al imponer en la ecuación :eq:`sw_05` que el extremo derecho de la cuerda también sea fijo, es decir, :math:`y(x=L,t)=0` se sigue que :math:`k=\frac{n\pi}{L}`, donde :math:`n=1,2,3,\ldots`. La anterior relación equivale a

.. math::
   :label: sw_06

   \begin{equation}
    \lambda_n = \frac{2L}{n}
   \end{equation}

o teniendo en cuenta la ecuaciones :eq:`sw_03` y :eq:`sw_04`

.. math::
   :label: sw_07

   \begin{equation}
    f_n=\frac{vn}{2L}=\frac{n}{2L}\sqrt{\frac{T}{\rho}}
   \end{equation}

Así, se presentan ondas estacionarias si se cumple la ecuación :eq:`sw_06` o la ecuación :eq:`sw_07`. La :numref:`set_modes_both_ends_fixed` muestra ondas estacionarias en una cuerda para valores de :math:`n=1,2,3,4,5,\text{y}\, 6`

.. figure:: /images/Oscilaciones_Termo/Standing_Waves/set_modes_both_ends_fixed.png
   :alt:
   :scale: 50
   :align: center
   :name: set_modes_both_ends_fixed

   Seis primeros modos normales en la cuerda para diferentes instantes de tiempo.


.. figure:: /images/Oscilaciones_Termo/Standing_Waves/set_modes_One_end_free.png
   :alt:
   :scale: 50
   :align: center
   :name: set_modes_One_end_free

   Seis primeros modos normales en la cuerda para diferentes instantes de tiempo.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:S_W_Setup_01` muestra la interfaz gráfica del usuario para estudiar las ondas estacionarias. Esta consta de una cuerda de longitud fija, la cual puede ser perturbada por su extremo libre de tres maneras diferentes: de manera manual, armónica y a través de pulsos. El extremo derecho se puede dejar fijo, libre o sin extremo. Cuando la cuerda se perturba de manera armónica el usuario puede fijar la amplitud de la perturbación, al igual que su frecuencia. De igual manera, se puede fijar la tensión de la cuerda y el rozamiento que actúa sobre ésta. Además, la interfaz ofrece dos herramientas clave para el desarrollo de la actividad como son la regla graduada y el cronómetro.

.. figure:: /images/Oscilaciones_Termo/Standing_Waves/SW_Setup_01.png
   :alt:
   :scale: 45
   :align: center
   :name: fig:S_W_Setup_01

   Interfaz gráfica del usuario para estudiar las ondas estacionarias.


**Mediciones y procedimientos**

**Cuerda con ambos extremos fijos**

   #. Fije la tensión de la cuerda al máximo y la amortiguación sobre la cuerda en cero. Para medir la velocidad de propagación de la onda en la cuerda envíe un pulso a lo largo de esta, mida el tiempo :math:`\Delta t` que tarda el pulso en recorrer una determinada distancia :math:`\Delta x`, ver :numref:`fig:S_W_Setup_02`. La velocidad :math:`v` de la cuerda es :math:`v=\frac{\Delta x}{\Delta t}`. Realice varias mediciones de manera sistemática y determine el mejor valor posible de :math:`v`, pues de su valor dependerán otras cantidades que utilizará en esta práctica. ¡Sacar un promedio no es una idea brillante!

      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/SW_Setup_02.png
         :alt:
         :scale: 45
         :align: center
         :name: fig:S_W_Setup_02

         Montaje para determinar la velocidad de propagación de la onda en la cuerda.

   #. Para observar en el simulador las ondas estacionarias en el modo fundamental (:math:`n=1`). Fije el simulador en la configuración mostrada en la :numref:`fig:S_W_Setup_03`. Nótese que se ha fijado una amplitud de oscilaciones pequeñas :math:`A=0.06\,\text{cm}` para observar mejor el fenómeno. El valor de la frecuencia XXXXX de la oscilación armónica lo debe calcular Usted a partir de la ecuación :eq:`sw_07`. La figura muestra la forma de la cuerda en el modo :math:`n=1`.

      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/SW_Setup_03.png
         :alt:
         :scale: 50
         :align: center
         :name: fig:S_W_Setup_03

         Montaje para determinar el modo fundamental (:math:`n=1`) de las ondas estacionarias.

   #. Determine los restantes modos de oscilación de la cuerda, compárelos con los de la :numref:`SW_Sixmodes` y complete la :numref:`freq_both_ends_fixed`.

      .. csv-table:: Frecuencias de los primeros siete modos de oscilación. Cuerda con ambos extremos fijos.
         :header: ":math:`n`", "Frecuencia, :math:`f` (Hz)"
         :widths: 1,1
         :width: 12 cm
         :name: freq_both_ends_fixed
         :align: center

         1,
         2,
         3,
         4,
         5,
         6,
         7,

      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/SixModes.png
         :alt:
         :scale: 30
         :align: center
         :name: SW_Sixmodes

         Seis primeros modos normales en la cuerda generados en el simulador de Phet.

   #. Demuestre que la energía total de los osciladores que forman la cuerda cuando esta presenta ondas estacionarias es :math:`E_t=\frac{1}{2}\rho LA^{2}\frac{n^{2}\pi^{2}v^{2}}{L^{2}}`. ¿Qué puede concluir acerca de la energía total de la cuerda con respecto al modo en que vibra?
   #. Si :math:`T_h`  y :math:`T_m` representan las tensiones máxima e intermedia de la cuerda, ver :numref:`fig:S_W_button` demuestre que :math:`T_h\approx 2.7 T_m`.


      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/tension.png
         :alt:
         :scale: 50
         :align: center
         :name: fig:S_W_button

         Botón que controla la tensión


   #. Discuta sus resultados y escriba sus conclusiones.


**Cuerda con un extremo fijo y el otro libre**

   #. Para estudiar las ondas estacionarias en la cuerda con un extremo fijo y el otro libre, configure el sistema tal como muestra la :numref:`fig:S_W_Setup_04`

      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/WS_Setup_04.png
         :alt:
         :scale: 50
         :align: center
         :name: fig:S_W_Setup_04

         Montaje para estudiar las ondas estacionarias en la cuerda cuando un extremo es fijo y el otro libre

   #. Calcule las frecuencias apropiadas y ponga a oscilar la cuerda de manera que sus modos de oscilación sean como los mostrados en la figura :numref:`fig:S_W_set_modes_One_end_free` y completa la :numref:`tab:S_W_freq_One_end_free`.

      .. figure:: /images/Oscilaciones_Termo/Standing_Waves/set_modes_One_end_free.png
         :alt:
         :scale: 50
         :align: center
         :name: fig:S_W_set_modes_One_end_free

         Seis primeros modos normales en la cuerda para diferentes instantes de tiempo.

      .. csv-table:: Frecuencias de los primeros siete modos de oscilación. Cuerda con un extremo fijo y el otro libre.
         :header: ":math:`n`", "Frecuencia, :math:`f` (Hz)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:S_W_freq_One_end_free
         :align: center

         1,
         2,
         3,
         4,
         5,
         6,
         7,

   #. Discuta sus resultados y escriba sus conclusiones.

**Aplicaciones**


   #. En el horno microondas  se forman ondas estacionarias solo que las ondas son ondas electromagnéticas. Explique a la luz de los nodos y antinodos formados en las ondas estacionarias, ¿por qué razón es necesario colocar los alimentos a calentar en la cavidad del microondas en una plataforma giratoria?
   #. ¿Tienen las ondas estacionarias aplicación en la música? Si la respuesta es afirmativa, explique.
   #. ¿Existe alguna relación entre resonancia y ondas estacionarias?


