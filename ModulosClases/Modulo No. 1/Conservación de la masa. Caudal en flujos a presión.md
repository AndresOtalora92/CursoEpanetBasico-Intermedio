# Curso de Epanet - Módulo 1 - Conservación de la masa y conservación de la energía 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/5e4e6f45e715bf4b5054fa289e045ede8dc073c9/.jpg/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

Keywords: `Energía` `Bernoulli` `Flujo` `Flujo másico` `masa`

## Introducción.

En este módulo se presentan de manera general los conceptos básicos y las ecuaciones que definen la conservación de la masa y la conservación de la energía en un sistema hidráulica a presión.

## Objetivos.


## Conservación de la masa. Definiciones.

La ley de conservación de la masa o ley de continuidad dice que en un sistema cerrado, la diferencia entre todas las entradas y todas las salidas son iguales al cambio del volumen con respecto al tiempo.

En la siguiente expresión se presenta la ecuación de continuidad para un flujo laminar e incompresible.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b911cf646e86e32832b69d3ec579c52bee55861f/ecuaciones/Ecuacion7.PNG" width="300px">
</div>

Para sistemas hidráulicos donde no existe acumulación temporal del fluido y también cuando el flujo está en codniciones permanentes, la ecuación de continuidad se puede presentar así:

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b911cf646e86e32832b69d3ec579c52bee55861f/ecuaciones/Ecuacion8.PNG" width="300px">
</div>

Esta es una de las ecuaciones que el software EPANET resuelve en cada uno de los nodos que componen una red. Para el uso de los signos de estas ecuaciones, se utiliza un sistema nemotécnico el asume que los caudales que ingresan al volumen de control son negativos y los caudales que salen del volumen de control son negativos. 

En la siguiente figura se muestra una representación del volumen de control de una tubería que trabaja con flujo a presión. En esta figura se detallan las fronteras en las cuales se definen los caudales de entrada y los caudales de salida.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/21c6dfa9c6ec4a19b5417773f9f65212f2912332/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.9.PNG" width="300px">
</div>

En algunos  casos particulares, cuando la densidad del fluido que ingresa a un volumen de control es diferente a la densidad del fluido que sale, la ecuación de continuidad debe expresarse en función del flujo másico. 

El flujo másico corresponde a la cantidad de masa que atraviesa una sección transversal. 

El flujo másico se puede expresar como:

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d533ca3d1ab70564657225da5b6563beb035ddbb/ecuaciones/Ecuacion10.PNG" width="150px">
</div>

Con base en lo anterior, la ecuación de continuidad para un sistema permanente y sin acumulación corresponde a:

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/d533ca3d1ab70564657225da5b6563beb035ddbb/ecuaciones/Ecuacion11.PNG" width="300px">
</div>

Está última ecuación es utilizada por EPANET para la aplicación de su módulo de "simulación de calidad del agua".

## Ecuaciones experimentales para la estimación de los caudales en tuberías a presión. 

Existen diferentes ecuaciones empíricas para la estimación del caudal en una tubería a presión. Estas ecuaciones en general depende de las propiedades del fluido transportado y del gradiente hidráulico. 

A continuación se presentan dos de las ecuaciones más utilizadas para la estimación del caudal en un sistema a presión.

###  Ecuación de Hagen-Poiseuille

Para la estimación de un flujo laminar incompresible en una tubería a presión de sección circular y en condiciones de régimen permanente para flujos con números de Reynolds menores a 2000, es posible utilizar la ecuación Hagen - Poiseuille.

Para nuestro curso, estas ecuaciones pueden ser utilizadas para comparar y analizar los resultados en tramos de tuberías una vez se ejecute el programa. También pueden ser utilizadas para el predimensionamiento de las tuberías que componen el sistema antes de cargar la geometría definitiva al programa. 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/ead0db5e3ae843a3bc497c937de37da2dc845938/ecuaciones/Ecuacion12.PNG" width="250px">
</div>


Donde,

<br> Q= Caudal de la tubería (m³/s)
<br> g = aceleración de la gravedad (m/s²)
<br> D = Diámetro (m)
<br> $\Delta(P/\gamma)$: Pendiente de la línea piezométrica
<br> $\vartheta$: Viscosidad cinemática del fluido (m²/s)


| [:arrow_backward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/1a82bdf77ecf33746dd6f0104d22f442e454a049/ModulosClases/Modulo%20No.%201/Conceptos%20generales%20de%20flujo%20a%20presi%C3%B3n.md)| [:house:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/wiki) | [:arrow_forward:](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/1a82bdf77ecf33746dd6f0104d22f442e454a049/ModulosClases/Modulo%20No.%201/Conservaci%C3%B3n%20de%20la%20energ%C3%ADa.md) |
|-----------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|