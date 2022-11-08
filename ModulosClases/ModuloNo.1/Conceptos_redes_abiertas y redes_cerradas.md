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

Como se ha visto en las demás actividades, las ecuaciones fundamentales para la solución de problemas relacionados con los flujos a presión corresponde a la conservación de la masa y la conservación de la energía. 

Para un sistema abierto generalmente la incognita corresponde al caudal que transita por cada tubería y la columna de presión en los nodos intermedios. Con base en estos, como primer paso se recomienda identificar las incógnitas que definen el problema y posteriormente plantear las ecuaciones.

En cada nodo es necesario plantear la conservación de la masa, identificando el caudal o los caudales que ingresas al nodo y el caudal o los caudales que salen del nodo así:

Posteriormente, debe plantearse la ecuación de conservación de energía o Bernoulli entre dos puntos tantas veces como caudales deban determinarse. Los puntos de inicio y fin en el planteamiento de la ecuación de energía generalmente se seleccionan desde el inicio de uno de los ramales hasta un nodo o desde un nodo particular hasta el final de un ramal. Esta identificación dependerá del problema. 

El usuario debe generar tantas ecuaciones como incógnitas tenga la red y solucionar el sistema de ecuaciones como mejor le convengan. En resumidas cuentas eso es lo que hace el código de EPANET, plantear sistemas de ecuaciones que permitan su solución con métodos numéricos. 

### Ejemplo conceptual. Solución de una red abierta

Con el propósito de reforzar el concepto definido anteriormente se plantearán las ecuaciones necesarias para la determinación de los caudales (Qi) de las presiones(Pi) en la red abierta presentada anteriormente y que a continuación se amplía.




### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.11.08 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   6   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conceptos_bombas_hidraulicas.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](Taller_aplicacion_tres_unidades_anteriores.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|