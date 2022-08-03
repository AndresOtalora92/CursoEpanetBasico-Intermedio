# Curso de Epanet - Módulo 1 - Conceptos generales de flujo a presión. 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/5e4e6f45e715bf4b5054fa289e045ede8dc073c9/.jpg/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

.

## **Conceptos generales de flujo a presión**
En el presente capítulo se describen algunos conceptos generales relacionados con el flujo en los sistemas a presión. Se definen algunos conceptos fundamentales de la hidráulica a presión que el lector debe conocer o recordar antes de iniciar los siguientes capítulos. Es importante que el estudiante tenga bases conceptuales con el propósito de que pueda entender las diferentes variables de entrada del modelo hidráulico y que tenga la capacidad de analizar cualitativa y cuantitativamente los resultados.

### Flujo a presión. Definiciones y características.

- Definición de flujo. Flujo a presión.

El flujo corresponde al movimiento de un fluido con respecto a un sistema inercial dentro de una  superficie sólida definida. Un flujo a presión corresponde a un flujo en el cual el fluido ocupa la totalidad de las paredes o fronteras de la superficie que contiene el fluido. Por definición un flujo a presión presenta presiones distintas a la presión atmosférica. En la Figura 1.1 se presenta gráficamente este concepto.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/2e2c3acbd34f6d67e573b2b9f52194832d4b6a83/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.1a.PNG" width="400px">
</div>

>Figura 1.1 Gradiente de presiones en una tubería con flujo a presión[^1].

<br>El flujo en un sistema se genera por la diferencia de presiones entre dos puntos en una longitud definida. La diferencia de presión genera un gradiente hidráulico.Por definición, el gradiente hidráulico se define por la expresión:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/4847e332f2955fb10e068b43afe10eb44e628e18/ecuaciones/Ecuacion1.PNG" width="200px">

</div>


- Definición de caudal.

El caudal corresponde a la cantidad de fluido, en unidades de volumen, que atraviesa por una sección transversal en una unidad de tiempo. En general la unidades del caudal se expresan en m³/s, L/s o ft³/s.

Si se asume que la velocidad del flujo en toda la sección transveral es la misma y que corresponde a una velocidad media, el caudal se define así:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/afab8848680381d32398accb9c7a3e528da39c4e/ecuaciones/Ecuacion6.PNG" width="150px">

</div>

Donde, 
<br> Q: Caudal
<br>V: Velocidad Media
<br>A: Área hidráulica de la sección transversal

Si se tiene en cuenta el perfil de velocidades real en una sección transversal el caudal se define aplicando el concepto de integral, así:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/64cf7b22fee77e0c9b79e395d9e6c3347a3bf65b/ecuaciones/Ecuacion3.PNG" width="200px">

</div>

- Definición de densidad y Viscosidad.
La densidad corresponde al peso, en unidades de masa, por unidad de volumen. En los fluidos líquidos, la densidad de los fluidos aumenta a medida que disminuye la temperatura. 

La viscosidad a un efecto de la resistencia molecular de las partículas a impedir su movimiento adhiriendose a las paredes de la supeficie. La viscosidad en términos  a impedir el movimiento o su "fluidez". En los fluidos líquidos, la viscosdidad de los fluidos aumenta al reducirse la temperatura. 

En la siguiente tabla se resumen los valores de densidad y viscosidad del agua para diferentes temperatura en Sistema Internacional y Sistema Inglés.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b324f792a527b5eab104f9e9c7fa067ebc0e6fe2/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.2.PNG" width="600px">
</div>

>Figura 1.2 Densidad y viscosidad del agua[^2].

- Definición de esfuerzo cortante.

El esfuerzo cortante corresponde a la fuerza por unidad de área ejercicida por un flujo (fluido en movimiento) en las paredes de la superficie que lo contiene. El esfuerzo cortante es proporcional a la magnitud de la viscosidad del fluido.

En la siguiente ecuación se presenta una de las formas más comunes para estimar el esfuerzo cortante en función del gradiente hidráulico en un flujo a presión.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/64cf7b22fee77e0c9b79e395d9e6c3347a3bf65b/ecuaciones/Ecuacion4.PNG" width="150px">
</div>

Donde, 
<br> tau: Esfuerzo Cortante
<br> R: Radio hidráulico. A/P
<br> P: Perímetro hidráulico.
<br> Sf: gradiente hidráulico.

###  Número de Reynolds. 

El número de Reynolds corresponde a un número adimensiones (conjunto organizado de variables con dimensiones que generan un resultado adimensional) que permite establecer la relación entre las fuerza generadas por las fuerzas de fricción y las fuerzas inerciales.

Este número permite clasificar el flujo en función de su régimen; clasificación que depende mayormente de la velocidad media del flujo. En la siguiente ecuación se presenta este número adimensional.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/cb4d3c1ade36c790faa5e87fa5f849da3e4e51de/ecuaciones/Ecuacion5.PNG" width="200px">
</div>

Donde, 
<br> $\tau$: Esfuerzo Cortante
<br> R: Radio hidráulico. A/P
<br> P: Perímetro hidráulico.
<br> Sf: gradiente hidráulico.

Este número adimensional desarrollado por Osborne Reynolds, tal como se verá más adelante permite clasificar los flujos a presión en flujos laminares, en flujos en transición y en flujos turbulentos.

Reynolds desarrollo un ensayo simple utilizando un sistema hidráulico compuesto por un tanque de nivel constante, una tubería lisa y una válvula en la salida del sistema. A partir de la inyección de tinta en la tubería y realizando una revisión visual del cambio en el comportamiento filamente de la tinta en el agua, Reynolds determinó diferentes intervalos que clasifican el régimen de fluo en laminar, en transición y turbulento. 

### Régimen de flujo. Flujo laminar, en transición y turbulento.
 
A partir de los rangos definidos por Reynolds, se tiene que:

<b> 1. Flujo Laminar (Re<2200):</b> El flujo se mueve en capas sin intercambio de cantidad de movimiento entre las partículas y sin componentes perpendiculares de la velocidad. 

</br><b>2. Flujo en transición (2200<Re<4000): </b> Condición intermedia, en el cual el flujo se desarrolla, pasando entre el flujo laminar y el flujo en transición o viceversa. Existen zona donde el flujo es organizado y zona donde el flujo es errático.

</br><b>3. Flujo turbulento (Re>4000): </b> El flujo se mueve de manera errática, con intercambio de cantidad de movimiento entre las partículas y con presencia de componentes de velocidad en todas las direcciones.

En la siguiente figura se presenta una representación esquemática del experimento de Reynolds para cada uno de los tres régimen de flujo.


<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/a034c28cfd68cf4cca1b0e7565e40ac925cf0a76/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.3.PNG" width="400px">
</div>


### Redes hidráulicas. Definición, usos y aplicaciones de los sistemas a presión.


#### Definición de red de drenaje.
Una red de drenaje corresponde a la disposición de tuberías y accesorios hidráulicos cuyo objetivo corresponde al transporte y disposición un fluido para cumplir las demandas en puntos particulares.

#### Consideraciones y limites de un diseño hidráulico una red de drenaje en función del caudal, la velocidad, las presiones y el esfuerzo cortante.

Como se analizará más adelante en los siguientes módulos, el diseño hidráulico de sistemas de tuberías a presión (trazado y dimensionamiento) depende del caudal que se requiera con el objetivo de cumplir un caudal mínimo demandado en los nodos o puntos de consumo. El diseño de los sistemas hidráulicos se limitan en función de la magnitud de la velocidad, las presiones y el esfuerzo cortante tanto en los tramos de tuberías como en lo nodos. 

Los límites mínimos y máximos de estas variables generalmente están definidos por el criterio y la experiencia del diseñador, el cumplimiento de normas o recomendaciones de referencia bibliográficas y el límite definido por la resistencia de los materiales que conforman las tuberías y accesorios. 

#### Usos y aplicaciones.

Son muchas las aplicaciones de las redes hidráulica de flujos a presión. Entre los más importantes se pueden destacar los siguientes:

<b>- Sistemas de riego:</b> Corresponde a los sistemas de tuberías que permite el transporte y riego de las zonas de cultivo. El trazado y disposición de esta red generalmente se debe adaptar a la distribución de los cultivos en las parcelas, fincas y predios. La red permite el transporte del flujo de manera controlada, tanto en tiempo como en cantidad, pemitiendo una riego adecuado para el crecimiento óptimo de las plantas. 

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.4.PNG" width="400px">
</div>

<b>- Acueductos:</b> Corresponde a la red que permite el transporte de agua potable desde una fuente hasta la población. En general, las fuentes de abastecimiento de los acueductos corresponde a embalses, ríos o pozos. 

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.5.PNG" width="350px">
</div>



<b> - Redes hidrosanitarias y contraincendios </b>:
Las redes hidrosanitarias de acueducto corresponden a las redes internas de las edificaciones, viviendas familiares, fábricas, estructuras comerciales, etc, que transportan el agua potable desde la red principal o secundaria del acueducto a los accesorios hidrosanitarios tales como grifos, cisternas, lavamanos, etc.

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
    <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.6.PNG" width="400px">
</div>

### Tipos de redes. Descripción.

Los sistemas y redes que utilizan flujo a presiones pueden clasificarse según la distribución especial de los elementos que componen una red hidráulica (nodos, accesorias y tuberías). Es común clasificar las redes como: redes abiertas y redes cerradas.

</br><b> Red cerrada: </b> Una red cerrada corresponde un sistema hidráulico compuesto por tuberías las cuales crean una matriz cerrada, donde el flujo podría recircular desde su punto de inicio hasta su punto final. 

En la siguiente imagen se presenta un ejemplo de un sistema de una red cerrada.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d3e14012243523316c9bb5c3d7932bda146077f9/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.7.PNG" width="450px">

</div>

</br><b> Red abierta: </b> Una red abierta, como su nombre lo indica corresponden a las redes en los cuales los caudales pueden salir del sistema en un nodo. En una red abierta no existen lo bluces o mallas cerradas. El caudal del punto de inicio nunca llegará completo al nodo final. 

En la siguiente imagen se presenta un ejemplo de un sistema de una red abierta.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d3e14012243523316c9bb5c3d7932bda146077f9/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.8.jpg" width="400px">

</div>

| [:arrow_backward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/wiki)| [:house:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/wiki) | [:arrow_forward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/be22d58a4322199c62bd8b9341fdd5a6a01f2e17/ModulosClases/Modulo%20No.%201/Conservaci%C3%B3n%20de%20la%20energ%C3%ADa.md) |
|-----------|-------------|---------------------|

[^1]: Saldarriaga, Juan. Hidráulica a Presión (2019).
[^2]: Frank M. White. Mecanica De Fluidos (2020).