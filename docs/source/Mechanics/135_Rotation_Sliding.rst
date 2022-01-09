Dinámica rotacional: Rodadura y deslizamiento
======================================================

**Objetivo**

El propósito de esta práctica es estudiar  el efecto de la fuerza de rozamiento y la velocidad inicial sobre el deslizamiento de un cuerpo antes de que este comience a rodar.


**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://ophysics.com/r1.html <https://ophysics.com/r1.html>`_.

**Resumen teórico**

Cuando un cuerpo sólido como por ejemplo una esfera, un aro, un cilindro, etc. se lanza horizontalmente a lo largo de una superficie horizontal su centro de masa se traslada y el cuerpo puede o no girar alrededor de su centro de masa dependiendo de la fuerza de rozamiento existente entre la superficie y el cuerpo. Qué tanto avanza el cuerpo antes de comenzar a rodar depende esencialmente de esta fuerza. Antes de rodar, el centro de masa del cuerpo se traslada y el cuerpo gira deslizándose por la superficie. Cuando el cuerpo rueda, se cumple que la relación entre la velocidad :math:`v_c` de su centro de masa (c.m) y su velocidad angular :math:`\omega` área :math:`v_{c}=\omega R`, siendo :math:`R` su radio (condición de rodadura). La anterior expresión equivale a :math:`a_{c}=\alpha R `, siendo :math:`a_{c}` y :math:`\alpha` las aceleraciones lineal y angular respectivamente.\newline
Consideremos la situación particular, donde el cuerpo de la izquierda en la :numref:`Fig:Rot_Slid_03` con masa :math:`m` y velocidad :math:`v_0` se desliza sobre una superficie sin fricción, por tanto no gira alrededor de su centro de masa. Para la situación de la derecha, el mismo cuerpo se mueve sobre una superficie, pero esta vez una fuerza de rozamiento actúa sobre éste que hace que la velocidad de traslación de su centro de masa vaya disminuyendo y su velocidad angular alrededor de su centro de masa vaya aumentando. Al aplicar la segunda ley de Newton al cuerpo resulta:

.. math::
   :label: Ec:Rot_Slid_01a

   -f=-\mu N=-\mu mg =ma_c

.. math::
   :label: Ec:Rot_Slid_01b

   \tau=fR=I_c\alpha

donde :math:`\mu` es el coeficiente de rozamiento entre el cuerpo y la superficie, y :math:`I_c` es su momento de inercia con respecto al centro de masa.

.. figure:: /images/Mecanica/Rotation_Sliding/forces_03.png
   :alt:
   :scale: 105
   :align: center
   :name: Fig:Rot_Slid_03

   Movimiento en ausencia y presencia de fuerza de friacción

De estas ecuaciones resulta :math:`a_c=-\mu g` y :math:`\alpha=\frac{\mu mgR}{I_c}`, y por tanto podemos escribir

.. math::
   :label: Ec:Rot_Slid_02a

   v_c=v_0-\mu gt

.. math::
   :label: Ec:Rot_Slid_02b

   \omega=\frac{\mu mgR}{I_c}t

Obsérvese que hemos considerado que la velocidad angular inicial del cuerpo es cero, es decir, :math:`\omega_0=0`.
La velocidad de traslación del centro de masa :math:`v_c` disminuye, y aumenta la de rotación :math:`\omega`.  El movimiento de rodadura (sin deslizar) se establece cuando :math:`v_c=\omega R`, es decir en el instante de tiempo


.. math::
   :label: Ec:Rot_Slid_03

   t=\frac{\frac{v_0}{R}}{\mu g(\frac{1}{R}+\frac{mR}{I_c})}=\frac{v_0}{\mu gk}

donde

.. math::
   :label: Ec:Rot_Slid_03a

   \begin{equation}
    k=1+\frac{mR^{2}}{I_c}
   \end{equation}

El desplazamiento :math:`s` del centro de masa y el desplazamiento angular :math:`\theta`, ángulo girado por el cuerpo en el tiempo :math:`t`, dado por la ecuación :eq:`Ec:Rot_Slid_03`, son respectivamente


.. math::
   :label: Ec:Rot_Slid_04a

   \begin{equation}
    s=v_0t-\frac{1}{2}\mu gt^{2}
   \end{equation}

.. math::
   :label: Ec:Rot_Slid_04b

   \begin{equation}
    \theta=\frac{1}{2}\frac{\mu mgR}{I_c}t^{2}
   \end{equation}


**Balance energético** Para la situación considerada, las energías totales antes y después de que el cuerpo ruede son

.. math::
   :label: Ec:Rot_Slid_05a

   \begin{equation}
    E_i=\frac{1}{2}mv_{0}^{2}
   \end{equation}

.. math::
   :label: Ec:Rot_Slid_05b

   \begin{equation}
    E_f=\frac{1}{2}mv_{c}^{2}+\frac{1}{2}I_c\omega^{2}=\frac{1}{2}mv_0^{2}(1-\frac{1}{k})^{2}+ \frac{1}{2}mv_0^{2}(\frac{k-1}{k^{2}})
   \end{equation}

donde hemos utilizado los valores de :math:`v_c` y :math:`\omega` dados por las ecuaciones :eq:`Ec:Rot_Slid_02a`, :eq:`Ec:Rot_Slid_02b`, :eq:`Ec:Rot_Slid_03` y :eq:`Ec:Rot_Slid_03a`. El trabajo :math:`W` realizado por la fuerza de fricción, el cual se convierte en calor (thermal energy), durante el deslizamiento está dado por

.. math::
   :label: Ec:Rot_Slid_06

   \begin{equation}
     W=E_f-E_i=-\frac{1}{2k}mv_{0}^{2}
   \end{equation}

donde :math:`k` está dado por la ecuación :eq:`Ec:Rot_Slid_03a`.

**Descripción de la interfaz de la aplicación**

La :numref:`fig:Rot_Slid_01` muestra la interfaz gráfica del usuario que permite estudiar los efectos del rozamiento sobre el deslizamiento y rodadura de cuerpos que se mueven sobre una superficie horizontal.  La aplicación permite no solamente seleccionar cuatro diferentes cuerpos: esfera sólida **Solid sphere**, esfera hueca **Spherical shell**, cilindro sólido **Solid cylinder** y un cilindro hueco **Cylindrical shell** sino también sus masas y radios a través de las barras de desplazamiento rotuladas **Mass** y **Radius**. De igual manera, se puede seleccionar la velocidad inicial del centro de masa de estos cuerpos y el coeficiente de rozamiento (:math:`\mu`) entre la superficie horizontal y los cuerpos a través de las barras de desplazamiento rotuladas **Initial velocity** (Velocidad inicial) y **Coefficient of friction** (Coeficiente de fricción) respectivamente. A medida que los cuerpos se mueven se puede observar la trayectoria seguida por un punto de la periferia de los mismos.

.. figure:: /images/Mecanica/Rotation_Sliding/gui_01.png
   :alt:
   :scale: 50
   :align: center
   :name: fig:Rot_Slid_01

   Interfaz gráfica del usuario.

**Mediciones y procedimientos**

   #. Fije los valores del radio, masa en :math:`R=1\,\text{m}` y :math:`m=1\,\text{kg}` y coeficiente de rozamiento :math:`\mu=0`. Sin cambiar estos valores y para cada uno de los cuatro cuerpos (esfera sólida, hueca, cilindro sólido y hueco) aplique velocidades diferentes. Observe el movimiento de cada uno de estos cuerpos. ¿Qué clase de movimiento realizan en términos de traslación y rotación?
   #. Fije los valores del radio, masa en :math:`R=1\,\text{m}` y :math:`m=1\,\text{kg}` y coeficiente de rozamiento :math:`\mu\neq0`.  Sin cambiar estos valores y para cada uno de los cuatro cuerpos (esfera sólida, hueca, cilindro sólido y hueco) aplique velocidades diferentes. Observe el movimiento de cada uno de estos cuerpos. ¿Qué clase de movimiento realizan en términos de traslación y rotación?
   #. Fije los valores del radio, masa en :math:`R=1\,\text{m}` y :math:`m=1\,\text{kg}` y coeficiente de rozamiento :math:`\mu=0.5`.  Sin cambiar estos valores y para cada uno de los cuatro cuerpos ( cilindro sólido, esfera sólida, cilindro hueco, y esfera hueca) tome mediciones de distancia de deslizamiento :math:`s` (slipping distance) como función de la velocidad inicial :math:`v_0`. Registre estas cantidades en la :numref:`tab:Rot_Slid_01`, la :numref:`tab:Rot_Slid_02`, la :numref:`tab:Rot_Slid_03` y la :numref:`tab:Rot_Slid_04`.
   #. A partir de los datos recopilados en el inciso 1 grafique  la distancia de deslizamiento :math:`s` para cada cuerpo en función de la velocidad inicial :math:`v_0`. Aplique sus conocimientos de linealización de funciones para demostrar que la relación entre :math:`s` y :math:`v_0` tiene la forma :math:`s=Av_0^{2}`, siendo :math:`A` una constante la cual debe determinar.
   #. Teniendo en cuenta los resultados del inciso 2 verifique que los valores de :math:`A` encontrados cumplen :math:`A=\frac{1}{\mu gk}(1-\frac{1}{2k})`, donde :math:`k` está definido por la ecuación :eq:`Ec:Rot_Slid_03a`. Este valor de :math:`A` se sigue de las ecuaciones :eq:`Ec:Rot_Slid_03` y :eq:`Ec:Rot_Slid_04a`.

   #. Verifique el balance de energía: Tome la esfera sólida con :math:`m=1\,\text{kg}`, :math:`R=1\,\text{m}` y :math:`v_0=`2 m/s, :math:`v_0=`5 m/s y :math:`v_0=` 10 m/s. Para cada velocidad, registre los valores de la energía cinética traslacional inicial, la energía cinética traslacional final, la energía cinética rotacional final y la energía disipada en forma de calor arrojados por el simulador. Compare estos valores con los obtenidos a partir de las ecuaciones teóricas :eq:`Ec:Rot_Slid_05a`, :eq:`Ec:Rot_Slid_05b` y :eq:`Ec:Rot_Slid_06`. Discuta sus resultados.

      .. csv-table:: Cilindro sólido.
         :header: ":math:`v_0` (m/s)", ":math:`s` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Rot_Slid_01
         :align: center

         2,
         3,
         4,
         5,
         6,
         7,
         8,
         9,
         10,

      .. csv-table:: Esfera sólida.
         :header: ":math:`v_0` (m/s)", ":math:`s` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Rot_Slid_02
         :align: center

         2,
         3,
         4,
         5,
         6,
         7,
         8,
         9,
         10,

      .. csv-table:: Cilindro hueco.
         :header: ":math:`v_0` (m/s)", ":math:`s` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Rot_Slid_03
         :align: center

         2,
         3,
         4,
         5,
         6,
         7,
         8,
         9,
         10,

      .. csv-table:: Esfera hueca
         :header: ":math:`v_0` (m/s)", ":math:`s` (m)"
         :widths: 1,1
         :width: 12 cm
         :name: tab:Rot_Slid_04
         :align: center

         2,
         3,
         4,
         5,
         6,
         7,
         8,
         9,
         10,