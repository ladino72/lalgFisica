Centro de masa
================
**Objetivo**
El propósito de esta práctica es determinar la posición del centro de masa de un sistema de partículas.

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `http://physics.bu.edu/~duffy/HTML5/centerofmass.html <http://physics.bu.edu/~duffy/HTML5/centerofmass.html>`_.

**Resumen teórico**
Cuando un cuerpo se encuentra en movimiento, por ejemplo, al lanzar un bate al aire (ver :numref:`fig:center_01`), todas sus partículas se mueven a la vez, aunque con distintas trayectorias. Para caracterizar la traslación del bate en su conjunto, sin embargo, nos basta con estudiar qué ocurre en un solo punto del mismo: su centro de masa. Este será el que determine su velocidad, su trayectoria, etc. La localización del centro de masa de un cuerpo depende de cómo se encuentra distribuida su masa.

.. figure:: /images/Mecanica/Centro_de_Masa/center_01.png
   :alt:
   :scale: 60
   :align: center
   :name: fig:center_01

   El centro de masa del bate (punto negro) sigue una trayectoria parabólica, como si fuese una partícula de masa igual a la masa del bate.


Para un sistema de masas puntuales :math:`m_1,\, m_2,\, m_3,\,...,\,m_n` cuyos vectores posición son :math:`\overrightarrow{r}_1,\overrightarrow{r}_2,\overrightarrow{r}_3,...,\overrightarrow{r}_n` como el mostrado en la :numref:`fig:center_02`, el centro de masa del sistema se define como

.. figure:: /images/Mecanica/Centro_de_Masa/center_02.png
   :alt:
   :scale: 45
   :align: center
   :name: fig:center_02

   :math:`n` partículas puntuales y sus respectivos vectores posición

.. math::
   :label: cente_ecu_01

   \begin{equation}
    \overrightarrow{r}_{cm}=\frac{m_1\overrightarrow{r}_1+m_2\overrightarrow{r}_2+m_3\overrightarrow{r}_3+,...,+m_n\overrightarrow{r}_n}{m_1+m_2+m_3+,...,+m_n}
   \end{equation}


**Descripción de la interfaz de la aplicación**

La :numref:`com_01` muestra la interfaz gráfica del usuario para localizar la posición del centro de masa de un sistema compuesto por tres partículas puntuales de masas :math:`m_1`, :math:`m_2` y :math:`m_3`. Las tres partículas se encuentran fijas. Dos de ellas sobre el eje :math:`x` en las posiciones :math:`x_1=2\,\text{m},y_1=0\,\text{m}` y :math:`x_2=8\,\text{m},y_2=0\,\text{m}` y la otra en la posición  :math:`x_3=5\,\text{m},y_3=4\,\text{m}`. Las masas de :math:`m_1`, :math:`m_2` y :math:`m_3` se pueden aumentar o disminuir con las barras de desplazamiento rotuladas *Mass of ball 1*, *Mass of ball 2* y *Mass of ball 3* respectivamente. El valor de cada masa puede ser variado en el rango comprendido entre 0 y 5 kg. A medida que se cambia el valor de cualquiera de las masas, la posición del centro de masa del sistema cambia (punto de color vino tinto).

.. figure:: /images/Mecanica/Centro_de_Masa/CMgui_01.png
   :alt:
   :scale: 75
   :align: center
   :name: com_01

   Interfaz gráfica del usuario para localizar la posición del centro de masa de un sistema compuesto por tres partículas puntuales.


**Mediciones y procedimientos**

   #. A partir de la ecuación :eq:`cente_ecu_01` demuestre que en caso que las tres partículas se encuentren en el plano :math:`xy`, las coordenadas cartesianas :math:`x_{cm}`, :math:`y_{cm}` del centro de masa del sistema vienen dadas por

      .. math::
         :label: cente_ecu_03a

         \begin{equation}
          x_{cm}= \frac{m_1x_1+m_2x_2+m_3x_3}{m_1+m_2+m_3}
         \end{equation}

      .. math::
         :label: cente_ecu_03b

         \begin{equation}
          y_{cm} = \frac{m_1y_1+m_2y_2+m_3y_3}{m_1+m_2+m_3}
         \end{equation}

   #. Fije el valor de la masa :math:`m_3` en cero y los valores de :math:`m_1=m_2=2\,\text{kg}`. A partir de las ecuaciones :eq:`cente_ecu_03a` y :eq:`cente_ecu_03b` verifique que el centro de masa del sistema se encuentra en el punto medio que une las dos masas y que sus coordenadas cartesianas son :math:`(5\,\text{m},0\,\text{m})`.
   #. Manteniendo el valor de la masa :math:`m_3` en cero haga :math:`m_1=m_2=4\,\text{kg}`. A partir de las ecuaciones :eq:`cente_ecu_03a` y :eq:`cente_ecu_03b` verifique que el centro de masa del sistema sigue permaneciendo en el punto medio que une las dos masas. Demuestre que este resultado es válido en general siempre y cuando las masas de las dos partículas sean iguales.
   #. Manteniendo el valor de la masa :math:`m_3` en cero haga :math:`m_2=\,5\text{kg}`. Varíe el valor de :math:`m_1` desde 0 hasta 5 kg. ¿Qué le sucede a la posición del centro de masa?
   #. Manteniendo el valor de la masa :math:`m_3` en cero haga :math:`m_1=\,5\text{kg}`. Varíe el valor de :math:`m_2` desde 0 hasta 5 kg. ¿Qué le sucede a la posición del centro de masa? Teniendo en cuenta el anterior resultado, ¿qué puede concluir?
   #. Fije valores de :math:`m_1=m_2=5\,\text{kg}`. Incremente el valor de la masa :math:`m_3` desde 0 hasta 5 kg. Observe que la coordenada :math:`x_{cm}` no cambia, pero la coordenada :math:`y_{cm}` si aumenta. Explique este comportamiento, utilice las ecuaciones :eq:`cente_ecu_03a` y :eq:`cente_ecu_03b`.

   #. Fije valores de :math:`m_1=1\,\text{kg}`, :math:`m_2=2\,\text{kg}` y :math:`m_1=5\,\text{kg}`. ¿Dónde esperaría que se encuentre el centro de masa? Encuentre la posición de las coordenadas del centro de masa al hacer la lectura directamente de la pantalla. Calcule las coordenadas a partir de las ecuaciones :eq:`cente_ecu_03a` y :eq:`cente_ecu_03b` ¿Se obtienen los mismos resultados? Explique
   #. Es posible que la posición del centro de masa del sistema considerado para :math:`m_1\neq 0,m_2\neq 0\,\text{y}\,m_3\neq 0` se encuentre por fuera del triángulo formado al trazar líneas que unen las tres partículas?  ¿Bajo qué condiciones sería esto posible? ¿Con anti materia?
   #. Explique lo que tendría que hacerse para calcular el centro de masa de un bate y de un clavadista olímpico en el momento de realizar un salto.
   #. Discuta sus resultados y escriba sus conclusiones.



