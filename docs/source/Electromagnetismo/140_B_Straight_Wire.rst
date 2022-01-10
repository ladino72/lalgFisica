Campo magnético creado por un conductor recto
===============================================

**Objetivo**

El propósito de esta práctica es determinar la dependencia de la magnitud del campo magnético generado por una corriente eléctrica que circula por un conductor rectilíneo muy largo de su corriente y de la distancia del punto de observación al conductor.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://www.thephysicsaviary.com/Physics/Programs/Labs/FieldFromWire/ <http://www.thephysicsaviary.com/Physics/Programs/Labs/FieldFromWire/>`_.

**Resumen teórico**

Las cargas eléctricas en movimiento generan corriente eléctrica. La corriente eléctrica a su vez genera un campo magnético cuya magnitud y dirección están dados por la ley de Biot y Savart. Esta ley afirma que para un elemento diferencial del conductor (ver :numref:`Biot-Savart_01`) de longitud :math:`d\overrightarrow{l}` y corriente :math:`I`, el campo magnético :math:`d\overrightarrow{B}` en el punto :math:`P` a una distancia :math:`r` está dado por

.. figure:: /images/Electromagnetismo/B_Straight_Wire/Biot-Savart_01.png
   :scale: 100
   :align: center
   :name: Biot-Savart_01

   La dirección del campo magnético creado por el elemento de longitud :math:`dl` y corriente :math:`I` está determinada por la dirección de :math:`dl \times \widehat{u}_{r}`

.. math::
   :label: Ec:B_Stright_Wire.1

   \begin{equation}
    d \overrightarrow{B}=\frac{\mu _{0}I}{4\pi }\frac{d\overrightarrow{l}\times \widehat{u}_{r}}{r^{2}}
   \end{equation}

donde :math:`\mu _{0}=4\pi \times 10^{-7}T\cdot m/A` es la permeabilidad
del vacío. El campo de todo el conductor con corriente, se obtiene a partir del principio de superposición. Es decir, por la suma vectorial de los campos producidos por cada uno de los elementos :math:`d\overrightarrow{l}` que constituyen el conductor.


A partir de la ecuación :eq:`Ec:B_Stright_Wire.1` se puede probar que el campo magnético creado por un conductor rectilíneo (ver :numref:`mffig4` con corriente :math:`I` en un punto :math:`P` a una distancia :math:`x` perpendicular al conductor está dado por

.. figure:: /images/Electromagnetismo/B_Straight_Wire/mffig4.png
   :scale: 70
   :align: center
   :name: mffig4

   Conductor rectilíneo con corriente :math:`I`.

.. math::
   :label: Ec:B_Stright_Wire.3

   \begin{equation}
    B=\frac{\mu _{0}I}{4\pi x}(\sin \theta _{1}+\sin \theta _{2})
   \end{equation}

Para el caso cuando la longitud del conductor es :math:`L` y el punto :math:`P` equidista de los extremos del conductor, la expresión :eq:`Ec:B_Stright_Wire.3` se reduce a

.. math::
   :label: Ec:B_Stright_Wire.31

   \begin{equation}
    B=\frac{\mu _{0}I}{2\pi x}\frac{L}{\sqrt{L^{2}+4x^{2}}}
   \end{equation}

**Descripción de la interfaz de la aplicación**

La :numref:`fig:B_rect_largo` muestra la interfaz gráfica del usuario que permite estudiar la dependencia de la magnitud del campo magnético :math:`\overrightarrow{B}` generado por un conductor rectilíneo muy largo de la corriente eléctrica :math:`I` y la distancia más corta :math:`x` del punto donde se mide el campo al conductor. Al presionar el botón rotulado **Field Strength**, ubicado en la parte superior derecha de la interfaz, aparece un medidor de campo magnético el cual da la lectura en micro teslas ( el valor positivo o negativo lo determina la dirección de la corriente por el conductor) del campo en el lugar donde se encuentra la punta del sensor. La posición de esta punta se puede variar en sentido horizontal o vertical con la ayuda de las cuatro flechas que aparecen al presionar el botón rotulado **Location of Field Sensor**. La distancia de la punta del sensor al conductor se mide con ayuda de la cuadrícula que aparece al presionar el botón rotulado **Grid** ubicado en la parte superior de la interfaz. Tanto la dirección como el valor de la corriente por el conductor se establecen al presionar los botones rotulados **Direction (electron flow)** y  **Current** respectivamente.

.. figure:: /images/Electromagnetismo/B_Straight_Wire/BWgui_01.png
   :scale: 85
   :align: center
   :name: fig:B_rect_largo

   Interfaz del usuario para estudiar el campo magnético generado por un conductor rectilíneo muy largo con corriente eléctrica

**Mediciones y procedimientos**

   #. Fije la distancia :math:`x` del punto donde se desea medir el valor del campo magnético :math:`\overrightarrow{B}` al conductor en :math:`x=2\,\text{cm}`. Varíe la corriente, lea el valor de :math:`B` y registre sus valores en la :numref:`tab:B_Stright_Wire_01`.  Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`B` y :math:`I`
   #. Repita los pasos del inciso anterior pero esta vez haga :math:`x=7\,\text{cm}`. Registre sus datos en la :numref:`tab:B_Stright_Wire_02`. Teniendo en cuenta los resultados anteriores, ¿cuál es la dependencia entre :math:`B` y :math:`I`?
   #. Fije el valor de la corriente en :math:`I=1.4\,\text{A}`. Varíe la distancia :math:`x`, lea el valor de :math:`B` y registre sus valores en la :numref:`tab:B_Stright_Wire_03`. Aplique sus conocimientos de linealización de funciones para encontrar la relación entre :math:`B` y :math:`x`
   #. Repita los pasos del inciso anterior pero esta vez haga :math:`I=5.9\,\text{A}`.  Registre sus datos en la :numref:`tab:B_Stright_Wire_04`. Teniendo en cuenta los resultados anteriores, ¿cuál es la relación entre :math:`B` y :math:`x`?
   #. ¿Por qué razón, los resultados anteriores son independientes de la posición horizontal de la punta del sensor de campo magnético?
   #. Verifique que en el límite cuando la longitud del conductor :math:`L\rightarrow \infty` la ecuación :eq:`Ec:B_Stright_Wire.31` se reduce a :math:`B=\frac{\mu _{0}I}{2\pi x}`.
   #. Teniendo en cuenta el resultado del inciso anterior y si se asume que el conductor se encuentra en el vacío determine el valor de la permeabilidad magnética del vacío :math:`\mu_0`. Compare el valor obtenido con el valor exacto :math:`1.2566370621\times 10^{-6}\text{H/m}`. ¿Cuál es el porcentaje de error? ¿Cuáles son las fuentes de error?
   #. Discuta sus resultados y escriba sus conclusiones.

      .. csv-table:: :math:`x=2\,\text{cm}`
         :header: "Corriente, :math:`I` (A)", "Campo magnético :math:`B` (T)"
         :widths: 1,1
         :width: 14 cm
         :name: tab:B_Stright_Wire_01
         :align: center

         0.0,.
         1.4,.
         2.9,.
         3.3,.
         4.3,.
         5.0,.
         5.9,.
         7.3,.
         8.1,.
         9.1,.

      .. csv-table:: :math:`x=7\,\text{cm}`
         :header: "Corriente, :math:`I` (A)", "Campo magnético :math:`B` (T)"
         :widths: 1,1
         :width: 14 cm
         :name: tab:B_Stright_Wire_02
         :align: center

         0.0,.
         1.4,.
         2.9,.
         3.3,.
         4.3,.
         5.0,.
         5.9,.
         7.3,.
         8.1,.
         9.1,.

      .. csv-table:: :math:`I=1.4 \,\text{A}`
         :header: "Distancia, :math:`x` (cm)", "Campo magnético :math:`B` (T)"
         :widths: 1,1
         :width: 14 cm
         :name: tab:B_Stright_Wire_03
         :align: center

         1.0,.
         1.5,.
         2.0,.
         2.5,.
         3.0,.
         3.5,.
         4.0,.
         4.5,.
         5.0,.
         5.5,.
         6.0,.
         6.5,.
         7.0,.
         7.5,.
         8.0,.


      .. csv-table:: :math:`I=5.9 \,\text{A}`
         :header: "Distancia, :math:`x` (cm)", "Campo magnético :math:`B` (T)"
         :widths: 1,1
         :width: 14 cm
         :name: tab:B_Stright_Wire_04
         :align: center

         1.0,.
         1.5,.
         2.0,.
         2.5,.
         3.0,.
         3.5,.
         4.0,.
         4.5,.
         5.0,.
         5.5,.
         6.0,.
         6.5,.
         7.0,.
         7.5,.
         8.0,.



