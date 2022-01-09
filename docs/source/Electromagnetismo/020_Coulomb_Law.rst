Ley de Coulomb
===============

**Objetivo**
El propósito de esta práctica es estudiar de manera cuantitativa la fuerza de interacción electrostática entre partículas puntuales cargadas eléctricamente (ley de Coulomb).

**Recursos**

   #. Computador o tablet con acceso a la internet.
   #. Simulación disponible en `https://ustboniface.ca/physique/file/CoulombPendulum.zip <https://ustboniface.ca/physique/file/CoulombPendulum.zip>`_.

**Resumen teórico**

Cuando dos cargas eléctricas puntuales :math:`Q_1` y :math:`Q_2` se encuentran separadas una distancia :math:`r`, entre estas existe una fuerza :math:`F` de interacción que es atractiva si las cargas tienen signos contrarios y repulsiva si las cargas tienen signos iguales, ver :numref:`Fig:coulomb`. El valor de esta fuerza depende de la magnitud de :math:`Q_1` y :math:`Q_2`, de la distancia de separación :math:`r` entre estas y del medio en el cual se encuentren (vacío, aire, agua, etc)

.. figure:: /images/Electromagnetismo/Coulomb_Law/coulomb1.png
   :scale: 80
   :align: center
   :name: Fig:coulomb

   Fuerza electrostática entre cargas

La fuerza de interacción tiene la forma :math:`F=k\frac{Q_1^{\alpha}Q_2^{\beta}}{r^{n}}`, donde :math:`k` es una constante y :math:`n`, :math:`\alpha` y :math:`\beta` son números reales.  La :numref:`Fig:coulomb2` muestra las fuerzas sobre el cuerpo que pende de la cuerda cuando este se encuentra en equilibrio. Al aplicar la segunda ley de Newton se encuentra:

.. figure:: /images/Electromagnetismo/Coulomb_Law/coulomb2.png
   :scale: 80
   :align: center
   :name: Fig:coulomb2

   Fuerzas sobre :math:`Q_1`

.. math::
   :label: Coulom_Ec_01a

   \begin{eqnarray}
    T\cos\theta = mg
   \end{eqnarray}

.. math::
   :label: Coulom_Ec_01b

   \begin{eqnarray}
    T\sin\theta = F
   \end{eqnarray}

donde :math:`F` es la fuerza electrostática. De estas ecuaciones se sigue que :math:`F=mg\tan\theta`. Si el ángulo :math:`\theta` es muy pequeño :math:`\tan\theta\approx\sin\theta=\frac{R_1}{L}` y por tanto

.. math::
   :label: Coulom_Ec_02

   \begin{equation}
    F=\frac{mgR_1}{L}
   \end{equation}

**Descripción de la interfaz de la aplicación**

La :numref:`Fig:Gui_Coulomb_01` muestra la interfaz gráfica del usuario que permite estudiar la interacción electrostática entre dos cuerpos esféricos pequeños  cargados eléctricamente con cargas :math:`Q_1`  y :math:`Q_2` de igual signo. Uno de ellos posee masa :math:`m` y pende de una cuerda ligera aislante de longitud :math:`L` muy grande. El otro cuerpo de carga :math:`Q_2` se encuentra fijo a un soporte aislante que se puede desplazar horizontalmente hacia la derecha o izquierda. Al presionar el botón **Charge both spheres** ambos cuerpos son cargados con igual carga. Una vez cargados, sus cargas se pueden duplicar o reducir a la mitad al presionar los botones **Double** :math:`Q_1`, **Double** :math:`Q_2` y **Divide** :math:`Q_1` by 2, **Divide** :math:`Q_2` by 2 respectivamente. La posición :math:`R_2` de la carga :math:`Q_2` fija al soporte móvil se puede cambiar mediante la barra de desplazamiento en el rango :math:`-40\,\text{mm}<R_2<\,10\,\text{mm}`. La posición de la carga :math:`Q_1`  viene dada por la coordenada :math:`R_1`. Los valores de :math:`R_1` y :math:`R_2` se leen directamente de la cinta métrica ubicada en la parte inferior de la interfaz. La magnitud de la fuerza de interacción entre los cuerpos viene dada por la expresión :eq:`Coulom_Ec_02`.

.. figure:: /images/Electromagnetismo/Coulomb_Law/Gui_Coulomb_02.png
   :scale: 60
   :align: center
   :name: Fig:Gui_Coulomb_01

   Sistema utilizado para estudiar la interacción electrostática entre cargas puntuales

**Mediciones y procedimientos**

Los valores de la longitud :math:`L` de la cuerda, la masa :math:`m` del cuerpo que pende de la cuerda se leen directamente de la interfaz gráfica, a igual que otras constantes que podría utilizar.

**Relación entre** :math:`F` y :math:`r`

   #. Para determinar la relación entre :math:`F` y :math:`r` mantenga :math:`Q_1` y :math:`Q_2` fijos, para ello cargue primero las esferas y modifique si es necesario la carga de las esferas de modo que la distancia entre éstas sea de unos 15 mm. Realice la toma de datos al ir acercando la carga :math:`Q_2` hacia :math:`Q_1`, lo cual se logra con la barra horizontal deslizadora cuyo rango es [-40 mm...10 mm]. Varíe la posición del dial de la barra cada 5 unidades y registre los correspondientes valores de :math:`R_1` y :math:`R_2` en la :numref:`tab:Coulomb_F_v_r`.

      .. csv-table:: Datos simulados para determinar la ralación entre :math:`F` y :math:`r`
         :header: ":math:`R_1` (mm)", ":math:`R_2` (mm)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:Coulomb_F_v_r
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

   #. Realice una gráfica de :math:`F` en función de :math:`r`.
   #. Haga uso de sus conocimientos de linealización de una función para encontrar la ecuación matemática que relaciona las variables :math:`F` y :math:`r`. Determine el valor de :math:`n`.

.. _Relac_FQ1:

**Relación entre** :math:`F` y :math:`Q_1`

   #. Para determinar la relación entre :math:`F` y :math:`Q_1` mantenga :math:`Q_2` constante tanto en valor como posición, para ello cargue primero las esferas y modifique si es necesario el valor de :math:`Q_1` de modo que la distancia entre las esferas sea de unos 15 mm.  Aumente el valor de :math:`Q_1` y registre los valores de :math:`R_1` y :math:`R_2` para cada nuevo valor de :math:`Q_1`. Complete la :numref:`tab:Coulomb_F_vs_q1`.

      .. csv-table:: Datos simulados para determinar la ralación entre :math:`F` y :math:`Q_1`
         :header: ":math:`Q_1` (mm)", ":math:`R_1` (mm)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:Coulomb_F_vs_q1
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

   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`F` y :math:`Q_1`. En este punto tenemos dos asuntos que considerar:

      a. El valor numérico de las cargas no se conoce, lo único que la aplicación nos permite hacer es duplicar o dividir la carga inicial tantas veces como queramos. Luego, ¿qué valor de carga tomamos?  Respuesta: asumimos que la carga inicial de cada una de las cargas inicialmente es :math:`Q_0` y trabajamos con múltiplos de esta carga. Sobre el eje horizontal de carga tomamos :math:`2` o  :math:`\frac{1}{2}` en caso de duplicar o dividir la carga entre 2 y el eje horizontal es multiplicado por :math:`Q_0`.
      b. Al variar la carga :math:`Q_1` la distancia :math:`r` entre las cargas cambia y debería permanecer constante. Así, para encontrar la dependencia entre :math:`F` y :math:`Q_1`, graficamos :math:`Fr^{2}` en función de :math:`Q_1` que son múltiplos de :math:`Q_0`. Determine el valor de :math:`\alpha`.

**Relación entre** :math:`F` y :math:`Q_2`

   #. Para determinar la relación entre :math:`F` y :math:`Q_2` mantenga :math:`Q_1` constante en valor, para ello cargue primero las esferas y modifique si es necesario el valor de :math:`Q_2` de modo que la distancia entre las esferas sea de unos 15 mm.  Aumente el valor de :math:`Q_2` sin modificar su posición y registre los valores de :math:`R_1` y :math:`R_2` para cada nuevo valor de :math:`Q_2`. Complete la :numref:`tab:Coulomb_F_v_q2`.

      .. csv-table:: Datos simulados para determinar la ralación entre :math:`F` y :math:`Q_2`
         :header: ":math:`Q_2`", ":math:`R_1` (mm)"
         :widths: 1,1
         :width: 15 cm
         :name: tab:Coulomb_F_v_q2
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

   #. Haga uso de sus conocimientos de linealización de una función para encontrar una ecuación matemática que relaciona las variables :math:`F` y :math:`Q_2`. Ver sugerencia hecha en la sección :ref:`Relación entre <Relac_FQ1>` :math:`F` y :math:`Q_1` inciso2.


Teniendo en cuenta los resultados anteriores escriba la relación entre :math:`F`, :math:`Q_1`, :math:`Q_2` y :math:`r`.

