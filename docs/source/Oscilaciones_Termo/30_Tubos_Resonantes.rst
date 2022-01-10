Tubos resonantes
==================

**Objetivo**

El propósito de esta práctica es determinar la velocidad del sonido mediante la utilización de un tubo (abierto-cerrado y abierto-abierto) donde se forman ondas estacionarias.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://thephysicsaviary.com/Physics/Programs/Labs/ResonanceTubeLab/ <http://thephysicsaviary.com/Physics/Programs/Labs/ResonanceTubeLab/>`_.


**Resumen teórico**

Cuando un parlante que produce sonido armónico o un diapasón vibrante se colocan cerca del extremo de un tubo hueco, este resuena a ciertas
frecuencias determinadas. Las ondas sonoras viajan a lo largo del tubo, se reflejan en el otro extremo del tubo y regresan al parlante. Para el caso cuando la longitud del tubo es mucho mayor que su diámetro se forman ondas estacionarias en su interior.
Se puede demostrar que las condiciones de contorno para extremo abierto requiere que el cambio de presión sea cero (respecto a la presión atmosférica), es decir :math:`\Delta P=0` y para el extremo cerrado :math:`\frac{\partial \Delta P}{\partial x}=0`. Lo anterior significa que, en el extremo cerrado de un tubo, se tiene un antinodo o vientre y en extremo abierto un nodo. La anterior condición implica también que para las ondas desplazamiento se cumple lo contrario, es decir, en el extremo  cerrado del tubo, se tiene  un nodo y en extremo abierto un antinodo o vientre.
La :numref:`setup_40` y la :numref:`setup_41` muestran los  primeros tres modos de oscilación  para los tubos abierto-cerrado y abierto-abierto.

.. figure:: /images/Oscilaciones_Termo/Tubos_Resonantes/TR_setup_040.png
   :alt:
   :scale: 80%
   :align: center
   :name: setup_40

   Frecuencia fundamental y sobretonos para las ondas de presión y desplazamiento en un tubo abierto-cerrado.


.. figure:: /images/Oscilaciones_Termo/Tubos_Resonantes/TR_setup_041.png
   :alt:
   :scale: 80%
   :align: center
   :name: setup_41

   Frecuencia fundamental y sobretonos para las ondas de presión  y desplazamiento en un tubo abierto-abierto.

Las frecuencias de resonancia para el tubo abierto-cerrado y abierto-abierto vienen dadas respectivamente por


.. math::
   :label: Ec:R_T_res_1a

   \begin{eqnarray}
        f_n&=&\frac{v}{4L}(2n-1)\qquad n=1,2,3\ldots
   \end{eqnarray}

.. math::
   :label: Ec:R_T_res_1b

   \begin{eqnarray}
        f_n&=&\frac{v}{2L}n    \qquad n=1,2,3\ldots
   \end{eqnarray}


donde :math:`v` es la velocidad de la onda sonora dentro del tubo, la cual depende de la naturaleza del gas, su temperatura y longitud :math:`L` del tubo. Las frecuencias :math:`f=\frac{v}{2L}` y :math:`f=\frac{v}{4L}`  se denominan frecuencias fundamentales para los tubos abierto-abierto y abierto-cerrado respectivamente. El resto de frecuencias corresponden a las frecuencias de los sobretonos.

**Descripción de la interfaz de la aplicación**

.. figure:: /images/Oscilaciones_Termo/Tubos_Resonantes/TR_setup_01.png
   :alt:
   :scale: 80%
   :align: center
   :name: setup_01.png

   Interfaz gráfica del usuario para estudiar las ondas estacionarias.

**Mediciones y procedimientos**

Nota: cada vez que inicia la aplicación esta genera de manera automática cinco longitudes del tubo diferentes.

**Tubo abierto-cerrado**

   #. De las cinco posibles longitudes del tubo escoja la de mayor valor, ver :numref:`R_T_setup_03`. Sin cambiar la longitud del tubo encuentre todas las frecuencias posibles para las cuales se forman ondas estacionarias. A partir de las frecuencias registradas encuentre la velocidad de las ondas sonoras en el tubo.

      .. figure:: /images/Oscilaciones_Termo/Tubos_Resonantes/TR_setup_03.png
         :alt:
         :scale: 45%
         :align: center
         :name: R_T_setup_03

         Montaje para estudiar las ondas estacionarias en un tubo abierto-cerrado.
   #. Repita el procedimiento anterior pero esta vez con la mínima longitud del tubo. ¿Los resultados obtenidos para la velocidad dependen de la longitud del tubo? Discuta sus resultados.
   #. Varíe la longitud del tubo y para cada longitud determine el valor de la mínima frecuencia para la cual se presentan ondas estacionarias, construya una tabla con entradas de longitud :math:`L` y frecuencia (Hz). De la ecuación :eq:`Ec:R_T_res_1a` es claro que la gráfica de :math:`f` en función de :math:`\frac{1}{L}` es lineal. Verifique esta dependencia y encuentre el valor de la velocidad :math:`v` del sonido en el tubo.
   #. Discuta sus resultados y escriba sus conclusiones.


**Tubo abierto-abierto**

   #. Configure el sistema de modo que la longitud del tubo sea máxima (98 cm), ver :numref:`R_T_setup_02`. Sin cambiar la longitud del tubo encuentre todas las frecuencias posibles para las cuales se forman ondas estacionarias. A partir de las frecuencias registradas encuentre la velocidad de las ondas sonoras en el tubo.

      .. figure:: /images/Oscilaciones_Termo/Tubos_Resonantes/TR_setup_02.png
         :alt:
         :scale: 45%
         :align: center
         :name: R_T_setup_02

         Montaje para estudiar las ondas estacionarias en un tubo abierto-abierto.
   #. Repita el procedimiento anterior pero esta vez con la mímima longitud del tubo (56 cm). ¿Los resultados obtenidos para la velocidad dependen de la longitud del tubo? Discuta sus resultados.
   #. Varíe la longitud del tubo y para cada longitud determine el valor de la mínima frecuencia para la cual se presentan ondas estacionarias, construya una tabla con entradas de longitud :math:`L` y frecuencia (Hz). De la ecuación :eq:`Ec:R_T_res_1b` es claro que la gráfica de :math:`f` en función de :math:`\frac{1}{L}` es lineal. Verifique esta dependencia y encuentre el valor de la velocidad :math:`v` del sonido en el tubo.
   #. Discuta sus resultados y escriba sus conclusiones.


**Preguntas**

   #. Investigue como los constructores de violines usan ondas estacionarias en dos dimensiones para producir violines de igual calidad.
   #. ¿Qué son los patrones de Chladni?
   #. ¿Qué son cavidades ópticas y para qué se utilizan?

