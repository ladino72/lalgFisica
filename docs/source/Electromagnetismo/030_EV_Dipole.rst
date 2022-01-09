Campo eléctrico, potencial eléctrico y lineas equipotenciales
==============================================================

**Objetivo**

El propósito de esta práctica es estudiar las líneas de campo eléctrico y líneas equipotenciales de diferentes configuraciones de cargas eléctricas puntuales. En particular se considera el dipolo eléctrico.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/sims/html/charges-and-fields/latest/charges-and-fields_en.html <https://phet.colorado.edu/sims/html/charges-and-fields/latest/charges-and-fields_en.html>`_.

**Resumen teórico**

Los campos eléctricos son producidos por cargas eléctricas (positivas o negativas) y su dependencia de las coordenadas espaciales depende de cómo se encuentren distribuidas éstas. En general, el campo eléctrico generado por cualquier distribución de carga eléctrica se puede considerar como la suma de los campos generados por configuraciones elementales de carga eléctrica como son el monopolo, dipolo, cuadrupolo, sextupolo, octopolo eléctricos, etc. Cada una de estas configuraciones juega un papel importante en la explicación del comportamiento de la materia. Por ejemplo, el dipolo eléctrico está formado por dos cargas iguales de signo contrario separadas una distancia :math:`d` muy pequeña, ver :numref:`fig:dipolo`. Se define el momento dipolar eléctrico como :math:`\overrightarrow{p}`, que va de la carga negativa a la positiva y su magnitud es :math:`qd`. Si el punto :math:`p`, se encuentra a gran distancia de las cargas, es decir, si :math:`r>>d`, las componentes radial y tangencial del campo eléctrico vienen dadas por

.. figure:: /images/Electromagnetismo/EV_Dipole/dipolo.png
   :scale: 60
   :align: center
   :name: fig:dipolo

   Dipolo eléctrico

.. math::
   :label: Ec:Dipolo_1

   \begin{equation}
    E_r =\frac{2p\cos\theta}{4\pi\varepsilon_0r^{3}}
   \end{equation}

.. math::
   :label: Ec:Dipolo_2

   \begin{equation}
    E_t = \frac{p\sin\theta}{4\pi\varepsilon_0r^{3}}
   \end{equation}

El potencial eléctrico asociado al campo anterior es dado por

.. math::
   :label: Ec:Dipolo_3

   \begin{equation}
    V=\frac{p\cos\theta}{4\pi\varepsilon_0r^{2}}
   \end{equation}


A pesar de que la carga total de una molécula es cero, la naturaleza de los enlaces químicos es tal que las cargas positivas y negativas no se solapan por completo en la mayoría de las moléculas. Dichas moléculas se dice que son polares debido a que poseen un momento dipolar permanente. Un buen ejemplo lo constituye la molécula de agua. El momento dipolar del agua proporciona una ``facilidad`` para la interacción con los campos eléctricos de microondas en un horno microondas. Las microondas pueden añadir energía a las moléculas del agua, mientras que las moléculas sin momento dipolar, quedarán inafectadas.


**Descripción de la interfaz de la aplicación**

La :numref:`fig:Dipolo_gui_05` muestra la interfaz gráfica del usuario. Esta permite colocar sobre la grilla tantas cargas puntuales como deseemos de valor 1.0 nC, para ello simplemente arrastre las cargas con el ratón a la posición deseada. Al seleccionar los botones **Electric Field** y **Direction only** podemos visualizar las direcciones del campo eléctrico en diferentes puntos del espacio. Si deseamos conocer el valor y dirección del campo eléctrico en un punto determinado, simplemente arrastramos el sensor (punto amarillo) ubicado en la parte inferior de la pantalla (junto a las cargas eléctricas)  y lo colocamos en el punto de interés. El valor del potencial eléctrico en cualquier punto de la grilla se puede determinar con el sensor denominado **Equipotencial**. Al presionar el lápiz de este sensor se traza de manera automática la línea equipotencial, es decir, el conjunto de puntos que se encuentran al mismo potencial eléctrico con respecto al infinito. La interfaz permite usar una grilla cuyo cuadrado más pequeño tiene dimensiones de 10 cm por 10 cm.

.. figure:: /images/Electromagnetismo/EV_Dipole/GUI_05.png
   :scale: 50
   :align: center
   :name: fig:Dipolo_gui_05

   Interfaz gráfica del usuario

**Mediciones y procedimientos**

   #. Coloque una única carga positiva en el centro de la pantalla. Con los sensores apropiados, tome datos que permitan demostrar que la magnitud del campo eléctrico generado por la carga :math:`q=1.0\,\text{nC}` decrece con el inverso del cuadrado de la distancia del punto de interés a la carga.
   #. Usando la misma configuración anterior, tome datos que permitan demostrar que el potencial eléctrico generado por la carga eléctrica varía con el inverso de la distancia del punto de interés a la carga.
   #. Use la herramienta **Equipotencial** y verifique que las líneas equipotenciales son circunferencias con centro en la carga eléctrica. ¿Qué puede concluir acerca de la dirección del campo eléctrico con respecto a la dirección de las líneas equipotenciales?  ¿Será que su respuesta es válida en general para cualquier número de cargas? Para verificar esto, coloque varias cargas positivas negativas (la cantidad no interesa) sobre la pantalla y trace tantas líneas equipotenciales como desee. ¡Observe, que las líneas equipotenciales no se cruzan entre sí! ¿Si se cruzaran, que implicaciones físicas se tendrían?

      a. Forme un dipolo sobre la pantalla como se indica en la :numref:`fig:dipole_01`. Demuestre a partir de datos adquiridos en el simulador que la componente tangencial :math:`E_t` del campo eléctrico depende del inverso del cubo de la distancia :math:`r` medida desde el punto de interés al centro de las cargas.  Para medir :math:`E_t`, coloque el sensor a lo largo del eje :math:`y`, (:math:`\theta=90^{o}`) para :math:`r=y>>d`, tal como indica la figura (lectura del sensor: 2.56 V/m = 2.56 N/C).
      b. Forme un dipolo sobre la pantalla como se indica en la :numref:`fig:dipole_01`. Demuestre a partir de datos adquiridos en el simulador que la componente radial :math:`E_r` del campo eléctrico depende del inverso del cubo de la distancia :math:`r` medida desde el punto de interés al centro de las cargas. Para medir :math:`E_r`, coloque el sensor a lo largo del eje :math:`x`, :math:`\theta=0` para :math:`r=x>>d`, tal como indica la figura (lectura del sensor: 2.17 V/m = 2.17 N/C).
      c. Forme un dipolo sobre la pantalla como se indica en la :numref:`fig:dipole_01`. Demuestre a partir de datos adquiridos en el simulador que el potencial eléctrico generado por el dipolo eléctrico depende del inverso del cuadrado de la distancia del punto de interés al centro de las cargas para :math:`r>>d`.
      d. La configuración de carga mostrada en la :numref:`fig:quadrupole_01` se denomina un cuadrupolo eléctrico. Trace las líneas de campo eléctrico de esta configuración a igual que algunas líneas equipotenciales. Investigue la importancia de esta configuración en el campo de la física nuclear.

.. figure:: /images/Electromagnetismo/EV_Dipole/dipole_01.png
   :scale: 70
   :align: center
   :name: fig:dipole_01

   Determinación de la dependencia de :math:`E` on :math:`r` en el dipolo eléctrico


.. figure:: /images/Electromagnetismo/EV_Dipole/qradrupole.png
   :scale: 60
   :align: center
   :name: fig:quadrupole_01

   Cuadrupolo eléctrico




