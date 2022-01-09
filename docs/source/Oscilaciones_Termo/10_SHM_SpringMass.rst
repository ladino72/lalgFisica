Movimiento armónico simple: Sistema masa resorte
=================================================

**Objetivo**

El propósito principal de esta práctica es determinar la dependencia del periodo de oscilación de un sistema masa-resorte de la masa del cuerpo que pende y la constante elástica del resorte.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/masses-and-springs/latest/masses-and-springs_es.html <https://phet.colorado.edu/sims/html/masses-and-springs/latest/masses-and-springs_es.html>`_.

**Resumen teórico**

Se denomina movimiento armónico simple a aquel movimiento periódico donde la aceleración :math:`a` de la partícula es proporcional a su desplazamiento
:math:`x`, es decir

.. math::
   :label: Ec:S_M_1

   \begin{equation}
    a=\frac{d^{2}x}{dt^{2}}=-\omega ^{2}x
   \end{equation}

el valor :math:`\omega ` es una constante que depende de las propiedades del sistema y se relaciona con el período :math:`T` del movimiento mediante la expresión

.. math::
   :label: Ec:S_M_2

    \begin{equation}
      T=\frac{2\pi }{\omega }
    \end{equation}

La solución de la ecuación :eq:`Ec:S_M_1` es

.. math::
   :label: Ec:S_M_3

   \begin{equation}
    x(t)=A\sin (\omega t+\phi )
   \end{equation}

donde :math:`A` y :math:`\phi` son constantes que dependen de la forma como el sistema
se puso a oscilar inicialmente.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Gui_spring-mass` muestra la interfaz gráfica del usuario que permite estudiar la dependencia del periodo de oscilación de su sistema masa-resorte de la masa del cuerpo y la constante elástica del resorte. El sistema oscila de manera vertical y las fuerzas de fricción se desprecian. La interfaz permite fijar los valores de la masa :math:`m` y la dureza del resorte **Masa** y **Constante del resorte**. Se puede escoger cualquiera de los dos resortes.
La interfaz proporciona dos herramientas: una regla graduada en centímetros y un cronómetro. La masa se pone a oscilar simplemente al suspender una cualquiera de las masas. La interfaz permite señalar la longitud natural del resorte, la posición de equilibrio al seleccionar las opciones **Longitud natural - - -** y **Posición de Equilibrio - - -**. La interfaz también permite seleccionar entre resortes cortos y largos.

La animación se puede detener y poner en marcha de nuevo de dos maneras: de manera continua al presionar el botón :math:`\blacktriangleright` o de manera pausada con el botón :math:`\mid\blacktriangleright` respectivamente. Los botones :math:`\rhd` y :math:`\blacktriangleright` del cronómetro y de la interfaz, se pueden sincronizar de modo que al hacer clic en el primero y luego en el segundo, el cronómetro se pone en marcha tan pronto como se inicia el movimiento, esta opción es útil para la medición del periodo de oscilación.

.. figure:: /images/Oscilaciones_Termo/SHM_SimplePendulum/Gui_spring-mass.png
   :alt:
   :scale: 80
   :align: center
   :name: fig:Gui_spring-mass

   Interfaz gráfica del usuario.

**Mediciones y Procedimientos**

Se asumirá una dependencia de la forma :math:`T=2\pi\frac{m^{\alpha}}{k^{\beta}}`. El propósito es determinar :math:`\alpha` y :math:`\beta`.

.. _S_M_sec_T_m:

**Relación entre** :math:`T` y :math:`m`

   #. Fije el valor de la constante elástica del resorte en el máximo valor posible. Suspenda del resorte valores diferentes de masa, y para cada una de ellas desplácela 10 cm hacia abajo medida desde la posición de equilibrio y libérela, mida el periodo de las oscilaciones. Para ello, cronometre el tiempo :math:`\Delta T` transcurrido en realizar :math:`N` oscilaciones completas, el periodo de una oscilación es :math:`T=\frac{\Delta T}{N}`. Complete la :numref:`tab:S_M_T_v_m`.
   #. A partir de la tabla de datos del inciso 1 construya una gráfica de :math:`T` en función de :math:`m`.
   #. Utilice sus conocimientos de linealización de una función para determinar la relación matemática entre :math:`T` y :math:`m` al encontrar el valor de :math:`\alpha`.

      .. csv-table:: Datos para determinar la relación entre :math:`T` y :math:`m`
         :header: "Masa, :math:`m` (m)", "Periodo, :math:`T` (s)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:S_M_T_v_m
         :align: center

         0.050,.
         0.100,.
         0.250,.

.. _S_M_sec_T_k:

**Relación entre** :math:`T` y :math:`k`

   #. Seleccione el menor valor de la constante elástica del resorte. Para determinar su valor, suspenda un cuerpo de masa conocida y mida la elongación :math:`\Delta x` del resorte una vez que el sistema se encuentre en equilibrio; el valor de la constante elástica del resorte es :math:`k=\frac{mg}{\Delta x}`
   #. Mantenga el mismo valor de masa suspendida en las siguientes mediciones. Varíe el valor de la constante elástica :math:`k` del resorte. Una vez alcanzado el equilibrio desplace la masa hacia abajo 10 mm y libérela. Mida el correspondiente periodo de oscilación con la ayuda del cronómetro para cada valor de :math:`k`. Complete la :numref:`tab:S_M_T_v_k`

      .. csv-table:: Datos para determinar la relación entre :math:`T` y :math:`k`
         :header: "Masa, :math:`m` (m)", "Periodo, :math:`T` (s)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:S_M_T_v_k
         :align: center

         .,.
         .,.
         .,.
         .,.
         .,.

   #. A partir de la tabla de datos del inciso 2 construya una gráfica de :math:`T` en función de :math:`k`.
   #. Utilice sus conocimientos de linealización de una función para determinar la relación matemática entre :math:`T` y :math:`k` al encontrar el valor de :math:`\beta`.


   #. De los resultados anteriores escriba la dependencia de :math:`T` con :math:`k` y :math:`m`.
   #. Use sus conocimientos de análisis dimensional para demostrar que :math:`\alpha=1/2` y :math:`\beta=1/2`. Compare sus resultados obtenidos en los apartados :ref:`Relación entre T y m <S_M_sec_T_m>` y :ref:`Relación entre T y k <S_M_sec_T_k>`  con los valores :math:`\gamma=\beta=\frac{1}{2}`. ¿A qué se debe la discrepancia?

**Preguntas}**

Basado en los datos de la simulación y las ecuaciones que relacionan las variables :math:`T`, :math:`m` y :math:`k`.

   #. ¿Qué sucede con el periodo de oscilación en el sistema masa-resorte si la masa se duplica?
   #. ¿Qué sucede con el periodo de oscilación en el sistema masa-resorte si la masa se triplica?
   #. ¿Qué sucede con el periodo de oscilación en el sistema masa-resorte si la constante elástica del resorte se duplica?
   #. ¿Qué sucede con el periodo de oscilación en el sistema masa-resorte si la constante elástica del resorte se triplica?
   #. ¿Qué sucede con el periodo de oscilación en el sistema masa-resorte si tanto la masa y  la constante elástica del resorte se duplican?
   #. ¿Depende el periodo de oscilación del sistema masa-resorte del lugar (tierra, luna, júpiter) donde oscile el sistema?

