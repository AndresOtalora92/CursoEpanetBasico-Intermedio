# Curso de Epanet - Módulo 1 - Submódulo 1.1. 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/5e4e6f45e715bf4b5054fa289e045ede8dc073c9/.jpg/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>



## **1.1 Conceptos generales de flujo a presión**
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
Q = V * A
</div>

Donde, 
<br> Q: Caudal
<br>V: Velocidad Media
<br>A: Área hidráulica de la sección transversal

Si se tiene en cuenta el perfil de velocidades real en una sección transversal el caudal se define aplicando el concepto de integral, así:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/64cf7b22fee77e0c9b79e395d9e6c3347a3bf65b/ecuaciones/Ecuacion3.PNG" width="100px">

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
<br> $\mu$: Esfuerzo Cortante
<br> R: Radio hidráulico. A/P
<br> P: Perímetro hidráulico.
<br> Sf: gradiente hidráulico.


Como se verá más adelante la magnitud de este número permite clasificar los flujos a presión en flujos laminares, en flujos en transición y en flujos turbulentos.


### Régimen de flujo. Flujo laminar, en transición y turbulento.

Descripción y gráficos de los tipos de flujo. Puede tomarse fotos del laboratorio de hidráulica


### Flujo en tuberías. Definición, usos y aplicaciones de los sistemas a presión.


#### Definición de un sistema hidráulico.


#### Consideraciones y limites de un diseño hidráulico en función del caudal, la velocidad, las presiones y el esfuerzo cortante.


Como se analizará más adelante en los siguientes módulos, el diseño hidráulico de sistemas de tuberías a presión (trazado y dimensionamiento) depende del caudal que se requiera con el objetivo de cumplir un caudal mínimo demandado en los nodos o puntos de consumo. El diseño de los sistemas hidráulicos se limitan en función de la magnitud de la velocidad, las presiones y el esfuerzo cortante tanto en los tramos de tuberías como en lo nodos. 

Los límites mínimos y máximos de estas variables generalmente están definidos por el criterio y la experiencia del diseñador, el cumplimiento de normas o recomendaciones de referencia bibliográficas y el límite definido por la resistencia de los materiales que conforman las tuberías y accesorios. 

#### Usos y aplicaciones.

- Sistemas de riego (agregar gráfico y descripción)
- Acueductos (agregar gráfico y descripción)
- Redes hidrosanitarias (agregar gráfico y descripción)




### Tipos de redes. Descripción.

- Definición de red.
- Concepto muy básico de redes abiertas (este tema se manejará en el módulo 3).
- Concepto muy básico de redes cerradas (este tema se manejará en el módulo 3).


[^1]: Saldarriaga, Juan. Hidráulica a Presión.
[^2]: Frank M. White. Mecanica De Fluidos (2020)