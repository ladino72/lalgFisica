+Permeabilidad magnética del aire
=================================


**Objetivo**

El propósito de esta práctica es determinar el valor de la permeabilidad magnética :math:`\mu_a` del aire. Para ello, se usan dos bobinas; la bobina :math:`1` (inductora) de radio :math:`R`, se conecta un variac el cual suministra una señal alterna de la forma :math:`V=V_0\sin2\pi f`, siendo :math:`V_0` la amplitud, y :math:`f=60` Hz. La bobina :math:`2` de radio :math:`r` (:math:`r<R`) se dispone concéntricamente con la bobina :math:`1`, y se mide el voltaje :math:`V_{ef}` eficaz inducido generado por la corriente eficaz :math:`I_{ef}` que circula por la bobina inductora. A partir de la mediciones de :math:`V_{ef}` e :math:`I_{ef}` se determina el valor de :math:`\mu_a`.


**Recursos**

   #. Una bobina (inductora) con radio :math:`R\approx 10.5\,\text{cm}` y 200 vueltas ó :math:`R\approx 6.5\,\text{cm}` y 320 vueltas.
   #. Una bobina con radio :math:`r\approx 13\,\text{mm}` y :math:`2000` vueltas
   #. Dos multímetros.
   #. Cables de conexión.
   #. Una regla graduada.

**Resumen teórico**

Las corrientes eléctricas son las fuentes de campo magnético. El campo magnético creado por una distribución de corriente se calcula a partir de la ley de Biot-Savart [#f1]_, [#f2]_ . Para el caso de una espira circular de radio :math:`R` y con corriente :math:`i`, el valor del campo magnético en un punto :math:`P` a una distancia :math:`x` de su centro y a lo largo de un eje que pasa perpendicularmente al plano que contiene la bobina es dado por

.. math::

   \begin{equation}
    \overrightarrow{B}=\frac{\mu_aiR^2}{2(R^2+x^2)^{3/2}}\widehat{u}
   \end{equation}

donde :math:`\widehat{u}` es una vector unitario en la dirección del eje. Si el valor de la corriente es :math:`i=I_0\sin(\omega t)` y si en lugar de una sola espira se tienen :math:`N`, el valor de campo magnético en el punto :math:`x` es

.. math::

   \begin{equation}
    \overrightarrow{B}=\frac{\mu_aI_0NR^2}{2(R^2+x^2)^{3/2}}\sin(\omega t)\widehat{u}
   \end{equation}

Ahora, si en el punto :math:`P` se coloca una bobina de radio :math:`r` y :math:`n` espiras con :math:`R>r` concéntrica con la primera,  el flujo magnético a través de ésta es aproximadamente dado por

.. math::

   \begin{equation}
    {\Phi}= \frac{\mu_aI_0N\pi nr^2R^2}{2(R^2+x^2)^{3/2}}\sin(\omega t)
   \end{equation}

Como el flujo cambia con el tiempo, entonces la fuerza electromotriz inducida de acuerdo a la ley de Faraday es

.. math::

   \begin{equation}
     \varepsilon=-\frac{d\Phi}{dt}=-\frac{\mu_aI_0N\pi nr^2R^2\omega}{2(R^2+x^2)^{3/2}}\cos(\omega t)
   \end{equation}

Haciendo uso de los valores eficaces [#f4]_, que es lo que miden los multímetros, entonces el valor eficaz del voltaje inducido es

.. math::
   :label: Ec:perm1

   \begin{equation}
     \varepsilon_{ef}=\frac{\mu_aI_{ef}N\pi nr^2R^2\omega}{2(R^2+x^2)^{3/2}}=B_{ef}r^2n\omega\pi
   \end{equation}

donde hemos defindo

.. math::
   :label: Ec:perm5

   \begin{equation}
     B_{ef}=\frac{\mu_aI_{ef}NR^2}{2(R^2+x^2)^{3/2}}
   \end{equation}

La ecuación :eq:`Ec:perm1` se puede reescribir como

.. math::
   :label: Ec:perm6

   \begin{equation}
     \varepsilon_{ef}=KI_{ef}
   \end{equation}

donde

.. math::
   :label: Ec:perm7

   \begin{equation}
    K= \frac{\mu_aNn\pi r^2R^2\omega}{2(R^2+x^2)^{3/2}}
   \end{equation}

**Métodos para medir** :math:`\mu_a`


   #. De la ecuación :eq:`Ec:perm6` se sigue que para una distancia :math:`x` fija entre la bobinas, la relación entre el voltaje inducido :math:`\varepsilon_{ef}` en la bobina :math:`2` y la corriente :math:`I_{ef}` en la bobina :math:`1` es lineal, y por tanto el valor de la pendiente :math:`m` de la línea recta es :math:`K` (ver :numref:`fig:perm1`). Determinado el valor de la pendiente :math:`m`, el valor de la permeabilidad magnética del aire de la ecuación :eq:`Ec:perm7`, (con :math:`\omega =2\pi f`, siendo :math:`f=60` Hz) es dado por

      .. math::
         :label: Ec:perm8

         \begin{equation}
         \mu_a=\frac{m(R^2+x^2)^{3/2}}{nN\pi^2r^2R^2f}
         \end{equation}

      .. figure:: /images/Electromagnetismo/Permeability/perm1.png
         :scale: 120
         :align: center
         :name: fig:perm1

         Relación entre :math:`\varepsilon_{ef}` y :math:`I_{ef}` para una distancia fija :math:`x` entre las dos bobinas.


   #. De las ecuaciones :eq:`Ec:perm1` y :eq:`Ec:perm5` se sigue que

      .. math::
         :label: Ec:perm9

         \begin{equation}
           B_{ef}=\frac{\varepsilon_{ef}}{nr^22\pi^2f}=\mu_aX
         \end{equation}

      donde

      .. math::
         :label: Ec:perm10

         \begin{equation}
            X=\frac{I_{ef}NR^2}{2(R^2+x^2)^{3/2}}
         \end{equation}

      Así, si la corriente en la bobina :math:`1` se mantiene constante entonces la relación entre :math:`B_{ef}` y :math:`X` es lineal y la pendiente de ésta línea recta es :math:`\mu_a` (ver :numref:`fig:perm2`). Note que :math:`X` es una función de la coordenada :math:`x` del punto :math:`P`, que es el lugar donde se encuentra la bobina :math:`2`.

      .. figure:: /images/Electromagnetismo/Permeability/perm2.png
         :scale: 120
         :align: center
         :name: fig:perm2

         Relación entre el campo magnético efectivo :math:`B_{ef}` a lo largo del eje :math:`x` para una corriente :math:`I_{ef}` fija en la bobina :math:`1`.

**Montaje experimental**

El arreglo experimental para determinar la permeabilidad magnética del aire (ver :numref:`fig:perm3`) consiste esencialmente de dos bobinas ubicadas de modo que los planos que las contienen son paralelos y sus centros están a lo largo del eje :math:`x`. La bobina :math:`1` ó bobina inductora tiene radio :math:`R\approx 10.5 \text{cm}` y :math:`200` vueltas ó :math:`R\approx 6.5\,\text{cm}` y :math:`320` vueltas, y la bobina :math:`2` tiene radio :math:`r\approx 13\, \text{mm}` y :math:`2000` vueltas. La bobina :math:`1` se conecta al variac [#f3]_ cuya tensión o voltaje de salida se puede variar. La corriente a través de la bobina inductora depende de la tensión del variac y se mide con un multímetro conectado en serie. En la bobina :math:`2` se mide el voltaje inducido eficaz mediante el voltímetro en el rango AC.

.. figure:: /images/Electromagnetismo/Permeability/perm3.png
   :scale: 100
   :align: center
   :name: fig:perm3

   Arreglo experimental para determinar :math:`\mu_a`.


**Mediciones**

   #. Arme el montaje experimental de la :numref:`fig:perm3` y fije la distancia entre las bobinas en cero, es decir :math:`x=0`. Se sugiere que construya la :numref:`tab:perm1`. Grafique :math:`\varepsilon _{ef}` en función de :math:`I_{ef}` y utilice la ecuación :eq:`Ec:perm6` para determinar :math:`\mu_a`.

      .. csv-table:: Datos para determinar :math:`\mu_a`
         :header: "Corriente :math:`I_{ef}` (A)", "Voltaje :math:`\\varepsilon _{ef}` (V)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:perm1
         :align: center
         :stub-columns: 0
         :header-rows: 0

         0.0   ,
         0.1  ,
         0.2  ,
         0.3  ,
         0.4  ,
         0.5   ,
         0.6   ,
         0.7  ,
         0.8  ,
         0.9  ,
         1.0   ,
         1.1  ,
         1.2  ,
         1.3  ,
         1.4  ,
         1.5  ,
         1.6  ,
         1.7  ,

   #. Determine el valor efectivo del campo magnético de la bobina :math:`1` como función de :math:`x`. Para ello, se sugiere que complete la :numref:`tab:perm2` manteniendo la corriente constante en la bobina :math:`1` igual a 1.7 A. Grafique :math:`B_{ef}` en función de :math:`x` y compare sus resultados con los predichos por la ecuación :eq:`Ec:perm5`.

      .. csv-table:: Datos para determinar la dependencia del campo magnético efectivo :math:`B_{ef}`  de la posición :math:`x`, medida a lo largo del eje de la bobina :math:`1`. La corriente :math:`I_{ef}` en la bobina 1 se mantiene fija e igual a 1.7 A. 
         :header: "Distancia :math:`x` (cm)", "Voltaje :math:`\\varepsilon _{ef}` (V)",":math:`B_{ef}=\\frac{\\varepsilon _{ef}}{2n\\pi^{2}f}(\\mu T)`"
         :widths: 1,1,1
         :width: 15 cm
         :name: tab:perm2
         :align: center
         :stub-columns: 0
         :header-rows: 0

         0.0 ,,
         0.5 ,,
         1.0 ,,
         1.5 ,,
         2.0 ,,
         2.5 ,,
         3.0 ,,
         3.5 ,,
         4.0 ,,
         4.5 ,,
         5.0 ,,
         5.5 ,,
         6.0 ,,
         6.5 ,,
         7.0 ,,
         7.5 ,,
         8.0 ,,
         8.5 ,,
         9.0 ,,
         9.5 ,,
         10.0 ,,
         10.5 ,,
         11.0 ,,
         11.5 ,,
         :math:`\vdots`, :math:`\vdots`, :math:`\vdots` 
         25.0 ,,

   #. Con los datos obtenidos en la :numref:`tab:perm2` grafique :math:`B_{ef}` como función de :math:`X`, donde :math:`X` es dado por la ecuación :eq:`Ec:perm10`. De la gráfica obtenga de nuevo :math:`\mu_a`. Compare los resultados obtenidos para :math:`\mu_a` y compárelos con el valor teórico :math:`\mu_a=1.25663753\times10^{-6}\,\text{N/A}^2`. Discuta sus resultados.

.. [#f4] Recuerde que si una señal de corriente o voltaje depende del tiempo según las leyes :math:`i=I_0\sin(\omega t)`, :math:`v=V_0\sin(\omega t)`, el valor que mediría un amperímetro o voltímetro sería su valor eficaz dado por :math:`i_{ef}=\frac{I_0}{\sqrt{2}}` ó :math:`V_{ef}=\frac{V_0}{\sqrt{2}}`, las cuales con cantidades constantes.
.. [#f3] El Variac es un transformador con varios devanados reductores conectados a un interruptor rotativo, con el fin de reducir el voltaje AC desde el devanado primario.
.. [#f1] Yuste.M, Revista Española de Física, Volumen 10, Numero 1, 1996.
.. [#f2] Serway, R., FISICA para ciencias e ingeniería, McGraw-Hill, Tomo 2, México, 2000.

