Ley de Faraday: Generador eléctrico
====================================

**Objetivo**

El propósito de esta práctica es estudiar el principio de funcionamiento de un generador de electricidad.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/es/simulation/generator <https://phet.colorado.edu/es/simulation/generator>`_.

**Resumen teórico**

La ley de de inducción de Faraday se basa en los experimentos que Michael Faraday realizó en 1831 y establece que el voltaje inducido en un circuito cerrado es directamente proporcional a la rapidez con que cambia en el tiempo el flujo magnético que atraviesa una superficie cualquiera con contorno :math:`C` como borde. Matemáticamente se escribe como

.. math::
   :label: Ec:Faraday_01

   \begin{equation}
     \oint_C \vec{E}\cdot d\vec{l}=-\frac{d}{dt}\oint_S \vec{B}\cdot d\vec{A}=-\frac{d\Phi}{dt}
   \end{equation}

donde :math:`\vec{E}` es el campo electrico, :math:`d\vec{l}` es un elemento diferencial de contorno :math:`C`, :math:`\vec{B}` es el campo magnético y :math:`S` es una superficie arbitraria cuyo borde es la superficie :math:`S`. :math:`C` y :math:`d\vec{A}` están dadas por la regla de la mano derecha.

En el caso de un inductor o bobina con :math:`N` vueltas de alambre, la fórmula anterior se transforma en:

.. math::
   :label: Ec:Faraday_02

   \begin{equation}
    v_i=-N\frac{d\Phi}{dt}
   \end{equation}

Donde :math:`v_i` es el voltaje inducido y :math:`\frac{d\Phi}{dt}` es la tasa de variación temporal del flujo magnético :math:`\Phi`. La dirección voltaje inducido (el signo negativo en la fórmula) se debe a la ley de Lenz.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Gui_B_Loop_Faraday` muestra la interfaz gráfica del usuario que permite estudiar el principio de funcionamiento de un generador de electricidad. La interfaz presenta un imán en forma de barra el cual puede girar alrededor de un eje bajo la acción de la caída de un chorro de agua cuyo caudal se puede graduar, y de esta manera controlar la velocidad angular del imán en un rango comprendido entre 0 y 100 rpm. La intensidad del imán se puede variar con la la barra de desplazamiento rotulada **Fueza** ubicado en la parte superior de la interfaz. Frente al imán, se encuentra una bobina circular con 1, 2  o 3 espiras; el número de espiras y su tamaño se puede controlar con los botones rotulados **Vueltas** y **Área de espiral**. A los terminales de la(s) espira(s) se puede conectar un resistor, una bombilla o un voltímetro análogo. Además, se cuenta con un medidor móvil de campo magnético el cual permite medir sus componentes cartesianas :math:`B_x` y :math:`B_y`.

.. figure:: /images/Electromagnetismo/Faraday/Gui_B_Loop_Faraday.png
   :scale: 50
   :align: center
   :name: fig:Gui_B_Loop_Faraday

   Interfaz gráfica del usuario.


.. _FM:

**Flujo magnético**

El cálculo del flujo magnético creado por el imán a través de la superficie de la espira no es fácil de hacer dada la naturaleza del campo,
pero esbozaremos la manera de hacerlo. Dividamos la superficie de la espira en cuadrados infinitesimales de área :math:`dA=dydz` como muestra
la :numref:`fig:Faraday_part`, el flujo magnético a través de uno cualquiera de los cuadrados es :math:`d\phi=\overrightarrow{B}\cdot d\overrightarrow{A}=B_xdA`,
donde :math:`B_x` es el campo en la superficie de área :math:`dA`. ¿Cómo determinamos :math:`B_x`? Colocamos el medidor de campo en el elemento de área :math:`dA`
con coordenadas (:math:`x=x_0`, :math:`y`, :math:`z`) y medimos :math:`B_x` como función del tiempo, multiplicamos :math:`B_x` por :math:`dA` y de esta manera tenemos
:math:`d\phi` para este elemento :math:`dA` como función del tiempo. Repetimos este proceso para cada uno de los cuadraditos que conforman la espira y finalmente
sumamos los flujos, siendo el resultado :math:`\Phi`, el cual también depende del tiempo. Aplicamos la ley de Fafaday, y el voltaje en los terminales de la espira es:
:math:`v=-\frac{d\Phi}{dt}`, el signo menos proviene de la ley de Lenz.

Definimos como unidad de longitud (u.l) la distancia entre dos agujas imantadas consecutivas dispuestas de manera vertical u horizontal.

.. figure:: /images/Electromagnetismo/Faraday/partition_2.png
   :scale: 80
   :align: center
   :name: fig:Faraday_part

   Superficie de la espira dividida en cuadrados de área :math:`dA=dydz`

.. figure:: /images/Electromagnetismo/Faraday/flux_Fringe_01.png
   :scale: 100
   :align: center
   :name: fig:Faraday_flux_Fringe_01

   Simulador configurado para determinar :math:`B_x` en función del tiempo.

.. _MyP:

**Mediciones y procedimientos**

   #. Configure el simulador con los parámetros que se indican en la figura :numref:`fig:Faraday_flux_Fringe_01` y demuestre a partir de mediciones que la gráfica de :math:`B_x` en función del tiempo :math:`t` en el centro de la espira (:math:`x=x_0`, :math:`y=0`, :math:`z=0`) para dos revoluciones completas del imán es como la mostrada en la :numref:`fig:Faraday_Plot_Flux_cent`. Utilice el botón de avance pausado :math:`|\triangleright` para hacer las mediciones de campo. Nótese que puede generar una base de tiempos a partir de la velocidad angular del imán y el hecho de que el imán gira en pasos de 24 :math:`^{o}` cuando su velocidad angular es 100 rpm (o pasos de 12 :math:`^{o}` cuando su velocidad angular es 50 rpm).

      .. figure:: /images/Electromagnetismo/Faraday/Plot_Flux_center_1.png
         :scale: 70
         :align: center
         :name: fig:Faraday_Plot_Flux_cent

         :math:`B_x` como función del tiempo en el centro de la espira. La variación de :math:`B_x` es periódica, pero no senoidal.

   #. Configure el simulador con los parámetros que se indican en la :numref:`fig:Faraday_flux_Fringe_02`, el medidor de campo de encuentra en un punto con coordenadas (:math:`x=x_0`, :math:`y=1.5 \,\text{u.l}`, :math:`z=0`) y construya una gráfica de :math:`B_x` en función del tiempo :math:`t` para dos revoluciones completas del imán.

      .. figure:: /images/Electromagnetismo/Faraday/flux_Fringe_02.png
         :scale: 50
         :align: center
         :name: fig:Faraday_flux_Fringe_02

         :math:`B_x` como función del tiempo  en un punto (:math:`y=\,\text{1.5 u.l},z=0`)

.. _Vfn:

**Efecto del número de espiras y frecuencia en el voltaje generado**

   #. Varíe la frecuencia del imán y mida el máximo voltaje en los terminales de la bobina cuando esta tiene 1, 2 y 3 espiras. Para ello utilice el voltímetro análogo y el botón de avance pausado :math:`|\triangleright`. Registre sus mediciones en la :numref:`tab:n_loops_freq`.
   #. Con los datos del inciso 1 construya gráficas apropiadas que permitan encontrar la relación entre el valor del voltaje máximo :math:`V_{max}` generado, la frecuencia :math:`f` del imán y el número :math:`n` de espiras del generador.

      .. csv-table:: Datos de voltaje máximo en las espiras y frecuencias del imán
         :header: "Frecuencia, :math:`f` (rpm)", ":math:`V_{max}` (unid.), n=1", ":math:`V_{max}` (unid.), n=2", ":math:`V_{max}` (unid.), n=3"
         :widths: 1,1,1,1
         :width: 18 cm
         :name: tab:n_loops_freq
         :align: center

         0,.,.,.
         20,.,.,.
         40,.,.,.
         60,.,.,.
         80,.,.,.
         100,.,.,.

**Análisis y preguntas**

   #. Explique por qué razón cuando la bobina (con cualquier número de espiras) tiene conectada entre sus terminales la bombilla y el imán se encuentra girando, la intensidad de la bombilla es máxima y cero para ciertos instantes de tiempo.
   #. Explique como calcularía el flujo magnético generado por el imán de la aplicación cuando la bobina tiene las 3 espiras. Un estudiante sugiere que basta medir el flujo de una sola espira y multiplicar el resultado por 3. ¿Tiene este estudiante la razón?
   #. ¿Qué puede concluir a partir de las gráfica de :math:`B_x` en función del tiempo mostrada en la :numref:`fig:Faraday_Plot_Flux_cent` y la obtenida por usted en la sección :ref:`Mediciones y Procedimientos <MyP>`, inciso 2 ?
   #. ¿Cuál es la relación entre el voltaje máximo generado :math:`V_{max}`, la frecuencia :math:`f` de giro del imán y el número :math:`n` de espiras? Su respuesta *debe* incluir una expresión matemática. Justifique sus resultados.
   #. En la vida real en lugar del grifo se utilizan las caídas de agua para generar electricidad, ¿qué sucede cuando el caudal no es regular?
   #. ¿Cómo funciona el dinamo de una bicicleta?


