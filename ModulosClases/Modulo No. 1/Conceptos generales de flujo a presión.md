# Curso de Epanet - Módulo 1 - Conceptos generales de los flujos a presión. 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/5e4e6f45e715bf4b5054fa289e045ede8dc073c9/.jpg/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

Keywords: `Presión` `Hidráulica` `Redes` `Flujo`

## Introducción.

En el presente capítulo se describen algunos conceptos generales relacionados con los flujos a presión. Se definen fundamentos de la hidráulica que el lector debe conocer o recordar antes de trabajar las siguientes actividades. También se describen los principales usos y aplicaciones de los flujos a presión y se mencionan algunas clasificaciones de los flujos a presión y de las redes que componen los sistemas hidráulicos.

Es importante que el estudiante tenga presente que unas adecuadas bases conceptuales son necesarias si su propósito es entender las diferentes variables que definen los modelos hidráulicos, en especial los modelos hidráulicos para la simulación de los sistemas a presión. Antes de iniciar el proceso de cargue y ejecución del modelo EPANET, el usuario debe conocer los conceptos detrás de las variables entrada del modelo para que pueda comprender y posteriormente analizar cualitativa y cuantitativamente los resultados.


## Objetivos. 

El objetivo principal de esta actividad es permitir que el estudiante aprenda, recuerde y practique los conceptos básicos de los flujos a presión con el propósito de adquirir habilidades para el uso, cargue y ejecución del modelo EPANET. 

## Flujo a presión. Definiciones y características.

El flujo corresponde al movimiento de un fluido en una superficie sólida, tomando como referencia un sistema inercial. Un flujo a presión corresponde a un flujo en el cual el fluido ocupa la totalidad del área del conducto que conduce que lo conduce. Por definición, un flujo a presión presenta presiones distintas a la presión atmosférica. 

En la Figura 1.1 se presenta gráficamente este concepto.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/2e2c3acbd34f6d67e573b2b9f52194832d4b6a83/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.1a.PNG" width="400px">
</div>

>Figura 1.1 Gradiente de presiones en una tubería con flujo a presión[^1].

<br> Para sistemas a presión, el flujo se genera debido a la diferencia de presiones entre dos puntos a lo largo de una tubería o un sistemas de tuberías. A partir de la diferencia de presiones entre dos puntos y la distancia longitudinal que los separa, es posible la estimación de su gradiente hidráulico.

Por definición, el gradiente hidráulico se puede expresar como:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/4847e332f2955fb10e068b43afe10eb44e628e18/ecuaciones/Ecuacion1.PNG" width="200px">

</div>


### Caudal

En términos generales, el caudal corresponde a la cantidad de fluido que atraviesa una sección transversal definida en un tiempo determinado. Las unidades del caudal usualmente utilizadas en la ingeniería aplicada corresponden a m³/s, L/s y ft³/s.

Si se asume que los vectores de velocidad del flujo a lo largo de la vertical de la sección transveral que contiene es flujo es uniforme, posible definir el caudal a partir de la siguiente expresión:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/afab8848680381d32398accb9c7a3e528da39c4e/ecuaciones/Ecuacion6.PNG" width="150px">

</div>

Donde, 
<br> Q: Caudal
<br>V: Velocidad Media
<br>A: Área hidráulica de la sección transversal

Si se tiene en cuenta el perfil de velocidades o lo que es lo mismo, la variación de los vectores de velocidad a lo largo de la vertical en una sección transversal, es posible calcular el caudal que fluye por el sistema a partir del concepto de integral, utilizando la siguiente expresión:

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/64cf7b22fee77e0c9b79e395d9e6c3347a3bf65b/ecuaciones/Ecuacion3.PNG" width="200px">

</div>

### Densidad y Viscosidad.

<b> - Densidad de los fluidos: </b> corresponde a una propiedad intrínseca de la material, que en términos simples, corresponde al peso del elemento, en este caso del fluido, por unidad de volumen. En los fluidos líquidos, la densidad aumenta a medida que la temperatura disminuye. En los fluidos gasesos, la variación de la densidad es función del tipo gas y de la presión. En los gases ideales la densidad del fluido gaseoso es inversamente proporcional a la temperatura.

<br>

</br>

<b> - Viscosidad: </b> corresponde al efecto generado por las fuerzas intermoleculares de las partículas que conforman el fluido. Estas interacciones entre las moléculas crean resistencia en contra del movimiento. La viscosidad permitir la adherencia de los fluidos en las fronteras de las superficies que lo contiene. En los fluidos líquidos, la viscosidad aumenta a medida que disminuye la temperatura. 


En la siguiente tabla se resumen los valores de densidad y viscosidad del agua líquida para diferentes temperaturas en unidades del Sistema Internacional y del Sistema Inglés.


<div align="center">


| T°c | $\rho$, Kg/m³ | $\mu$, N*s/m² | $\nu$, m²/s |
|-----|---------------|---------------|-------------|
| 0   | 1000          | 1.788*10^-3   | 1.788*10^-6 |
| 10  | 1000          | 1.307*10^-3   | 1.307*10^-6 |
| 20  | 998           | 1.003*10^-3   | 1.005*10^-6 |
| 30  | 996           | 0.799*10^-3   | 0.802*10^-6 |
| 40  | 992           | 0.657*10^-3   | 0.662*10^-6 |
| 50  | 988           | 0.548*10^-3   | 0.555*10^-6 |
| 60  | 983           | 0.457*10^-3   | 0.475*10^-6 |
| 70  | 978           | 0.405*10^-3   | 0.414*10^-6 |
| 80  | 972           | 0.355*10^-3   | 0.365*10^-6 |
| 90  | 965           | 0.316*10^-3   | 0.327*10^-6 |
| 100 | 958           | 0.283*10^-3   | 0.295*10^-6 |

</div>

>Figura 1.2 Densidad y viscosidad del agua[^2].

### Esfuerzo cortante.

Corresponde a la fuerza por unidad de área ejercicida por un flujo (fluido en movimiento) en las paredes de la superficie que lo contiene. El esfuerzo cortante es proporcional a la viscosidad del fluido, por tanto, a mayor viscosidad, mayor es el esfuerzo cortante.

A continuación se presenta una de las expresiones más usada para la estimación del esfuerzo cortante en una tubería a presión. Esta expresión es función del gradiente hidráulico:

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/64cf7b22fee77e0c9b79e395d9e6c3347a3bf65b/ecuaciones/Ecuacion4.PNG" width="150px">
</div>

Donde, 
<br> tau: Esfuerzo Cortante
<br> R: Radio hidráulico. A/P
<br> P: Perímetro hidráulico.
<br> Sf: gradiente hidráulico.


###  Número de Reynolds. 

El número de Reynolds corresponde a un número adimensional que permite establecer la relación entre las fuerzas generadas por las fuerzas de fricción y las fuerzas inerciales. Un número adimensional corresponde al conjunto organizado de variables dimensionales que generan un resultado adimensional. 

Este número adimensional desarrollado por Osborne Reynolds, permite clasificar los flujos a presión en flujos laminares, flujos en transición y flujos turbulentos.

En la siguiente ecuación se presenta el número de Reynolds.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/cb4d3c1ade36c790faa5e87fa5f849da3e4e51de/ecuaciones/Ecuacion5.PNG" width="200px">
</div>

Donde, 
<br> $\tau$: Esfuerzo Cortante
<br> R: Radio hidráulico. A/P
<br> P: Perímetro hidráulico.
<br> Sf: gradiente hidráulico.


Para la definición de los tres régimenes de flujo, Reynolds desarrollo un ensayo de laboratorio muy simple, utilizando un sistema hidráulico compuesto por un tanque de nivel constante, una tubería lisa transparente y una válvula en la salida del sistema. A partir de la inyección de tinta en la tubería y de la revisión visual del cambio de la forma del filamento de la tinta en el agua, Reynolds clasificó empíricamente los flujos. En el siguiente apartado se explica en detalle las tres régimenes de flujo en tuberías a presión.

### Régimen de flujo. Flujo laminar, en transición y turbulento.
 
A partir de los rangos definidos por Reynolds, se tiene que:

<b> 1. Flujo Laminar (Re<2200):</b> El flujo se mueve en capas sin intercambio de cantidad de movimiento entre las partículas. No existen componentes de la velocidad perpendicular a la dirección del flujo. 

</br><b>2. Flujo en transición (2200<Re<4000): </b> Condición intermedia, en el cual el flujo se desarrolla, pasando entre el flujo laminar y el flujo turbulento. Existen zonas donde el flujo es organizado y zonas donde el flujo es errático.

</br><b>3. Flujo turbulento (Re>4000): </b> El flujo se mueve de manera errática, con intercambio de cantidad de movimiento entre las partículas y con presencia de componentes de velocidad en todas las direcciones.

En la siguiente figura se muestra un ejemplo de como se ve el filamento de tinta en el experimento de Reynolds para cada uno de los tres régimen de flujo.


<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/a034c28cfd68cf4cca1b0e7565e40ac925cf0a76/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.3.PNG" width="400px">
</div>


## Redes hidráulicas. Definición, usos y aplicaciones de los sistemas a presión.


### Red hidráulica.
Una red hidráulica corresponde a la disposición de tuberías y accesorios cuyo objetivo principal el transporte y disposición de un fluido, desde un punto inicial hasta un punto final. cumpliendo las demandas de caudal del sistema.

### Consideraciones generales y límites de diseño de una red.

Como se analizará más adelante en los siguientes módulos, el diseño hidráulico de un sistema de tuberías a presión (trazado y dimensionamiento) depende del caudal demandado, las diferencias topográficas y de las condiciones particulares del proyecto. El diseño de las redes hidráulicas, está limitado generalmente por las velocidades máximas y mínimas en las tuberías, las presiones de trabajo en los nodos y los esfuerzos cortantes máximos y mínimos en el sistema.

Los límites de estas variables generalmente se definen a partir del criterio y la experiencia del diseñador y del cumplimiento de normas o recomendaciones presentadas en la literatura. El diseñador también debe tener en cuenta los límites definidos por la resistencia de los materiales que conforman las tuberías y accesorios. 

### Usos y aplicaciones.

Son muchas las aplicaciones de las redes que trabajan con flujos a presión. Entre los usos más importantes se pueden destacar los siguientes:

<b>- Sistemas de riego:</b> Corresponden a los sistemas de tuberías que permite el transporte y riego de las plantas en zonas de cultivo. El trazado y disposición de estas redes es función de la distribución espacial de los cultivos en las parcelas, fincas y predios. Este tipo de redes permite el transporte del flujo de manera controlada, tanto en tiempo como en cantidad, permitiendo una riego adecuado para el crecimiento óptimo de las plantas. 

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.4.PNG" width="400px">
</div>

<b>- Acueductos:</b> Corresponden a las redes que permite el transporte de agua potable desde una fuente hasta una población. En general, las fuentes de abastecimiento de los acueductos corresponde a embalses, ríos o pozos. 

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.5.PNG" width="350px">
</div>



<b> - Redes hidrosanitarias </b>:
Las redes hidrosanitarias corresponden a las redes internas en las edificaciones, viviendas familiares, fábricas, bodegas y estructuras comerciales que permiten el transporte del agua potable desde la red del acueducto hasta los accesorios hidrosanitarios. Entre los accesorios hidrosanitarios más comunes se destacan los grifos, las cisternas, los lavamanos y las duchas.

En la siguiente imagen se presenta un ejemplo de estas redes.

<div align="center">
    <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/c20a650d6356260a96d940e3a1c2df40c4e1191e/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.6.PNG" width="400px">
</div>

### Tipos de redes. Descripción.

Los sistemas y redes que trabajan con flujos a presiones pueden clasificarse según la distribución espacial de los elementos que componen la red. Es común clasificar las redes em: redes abiertas y redes cerradas.

</br><b> Red cerrada: </b> Una red cerrada corresponde a un sistema hidráulico compuesto por tuberías y accesorios cuya disposición permite crear una malla cerrada, donde el flujo puede recircular desde su punto de inicio hasta su punto final. 

En la siguiente imagen se presenta un ejemplo de un sistema hidráulico compuesto por una red cerrada.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d3e14012243523316c9bb5c3d7932bda146077f9/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.7.PNG" width="450px">

</div>

</br><b> Red abierta: </b> Una red abierta, como su nombre lo indica, corresponde a una red cuya disposición final no permite la existencia bluces o mallas cerradas. El caudal del punto de inicio nunca llegará completo al nodo final, ya que los caudales pueden salir del sistema.

En la siguiente imagen se presenta un ejemplo de un sistema hidráulico compuesto por una red abierta.

<div align="center">

  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d3e14012243523316c9bb5c3d7932bda146077f9/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.8.jpg" width="400px">

</div>

| [:arrow_backward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/wiki)| [:house:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/wiki) | [:arrow_forward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/main/ModulosClases/Modulo%20No.%201/Conservaci%C3%B3n%20de%20la%20masa.%20Caudal%20en%20flujos%20a%20presi%C3%B3n.md) |
|-----------|-------------|----------------------------------------------------------------------------------------------------------|

[^1]: Saldarriaga, Juan. Hidráulica a Presión (2019).
[^2]: Frank M. White. Mecanica De Fluidos (2020).