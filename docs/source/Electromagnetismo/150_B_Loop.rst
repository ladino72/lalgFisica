+Campo magnético creado por una espira circular con corriente directa y alterna
===============================================================================

**Objetivo**

El propósito de esta práctica es determinar la dependencia de la magnitud del campo magnético  creado por una espira circular con corriente DC y AC de la posición en puntos sobre un eje que pasa por su centro y es perpendicular al plano que la contiene.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://phet.colorado.edu/en/simulation/magnets-and-electromagnets <https://phet.colorado.edu/en/simulation/magnets-and-electromagnets>`_.

**Resumen teórico**

Las cargas eléctricas en movimiento generan corrientes eléctricas. La corriente eléctrica a su vez genera un campo magnético cuya magnitud y dirección están dados por la ley de Biot y Savart. Esta ley afirma que para un conductor de longitud :math:`d\overrightarrow{l}` y corriente :math:`I`, (ver :numref:`fig:B_Loop_01`) el campo magnético :math:`d\overrightarrow{B}` en el punto `P` a una distancia `r` es dado por

.. figure:: /images/Electromagnetismo/B_Loop/Loop_mffig6.png
   :scale: 120
   :align: center
   :name: fig:B_Loop_01

   Espira de corriente. La dirección del campo magnético creado por el elemento de longitud :math:`dl` y corriente :math:`I` es determinada por la dirección de :math:`dl \times \widehat{u}_{r}`


.. math::
   :label: Ec:B_Loop1

   \begin{equation}
     d \overrightarrow{B}=\frac{\mu _{0}I}{4\pi }\frac{d\overrightarrow{l}\times \widehat{u}_{r}}{r^{2}}
   \end{equation}

donde :math:`\mu _{0}=4\pi \times 10^{-7}\,\text{T}\, \cdot \text{m/A}` es la permeabilidad magnética del vacío. El campo de toda la espira con corriente, se obtiene a partir del principio de superposición. Es decir, debemos sumar vectorialmente los campos producidos por cada uno de los elementos de longitud infinitesimal que constituyen la espira.


**Descripción de la interfaz de la aplicación**

La :numref:`Gui_B_Loop_01` muestra la interfaz gráfica del usuario que permite estudiar el efecto de la corriente en el campo magnético de la espira. Desde la interfaz se puede seleccionar el tipo de corriente que circula por la(s) espira(s): corriente directa DC o alterna AC. Al seleccionar la batería, la polaridad y valor de la diferencia de potencial se fija al desplazar el botón hacia la izquierda o derecha en un rango comprendido entre 0 y 10 V. Si se selecciona la fuente de voltaje alterno, la amplitud y frecuencia de la señal se varían con los botones vertical y horizontal en forma porcentual respectivamente. El número de espiras 1, 2 o 3 se selecciona con el menú rotulado **Loops**.
La aplicación suministra un medidor de campo magnético móvil que permite leer las componentes cartesianas :math:`B_x` y :math:`B_y` del campo magnético en Gauss, al igual que su magnitud :math:`B` y el ángulo :math:`\theta` que forma con el eje horizontal. El fondo de la pantalla muestra una serie de agujas imantadas fijas igualmente espaciadas que se orientan de acuerdo al campo generado por la corriente circular. La aplicación también suministra una brújula movible.

.. figure:: /images/Electromagnetismo/B_Loop/Gui_B_Loop.png
   :scale: 50
   :align: center
   :name: Gui_B_Loop_01

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

.. _Relac_BVn:

**Corriente DC: Dependencia de** :math:`B` con :math:`V` y :math:`n`

   #. Varíe la dirección de la corriente en la espira al cambiar la polaridad de la pila. ¿Cuál es el efecto de la dirección de la corriente en la dirección del campo magnético? Utilice la brújula móvil para ver el efecto.
   #. Fije la espira de modo que su eje principal sea paralelo y superpuesto a una línea que pase por un conjunto de agujas imantadas horizontales y además en un punto donde la componente :math:`B_x` del campo magnético tome el mismo valor en puntos a igual distancia del centro a ambos lados de la espira, use el medidor de campo magnético para este fin.
   #. Coloque el medidor de campo en el centro de la espira :math:`x=0`. Varíe la diferencia de potencial :math:`V` de la batería entre 0 y +10 V sin cambiar su polaridad (-+) y registre los correspondientes valores :math:`B_x`. Registre sus mediciones en la :numref:`tab:B_Loop_01`.
   #. Realice una gráfica de :math:`B_x` en función de :math:`V` y aplique sus conocimientos de linealización de funciones para determinar la relación entre este par de variables.
   #. Sin cambiar la configuración anterior, repita los pasos de los incisos 3 y 4 pero esta vez con :math:`n=2` y :math:`n=3` espiras. Registre sus mediciones en la :numref:`tab:B_Loop_02` y la :numref:`tab:B_Loop_03`.


.. _Relac_Bx:

**Corriente DC: Dependencia de** :math:`B` con :math:`x`

   #. Fije la espira en el mismo lugar que utilizó en el inciso 2 de la sección :ref:`Corriente DC: Dependenceia de B con V <Relac_BVn>`.
   #. Fije el valor de la diferencia de potencial en 5V (-+). Asumiremos la distancia de separación entre las brújulas sobre el eje :math:`x` como unidad de longitud (u.l).  Coloque el medidor de campo magnético a diferentes distancias :math:`x` medidas desde el centro de la espira a lo largo de su eje y registre los correspondientes valores de :math:`B_x`. Registre sus mediciones en la :numref:`tab:B_Loop_04`.
   #. Realice una gráfica de :math:`B_x` en función de :math:`R^{2}(R^{2}+x^{2})^{-3/2}`, con :math:`R=\,1\,\text{u.l}`  y verifique que la relación es lineal.
   #. Sin cambiar la configuración anterior, repita los pasos de los incisos 2 y 3 pero esta vez con :math:`V=10\,\text{V}`. Registre sus mediciones en la :numref:`tab:B_Loop_05`.


**Corriente AC: Dependencia de** :math:`B` con :math:`I_0` y :math:`f`

Asumiremos que la corriente por la espira tiene la forma :math:`I=I_0\cos(2\pi f)` donde :math:`I_0` y :math:`f` representan la amplitud y la frecuencia. Nótese que no tenemos un medidor de tiempo, ni podemos leer los valores de :math:`I_0` y :math:`f` de manera absoluta, solo de manera relativa. Podemos medir tiempo de la siguiente manera: presione el botón de avance pausado :math:`|\triangleright` repetidas veces y cuente el número :math:`N` de pulsaciones requeridas para hacer que la línea roja vertical en la gráfica avance un periodo. Determine este número lo más exactamente posible. Así, el tiempo transcurrido desde un máximo (:math:`t=0`) a cualquier otro punto donde hemos tenido que realizar :math:`n_1` pulsaciones para llegar allí, está dado por :math:`t=\frac{n_1}{N}\frac{1}{f}`. Definimos nuestra unidad de tiempo (u.t) como :math:`\frac{1}{f}`.

   #. Aplique corriente alterna a la espira y observe el comportamiento del campo magnético.
   #. Fije :math:`f` en 10\% y :math:`I_0` en 50\%. Coloque el medidor de campo en el centro de la espira, :math:`x=0`. Registre la componente :math:`B_x` del campo magnético en función del tiempo durante un periodo de la corriente. Registre sus resultados en la :numref:`tab:Bx_t`.
   #. Use la misma posición del medidor de campo y frecuencia :math:`f` de la fuente del inciso 1. Varíe :math:`I_0` y registre el correspondiente valor del máximo valor de :math:`B_x` con la ayuda del botón de avance pausado :math:`|\triangleright`. Registre sus mediciones en la :numref:`tab:Bx_I_0`.
   #. Realice una gráfica de :math:`B_{x,max}` en función de :math:`I_0` y aplique sus conocimientos de linealización de funciones para determinar la relación entre este par de variables.
   #. Fije :math:`I_0` en 100\%,  coloque el medidor de campo en el centro de la espira, :math:`x=0` o cualquier otro punto que desee. Varíe la frecuencia :math:`f` y observe el comportamiento del campo magnético

      .. csv-table:: Diferencia de potencial V, componente x de campo magnético en el centro de la espira :math:`x=0`, n=1
         :header: "Dif. Pot, :math:`V` (V)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:B_Loop_01
         :align: center

         0,.
         1,.
         2,.
         3,.
         4,.
         5,.
         6,.
         7,.
         8,.
         9,.
         10,.

      .. csv-table:: Diferencia de potencial V , componente x de campo magnético en el centro de la espira :math:`x=0`, n=2
         :header: "Dif. Pot, :math:`V` (V)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:B_Loop_02
         :align: center

         0,.
         1,.
         2,.
         3,.
         4,.
         5,.
         6,.
         7,.
         8,.
         9,.
         10,.


      .. csv-table:: Diferencia de potencial V , componente x de campo magnético en el centro de la espira :math:`x=0`, n=3
         :header: "Dif. Pot, :math:`V` (V)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:B_Loop_03
         :align: center

         0,.
         1,.
         2,.
         3,.
         4,.
         5,.
         6,.
         7,.
         8,.
         9,.
         10,.

      .. csv-table:: Distancia x, componente x de campo magnético, :math:`V=5` V
         :header: "Distancia x, (u.l)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:B_Loop_04
         :align: center

         -7,.
         -6,.
         -5,.
         -4,.
         -3,.
         -2,.
         -1,.
         0,.
         1,.
         2,.
         3,.
         4,.
         5,.
         6,.
         7,.

      .. csv-table:: Distancia x, componente x de campo magnético, :math:`V=10` V
         :header: "Distancia x, (u.l)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:B_Loop_05
         :align: center

         -7,.
         -6,.
         -5,.
         -4,.
         -3,.
         -2,.
         -1,.
         0,.
         1,.
         2,.
         3,.
         4,.
         5,.
         6,.
         7,.

      .. csv-table:: Tiempo (u.t) y componente :math:`B_x` (G) en el centro de la espira.
         :header: "Tiempo :math:`B_x`, (u.t)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Bx_t
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

      .. csv-table:: :math:`I_0` y componente :math:`B_x` (G) en el centro de la espira.
         :header: "Amplitud :math:`I_0`, (%)", ":math:`B_x` (G)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Bx_I_0
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

**Análisis**

   #. Teniendo en cuenta los resultados de las secciones :ref:`Corriente DC: Dependenceia de B con V <Relac_BVn>` y :ref:`Corriente DC: Dependenceia de B con x <Relac_Bx>`, escriba una ecuación que muestre la dependencia de :math:`B` con :math:`V`, :math:`n` y :math:`x`.
   #. Escriba la expresión anterior en términos de la corriente :math:`I` de la espira. (Ayuda: utilice la ley de Ohm). Compare sus resultados con los del inciso 7 de esta sección.
   #. ¿Qué le sucede al campo magnético cuando la corriente por la espira es alterna? ¿Se encuentra la corriente en fase con el campo magnético?
   #. ¿Qué relación existe entre el campo magnético y la corriente DC?
   #. ¿Qué relación existe entre el campo magnético y la corriente AC?
   #. ¿Cuál es el efecto de la frecuencia de la corriente en el campo magnético?
   #. Use la ecuación :eq:`Ec:B_Loop1` y demuestre que para el caso de una espira circular de radio :math:`R` con corriente :math:`I` (ver :numref:`fig:B_Loop_mffig3`), el valor del campo magnético en un punto sobre su eje principal a una distancia :math:`x` de su centro es dado por

      .. math::
         :label: Ec:B_Loop2

         \begin{equation}
           B=\frac{\mu _{0}IR^{2}}{2(R^{2}+x^{2})^{\frac{3}{2}}}
         \end{equation}

      .. figure:: /images/Electromagnetismo/B_Loop/mffig3.png
         :scale: 100
         :align: center
         :name: fig:B_Loop_mffig3

         Campo magnético creado por una espira circular con corriente en un punto que está sobre el eje :math:`x`.



