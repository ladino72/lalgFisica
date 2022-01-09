Movimiento armónico simple: Peńdulo simple
==========================================

**Objetivo**

El propósito principal de esta práctica es investigar la dependencia del periodo de oscilación de un péndulo simple de la longitud de la cuerda, la masa del cuerpo que pende y el valor de la aceleración de la gravedad. El péndulo realiza pequeñas oscilaciones y se desprecia la fricción.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/pendulum-lab/latest/pendulum-lab_es.html <https://phet.colorado.edu/sims/html/pendulum-lab/latest/pendulum-lab_es.html>`_.

**Resumen teórico**

Se denomina movimiento armónico simple a aquel movimiento periódico  donde la aceleración :math:`\alpha` de la partícula es proporcional a su desplazamiento
:math:`\theta`, es decir

.. math::
   :label: Ec:Simp_Pend_1

   \begin{equation}
    \alpha=\frac{d^{2}\theta}{dt^{2}}=-\omega ^{2}\theta
   \end{equation}

el valor :math:`\omega ` es una constante que depende de las propiedades del
sistema y se relaciona con el período :math:`T` del movimiento mediante la
expresión

.. math::
   :label: Ec:Simp_Pend_2

   \begin{equation}
    T=\frac{2\pi }{\omega }
   \end{equation}

La solución de la ecuación :eq:`Ec:Simp_Pend_1` es

.. math::
   :label: Ec:Simp_Pend_3

   \begin{equation}
     \theta(t)=\Theta\sin (\omega t+\phi )  \label{Ec:Simp_Pend_3}
   \end{equation}

donde :math:`\Theta` y :math:`\phi` son constantes que dependen de la forma como el sistema se puso a oscilar inicialmente.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Gui_simple_pend` muestra la interfaz gráfica del usuario que permite estudiar la dependencia del periodo de oscilación del péndulo simple con la longitud de la cuerda, la masa del cuerpo que cuelga de la cuerda y la aceleración de la gravedad. La interfaz permite fijar los valores de la masa :math:`M` y longitud :math:`L` del péndulo mediante las barras de desplazamiento rotuladas como **Masa** y **Longitud**. De igual manera, los valores de la aceleración de la gravedad donde oscila el péndulo y la fuerza de fricción sobre la masa se fijan con las barras de desplazamiento rotuladas como **Gravedad** y **Fricción** respectivamente. La interfaz proporciona dos herramientas: una regla graduada en centímetros y un cronómetro. El péndulo se pone a oscilar simplemente desplazando la masa de la posición de equilibrio al arrastrar la masa hacia la izquierda o derecha con el puntero del ratón y liberándola. La animación se puede detener y ponerla en marcha de nuevo de dos maneras: de manera continua al presionar el botón :math:`\blacktriangleright` o de manera pausada con el botón :math:`\mid\blacktriangleright` respectivamente. Los botones :math:`\rhd` y :math:`\blacktriangleright` del cronómetro y de la interfaz, se pueden sincronizar de modo que al hacer clic en el primero y luego en el segundo, el cronómetro se pone en marcha tan pronto como se inicia el movimiento, esta opción es útil para la medición de periodos de oscilación.

.. figure:: /images/Oscilaciones_Termo/SHM_SimplePendulum/Gui_simple_pendulum.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:Gui_simple_pend

   Interfaz gráfica del usuario.

**Mediciones y Procedimientos**

Se asumirá una dependencia de la forma :math:`T=2\pi\frac{\ell^{\alpha}}{m^{\gamma}g^{\beta}}`. El propósito es determinar :math:`\alpha`, :math:`\beta` y :math:`\gamma`. Para cada una de las situaciones que se consideran a continuación cuando ponga a oscilar el péndulo, desplace la masa de su posición de equilibrio a un ángulo de 15 :math:`^{\circ}` y libérela (pequeñas oscilaciones).

**Relación entre** :math:`T` y :math:`\ell`

   #. Asegúrese de seleccionar Gravedad: Tierra y fricción: Ninguna
   #. Seleccione el valor de la masa del cuerpo igual a 0.1 kg
   #. Varíe la longitud de la cuerda desde 10 cm hasta 100 cm en pasos de 10 cm y mida el correspondiente periodo de oscilación con la ayuda del cronómetro para cada longitud :math:`\ell` de la cuerda. Para mayor exactitud cronometre el tiempo de 10 oscilaciones y divida entre 10 después para hallar :math:`T`. Registre sus valores en la :numref:`tab:Simp_Pend_T_v_L`.
   #. A partir de la tabla de datos del inciso 2 construya una gráfica de :math:`T` en función de :math:`\ell`.
   #. Utilice sus conocimientos de linealización de una función para determinar la relación matemática entre :math:`T` y :math:`\ell` al encontrar el valor de :math:`\alpha`.

      .. csv-table:: Datos para determinar la relación entre :math:`T` y :math:`\ell`
         :header: "Longitud, :math:`\\ell` (m)", "Periodo, :math:`T` (s)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Simp_Pend_T_v_L
         :align: center

         0.10,.
         0.20,.
         0.30,.
         0.40,.
         0.50,.
         0.60,.
         0.70,.
         0.80,.
         0.90,.
         1.00,.

**Relación entre** :math:`T` y :math:`m`

   #. Asegúrese de seleccionar Gravedad: Tierra y fricción: Ninguna.
   #. Seleccione el valor de la longitud de la cuerda igual a 50 cm.
   #. Varíe el valor de la masa :math:`m` del cuerpo desde 0.1 kg hasta 1.5 kg en incrementos de 0.3 kg y mida el correspondiente periodo de oscilación con la ayuda del cronómetro para cada valor de masa. Para mayor exactitud cronometre el tiempo de 10 oscilaciones y divida entre 10 después para hallar :math:`T`. Registre sus valores en la :numref:`tab:Simp_Pend_T_v_m`.
   #. A partir de la tabla de datos del inciso 3 construya una gráfica de :math:`T` en función de :math:`m`.
   #. Utilice sus conocimientos de linealización de una función para determinar la relación matemática entre :math:`T` y :math:`m` al encontrar el valor de :math:`\gamma`.

      .. csv-table:: Datos para determinar la relación entre :math:`T` y :math:`m`
         :header: "Masa, :math:`m` (kg)", "Periodo, :math:`T` (s)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Simp_Pend_T_v_m
         :align: center

         0.2,.
         0.4,.
         0.6,.
         0.8,.
         1.0,.
         1.2,.
         1.4,.

   #. Use sus conocimientos de análisis dimensional para demostrar que en el caso de pequeñas oscilaciones :math:`\gamma=0` y :math:`\beta=1/2`. Compare su resultado obtenido en el inciso 5 con el valor :math:`\gamma=0`. ¿A qué se debe la discrepancia?
   #. De los resultados anteriores escriba la dependencia de :math:`T` con :math:`\ell`, :math:`g` y :math:`m`.
   #. A partir de la relación obtenida para :math:`T` en el inciso 7 determine el valor de la aceleración de la gravedad en la luna, Júpiter y el planeta X. Para los dos primeros casos, compare estos valores con los que arroja el simulador y los reportados en la literatura (:math:`g_{luna}=1.625\,\text{m/s}^{2}`, :math:`g_{jupiter}=24.79\,\text{m/s}^{2}`). Explique las posibles discrepancias.



