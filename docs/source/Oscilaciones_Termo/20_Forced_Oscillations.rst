Oscilaciones forzadas en el sistema masa resorte
======================================================

**Objetivo**

El propósito de esta práctica es estudiar el fenómeno de la resonancia en un sistema masa-resorte que realiza oscilaciones verticales al mover su punto de suspensión armónicamente. Se asume que la fuerza :math:`f` de rozamiento sobre la masa es proporcional a su velocidad :math:`v`, es decir :math:`f=-bv`, donde :math:`b` es la constante de amortiguamiento. A partir de las mediciones de la frecuencia de excitación, la amplitud de las oscilaciones  y del modelo desarrollado en la guia se encuentra el valor de :math:`b`.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://www.walter-fendt.de/html5/phen/resonance_en.htm <https://www.walter-fendt.de/html5/phen/resonance_en.htm>`_.

**Resumen teórico**

Los sistemas tanto mecánicos como eléctricos manifiestan un fenómeno interesante cuando estos son perturbados por fuerzas o señales periódicas. La respuesta de estos sistemas crece notablemente cuando la frecuencia de excitación aplicada es próxima a la frecuencia natural de ellos. La frecuencia para la cual la respuesta es máxima se denomina frecuencia de resonancia. Entre menos rozamiento tengan estos sistemas, la frecuencia de resonancia tiende a coincidir con la frecuencia natural. Los sistemas mecánicos simples tales como el sistema masa-resorte poseen una frecuencia de resonancia que depende de la masa, constante elástica del resorte y la resistencia que ofrezca el medio al movimiento de la masa. Los sistemas complejos  pueden tener varias frecuencias de resonancia.


**Descripción del problema**

Consideremos el sistema mostrado en la :numref:`fig:SM_Forced_osc_00`, el cual consta de una masa :math:`m`  conectada a un resorte ligero de constante elástica :math:`k` y longitud natural :math:`x_0`; el extremo superior del resorte pende del punto :math:`p` que se mueve verticalmente y realiza oscilaciones armónicas con frecuencia :math:`\omega` y amplitud :math:`\eta_0` con respecto al punto fijo :math:`o`, es decir :math:`\eta(t)=\eta_0\cos \omega t`.

Las fuerzas que actuan sobre la masa se indican en la :numref:`fig:SM_Forced_osc_02`; donde :math:`F` es la fuerza elástica del resorte dada por :math:`F=-k(z-\eta-x_0)` y :math:`f=-b\frac{dz}{dt}` es la fuerza de rozamiento sobre la masa, siendo :math:`b`  la constante de amortiguamiento. La posición vertical de la masa se denota por la variable :math:`x` y su posición de equilibrio es :math:`x_1=\frac{mg}{k}+x_0`, la cual se deriva de la condición :math:`mg=k(x_1-x_0)`.

.. figure:: /images/Oscilaciones_Termo/Forced-Oscillations/Forced_oscilations_00.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:SM_Forced_osc_00

   Arreglo experimental para determinar la constante de amortiguamiento del sistema masa-resorte forzado cuyo punto de suspensión realiza oscilaciones armónicas con frecuencia :math:`\omega` y amplitud :math:`\eta_0`




.. figure:: /images/Oscilaciones_Termo/Forced-Oscillations/Forced_oscilations_02.png
   :alt:
   :scale: 90
   :align: center
   :name: fig:SM_Forced_osc_02

   Fuerzas y coordenadas sobre la masa del sistema masa-resorte.

Al aplicar la segunda ley de Newton a la masa :math:`m` en sentido vertical, una vez que el punto :math:`p` se encuentra en movimiento resulta:

.. math::
   :label: Ec:Forced_Osc_01

   \begin{equation}
    -mg-k(z-\eta-x_0)-b\frac{dz}{dt}=m\frac{d^{2}z}{dt^{2}}
   \end{equation}

o

.. math::
   :label: Ec:Forced_Osc_02

    \begin{equation}
        \frac{d^{2}z}{dt^{2}}+\frac{b}{m}\frac{dz}{dt}+\frac{k}{m}(z-x_0-\frac{mg}{k})=\frac{k}{m} \eta
    \end{equation}

al definir :math:`y=z-x_0-\frac{mg}{k}=z-x_1`, :math:`\omega_0^{2}=\frac{k}{m}`, :math:`2\lambda=\frac{b}{m}` y teniendo en cuenta que :math:`\eta(t)=\eta_0\cos \omega t`, la ecuación :eq:`Ec:Forced_Osc_02` se convierte en:

.. math::
   :label: Ec:Forced_Osc_03

   \begin{equation}
    \frac{d^{2}y}{dt^{2}}+ 2\lambda\frac{dy}{dt}+\omega_0^{2}y=\omega_0^{2} \eta_0\cos\omega t
   \end{equation}

la solución de la ecuación :eq:`Ec:Forced_Osc_03` en el régimen estacionario viene dada por:

.. math::
   :label: Ec:Forced_Osc_04

   \begin{equation}
     x(t)=A(\omega)\cos(\omega_0 t-\phi)
   \end{equation}

donde

.. math::
   :label: Ec:Forced_Osc_05

   \begin{equation}
    A(\omega)=\frac{\omega_0^{2}\eta_0}{\sqrt{(\omega_0^{2}-\omega^{2})^{2}+(2\lambda\omega)^{2}}}
   \end{equation}

y

.. math::
   :label: Ec:Forced_Osc_06

   \begin{equation}
    \tan\phi=\frac{2\lambda\omega}{\omega_0^{2}-\omega^{2}}
   \end{equation}

Obsérvese que tanto la amplitud :math:`A` de las oscilaciones resultantes como la fase :math:`\phi` dependen de la frecuencia angular :math:`\omega` del punto de suspensión :math:`p` del resorte.
Se puede demostrar que la amplitud :math:`A` presenta un máximo cuando :math:`\omega = \sqrt{\omega_0^{2}-2\lambda^{2}}=\sqrt{\frac{k}{m}-\frac{b^{2}}{2m^{2}}}`. Es decir, la frecuencia en Hertz para la cual la amplitud es máxima viene dada por:

.. math::
   :label: Ec:Forced_Osc_07

   \begin{equation}
    f_r= \frac{1}{2\pi}\sqrt{\frac{k}{m}-\frac{b^{2}}{2m^{2}}}
   \end{equation}

la cual se denomina frecuencia de resonancia del sistema.


**Mediciones**

La :numref:`fig:SM_Forced_osc_03` muestra la interfaz gráfica del usuario que perimite la simulación de las oscilaciones forzadas. Fije los valores del sistema masa-resorte igual a :math:`k=9` N/m y :math:`m=1` kg. Tomaremos como constante de amortiguamiento :math:`b=0.2` kg/s. La amplitud :math:`\eta=2.0\,\text{cm}` de las oscilaciones del punto de suspensión del resorte es fija (no se puede variar). Varíe la frecuencia :math:`\omega` del punto de suspensión del resorte en el rango [0..8] rad/s en pasos de 0.5 y registre el valor de la amplitud :math:`A` de las oscilaciones en la :numref:`tab:SM_forced_osc`.

.. figure:: /images/Oscilaciones_Termo/Forced-Oscillations/FO_GUI.png
   :alt:
   :scale: 75
   :align: center
   :name: fig:SM_Forced_osc_03

   Interfaz gráfica del usuario


.. csv-table:: Datos medidos de :math:`\omega` y :math:`A`
   :header: "Frecuencia :math:`\\omega` (rad/s)", "Amplitud, :math:`A` (cm)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:SM_forced_osc
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
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.
   .,.


.. figure:: /images/Oscilaciones_Termo/Forced-Oscillations/Force_Oscilations_fase.png
   :alt:
   :scale: 70
   :align: center
   :name: fig:SM_Forced_osc_04

   Fase :math:`\phi` en función de la frecuencia angular :math:`\omega`

**Procedimiento**

   #. A partir de los datos de la :numref:`tab:SM_forced_osc` grafique :math:`A` en función de :math:`\omega` y compruebe que los datos se ajustan a la ecuación :eq:`Ec:Forced_Osc_05`.
   #. Determine el valor de la frecuencia :math:`\omega_r` para el cual la amplitud de las oscilaciones es máxima. Compare este valor con el dado por la ecuación :eq:`Ec:Forced_Osc_07`
   #. Grafique :math:`Y` como función de :math:`X` donde :math:`Y=A^{2}(\omega_0^{2}-\omega^{2})^{2}` y :math:`X=\omega^{2}A^{2}`. A partir de la gráfica obtenida encuentre los valores de la pendiente :math:`p` y punto de corte :math:`q` con el eje vertical. A partir de los valores de :math:`p` y :math:`q`  encuentre los valores de la constante de amortiguamiento :math:`b` y el valor de la amplitud :math:`\eta_0` de las oscilaciones del punto :math:`p`. Compare estos valores con los establecidos inicialmente.
   #. A partir de los datos de la :numref:`tab:SM_forced_osc` demuestre que la fase :math:`\phi`  es la que se muestra en la :numref:`fig:SM_Forced_osc_04`.
   #. Discuta sus resultados y escriba sus conclusiones.

**Lectura complementaria**

Si estamos en un mundo sometido continuamente a fuerzas oscilantes, y si además estamos rodeados de estructuras
elásticas tales como ventanas, puentes, edificios, etc., es factible que en muchos casos la frecuencia de las fuerzas
oscilantes coincida con alguna de las frecuencias naturales de las estructuras elásticas provocando fenómenos de
resonancia. Veamos algunos ejemplos [#f4]_.

   #. Cuando decenas o cientos de soldados marchan dando golpes rítmicos de frecuencia muy constante en el piso, al cruzar sobre un puente, que como se ha señalado es una estructura elástica con sus propias frecuencias naturales de vibración, en caso de que conserven su marcha acompasada se corre el peligro de que su frecuencia de golpeteo (aproximadamente de 1 Hz) coincida con alguna de las frecuencias naturales del puente; hay que tomar en cuenta además que la fuerza del golpe colectivo puede alcanzar magnitudes de decenas de miles de N, para evitar ese peligro es que a las formaciones de soldados se les ordena romper la marcha cuando cruzan un puente.
   #. Es una experiencia común que cuando se escucha música dentro de un cuarto, algunas veces al aparecer sonidos de frecuencia muy baja los vidrios de las ventanas empiezan a vibrar violentamente. Esto ocurre, naturalmente, porque hay un fenómeno de resonancia, ya que en tales casos la frecuencia de los sonidos graves coincide con alguna de las frecuencias naturales de oscilación de los vidrios de las ventanas.
   #. Los autos están hechos de muchas partes elásticas, como por ejemplo el volante, la palanca de velocidades, los vidrios de las ventanas, etc.; de hecho, cuando al volante se le da un golpe, se siente inmediatamente su vibración; pues bien, cuando el motor genera vibraciones que coinciden con la frecuencia natural de vibración de algunas de estas partes sucede el fenómeno de resonancia; es por ello que los diseñadores de las carrocerías deben tener en cuenta que la potente fuente de vibraciones del motor no provoque la coincidencia con las frecuencias naturales de los diversos componentes de los automotores.
   #. El cuerpo humano está conformado por estructuras elásticas como son los huesos, y es así que en el mundo de la medicina laboral se debe cuidar que la frecuencia de golpeteo de máquinas como los taladros que rompen las capas de pavimento, no coincida con la frecuencia natural de algunas de las partes de la estructura ósea. Cuando el cuerpo humano está sometido a vibraciones de baja frecuencia, éste se mueve como un todo, pero a frecuencias altas la respuesta del cuerpo es específica; así de 4 a 12 Hz las caderas y los hombros comienzan a resonar, entre 20 y 30 Hz es el cráneo el que resuena, a frecuencias más altas de 60 a 90 Hz son los globos oculares los que pueden entrar en resonancia [#f2]_.
   #. Un caso muy conocido de resonancia es cuando un o una cantante dirigen su voz hacia una copa de cristal; es aparente que la copa es una estructura elástica que vibra a frecuencias claramente reconocibles por el oído humano, por tanto, el afinado oído de los cantantes se entona con esos sonidos y lanza contra la copa un sonido potente de la misma frecuencia, con ello se forman en la copa ondas estacionarias, y si la intensidad y la frecuencia se mantienen el tiempo suficiente, se produce el fenómeno de resonancia hasta que la copa a causa de sus intensas vibraciones se rompe.
   #. En el mundo animal se tienen también ejemplos muy hermosos de resonancia; por ejemplo ¿cómo pueden los mosquitos machos detectar a los mosquitos hembras? De acuerdo a H. Schmidt  [#f3]_, las frecuencias de aleteo de los machos y las hembras son diferentes; los machos aletean a una frecuencia aproximada de 500 Hz, mientras que las hembras lo hacen a una frecuencia aproximada de 300 Hz; pues bien, se encuentra que las antenas de los machos tienen una frecuencia natural de vibración muy cercana a los 300 Hz, por tanto, el aleteo de las hembras provoca en ellos resonancia de sus antenas y es así como se efectúa el reconocimiento.

.. [#f2] http://www.fio.unicen.edu.ar/usuario/segumar/Laura/material/Vibraciones.pdf.

.. [#f3] Schmid, H., Cómo se comunican los animales, (Salvat,España, 1986).

.. [#f4] Peralta et al. El fenómeno de la resonancia. Lat. Am. J. Phys. Educ. Vol. 3, No. 3, Sept. 2009


