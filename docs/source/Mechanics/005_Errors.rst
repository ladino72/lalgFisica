+Teoría de errores
==================

**Objetivo**

El objetivo de esta práctica es aprendar a reportar de manera correcta el resultado de mediciones experimentales.
En particular, se determina el diámetro de una esfera, el área total de la superficie y volumen de un paralelepípedo teniendo en cuenta la teoría de errores.

**Resumen teórico**

Siempre que se realiza la medición de una cantidad física inevitablemente
existen errores. Aun si se repitan las mediciones siempre encontraremos que
los resultados de las diferentes mediciones en general no coinciden. Surge
entonces la pregunta, como se puede determinar el verdadero valor de una
cantidad física? La respuesta es que no se puede saber. No obstante, si las
mediciones se realizan con cuidado y se aplican métodos experimentales
refinados entonces podemos reducir los errores y por tanto tener mayor
certeza de que las mediciones están mas cerca el valor verdadero. La
teoría de errores se encarga del estudio de las incertidumbres de las
cantidades físicas y suministra métodos que permiten su tratamiento.

**Definiciones básicas**

El error experimental es la diferencia entre una medida y su verdadero valor
o entre dos valores medidos. El error experimental mismo se mide por su
exactitud y precisión.

La *exactitud* mide que tan cerca un valor medido se encuentra del valor
verdadero o valor aceptado. Dado que el valor verdadero o aceptado de una
cantidad física usualmente se desconoce, la exactitud de una medición no se
puede determinar.

La *precisión* mide  cuanto concuerdan dos o mas mediciones de una misma
cantidad. La precisión esta relacionada con la repetitividad o
reproducibilidad. Así, una medida que es altamente reproducible tiende a dar
valores muy cercanos entre si.

La :numref:`Figure 1` y :numref:`Figure 2` muestran una analogía de la definición de exactitud y precisión
con las flechas que hace impacto sobre un blanco y con mediciones representadas sobre el eje horizontal.

.. figure:: /images/Mecanica/Errors/Error0.png
   :alt: error_1
   :scale: 50%
   :align: center
   :name: Figure 1

   Exactitud y precisión.



.. figure:: /images/Mecanica/Errors/Error1.png
   :alt: error_2
   :scale: 50%
   :align: center
   :name: Figure 2

   Exactitud y precisión.


*Aclaración:* cuando un científico o ingeniero hace referencia a errores
experimentales no se refiere a equivocaciones, cálculos mal hechos, metidas
de pata, etc. Por ejemplo, el medir un ancho cuando lo que se requería medir una longitud; el olvidar dividir el
diámetro por 2 antes de calcular el área de un circulo en la formula :math:`A=\pi r^{2}`; el usar la temperatura en
grados Celsius en una expresión donde la temperatura se debe expresar en
grados Kelvin, etc. Este tipo de errores son significativos pero se pueden
eliminar al repetir el experimento cuidadosamente.

**Tipos de errores experimentales: sistemáticos y aleatorios**

   #. Los errores sistematicos afectan la exactitud de la medicion. Ejemplo de
      fuentes errores sistemáticos: un instrumento mal calibrado, error debido al
      paralaje en la lectura de una escala con aguja, variaciones de frecuencia,
      variaciones de la tension de la fuente de alimentación, variación
      de temperatura, variación de humedad, envejecimiento de componentes,
      etc. Este tipo de errores no puede analizarse usando la teoria de errores,
      pueden ser dificiles de detectar, pero una vez detectados se pueden
      reducir usando un método de medición mas refinado.
   #. Los errores aleatorios afectan la precisión de la medición. Estos errores se
      presentan cuando al hacer multiples mediciones de la misma cantidad física
      obtenemos valores diferentes debido al azar, es decir a variaciones
      impredecibles en el proceso de medición, sus causas o leyes de variación
      son desconocidas. Este tipo de errores  puede analizarse usando la teoria de
      errores.  La precisión de una medición sujeta solo a errores aleatorios se
      puede mejorar al repetir muchas veces las medición o usando un método más
      refinado en la medición.


**Calculo de errores experimentales**

Cuando un científico o ingeniero reporta los resultados un experimento, el
reporte debe incluir la exactitud y precisión de las mediciones. Veamos como
se realizan estos estimativos.

**Cifras significativas**

El dígito menos significativo en una medición depende de la unidad mas pequeña del instrumento de medición usado.
La precisión de la medida queda determinada por el numero de cifras significativas con la cual se reporta la
medida. \ Como norma, una medida se reporta con una precisión igual a :math:`\frac{1}{10}` de la división mas pequeña del instrumento. Por ejemplo, una
medida de longitud usando una regla graduada en milimetros se reporta con
una precisión de :math:`\pm 0.1\,\text{mm}`. Una medición de un volumen \ usando una
probeta graduada en mililitros  se reporta con una precisión de :math:`\pm\, 0.1\,\text{ml}`.

Los instrumentos digitales se tratan de manera diferente a menos que que
fabricante suministre la precisión. La precisión de una medición hecha con
un instrumento digital se reporta con una precisión de :math:`\pm \frac{1}{2}` del
valor de la unidad mas pequeña que el instrumento puede medir. Por
ejemplo, un voltímetro digital indica 1.493 voltios; la precisión de la
lectura del voltaje es  :math:`\pm \frac{1}{2}` de 0.001 voltios o 0.0005 voltios.

\textbf{Error porcentual:} mide la exactitud de la medición y se define como

.. math::
   :nowrap:

    \[
    \%\text{ }Error=\frac{\mid E-A\mid }{A}\times 100
    \]

donde :math:`E` representa  el valor medido o experimental y :math:`A` representa el
valor verdadero o aceptado.

\textbf{Diferencia porcentual:} mide la precisión de dos mediciones  :math:`E_{1}` y :math:`E_{2}`, y se define como

.. math::
   :nowrap:

    \[
    \%\text{ }diferencia=\frac{\mid E_{1}-E_{2}\mid }{\frac{E_{1}+E_{2}}{2}}
    \]

\subsection{Media y desviación estandar}


Cuando una medición se realiza varias veces, se observa que los valores
obtenidos se agrupan o distribuyen  alrededor de un valor central. Este
agrupamiento o distribución se describe suministrando dos numeros: la media
o promedio la cual mide el valor central y la desviación estándar la cual
describe al ancho o desviación de los valores medidos alrededor de la media.

Para un conjunto de :math:`N` mediciones de una cantidad física :math:`x` , la media o
promedio de :math:`x` se representa con el simbolo :math:`<x>` o :math:`\overline{x}` y se
calcula como


.. math::
   :label: Error_avg

   \begin{equation}
        <x>=\overline{x}=\frac{1}{N}\sum_{i=1}^{N}x_{i}=\frac{1}{N}%
        (x_{1}+x_{2}+x_{3}+\cdots x_{N-1}+x_{N})
   \end{equation}


donde representa :math:`x_i` el i-esimo valor medido de :math:`x`.

La desviación estándar de los valores medidos se representa por el simbolo :math:`\sigma _{x}` y es dado por la fórmula


.. math::
   :label: Error_std

   \begin{equation}
        \sigma _{x}=\sqrt{\frac{1}{N-1}\sum_{i=1}^{N}(x_{i}-\overline{x})^{2}}
   \end{equation}


La desviación estándar también se le denomina la desviación cuadrática media
y mide que tan dispersos se encuentran los datos medidos a lado y lado de la
media o promedio. El significado :math:`\sigma _{x}` es el siguiente: para
mediciones sujetas solamente a errores aleatorios una desviación estándar de
:math:`\sigma _{x} ` significa que el 68\% de los valores medidos se encuentran en
el intervalo :math:`<x>-\sigma _{x}` y  :math:`<x>+\sigma _{x}`, que el 95\%  de los
valores medidos se encuentran en el intervalo :math:`<x>-2\sigma _{x}` y :math:`<x>+2\sigma _{x}` y que el 99\% de los valores medidos se encuentran en el
intervalo :math:`<x>-3\sigma _{x}` y  :math:`<x>+3\sigma _{x}`.

Asi, los resultados de una cantidad física :math:`x` se deben reportar indicando su
valor medio o promedio y la desviación estándar

.. math::
   :nowrap:

    \[
    x=\overline{x}\pm \sigma _{x}
    \]

**Ejemplo 1** Supongamos que un científico o ingeniero necesita reportar el valor
de la masa de una muestra. Para ello, el realiza 30 mediciones de la masa y
consigna sus resultados en la :numref:`tab:error`.


.. csv-table:: Mediciones para determinar la masa de la muestra. Masa dada en kg.
   :header: "", "", "", "", ""
   :widths: auto
   :name: tab:error
   :align: center

    1.09,1.01,1.10,1.14,1.16
    1.11,1.04,1.16,1.13,1.17
    1.14,1.03,1.17,1.09,1.09
    1.15,1.06,1.12,1.08,1.20
    1.08,1.07,1.14,1.11,1.05
    1.06,1.12,1.00,1.10,1.07


Para las 30 mediciones el valor de la media es

.. math::
   :nowrap:

   \[
   <x>=\overline{x}=\frac{1}{30}\sum_{i=1}^{30}x_{i}=\frac{1}{30}(33.04\text{ kg})=1.10\text{ kg}
   \]

La desviación estándar es

.. math::
   :nowrap:

   \[
   \sigma _{m}=\sqrt{\frac{1}{30-1}\sum_{i=1}^{30}(x_{i}-1.10)^{2}}=0.05\text{kg}
   \]

El resultado del valor de la muestra se debería  reportar como

.. math::
   :nowrap:

   \[
   m=1.10\text{kg }\,\pm 0.05\,\text{kg}
   \]

Otro ejemplo: https://www.youtube.com/watch?v=g5dSFQQ3I68


**Propagación de Errores**

En muchos experimentos se miden cantidades físicas de manera directa cuyos
valores son importantes para determinar otra cantidad de manera indirecta.
Cada una de las cantidades medidas de manera directa presenta una
incertidumbre y por tanto es de esperarse que la cantidad indirecta
calculada a partir de ésta, también presente una incertidumbre. Asi, por
ejemplo si desea medir el volumen de un paralelepípedo lo podemos hacer
midiendo su longitud, ancho y altura; con estos valores el valor del volumen
es el producto de estas tres cantidades. Pero, si la medición de cada una de
estas longitudes tiene una incertidumbre, la pregunta que surge es: ¿cuál es
la incertidumbre en el volumen de esta figura? ¿cómo se calcula esta
incertidumbre?

Consideremos el caso general. Supongamos que las variables :math:`x,y,z,...`
representan cantidades a medir y que se utilizan para calcular el valor de
una cantidad :math:`U`. Por supuesto que :math:`U` es una función de :math:`x,y,z,...` y esto
se escribe como :math:`U=f(x,y,z,...)`. Los valores de las cantidades medidas
se notan como :math:`\overline{x},\overline{y},\overline{z},\ldots` y las
correspondientes incertidumbres como :math:`\Delta x,\Delta y,\Delta z,,...`
para cada variable. Para encontrar el valor esperado o mejor estimativo de
la cantidad :math:`U`, el valor esperado o promedio  de cada cantidad medida se
reemplaza en la ecuación de :math:`U`:

.. math::
   :nowrap:

   \[
   \overline{U}=f(\overline{x},\overline{y},\overline{z},\ldots )
   \]

Si los errores de :math:`x,y,z,...` son independientes y aleatorios y
suficientemente pequeños, se puede demostrar que la incertidumbre en el
valor de :math:`U`\ es dado por


.. math::
   :label: Error_0

   \begin{equation}
   \Delta U=\sqrt{\left( \frac{\partial U}{\partial x}\right) ^{2}(\Delta
   x)^{2}+\left( \frac{\partial U}{\partial y}\right) ^{2}(\Delta y)^{2}+\left(
   \frac{\partial U}{\partial z}\right) ^{2}(\Delta z)^{2}+\cdots }
   \end{equation}


donde las derivadas parciales son evaluadas usando la valores medios :math:`\overline{x},\overline{y},\overline{z},\ldots`
como valores de las variables independientes. Finalmente, la notación correcta que expresa el valor de la
cantidad :math:`U` es dado por

.. math::
   :nowrap:

    \[
    U=\overline{U}\pm \Delta U
    \]

La expresión :eq:`Error_0` involucra el cálculo de derivadas
parciales, temas que todavía probablemente no manejamos, pero esto no nos
impide su uso. Consideraremos algunos casos especiales de funciones :math:`U`
encontradas en situaciones tipicas de trabajo en el laboratorio y cuyo valor
de  :math:`\Delta U` es fácil de recordar y aplicar y que no requiere que
sepamos derivar.

**Caso I**

.. math::
   :label: Error1

   \begin{equation}
     U=C^{te}\cdot \frac{x^{\alpha }\times y^{\beta }\times w^{\delta }\ldots }{%
     z^{\gamma }\ldots }
   \end{equation}

donde :math:`\alpha,\, \beta,\, \delta,\, \gamma,\, \ldots` son exponentes enteros o
fraccionarios positivos.

En este caso :math:`U` es una función de las variables :math:`x,\, y, \, w,\, z,\,\ldots` y la
incertidumbre se calcula como


.. math::
   :label: Error2

   \begin{equation}
   \Delta U=\overline{U}\sqrt{\left( \alpha \frac{\Delta x}{\overline{x}}%
   \right) ^{2}+\left( \beta \frac{\Delta y}{\overline{y}}\right) ^{2}+\left(
   \delta \frac{\Delta w}{\overline{w}}\right) ^{2}+\left( \gamma \frac{\Delta z%
   }{\overline{z}}\right) ^{2}+\cdots }
   \end{equation}


**Ejemplo 1** Suponga que se desea medir el valor de la aceleración de la
gravedad dejando caer una bola en un pozo de profundidad  :math:`495.21 \,\text{m} \pm 5\,\text{mm}`.
La duración de la caida es  :math:`10.05\,\text{s}\,\pm\, 1/100\,\text{s}`. Calcular el valor de :math:`g` y
la incertidumbre de la medición.

La expresión que permite calcular la aceleración de la gravedad es :math:`g=\frac{2h}{t^{2}}`. En este caso, las variables independientes son :math:`h` y :math:`t`.
Comparando esta expresión con la expresión :eq:`Error1` observamos que

.. math::
   :nowrap:

    \begin{eqnarray*}
    U &\rightarrow &g \\
    C^{te} &\rightarrow &2 \\
    x &\rightarrow &h,\alpha \rightarrow 1 \\
    z &\rightarrow &t,\gamma \rightarrow 2
    \end{eqnarray*}

:math:`\overline{t}=10.05\,\text{5}`, :math:`\Delta t=\frac{1}{100}\,\text{s}`, :math:`\overline{h}=495.21\,\text{m}`,
:math:`\Delta h=5\,\text{mm}=5\times 10^{-3}\,\text{m}`; :math:`\overline{g}=\frac{2\overline{h}}{\overline{t}^{2}}=\frac{2\times 495.21}{10.05^{2}}= 9.80\,\text{m/s}^{2}`

.. math::
   :nowrap:

    \begin{eqnarray*}
    \Delta g &=&\overline{g}\sqrt{\left( \frac{\Delta h}{\overline{h}}\right)
    ^{2}+\left( 2\frac{\Delta t}{\overline{t}}\right) ^{2}} \\
    &=& 9.80\sqrt{\left( \frac{5\times 10^{-3}}{495.21}%
    \right) ^{2}+\left( 2\frac{\frac{1}{100}}{10.05}\right) ^{2}}%
    =1.950\,3\times 10^{-2}\approx 0.02\text{ }m/s^{2}\text{ }
    \end{eqnarray*}

Por lo tanto, el valor de la medición se expresa como :math:`g=9.8\,\text{m/s}^{2}\,\pm
0.02\,\text{m/s}^{2}`.


**Ejemplo 2** Un pepéndulo de longitud :math:`\ell =100\,\text{cm}\,\pm\, 0.5\,\text{cm}` oscila en un
lugar donde :math:`g=9.8\,\text{m/s}^{2}\,\pm\, 0.02 \,\text{m/s}^{2}`. Determine el periodo y la incertidumbre en la medición.

El periodo de las oscilaciones es dado por :math:`T=2\pi \sqrt{\frac{\ell }{g}}=2\pi \frac{\ell ^{\frac{1}{2}}}{g^{\frac{1}{2}}}`. En este caso las
variables independientes son :math:`\ell` ` y :math:`g`. Comparando esta expresión con la
expresión :eq:`Error1` observamos que

.. math::
   :nowrap:

    \begin{eqnarray*}
    U &\rightarrow &T \\
    C^{te} &\rightarrow &2\pi \\
    x &\rightarrow &\ell ,\alpha \rightarrow \frac{1}{2} \\
    z &\rightarrow &g,\gamma \rightarrow \frac{1}{2}
    \end{eqnarray*}

:math:`\ell =100` cm = 1.0 m, :math:`\Delta \ell =0.5\times 10^{-2}m,` :math:`\Delta g=0.02` :math:`%
m/s^{2}`, :math:`\overline{g}=` :math:`9.8` :math:`m/s^{2}`, :math:`\overline{T}=2\pi \sqrt{\frac{%
\ell }{g}}=2\pi \sqrt{\frac{1.0}{9.8}}= 2.0` :math:`s.`

.. math::
   :nowrap:

    \begin{eqnarray*}
    \Delta T &=&\overline{T}\sqrt{\left( \frac{1}{2}\frac{\Delta \ell }{%
    \overline{\ell }}\right) ^{2}+\left( \frac{1}{2}\frac{\Delta g}{\overline{g}}%
    \right) ^{2}} \\
    &=&2.0\sqrt{\left( \frac{1}{2}\frac{0.5\times 10^{-2}}{1.0}%
    \right) ^{2}+\left( \frac{1}{2}\frac{0.02}{9.8}\right) ^{2}}=5.400\,5\times 10^{-3}\approx 0.005\text{ }s
    \end{eqnarray*}

Por lo tanto, el valor de la medición se expresa como :math:`T=2.0\,\pm\,0.005\,\text{s}`.



**Caso II**

.. math::
   :label: Error_3

    \begin{equation}
    U=C_{1}^{te}x\pm C_{2}^{te}y\pm C_{3}^{te}z+\cdots \pm C_{n}^{te}w
    \end{equation}

.. math::
   :label: Error_4

    \begin{equation}
    \Delta U=\sqrt{\left( C_{1}^{te}\Delta x\right) ^{2}+\left( C_{2}^{te}\Delta
    y\right) ^{2}+\left( C_{3}^{te}\Delta z\right) ^{2}+\cdots +\left(
    C_{n}^{te}\Delta w\right) ^{2}}
    \end{equation}

**Ejemplo 1**  Suponga que se desea medir el valor del perímetro :math:`P` de un
rectángulo cuya longitud y ancho son  :math:`\ell =88.21\,\text{m}\,\pm\, 0.4\,\text{cm}` y
:math:`w=22.56\,\text{m}\,\pm \, 0.5 \,\text{cm}`.
Calcular el valor de :math:`P` y la incertidumbre de la
medición.

La expresión que pertmite calcular el perímetro es :math:`P=2\ell +2w.` En este
caso las variables independientes son :math:`\ell` y :math:`w`. Comparando esta
expresión con la expresión :eq:`Error_3` observamos que

.. math::
   :nowrap:

    \begin{eqnarray*}
    U &\rightarrow &P \\
    C_{1}^{te} &\rightarrow &2,x\rightarrow \ell  \\
    C_{2}^{te} &\rightarrow &2,y\rightarrow w
    \end{eqnarray*}

:math:`\overline{\ell}= 88.21 \,\text{m}`, :math:`\Delta \ell =0.4 \, \text{cm}=0.4\times 10^{-2}\,\text{m}`,  :math:`%
\overline{w}=22.56\,\text{m}` :math:`\Delta w=0.5\,\text{cm}=0.5\times 10^{-2}\,\text{m},` :math:`\overline{P}=2\overline{\ell }+2\overline{w}=\ 2(88.21)+2(22.56)=221.\, 54\,\text{m}`

.. math::
   :nowrap:

    \begin{eqnarray*}
    \Delta P &=&\sqrt{\left( C_{1}^{te}\Delta \ell \right) ^{2}+\left(
    C_{2}^{te}\Delta w\right) ^{2}} \\
    &=&\sqrt{\left( 2\times 0.4\times 10^{-2}\right) ^{2}+\left( 2\times
    0.5\times 10^{-2}\right) ^{2}}=1.280\,6\times 10^{-2}\text{ }%
    m\approx 0.01\text{ }m\ \text{ }
    \end{eqnarray*}

Por lo tanto, el valor de la medición se expresa como :math:`P=221.54 \,\text{m}\,\pm \,0.01\,\text{m}`.

**Caso III**

Algunas funciones de uso comun

.. math::
   :label: Error_5

   \begin{equation}
    U=C^{te}e^{\pm bx}\Longrightarrow \Delta U=C^{te}be^{\pm bx}\Delta x
   \end{equation}


.. math::
   :label: Error_6

   \begin{equation}
    U=C^{te}x^{\pm b}\Longrightarrow \Delta U=C^{te}bx^{\pm b-1}\Delta x
   \end{equation}


.. math::
   :label: Error_7

   \begin{equation}
    U=C^{te}\sin (kx)\Longrightarrow \Delta U=C^{te}k\cos (kx)\Delta x
    \end{equation}


.. math::
   :label: Error_8

   \begin{equation}
    U=C^{te}\cos (kx)\Longrightarrow \Delta U=C^{te}k\sin (kx)\Delta x
   \end{equation}

**Ejercicios propuestos**


  #.  Suponga que se desea medir el volumen :math:`V` de un paralelepípedo. Para ello se miden sus tres dimensiones :math:`\ell`, :math:`w` y :math:`h` independientemente y las respectivas incertidumbres :math:`\Delta \ell`, :math:`\Delta w` y :math:`\Delta h`. Demostrar que el volumen es dado por :math:`V=\overline{\ell }\overline{w} \overline{h}(1\pm \sqrt{\left( \frac{\Delta \ell }{\overline{\ell }}\right)^{2}+\left( \frac{\Delta w}{\overline{w}}\right) ^{2}+\left( \frac{\Delta h}{\overline{h}}\right) ^{2}})`.
  #.  Suponga que se desea medir el volumen :math:`V` de una esfera. Para ello se mide su radio :math:`r` y la respectiva incertidumbre  :math:`\Delta r`. Demostrar que el volumen de la esfera es dado por :math:`V=\frac{4}{3}\pi \overline{r}^{3}\left(1\pm 3\frac{\Delta r}{\overline{r}}\right)`.
  #.  Suponga que se desea medir el área :math:`A` de una esfera. Para ello se mide su radio :math:`r` y la respectiva incertidumbre  :math:`\Delta r`. Demostrar que el área de la esfera es :math:`A=4\pi \overline{r}^{2}\left( 1\pm 3\frac{\Delta r}{\overline{r}}\right)`
  #.  Suponga que se desea medir el volumen :math:`V` de un cilindro. Para ello se miden su radio :math:`r` y altura :math:`h` independientemente y las respectivas incertidumbres :math:`\Delta r` y :math:`\Delta h`. Demostrar que el volumen del cilindro es dado por :math:`V=\pi \overline{r}^{2}\overline{h}(1\pm \sqrt{\left( 2\frac{\Delta r}{\overline{r}}\right) ^{2}+\left( \frac{\Delta \overline{h}}{\overline{h}}\right) ^{2}})`.

