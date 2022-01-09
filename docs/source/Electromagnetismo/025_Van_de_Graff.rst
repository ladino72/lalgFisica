+Generador de Van de Graaff
============================


**Objetivo**

El propósito de esta práctica es introducir de manera heurística los conceptos de carga eléctrica, corriente eléctrica, condensador como dispositivo para almacenar carga eléctrica, diferencia de potencial, etc. Para ello, se usa el generador de Van de Graaff como fuente de corriente constante. En particular, se carga un condensador y se encuentra de manera cuantitativa el crecimiento lineal de su carga con el tiempo.

**Medidas de Seguridad**

Generador de Van de Graaff (GDVG)

   * Esta es una práctica demostrativa y por tanto las únicas personas que manipularán el GDVG es el profesor o los técnicos de laboratorio.  Los estudiantes deben permanecer por lo menos a dos metros de distancia del GDVG.
   * Personas con implantes cocleares en el oído, marcapasos, etc deben permanecer lejos del GVDG!, estos podrían ser dañados por los grandes campos eléctricos que rodean a un GVDG.
   * Evite entrar al laboratorio con encendedores de cigarrillo que funcionen con gas butano, puestos pordrían incendiarse por una chispa del GVDG.
   * Evite acercar cualquier dispositivo electrónico como laptops, tablets, teléfonos móviles al GVDG en operación, estos podrían dañarse debido al fuerte campo eléctrico.
   * No toque directamente con las manos el domo del GDVG, este podría descargarse a través de su mano y producir un fuerte choque eléctrico.

**Recursos**

   #. Un generador de Van de Graaff.
   #. Un capacitor electrolítico de 470 :math:`\mu \text{F}`, 25 V.
   #. Un cronómmetro.
   #. Dos multímetros digitales.
   #. Cables de conexión


**Resumen teórico**

El generador de Van de Graaff (inventado en 1931) es una máquina electrostática que utiliza una cinta móvil para acumular grandes cantidades de carga eléctrica en la superficie de una esfera metálica hueca. Se fundamenta en los fenómenos de electrización por contacto y en la inducción de carga. El generador tiene un motor, una correa, dos rodillos uno superior (que gira libre arrastrado por la correa) y otro inferior (manejado por un motor conectado a su eje), dos peines metálicos (superior e inferior) para ionizar el aire (el inferior esta conectado a tierra y el superior al interior de la esfera), y una esfera hueca donde se acumula la carga transportada por la cinta. Algunas definiciones:


   #. *Carga eléctrica:* es una propiedad intrínseca que presentan algunas partículas subatómicas la cual se manifiesta a través de interacciones de tipo atractivo o repulsivo entre ellas.  Existen dos tipos de carga eléctrica: negativa y positiva. Al electrón se le asigna una carga negativa y al protón una carga positiva. Cargas de igual signo se repelen y de diferente signo se atraen. La carga eléctrica se mide en culombios, y la interacción entre las partículas cargadas se mide a través de la ley de Coulomb. La carga del electrón es :math:`-1.6\times 10^{-19}` C y la del protón :math:`+1.6\times 10^{-19}` C.
   #. *Corriente eléctrica:* es la cantidad de carga eléctrica :math:`\Delta q` que pasa por un punto del espacio en un intervalo de tiempo :math:`\Delta t`.  Así, la corriente media o promedio que pasa por dicho punto es :math:`\overline{I}=\frac{\Delta q}{\Delta t}`. Cuando :math:`\Delta t\rightarrow 0`, se tiene la corriente instantánea o simplemente corriente :math:`I`, y es dada por :math:`I=\frac{dq}{dt}`. La corriente eléctrica se mide en amperios.
   #. *Capacitancia:* la capacitancia de un dispositivo es una medida de su capacidad para almacenar carga eléctrica y energía potencial eléctrica. La capacitancia se mide en faradios.
   #. *Diferencia de potencial eléctrico:* es el trabajo :math:`W` que se requiere para llevar la unidad de carga eléctrica :math:`q` de un punto a otro en el espacio. Así, :math:`V= \frac{W}{q}`.


**Descripción del método**

La expresión :math:`V =\frac{q}{C}`, da la relación entre la diferencia de potencial :math:`V` entre las placas de un condensador con capacitancia :math:`C` y su carga almacenada :math:`q`. La dependencia entre las variables :math:`q` y :math:`V` es lineal siempre y cuando  :math:`C` se mantenga constante. Si el condensador gana la carga a una tasa constante :math:`I` (igual a la corriente eléctrica) entonces

.. math::
   :label: Ec:equ_1

   \begin{equation}
    V = \frac{I}{C}t
   \end{equation}

donde :math:`t` es el tiempo. Así, la  diferencia de potencial  entre los terminales del condensador aumenta linealmente con el tiempo. Lo anterior implica que al graficar :math:`V` en función del tiempo :math:`t`, la curva obtenida es una línea recta con pendiente :math:`m=\frac{I}{C}` y por tanto el valor de la capacitancia :math:`C` del condensador en términos de :math:`m` es


.. math::
   :label: Ec:equ_2

   \begin{equation}
     m=\frac{I}{C}
   \end{equation}

Un diagrama esquemático del montaje experimental usado para cargar el condensador se muestra en la :numref:`fig:Van_de_Graaff_01`, [#f5]_. El generador de van de Graaff utilizado presenta grandes diferencias de potencial entre la esfera conductora y tierra en el rango de 200 kV a 300 kV. El generador se comporta como una fuente de corriente constante. Esto significa que al conectar el terminal de salida en la esfera con un objeto conectado a tierra, el voltaje disminuirá, pero la corriente seguirá siendo la misma. En otras palabras, el generador Van de Graaff es como una fuente de corriente con una alta resistencia interna.


.. figure:: /images/Electromagnetismo/Van_de_Graaff/Van_de_Graaff_01.png
   :alt:
   :scale: 100
   :align: center
   :name: fig:Van_de_Graaff_01

   Diagrama esquemático para cargar el condensador con el generador.


Obsérvese que uno de los terminales del condensador electrolítico (C = 470 F, a 25 V) está conectado a la cúpula metálica del generador a través de un amperímetro convencional y que el otro terminal está conectado a tierra. La diferencia de potencial en el condensador se mide en función del tiempo. Con este valor de capacitancia, los cambios en la diferencia potencial en el condensador ocurren a una rapidez de 2 mV / s. Esta baja tasa de cambio permite realizar lecturas de tiempo manualmente, un par de segundos entre mediciones consecutivas,
haciendo el experimento rápido y fácil de realizar. La cantidad de corriente eléctrica que el generador de Van de Graaff puede suministrar depende en cierta medida de la velocidad angular del motor que acciona el generador y de las condiciones de humedad existentes en el momento de la práctica. El valor de la corriente eléctrica no aumenta indefinidamente con la velocidad de giro del motor. Por el contrario, alcanza un valor máximo y permanece constante. En el generador de Van de Graaff utilizado en el experimento, la corriente obtenida puede estar en el rango comprendido entre 0.5 y 5.0 :math:`\mu A`. La figura 2  muestra una imagen de la configuración experimental real del experimento.

.. figure:: /images/Electromagnetismo/Van_de_Graaff/Van_de_Graaff_02.png
   :alt:
   :scale: 120
   :align: center
   :name: fig:Van_de_Graaff_02

   Montaje experimental real para cargar el condensador


**Mediciones**

Realice el montaje que se muestra en la :numref:`fig:Van_de_Graaff_02` con el generador apagado. Encienda el generador y fije la velocidad del motor con el control ubicado en la base del mismo hasta que alcance un valor de corriente constante igual a 1.0 :math:`\mu A`. Asegérese de mantener el valor de la corriente constante en el transcurso de la toma de datos. Observe como cambia la lectura del voltímetro conectado en paralelo con el condensador. Cuando esté listo para tomar medidas, sin apagar el generador, *descargue el condensador* cortocircuitándolo, simplemente conectando un alambre entre sus terminales. Esta operación no representa ningún riesgo de choque eléctrico para el usuario, pues la corriente es muy baja y la diferencia de potencial entre la esfera del generador y tierra es pequeña! [#f4]_. En nuestro caso, la esfera conductora se esta descargando permanentemente y por tanto la diferencia de potencial entre la esfera y tierra es muy pequeña, tanto así que el usuario puede tocar la esfera con la mano y no experimentar choque eléctrico alguno.} En el instante de cortocircuitar el condensador, tome el tiempo como :math:`t=0` y realice las mediciones. La medición de tiempo la puede realizar con el cronómetro convencional suministrado ó el cronómetro de una aplicación de su tablet. Registre sus datos para cada valor de corriente fijo (:math:`I_1=1.0\,\mu\,\text{A}`, :math:`I_2=2.0\,\mu \text{A}` y :math:`I_3=3.0\,\mu\text{A}`) en la :numref:`tab:VandeGraff`. A partir de los datos de esta tabla

   #. Realice la gráfica de :math:`V` en función del tiempo para :math:`I_1=` constante. Calcule el valor de la pendiente :math:`m_1` de la recta obtenida.
   #. Realice la gráfica de :math:`V` enfunción del tiempo para :math:`I_2=` constante. Calcule el valor de la pendiente :math:`m_2` de la recta obtenida.
   #. Realice la gráfica de :math:`V` en función del tiempo para :math:`I_3=` constante. Calcule el valor de la pendiente :math:`m_3` de la recta obtenida.

Utilice los valores :math:`m_1`, :math:`m_2` y :math:`m_3` obtenidos junto con la ecuación :eq:`Ec:equ_2` para determinar :math:`C`. Compare el valor de la capacitancia obtenido con el valor del capacitor utilizado. Discuta sus resultados.

Pregunta:


   #. Para cada una de las corrientes utilizadas calcule el número de electrones por segundo que están acumulándose en el capacitor.
   #. Si cada electrón que llega al condensador fuera un centavo y el condensador fuera su cuenta bancaria, ¿a qué rapidez estaría creciendo su saldo?

.. csv-table:: Mediciones de diferencias de potencial (voltajes) en el condensador  en función del tiempo para tres valores de corrientes fijas.
   :header: "Tiempo (s)", ":math:`V_1\\,\\text{(mV)}, I_1=\\,\\text{const}`", ":math:`V_2\\,\\text{(mV)}, I_2=\\,\\text{const}`", ":math:`V_3\\,\\text{(mV)}, I_3=\\,\\text{const}`"
   :widths: 1,1,1,1
   :width: 16 cm
   :name: tab:VandeGraff
   :align: center

   0,.,.,.
   5,.,.,.
   10,.,.,.
   15,.,.,.
   20,.,.,.
   25,.,.,.
   30,.,.,.
   35,.,.,.
   40,.,.,.
   45,.,.,.
   50,.,.,.
   55,.,.,.
   60,.,.,.
   65,.,.,.
   75,.,.,.
   80,.,.,.
   85,.,.,.
   90,.,.,.
   95,.,.,.
   100,.,.,.



.. [#f4] El generador en plena operación puede producir una descarga peligrosa en una persona cuando la esfera conductora no está conectada a tierra. Nunca toque con la mano la esfera del generador bajo estas circunstancias. El manejo del generador debe ser realizado por el profesor.
.. [#f5] *Charging a capacitor at a constant rate*.2015 Phys. Educ. 50 713, doi:10.1088/0031-9120/50/6/713