# Curso de Epanet - Módulo 1 - Conceptos generales de redes abiertas y redes cerradas

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>


Keywords: `Redes cerradas` `Redes abiertas` `Solución de sistemas` `Nodos`

## Introducción

En esta actividad se describen los conceptos generales y las principales características de los sistemas hidráulicos compuestos por redes, los cuales pueden ser clasificados como redes abiertas y redes cerradas. Se describirán conceptualmente algunas metodologías numéricas para la solución de los sistemas de ecuaciones que se generan cuando se requiere la estimación del caudal en estos sistemas. Finalmente, se describirán algunas recomendaciones a la hora de plantear estos sistemas matemáticos.

## Objetivos

El objetivo principal de esta actividad es crear al usuario las nociones fundamentales que gobiernan la hidráulica de una red cerrada y de una red abierta y sus posibles métodos de estimación del caudal circulante por cada tubería o circuito, con el propósito de que se tengan los conceptos generales a la hora de trazar y posteriormente solucionar el sistema utilizando el software de modelación EPANET y sus complementos de trazado tales como EPA-CAD y el mismo AutoCAD.

## Redes abiertas. Conceptos

Por definición una red hidráulica abierta corresponda a aquellas tuberías que están dispuestas de tal manera que no crean una malla o circuito cerrado. En una red abierta las tuberías están configuradas están ramificadas sin interceptar, sin crear ciclos o mallas continuas. Los extremos de los ramales pueden finalizar en un tanque o pueden descargar a la atmósfera.

En la siguiente imagen se presenta un ejemplo de una típica red abierta. En este caso tres tanques de nivel constante alimentan un tanque. Los tres tanques se conectan, en el nodo A, permitiendo que el caudal generado por los tres tanques llegue al cuarto.

<div align="center">

  <img src="Imagenes/FiguraNo.1.31.PNG" width="300px">

</div>

## Planteamiento y solución de sistemas hidráulicos de redes abiertas

En un sistema hidráulico compuesto por tuberías que funcionan con flujo a presión es necesario identificar los elementos que componen el sistema (tramos de tubería, nodos, accesorios, etc.) antes de plantera cualquier ecuación o cualquier sistema de ecuaciones.

En el caso particular de una red abierta es posible la estimación de las variables hidráulicas (caudales, presiones, velocidad y esfuerzos cortantes) utilizando las ecuaciones de conservación de la energía y conservación de la masa. A continuación se explica de manera general los conceptos y procedimientos que deben tenerse en cuenta para el planteamiento de las ecuaciones que rigen el comportamiento hidráulico de las redes abiertas. 

### Ecuaciones y variables. Solución de una red abierta

Como se ha visto en las demás actividades, las ecuaciones fundamentales para la solución de problemas relacionados con los flujos a presión corresponden a la conservación de la masa y la conservación de la energía. 

Para un sistema abierto generalmente la incógnita corresponde al caudal que transita por cada tubería y la columna de presión en los nodos intermedios. Con base en esto,  se recomienda como primer paso identificar las incógnitas que definen el problema, posteriormente plantear las ecuaciones y finalmente solucionar el sistema de ecuaciones planteadas.

En cada nodo es necesario plantear la ecuación de conservación de la masa, identificando el caudal o los caudales que ingresas al nodo y el caudal o los caudales que salen del nodo así:

ECUACIÓN

Posteriormente, debe plantearse la ecuación de conservación de energía o Bernoulli entre dos puntos tantas veces como caudales deban determinarse. Los puntos de inicio y fin en el planteamiento de la ecuación de energía generalmente se seleccionan desde el inicio de uno de los ramales hasta un nodo o desde un nodo particular hasta el final de un ramal. Esta identificación dependerá del problema. 

El usuario debe generar tantas ecuaciones como incógnitas tenga la red y solucionar el sistema de ecuaciones como mejor le convenga. En resumidas cuentas, este procedimiento es lo que los desarrolladores del código de EPANET han planteado: La solución de sistemas de ecuaciones que permitan la determinación de las variables hidráulicas a partir de la aplicación de métodos numéricos. 

### Ejemplo conceptual. Solución de una red abierta

Con el propósito de reforzar los conceptos definidos anteriormente se plantearán las ecuaciones necesarias para la determinación de los caudales (Qi) y las presiones(Pi) en la red abierta presentada anteriormente y que a continuación se amplía.

IMAGEN

Siguiendo las recomendaciones mencionadas, inicialmente se deben identificar las particularidades del sistema. En este caso se observa que el sistema está compuesto por tres tanques que alimentan una cuarto tanque. Las tres primeras tuberías se unen al nodo A y desde el nodo A, el agua fluye hasta el cuarto tanque.

**Nota:** Para suponer la dirección del flujo en cada tubería debe identificarse la altura de los tanques o las presiones en el inicio de cada tubería.

En este problema se reconocen 4 tuberías, en los cuales deben fluir cuatro (4) caudales. En el nodo A debe existir conservación de la masa (sumatoria de caudales) y una columna de presión, diferente a la presión atmosférica.

Posteriormente, se deben identificar las incógnitas. En este caso se identificaron cinco (5) incógnitas: Los cuatro caudales que fluyen por los cuatro tramos de tuberías y la presión en el nodo A. 

Finalmente, se deben crear tantas ecuaciones como incógnitas tenga la red. Para este caso particular se plantearán cinco ecuaciones, las cuales corresponde a:

1. Para el nodo A, se plantea la ecuación de conservación de la masa así:

2. Entre el tanque 1 y el nodo A se plantea la ecuación de conservación de energía considerando las pérdidas en el sistema 1-a.

3. Entre el tanque 2 y el nodo A se plantea la ecuación de conservación de energía considerando las pérdidas en el sistema 2-a. 

4. Entre el tanque 3 y el nodo A se plantea la ecuación de conservación de energía considerando las pérdidas en el sistema 3-a.

5. Entre el nodo A y el tanque 4 se plantea la ecuación de conservación de energía considerando las pérdidas en el sistema a-4.

El usuario debe solucionar este sistema de 5x5 tal como lo considere adecuado.


### Ejercicio de aplicación solucionado

Para aplicar los conceptos vistos en esta actividad por favor diríjase a la sección ["Taller de aplicación de las unidades anteriores"]((Taller_aplicacion_tres_unidades_anteriores.md)) y analice los ejercicios solucionados 1F y 1G.


## Redes cerradas. Conceptos

## Planteamiento y solución de sistemas hidráulicos de redes cerradas

### Ecuaciones y variables. Solución de una red cerrada

### Ejemplo conceptual. Solución de una red abierta


### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.11.08 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   6   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conceptos_bombas_hidraulicas.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](Taller_aplicacion_tres_unidades_anteriores.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|