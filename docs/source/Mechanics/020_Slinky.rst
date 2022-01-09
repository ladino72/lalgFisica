+Resorte de juguete (Slinky)
============================

**Objetivo**

El propósito de esta práctica es encontrar la manera como se distribuyen las espiras en un slinky en equilibrio cuando este se suspende por uno de sus extremos.

**Recursos**


   #. Un slinky.
   #. Una regla graduada en mm.


**Resumen teórico**

Un slinky es un juguete inventado en 1940 y consiste de un muelle en espiral. Los modelos básicos son en acero o plástico en colores, como un arco iris. Una de sus características fundamentales desde el punto de vista físico, es que cuando este se suspende por uno de sus extremos, la distancia de separación entre espiras consecutivas disminuye significativamente a lo largo del mismo. Así, su masa por unidad de longitud es variable y aumenta desde su punto de suspensión hasta su parte más baja. Al aplicar las leyes de Newton al slinky suspendido y en equilibrio, se encuentra que la distancia :math:`y` a la cual se encuentra la :math:`n` -ésima espira con respecto a la primera (ubicada en la parte inferior) es dada por

.. math::
   :label: Ec:slinky0

   \begin{equation}
    y=\frac{L_0}{N}n+\frac{(L-L_0)}{N^{2}}n^{2}
   \end{equation}

donde :math:`L_0` es la longitud natural del slinky cuando este reposa sobre una superficie horizontal, :math:`N` es el número de espiras y :math:`L` es su longitud total cuando se encuentra suspendido y en equilibrio. Las espiras también se cuentan a partir de la espira inferior del slinky (:math:`n=0,1,2,3 \ldots`).


**Descripción del problema**

El arreglo experimental para determinar la posición de las espiras con respecto al número de la espira se muestra en la :numref:`Fig:slinky_04`, el cual consta esencialmente de un slinky suspendido de un soporte y una regla graduada en mm.


.. figure:: /images/Mecanica/Slinky/Slinky_04.png
   :alt:
   :scale: 110
   :align: center
   :name: Fig:slinky_04

   Slinky en equilibrio.


**Mediciones**

Asegúrese que durante las mediciones, el slinky se encuentre en equilibrio. Mida la distancia de cada una de las espiras del slinky suspendido a partir de la espira ubicada en la parte más baja de este. Complete la :numref:`tab:slinky00`.
A partir de los datos grafique :math:`y` en función de :math:`n`. Para verificar que la relación :eq:`Ec:slinky0` es cuadrática se debe linealizar esta ecuación. Para ello, reescribimos dicha ecuación como :math:`\frac{y}{n}=a+bn`. De esta relación, es claro que :math:`\frac{y}{n}` depende linealmente de :math:`n`. Luego, al graficar :math:`\frac{y}{n}` como función de :math:`n` el resultado es una línea recta (:math:`Y=mx+b`) con pendiente :math:`m=\frac{(L-L_0)}{N^{2}}` e intercepto con el eje vertical igual a :math:`b=\frac{L_0}{N}`, ver :numref:`Fig:slinky_03`. De estas dos últimas expresiones se obtiene :math:`L=mN^{2}+bN`. Los valores de :math:`m` y :math:`b` se encuentran al realizar una regresión lineal con los datos experimentales. Determine experimentalmente los valores de :math:`L` y :math:`N`, y compare este valor con el valor dado por :math:`L=mN^{2}+bN`. Discuta sus resultados.


.. figure:: /images/Mecanica/Slinky/Slinky_03.png
   :alt:
   :scale: 110
   :align: center
   :name: Fig:slinky_03

   Linealización de la ecuación :eq:`Ec:slinky0`



.. csv-table:: Mediciones para determinar la relación entre :math:`y` y :math:`n`
   :header: ":math:`n`", ":math:`y` (mm)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:slinky00
   :align: center

   0,
   1,
   2,
   3,
   4,
   5,
   :math:`\vdots`,
   32,
   33,
   34,
   35,


**Análisis y Preguntas**

   #. Discuta la razón por la cual se realiza todo este procedimiento largo y tedioso para determinar los valores de :math:`L` y :math:`N` cuando estos se obtien de manera inmediata simplemente midiendo :math:`L` con la regla y contando :math:`N`.
   #. ¿Tiene alguna utilidad la linealización de una ecuación? Explique.
