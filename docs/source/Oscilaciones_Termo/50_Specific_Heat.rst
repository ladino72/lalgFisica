Calor específico de un líquido
===============================

**Objetivo**

El propósito de esta práctica es determinar el calor específico de un líquido.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.thephysicsaviary.com/Physics/Programs/Labs/ElectricalDeterminationOfSpecificHeatLab/ <https://www.thephysicsaviary.com/Physics/Programs/Labs/ElectricalDeterminationOfSpecificHeatLab/>`_.

**Resumen teórico**

Supongamos que agregamos cierta cantidad de calor :math:`dQ` a un cuerpo (sólido o líquido) sin producir cambio de fase alguno, como consecuencia su temperatura se incrementa en :math:`dT`. Se define capacidad calorífica, :math:`C`, del cuerpo como:

.. math::
   :label: Ec:Spec_Heat_01

   \begin{equation}
     C=\frac{dQ}{dT}
   \end{equation}

Así, la cantidad de calor, :math:`Q`, necesaria para producir en el cuerpo un cambio finito de temperatura :math:`\Delta T` lo podremos obtener como:

.. math::
   :label: Ec:Spec_Heat_02

   \begin{equation}
    Q=\int_{T}^{T+\Delta T}CdT=C\Delta T
   \end{equation}

donde hemos asumido que :math:`C` permanece constante entre las temperaturas :math:`T` y :math:`T+\Delta T`.
La capacidad calorífica es proporcional a la cantidad de materia del sistema, por lo que se define la correspondiente magnitud específica: calor específico.
El calor específico, :math:`c`, es la capacidad calorífica por unidad de masa,

.. math::
   :label: Ec:Spec_Heat_03

   \begin{equation}
    c=\frac{C}{m}=\frac{1}{m}\frac{dQ}{dT}
   \end{equation}

En función del calor específico, el calor, :math:`Q`, necesario para producir en un sistema de masa :math:`m` un cambio finito de temperatura :math:`\Delta T` lo podremos expresar como:

.. math::
  :label: Ec:Spec_Heat_04

  \begin{equation}
    Q=mc\Delta T
  \end{equation}

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Spec_Heat_Gui_01` muestra la interfaz gráfica del usuario que permite determinar el calor específico de un líquido. La aplicación muestra un calorímetro (recipiente con paredes aisladas), el cual en general tiene una pared doble entre las que se ha hecho el vacío o se introduce un material aislante térmico, que impide o minimiza la conducción de calor. De esta forma, los procesos que tengan lugar en el interior del calorímetro estarán térmicamente aislados del exterior. El calorímetro tiene incorporado un elemento calefactor (resistor) que se alimenta a través de dos conectores que atraviesan la tapa, y se conectan a una fuente de voltaje DC la cual suministra una diferencia de potencial :math:`V`. En serie se encuentra un amperímetro, el cual registra la corriente :math:`I` que pasa por el resistor. Inmerso en el líquido se encuentra una sonda termométrica que se encuentra conectada al medidor de temperatura y registra la temperatura :math:`T` del líquido. Además, la aplicación cuenta con un medidor de tiempo el cual registra el tiempo :math:`t` que dura suministrándosele energía al líquido del calorímetro. Antes de encender la fuente de voltaje, el medidor de temperatura registra la temperatura ambiente :math:`T_0` del líquido. Tan pronto se enciende la fuente de voltaje, el tiempo comienza a correr. Nota: si desea realizar una lectura de temperatura en un determinado instante de tiempo, simplemente apague la fuente de voltaje y realice las lecturas; al encenderla de nuevo el tiempo y la temperatura siguen cambiando como si la fuente no se hubiese apagado. Este proceso se puede repetir cuantas veces se requiera.

.. figure:: /images/Oscilaciones_Termo/Specific_Heat/Specific_Heat_Gui.png
   :scale: 85
   :align: center
   :name: fig:Spec_Heat_Gui_01

   Interfaz gráfica del usuario.

.. _Spec_Heat_sec_met_prc:

**Mediciones y procedimientos**

Si el calorímetro contiene una cierta cantidad de líquido, :math:`m`, y por el resistor circula una corriente :math:`I`, al ser las paredes del calorímetro adiabáticas, el
calor disipado en la resistencia por efecto Joule será completamente absorbido por el sistema (agua+calorímetro) produciendo un aumento de su temperatura. Si :math:`T` representa la temperatura en el interior del calorímetro en el instante :math:`t` y :math:`T_0` la temperatura en :math:`t=0`, justo cuando empieza a circular corriente por la resistencia, al hacer un balance de energía, en el instante :math:`t` se tiene:

.. math::
  :label: Ec:Spec_Heat_05

  \begin{equation}
    VIt=mc(T-T_0)=mc\Delta T
  \end{equation}

donde :math:`\Delta T=T-T_0`

   #. Registre los valores de la cantidad de la masa :math:`m` del líquido y su temperatura inicial :math:`T_0`.
   #. Encienda la fuente y tome mediciones de temperatura :math:`T` en función del tiempo cada 10 segundos y registre las mediciones en la :numref:`tab:Specific_heat_01`.
   #. En cualquier momento que la fuente de voltaje se encuentre encendida registre los valores de la diferencia de potencial :math:`V` suministrada por la fuente y la intensidad de la corriente :math:`I` que circula por el resistor.
   #. A partir de los datos de la :numref:`tab:Specific_heat_01`:

      a. Construya una gráfica de :math:`T` en función del tiempo :math:`t`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`T` y :math:`t`. Demuestre que el calor específico del líquido viene dado por :math:`c=\frac{VI}{mp_1}`, donde :math:`p_1` es la pendiente de la recta.
      b. Construya una gráfica de :math:`\Delta T` en función del tiempo :math:`t`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`\Delta T` y :math:`t`. Demuestre que el calor específico del líquido viene dado por :math:`c=\frac{VI}{mp_2}`, donde :math:`p_2` es la pendiente de la recta.


**Análisis y preguntas**

   #. Compare los resultados que se derivan de la sección :ref:`Mediciones y Procedimientos <Spec_Heat_sec_met_prc>` inciso 4. ¿Deberían ser iguales?
   #. ¿Cómo identificaría usted el tipo de líquido del calorímetro?
   #. ¿Cómo tendría que modificarse la ecuación :eq:`Ec:Spec_Heat_05` en caso que se tuvieran en cuenta las masas  y calores específicos de la sonda para medir temperatura y el calorímetro?

      .. csv-table:: Datos de tiempo :math:`t` y temperatura :math:`T` del líquido
         :header: "Tiempo, :math:`t` (s)", "Temperatura, :math:`T\\,(^o \\,\\text{C}`)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Specific_heat_01
         :align: center

         10,.
         20,.
         30,.
         40,.
         50,.
         60,.
         70,.
         80,.
         90,.
         100,.


