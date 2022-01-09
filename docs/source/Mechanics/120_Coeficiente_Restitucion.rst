+Coeficiente de restitución
============================

**Objetivo**

El propósito de esta práctica es encontrar el coeficiente de restitución :math:`\varepsilon` cuando un cuerpo choca contra una superficie. Para ello, se suelta una esfera desde cierta altura, la esfera impacta una superficie plana sólida y se miden los instantes de tiempo cada vez que la esfera rebota. Los tiempos se miden con la ayuda de **Audacity** (software libre), el cual registra las señales sonoras provenientes de la colisión en función del tiempo. Conocidos los tiempos entre colisiónes consecutivas y con el modelo propuesto abajo se determina :math:`\varepsilon`.


**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Esferas de diferentes materiales.
   #. Superficie sólida.
   #. Regla graduada en mm.
   #. Software (Audacity) [#f1]_ disponible en `https://www.audacityteam.org/ <https://www.audacityteam.org/>`_.

**Resumen teórico**

El conocimiento del coeficiente de restitución es de gran importancia en muchas situaciones. Por ejemplo, en el diseño de implementos deportivos como tenis, bolas etc. En el diseño de neumáticos de alto rendimiento para todo tipo de vehículos, por citar algunos casos. El coeficiente de restitución :math:`\varepsilon` es una medida de que tanto una colisión es elástica. Así, si :math:`\varepsilon =1` se dice que la colisión es perfectamente elástica; si :math:`\varepsilon =0` entonces se dice que la colisión es totalmente inelástica. Si asumimos que una esfera de masa :math:`m`  se suelta desde una altura :math:`h` y si además ignoramos las fuerzas
de rozamiento durante la caída, la velocidad con la cual llega la esfera a la superficie del piso es :math:`v_{0}=\sqrt{2gh}`. Definimos el coeficiente de
restitución :math:`\varepsilon` como el cociente entre las rapideces de la esfera justamente después (:math:`v_{f}`) e inmediatamente antes (:math:`v_{i}`) de la colisión con la superficie. Así,

.. math::
   :label: Eq:coefRest_01

   \begin{equation}
    \varepsilon =\frac{v_{f}}{v_{i}}  \label{Eq:coefRest_01}
   \end{equation}

Si después de la colisión la esfera sale disparada hacia arriba con rapidez :math:`v`, el tiempo que gasta la esfera en subir y bajar es dado por :math:`t=\frac{2v}{g}`. Luego, el tiempo total desde que se suelta la esfera hasta que queda en reposo después de rebotar multiples veces es

.. math::

   t_{total}=t_{0}+t_{1}+t_{2}+t_{3}+\ldots t_{n}+\ldots

donde :math:`t_{0}` :math:`=\sqrt{\frac{2h}{g}}=\frac{v_{0}}{g}` es el tiempo de caída antes de la primera colisión. Los tiempos de subida-bajada
de las subsiguientes colisiones vienen dados por

.. math::

    t_{1}=\frac{2v_{1}}{g}=\frac{2\varepsilon v_{0}}{g}

.. math::

    t_{2}=\frac{2v_{2}}{g}=\frac{2\varepsilon v_{1}}{g}=\frac{2\varepsilon^{2}v_{0}}{g}

.. math::

   t_{3}=\frac{2v_{3}}{g}=\frac{2\varepsilon v_{2}}{g}=\frac{2\varepsilon^{2}v_{1}}{g}=\frac{2\varepsilon ^{3}v_{0}}{g}

y después de la n-ésima colisión es

.. math::
   :label: Eq:coefRest_02

   \begin{equation}
    t_{n}=\frac{2v_{n}}{g}=\frac{2\varepsilon ^{n}v_{0}}{g}
   \end{equation}

en estas expresiones hemos despreciado el tiempo que dura la colisión. Tomando logaritmos a ambos lados
de la ecuación :eq:`Eq:coefRest_02` se tiene

.. math::
   :label: Eq:coefRest_03

   \begin{equation}
    \log_{10}(t_{n})=\log_{10}(\frac{2v_{0}}{g})+n\times \log_{10}(\varepsilon )
   \end{equation}

De esta expresión se sigue que si la relación entre :math:`Log_{10}(t_{n})` y :math:`n` es
lineal (ver :numref:`fig:RestCoef2`) entonces el valor del coeficiente de restitución
:math:`\varepsilon` se puede obtener como la pendiente :math:`m^{\ast}` de la recta; es decir :math:`m^{\ast }=\log_{10}(\varepsilon)` o

.. math::
   :label: Eq:coefRest_04

   \begin{equation}
    \varepsilon =10^{m^{\ast}}
   \end{equation}


.. figure:: /images/Mecanica/Coeficiente_Restitucion/RestCoef2.png
   :scale: 80
   :align: center
   :name: fig:RestCoef2

   Pendiente de la recta igual a :math:`m^*=\log_{10}(\varepsilon)`


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Gui_Rest_Coeff_02` muestra la interfaz gráfica del usuario que permite investigar el coeficiente de restitución.

.. figure:: /images/Mecanica/Coeficiente_Restitucion/Gui_Rest_Coeff_02.png
   :scale: 50
   :align: center
   :name: fig:Gui_Rest_Coeff_02

   Interfaz gráfica del usuario para estudiar el coeficiente de restitución.



Audacity es un editor de audio se puede usar para grabar sonidos, reproducir sonidos, importar y exportar archivos WAV, AIFF, y MP3, y más. Con éste se puede editar sonidos usando Cortar, Copiar y Pegar (con ilimitados Deshacer), mezclar pistas, o aplicar efectos a grabaciones pre existentes. Para lo que realizaremos en esta actividad, usaremos solo unas funciones muy básicas de esta aplicación.  Los botones ubicados en la parte superior izquierda de la consola permiten iniciar la grabación \texttt{sonora}, a igual que detenerla y reproducirla. La forma de la señal sonora se va grabando en función del tiempo. De igual manera, la interfaz presenta una serie de herramientas que nos permiten ampliar y visualizar la forma de la señal sonora en detalle para un determinado intervalo de tiempo. En la parte inferior de la interfaz se presentan tres menús que permiten establecer tiempos relacionados con la edición de la señal señora: Comienzo de la selección, :math:`\bigcirc` fin :math:`\,\,\circledcirc` longitud y posición de audio; seleccione el tiempo en el formato **hh:mm:ss+milisegundos** para los tres. En la parte superior de la interfaz, justamente después del botón de color rojo que inicia el proceso de grabación, se encuentra un botón en forma de barra vertical llamado *herramienta de selección*, ésta herramienta nos permite determinar el instante de tiempo para el cual se detectó la señal sonora. Al hacer clic en diferentes partes de la señal podemos leer los diferentes tiempos.




**Mediciones y procedimientos**

El arreglo experimental para determinar el coeficiente de restitucion :math:`\varepsilon`  se muestra en la :numref:`fig:Gui_Rest_Coeff_01`, el cual consta de una esfera, una superficie sólida y un computador con el software Audacity instalado. Audacity hace uso del micrófono ya incorporado en los computadores modernos, y capta las señales sonoras que se generan cuando la bola choca con la superficie. Estas señales son registradas en tiempo real. Como esfera puede usar por ejemplo un ping-pong, el cual al chocar con la superficie de una mesa de madera emite un sonido captable por el micrófono del PC. (Puede intentar esferas y superficies de otra naturaleza, use lo que mejor le funcione). La forma de las señales registradas no importa, lo que realmente nos interesa son los instantes de tiempo en que se generan y que con las herramientas del software utilizado se pueden determinar.

   #. Realice mediciones que le permitan determinar el valor de :math:`\varepsilon`. Para ello, deje caer la esfera desde una altura :math:`h` y registre las señales de sonido generadas por el impacto de la esfera con la superficie sólida con el micrófono del computador. Una vez capturadas las señales en función del tiempo con la ayuda del software, construya la :numref:`tab:RestCoef1`. A partir de los datos determine :math:`\varepsilon`.

      .. csv-table:: :math:`t_i` = tiempo de subida-bajada de la esfera para el impacto n-ésimo con la superficie.
         :header: ":math:`t` (s)", ":math:`n`"
         :widths: 1,1
         :width: 12 cm
         :name: tab:RestCoef1
         :align: center

         :math:`t_{1}` , 1
         :math:`t_{2}` , 2
         :math:`t_{3}` , 3
         :math:`t_{4}` , 4
         :math:`t_{5}` , 5
         :math:`t_{6}` , 6
         :math:`t_{7}` , 7
         :math:`t_{8}` , 8
         :math:`t_{9}` , 9
         :math:`t_{10}` , 10

   #. Repita el mismo procedimiento para diferentes alturas :math:`h`.
   #. Repita los procedimientos de los incisos 1 y 2 cambiando la naturaleza de la esfera o la superficie de la mesa

.. figure:: /images/Mecanica/Coeficiente_Restitucion/Gui_Rest_Coeff_01.png
   :scale: 80
   :align: center
   :name: fig:Gui_Rest_Coeff_01

   Arreglo experimental para determinar :math:`\varepsilon`.



**Análisis**

   #. ¿Depende :math:`\varepsilon`  de la naturaleza de la superficie con la cual choca la esfera ? Justifique su respuesta
   #. ¿Por qué razón la esfera finalmente se detiene después de múltiples choques con la superficie?



.. [#f1] Audacity es un editor y grabador de audio multipista fácil de usar para Windows, macOS, GNU / Linux y otros sistemas operativos
