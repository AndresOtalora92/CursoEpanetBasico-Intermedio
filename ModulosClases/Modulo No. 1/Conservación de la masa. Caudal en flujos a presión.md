# Curso de Epanet - Módulo 1 - Conservación de la masa y conservación de la energía 

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/5e4e6f45e715bf4b5054fa289e045ede8dc073c9/.jpg/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

## Conservación de la energía. 
 
Keywords: `Energía` `Bernoulli` `Flujo` `Flujo másico` `masa`

En este módulo se presenta de manera general los conceptos básicos y las ecuaciones que definen la conservación de la masa y la conservación de la energía en un sistema hidráulica a presión.

### Conservación de la masa.

La ley de conservación de la masa o ley de continuidad versa que en un sistema definido y limitado, la diferencia entre todas las entradas y todas las salidas son iguales al cambio del volumen (almacenamiento) con respecto al tiempo.

En la siguiente expresión se presenta la ecuación de continuidad para un flujo laminar e incompresible.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b911cf646e86e32832b69d3ec579c52bee55861f/ecuaciones/Ecuacion7.PNG" width="300px">
</div>

Para sistemas donde no existe acumulación temporal de fluido y para flujos permanentes, la ecuación de continuidad se puede presentar así:

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b911cf646e86e32832b69d3ec579c52bee55861f/ecuaciones/Ecuacion8.PNG" width="300px">
</div>

Esta es una de las ecuaciones que el software EPANET resuelve en cada uno de los nodos que componen una red. Para el uso de los signos de estas ecuaciones, en general se utiliza el sistema nemotécnico en el que se asume que los caudales que ingresan al volumen de control son negativos y los caudales que salen del volumen de control son negativos. 

En la siguiente figura se muestra una representación del volumen de control de una tubería en el que se detallan las fronteras en las cuales se definen los caudales de entrada y los caudales de salida.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/21c6dfa9c6ec4a19b5417773f9f65212f2912332/ModulosClases/Modulo%20No.%201/Imagenes/Figuras%20No.%201.9.PNG" width="400px">
</div>

### Conservación de la energía total. Ecuación de Bernoulli

- Conceptos y ecuación, explicando los términos.

<div align="center">
  <img src="https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/7adbd7306d46c6691be5d78d4677b544672284fe/ecuaciones/Ecuacion9.PNG" width="200px">
</div>

Donde,

<br>Q= Calor [J]</b>
<br>W= Trabajo [J]</b>
<br>E= Energía total en el sistema [J]</b>

- Energía de bombas (general ya que en el módulo 1.4 se ampliará este  tema)
- Pérdida de Energía (general ya que en el módulo 1.3 se ampliará este  tema)
- Línea de energía (concepto y aplicación. Agregar dibujo)
- Linea piezométrica (concepto y aplicación. Agregar dibujo)


