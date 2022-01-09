+Procesos de redistribución de carga eléctrica en condensadores
===============================================================

**Objetivo**

El propósito de esta práctica es estudiar los procesos de redistribución de carga eléctrica cuando dos condensadores cargados se conectan en paralelo. Para ello, se estudian procesos de carga y descarga de un condensador de manera gradual y controlada.

**Recursos**

   #. Proceso de descarga (método 1): `http://tinyurl.com/ydduu9zv <http://tinyurl.com/ydduu9zv>`_
   #. Proceso de descarga (método 2):  `http://tinyurl.com/y89sfntw <http://tinyurl.com/y89sfntw>`_
   #. Proceso de carga: `http://tinyurl.com/ycfy2czk <http://tinyurl.com/ycfy2czk>`_

**Resumen teórico**

Un condensador es un sistema compuesto por un par de placas metálicas separadas por un material dielétrico (aislante). Cuando una diferencia de potencial :math:`V` se aplica entre las placas se crea un campo eléctrico, el cual almacena energía eléctrica; las placas almacenan carga eléctrica :math:`+Q` y :math:`-Q`. Que tanta carga eléctrica se almacena en el condensador depende del valor de la capacitancia :math:`C` del sistema, la cual se mide en faradios. La relación entre estas tres cantidades es :math:`V=Q/C` .

**Proceso de Descarga (método 1)**

Consideremos el circuito de la :numref:`Fig:Charge_Discharge_1` el cual consiste de dos condensadores :math:`C_x` y :math:`C_y`, una batería :math:`U` y tres interruptores :math:`S_1`, :math:`S_2` y :math:`S_3`. Cuando :math:`S_1` y :math:`S_3` se cierran, :math:`C_x`, :math:`C_y` adquiren las cargas :math:`Q_0=C_xU` y :math:`q_0=-C_yU`. La descarga de :math:`C_x` comienza cuando este se connecta a :math:`C_y` con polaridad inversa. La carga que pierde :math:`C_x` es peque\~na si :math:`C_x  >> C_y` y la diferencia de potencial en los condensadores es igual. Así, despues de abrir :math:`S_1` y :math:`S_3`; y cerrar :math:`S_2` la carga se redistribuye en los condensadores y sus cargas ahora son :math:`Q_1` y :math:`q_1`. Los valores de estas cargas se encuentran usando la conservación de la carga eléctrica: :math:`Q_0+q_0=Q_1+q_1` y la igualdad en las diferencias de potencial eléctrico en los condensadores: :math:`Q_1/C_x =q_1/C_y` . De estas ecuaciones resulta

.. figure:: /images/Electromagnetismo/Charge_Discharge/fig1.jpg
   :scale: 25
   :align: center
   :name: Fig:Charge_Discharge_1

   Izquierda: Los condensadores :math:`C_x` y :math:`C_y` se cargan a los voltaje :math:`U`  y :math:`-U` cerrando :math:`S_1` y :math:`S_3` temporalmente. Derecha: Los condensadores :math:`C_x` y :math:`C_y` se conectan en paralelo al cerrar :math:`S_2`, adquiriendo cargas :math:`Q_1` y :math:`q_1` respectivamente.

.. math::
   :label: eq.1

   \begin{equation}
    Q_1 = \frac{U}{\alpha}[C_x-C_y]
   \end{equation}

hemos definido :math:`{\alpha=1+\frac{C_y}{C_x}}`.

De ahora en adelante, :math:`S_1` se mantiene abierto y continuamos con la descarga gradual de :math:`C_x`. Para esto, :math:`S_2` y :math:`S_3` se abren y cierran respectivamente, ver :numref:`Fig:Charge_Discharge_2`. Como resultado, :math:`C_y` gana carga :math:`C_y U`.  Una vez que :math:`C_y` se carga :math:`S_3` se abre de nuevo y :math:`S_2` se cierra. Las cargas de :math:`C_x` y :math:`C_y` se redistribuyen y ahora son :math:`Q_2` y :math:`q_2` respectivamente. Asumiendo de nuevo la conservación de la carga eléctrica: :math:`Q_1-C_y U=Q_2+q_2` y la igualdad en las diferencias de potencial eléctrico en los condensadores: :math:`Q_2/C_x =q_2/C_y`.

.. figure:: /images/Electromagnetismo/Charge_Discharge/fig2.jpg
   :scale: 25
   :align: center
   :name: Fig:Charge_Discharge_2

   Izquierda:  El condensador :math:`C_y`  se carga el voltaje :math:`-U` al cerrar :math:`S_3` temporalmente mientras :math:`C_x` mantiene su carga del paso anterior. Derecha: Los condensadores :math:`C_x` y :math:`C_y` se conectan en paralelo al cerrar :math:`S_2`, adquiriendo cargas :math:`Q_2` y :math:`q_2` respectivamente

De estas ecuaciones resulta

.. math::
   :label: eq.2

   \begin{equation}
     Q_2 = \frac{U}{\alpha^2}[C_x-C_y(1+\alpha)]
   \end{equation}

Después de inspeccionar las ecuaciones :eq:`eq.1`  y :eq:`eq.2`, se sigue que la carga después de repetir el proceso :math:`n` veces es

.. math::
   :label: eq.3

   \begin{equation}
      Q_n = \frac{U}{\alpha^n}[C_x-C_y(1+\alpha+\alpha^2+\ldots+\alpha^{n-1})]=\frac{U}{\alpha^n}[C_x-C_y\frac{\alpha^{n}-1}{\alpha-1}]
   \end{equation}

De la ecuación :eq:`eq.3` se desprende que el voltaje en :math:`C_x` después de :math:`n` pasos es dado por

.. math::
   :label: eq.4

   \begin{equation}
    V_n = \frac{Q_n}{C_x}=U[\frac{2}{\alpha^n}-1]=U[2e^{{-\ln(\alpha)\cdot n}}-1]
   \end{equation}

De esta ecuación se sigue que :math:`V_n`  varía desde  :math:`+U` hasta :math:`-U` al variar :math:`n` desde 1 hasta infinito como es de esperarse.  El voltaje :math:`V_n`  en :math:`C_x` se hace cero para  :math:`n=n^{*}`, es decir cuando  :math:`\frac{2}{\alpha^{n^*}}=1` .  De la definición de  :math:`\alpha` se sigue que

.. math::
   :label: eq.5

   \begin{equation}
    C_y = (\sqrt[n^*]{2}-1)C_x
   \end{equation}

La ecuación :eq:`eq.5` permite encontrar :math:`C_y` si conocemos :math:`C_x` y si se determina :math:`n^*` del experimento.

**Proceso de Descarga (método 2)**

El circuito para descargar el condensador gradualmente se muestra en la :numref:`Fig:Charge_Discharge_9`. La descarga de :math:`C_x` se logra al cerrar :math:`S_2` y :math:`S_3` alternadamente y mantenidendo :math:`S_1` abierto. Asumiendo de nuevo la conservación de la carga eléctrica y la igualdad en las diferencias de potencial eléctrico de los condensadores en paralelo, el voltaje de :math:`C_x` después de :math:`n` pasos es dado por

.. figure:: /images/Electromagnetismo/Charge_Discharge/fig9.jpg
   :scale: 25
   :align: center
   :name: Fig:Charge_Discharge_9

   Los condensadores :math:`C_x`  y :math:`C_y` se cargan y descargan inicialmente cerrando :math:`S_1` y :math:`S_3` . El proceso de descarga de :math:`C_x` se realiza cerrando y abriendo :math:`S_2`  y :math:`S_3` alternadamente; manteniendo :math:`S_1` abierto.

.. math::
   :label: eq.6

   \begin{equation}
    V_n = \frac{U}{\alpha^n}=Ue^{{-\ln(\alpha)\cdot n}}
   \end{equation}

donde :math:`{\alpha=1+\frac{C_y}{C_x}}`.

**Proceso de Carga**

El circuito para cargar el condensador gradualmente se muestra en la :numref:`Fig:Charge_Discharge_8`. La carga de  :math:`C_x` se logra al cerrar :math:`S_2`  y :math:`S_3` alternadamente. Usando los mismos argumentos para la descarga del condensador, el voltaje de :math:`C_x` después de :math:`n` pasos es dado por

.. figure:: /images/Electromagnetismo/Charge_Discharge/fig8.jpg
   :scale: 25
   :align: center
   :name: Fig:Charge_Discharge_8

   El condensador :math:`C_x` se encuentra inicialmente descargado. :math:`C_y` se carga al cerrar :math:`S_3`. El proceso de carga de :math:`C_x` se realiza cerrando y abriendo :math:`S_2`  y :math:`S_3` alternadamente.

.. math::
   :label: eq.7

   \begin{equation}
    V_n = U(1-\frac{1}{\alpha^n})=U(1-e^{{-\ln(\alpha)\cdot n}})
   \end{equation}

donde :math:`{\alpha=1+\frac{C_y}{C_x}}`.

**Mediciones**

En los circuitos montados en el simulador aparecen unos resistores de resistencia 1 :math:`\Omega`, los cuales no aparecen en los circuitos que se describen arriba. Estos resistores de resistencia pequeña no afectan para nada nuestros resultados, simplemente el simulador los necesita para que funcione correctamente. En las simulaciones se utiliza: :math:`C_x=50\,\mu\text{F}` y :math:`C_y=11\,\mu\text{F}` y :math:`U=\pm 15\,\text{V}`. Los circuitos ya están montados, lo único que tiene que hacer es cerrar y abrir los interruptores con el puntero del ratón haciendo clic sobre estos. Si desea conocer el valor del voltaje en un elemento simplemente coloque el puntero del ratón sobre este y su valor aparece en la pantalla.

**Proceso de descarga: método 1**

   #. Abra el simulador ubicado en: http://tinyurl.com/ydduu9zv. Estudie el proceso de descarga de :math:`C_x` tal como se describe arriba. Para ello, complete la :numref:`tab:Charg_Disch_01`. A partir de las mediciones de :math:`V_n` como función de :math:`n` determine el valor de :math:`n^{*}` para el cual la curva intercepta el eje :math:`n`. Utilice la ecuación :eq:`eq.5` para determinar :math:`C_y`. Compare el valor obtenido con el valor nominal de :math:`C_y=11` :math:`\mu F`. Verifique matemáticamente que los datos medidos satisfacen la ecuación :eq:`eq.4`. Para ello, linealice dicha ecuación y demuestre que :math:`\ln(1+V_n/U)` en función de :math:`n` es una línea recta.

**Proceso de descarga: método 2**

   #. Abra el simulador ubicado en: http://tinyurl.com/y89sfntw. Estudie el proceso de descarga de :math:`C_x` tal como se describe arriba. Para ello, complete la :numref:`tab:Charg_Disch_02`. A partir de las mediciones grafique :math:`V_n` como función de :math:`n` y discuta la tendencia de la curva para valores grandes de :math:`n`. Verifique matemáticamente que los datos medidos satifacen la ecuación :eq:`eq.6`. Para ello, linealice dicha ecuación y demuestre que :math:`\ln(V_n/U)` en función de :math:`n` es una línea recta.

**Proceso de carga**

   #. Abra el simulador ubicado en: http://tinyurl.com/ycfy2czk. Estudie el proceso de carga de :math:`C_x` tal como se describe arriba. Para ello, complete la :numref:`tab:Charg_Disch_03`. A partir de las mediciones grafique :math:`V_n` como función de :math:`n` y discuta la tendencia de la curva para valores grandes de :math:`n`. Verifique matemáticamente que los datos medidos satisfacen la ecuación :eq:`eq.7`. Para ello, linealice dicha ecuación y demuestre que :math:`\ln(1-V_n/U)` en función de :math:`n` es una línea recta.

**Análisis**


   #. Realice los pasos necesarios para demostrar la veracidad de la expresión :eq:`eq.4`.
   #. Realice los pasos necesarios para demostrar la veracidad de la expresión :eq:`eq.6`.
   #. Realice los pasos necesarios para demostrar la veracidad de la expresión :eq:`eq.7`.



.. csv-table::  Descarga (método 1)
   :header: ":math:`n`", ":math:`V_n` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Charg_Disch_01
   :align: center

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
   11,.
   12,.
   13,.
   14,.
   15,.
   16,.
   17,.
   18,.
   19,.
   20,.
   21,.
   22,.
   23,.
   24,.
   25,.
   26,.
   27,.
   28,.
   29,.
   30,.

.. csv-table::  Descarga (método 2)
   :header: ":math:`n`", ":math:`V_n` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Charg_Disch_02
   :align: center

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
   11,.
   12,.
   13,.
   14,.
   15,.
   16,.
   17,.
   18,.
   19,.
   20,.
   21,.
   22,.
   23,.
   24,.
   25,.
   26,.
   27,.
   28,.
   29,.
   30,.

.. csv-table::  carga
   :header: ":math:`n`", ":math:`V_n` (V)"
   :widths: 1,1
   :width: 12 cm
   :name: tab:Charg_Disch_03
   :align: center

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
   11,.
   12,.
   13,.
   14,.
   15,.
   16,.
   17,.
   18,.
   19,.
   20,.
   21,.
   22,.
   23,.
   24,.
   25,.
   26,.
   27,.
   28,.
   29,.
   30,.


