Efecto fotoeléctrico
=====================

**Objetivo**

El propósito de esta práctica es estudiar uno de los fenómenos más importantes que dieron origen a la fsica cuántica: el efecto fotoeléctrico.

**Recursos**

   #. Computador o tablet con acceso a la Internet
   #. Simulación disponible en `https://phet.colorado.edu/sims/cheerpj/photoelectric/latest/photoelectric.html?simulation=photoelectric&locale=es <https://phet.colorado.edu/sims/cheerpj/photoelectric/latest/photoelectric.html?simulation=photoelectric&locale=es>`_.


**Resumen teórico**

Una forma de extraer electrones de un metal es haciendo incidir radiación sobre su superficie. Los electrones absorben la luz que golpea el metal, y si un electrón absorbe una cantidad de energía mayor que :math:`W_c` (función trabajo), este es expulsado del metal como se muestra en la :numref:`fig:Photo-elect_01`.
Este fenómeno se llama efecto fotoeléctrico. Los estudios experimentales del efecto fotoeléctrico realizados alrededor de 1900 encontraron que no se emiten electrones a menos que la frecuencia de la luz sea mayor que un valor crítico :math:`f_c`. Cuando la frecuencia está por encima de :math:`f_c`, la energía cinética de los electrones emitidos varía linealmente con la frecuencia :math:`f` como se muestra en la :numref:`fig:Photo-elect_02`. Inicialmente, los físicos trataron de explicar estos resultados utilizando la teoría clásica de la onda de la luz, pero había dos dificultades con las explicaciones clásicas.

.. figure:: /images/Oscilaciones_Termo/PhotoElectricEffect/Photo_electric_01.png
   :scale: 65
   :align: center
   :name: fig:Photo-elect_01

   Efecto fotoeléctrico

.. figure:: /images/Oscilaciones_Termo/PhotoElectricEffect/Photo_electric_02.png
   :scale: 80
   :align: center
   :name: fig:Photo-elect_02

   Efecto fotoeléctrico

**Puntos importantes**

   #. La frecuencia :math:`f_c` es independiente de la intensidad de la luz. Segun la teora clásica de las ondas, la energa transportada por una onda de luz es proporcional a la intensidad, por lo que siempre debera ser posible expulsar electrones aumentando la intensidad a un valor suficientemente alto.  Los experimentos revelaron que cuando la frecuencia de la luz está por debajo de :math:`f_c`, sin embargo, no hay electrones expulsados sin importar cuán grande se la intensidad de la luz.
   #. En segundo lugar, la energa cinética de un electrón expulsado es independiente de la intensidad de la luz.  La teoría clásica predice que aumentar la intensidad hará que los electrones expulsados tengan mayor energía cinética, pero los experimentos no muestran este resultado.  De hecho, los experimentos muestran que la energa cinética de los electrones depende de la frecuencia de la luz (:numref:`fig:Photo-elect_02`) en lugar de la intensidad.

La teoría clásica de la onda de la luz no puede explicar los experimentos del efecto fotoeléctrico. A. Einstein soluciona el problema en 1905 cuando propuso que la luz transporta energía en cuantos discretos, llamados fotones. Según Einstein, cada fotón lleva un paquete de energía :math:`E_{foton}=hf` donde :math:`h` es una constante de la naturaleza llamada constante de Planck, que tiene el valor :math:`h=6.626\times10^{-34}\,\text{Js}`  y :math:`f` es la frecuencia de la luz.

Einstein sugirió que un haz de luz debería considerarse como una colección de partículas (fotones), cada una de las cuales tiene una energía que depende de la frecuencia. Si aumenta la intensidad de un haz de luz monocromática (frecuencia única), aumenta el número de fotones, pero la energía transportada por cada fotón no cambia.
Si aumenta la intensidad de un haz de luz monocromática (frecuencia única), aumenta el número de fotones, pero la energía transportada por cada fotón no cambia. Esta teoría explica los dos acertijos mencionados antes:


   #. La absorción de luz por un electrón es como una colisión entre dos partículas, un fotón y un electrón. El fotón lleva una energía :math:`hf` que es absorbida por el electrón. Si esta energía es menor que la función de trabajo, el electrón no puede escapar del metal. Para la luz monocromática, el aumento de la intensidad de la luz aumenta el número de fotones que llegan cada segundo, pero si la energía del fotón :math:`hf` es menor que la función de trabajo, incluso una alta intensidad no expulsará electrones. La energía de un solo fotón, y por lo tanto la energía obtenida por cualquier electrón en particular, depende de la frecuencia :math:`f` pero no de la intensidad de la luz.
   #. La teoría de Einstein también explica la razón por la cual la energía cinética de los electrones expulsados depende de la frecuencia de la luz, pero no de la intensidad. La frecuencia crítica en el efecto fotoeléctrico (:numref:`fig:Photo-elect_02`) corresponde a fotones cuya energía es igual a :math:`W_c=hf_c`. Tal fotón tiene apenas energía suficiente para expulsar un electrón del metal, pero el electrón expulsado no tiene energía cinética. Si un fotón tiene una frecuencia más alta y, por lo tanto, una mayor energía, la energía adicional por encima de la función de trabajo se destina a la energía cinética del electrón. Así,


.. math::
   :label: Photoelectric_ec_02

   \begin{equation}
     E_{foton}=hf-W_c
   \end{equation}

la cual es la ecuación de una línea recta; por lo tanto, la energía cinética de un electrón expulsado debe ser linealmente proporcional a :math:`f`. Este comportamiento lineal es precisamente lo que es encontrado en experimentos como se muestra en la :numref:`fig:Photo-elect_02`. La pendiente de esta línea es el factor que multiplica :math:`f` en la ecuación :eq:`Photoelectric_ec_02`, que es solo la constante :math:`h` de Planck. Por lo tanto, los experimentos fotoeléctricos brindan una forma de medir :math:`h`, y los valores encontrados coinciden con el valor conocido antes de la teoría de Einstein.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:gui_01_Photoelectric` muestra la interfaz gráfica del usuario que permite estudiar el efecto fotoeléctrico. La interfaz permite seleccionar no solamente el tipo de radiación (ultravioleta, visible o infrarroja) incidente sobre el electrodo metálico donde se producirá el efecto fotoeléctrico sino también su intensidad. Esta radiación tiene un rango de longitudes de onda comprendidas entre 100 nm y 850 nm. Frente al electrodo emisor de electrones se tiene otro, el cual en principio colecta los electrones dependiendo de la polaridad de la fuente de voltaje (pila). El valor de la diferencia de potencial entre los electrodos se puede variar entre -8 V y +8 V. Si el electrodo de la derecha es positivo, este captura cualquier electrón emitido por el electrodo y entre mayor sea este número mayor es el valor de la corriente fotoeléctrica registrada por el amperímetro. Si el electrodo de la derecha es negativo, este repele los electrones emitidos; entre más negativo sea este electrodo, mayor será la repulsión y el mayor valor de la diferencia de potencial para la cual ningún electrón llega al electrodo (lo que equivale a una corriente nula) de la derecha se denomina potencial de frenado (se mide en voltios). La simulación permite seleccionar seis tipos diferentes de materiales del electrodo de la izquierda (sodio, zinc, cobre, platino, calcio y otro de naturaleza desconocida). Además, la simulación permite visualizar las gráficas de a) corriente eléctrica en función del voltaje aplicado, b) corriente eléctrica en función de la intensidad de la radiación y c) energía cinética máxima de los electrones en función de la frecuencia de los mismos.

.. figure:: /images/Oscilaciones_Termo/PhotoElectricEffect/Photoelectric_gui_01.png
   :scale: 50
   :align: center
   :name: fig:gui_01_Photoelectric

   Interfaz gráfica del usuario

**Mediciones y procedimientos**

**Frecuencia umbral**

   #. Seleccione: el sodio como material de trabajo, la intensidad de la fuente de radiación en 100\%, voltaje de la fuente de voltaje en cualquier valor mayor que cero y opción de gráfica: energía de los electrones en función de la frecuencia.
   #. Varíe la longitud de onda :math:`\lambda` de la radiación incidente sobre el electrodo desde valores bien bajos (ultravioleta) hasta valores mayores y registre el valor mínimo de la longitud de onda para el cual ya no se expulsan más electrones; esta es la longitud de onda umbral, :math:`\lambda_{umbral}`. La frecuencia crítica o umbral se calcula como :math:`f_c=\frac{c}{\lambda}`, donde :math:`c=3\times10^{8}` es la velocidad de la luz.
   #. Repita los mismos pasos de los incisos 1 y 2, pero esta vez usando zinc, cobre, platino, calcio y material desconocido. ¿Depende la frecuencia umbral del tipo de material?

**Efecto de la intensidad de la luz**

   #. Seleccione: el sodio como material de trabajo, voltaje de la fuente de voltaje en cualquier valor mayor que cero, longitud de onda de la radiación en un valor que sea menor que :math:`\lambda_{c}`, por ejemplo :math:`\lambda=350\,\text{nm}` y opción de gráfica: corriente en función de la intensidad de la luz.
   #. Varíe la intensidad de la radiación incidente sobre el electrodo desde 0\% hasta 100\%. ¿Qué tipo de relación existe entre la corriente y la intensidad de la radiación? ¿Qué le sucede a la corriente si la intensidad se duplica?
   #. Repita los mismos pasos de los incisos 1 y 2, pero esta vez usando zinc, cobre, platino, calcio y material desconocido. ¿Qué le sucede a la dependencia entre la corriente y la intensidad de la radiación? ¿Depende esta dependencia del tipo de material del electrodo?


**Función trabajo**

   #. Seleccione: el sodio como material de trabajo, intensidad de la radiación el valor que desee y opción de gráfica: energía de los electrones en función de la intensidad de la luz.
   #. Varíe la longitud de onda de la radiación desde el ultravioleta hasta la longitud de onda umbral del sodio. Para cada valor de :math:`\lambda`, disminuya gradualmente el valor del voltaje aplicado a los electrodos comenzando en +8 V hasta encontrar el valor del potencial o voltaje de frenado, :math:`V_s`. El potencial de frenado :math:`V_s` está relacionado con la energía cinética máxima :math:`E_k` de los electrones a través de la expresión :math:`E_K=|e|V_s`, donde :math:`e` es la carga del electrón. Registre sus datos en la :numref:`tab:Photo-Elect_01`.
   #. A partir de los datos obtenidos en el inciso 2 construya la gráfica de :math:`E_k` en función de la frecuencia :math:`f` de la radiación incidente\footnote{Recuerde que por tratarse de una onda :math:`c=\lambda f`, donde :math:`\text{c}=3\times10^{8},\text{m/s}`}. Aplique sus conocimientos de linealización de funciones y encuentre la relación :math:`E_k` y :math:`f`. Use la ecuación :eq:`Photoelectric_ec_02` para encontrar el valor de la función trabajo :math:`W_c` del material y el valor de la constante de Planck.
   #. Repita los mismos pasos de los incisos 1, 2 y 3, pero esta vez usando zinc, cobre, platino, calcio y material desconocido. Registre sus mediciones en la :numref:`tab:Photo-Elect_02`, la :numref:`tab:Photo-Elect_03`, la :numref:`tab:Photo-Elect_04`, la :numref:`tab:Photo-Elect_05` y la :numref:`tab:Photo-Elect_06`. Encuentre los valores de las funciones de trabajo para estos materiales y compárelos con los valores reportados en la literatura. Explique las diferencias. Identifique el material desconocido.
   #. A partir de los resultados anteriores, ¿cuál es el valor que usted reporta para la constante de Planck?

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{Na}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_01
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

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{Zn}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_02
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

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{Cu}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_03
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

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{Pt}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_04
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

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{Ca}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_05
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

.. csv-table:: Datos de frecuencia :math:`f` y voltajes de frenado :math:`V_s` para el :math:`\text{????}`.
   :header: "Frecuencia, :math:`f` (Hz)", "Voltaje, :math:`V_s` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Photo-Elect_06
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

