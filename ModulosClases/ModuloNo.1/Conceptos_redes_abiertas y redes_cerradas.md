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

Por definición una red hidráulica abierta corresponda a aquella red conformada por tuberías dispuestas de tal manera que no crean una malla o circuito cerrado. En una red abierta las tuberías están configuradas de tal manera que pueden crear ramificación, sin crear ciclos o mallas continuas. Los extremos de los ramales pueden finalizar en un tanque o pueden descargar a la atmósfera.

En la siguiente imagen se presenta un ejemplo de una típica red abierta. En este caso tres tanques de nivel constante alimentan un tanque. Los tres tanques se conectan, en el nodo A, permitiendo que el caudal generado por los tres tanques llegue al cuarto.

<div align="center">

  <img src="Imagenes/FiguraNo.1.31.PNG" width="300px">

</div>

## Planteamiento y solución de sistemas hidráulicos de redes abiertas

En un sistema hidráulico compuesto por tuberías que funcionan con flujo a presión es necesario identificar los elementos que componen el sistema (tramos de tubería, nodos, accesorios, etc.) antes de plantera cualquier ecuación o cualquier sistema de ecuaciones.

En el caso particular de una red abierta es posible la estimación de las variables hidráulicas (caudales, presiones, velocidad y esfuerzos cortantes) utilizando las ecuaciones de conservación de la energía y conservación de la masa. A continuación se explica de manera general los conceptos y procedimientos que deben tenerse en cuenta para el planteamiento de las ecuaciones que rigen el comportamiento hidráulico de las redes abiertas. 

### Ecuaciones y variables. Solución de una red abierta

Como se ha visto en las demás actividades, las ecuaciones fundamentales para la solución de problemas relacionados con los flujos a presión corresponden a la conservación de la masa y a la conservación de la energía. 

Para un sistema abierto generalmente las incógnitas corresponden a los caudales que transitan por cada una de las tuberías y las columnas de presión en los nodos intermedios. Con base en esto, se recomienda como primer paso identificar las incógnitas que definen el problema, posteriormente plantear las ecuaciones y finalmente solucionar el sistema de ecuaciones planteadas.

En cada nodo es necesario plantear la ecuación de conservación de la masa, identificando el caudal o los caudales que ingresas al nodo y el caudal o los caudales que salen del nodo así:

<div align="center">

  <img src="ecuaciones/Ecuacion35.PNG" width="100px">

</div>


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

## Redes cerradas. Conceptos

Una red cerrada corresponde a aquella red cuyo elementos (tuberías y accesorios) generan o conforman un ciclo, circuito o malla. 

Este tipo de redes en su mayoría son usadas para la distribución del agua potable en las ciudades y en algunos casos para la distribución del agua de riego en distritos o cultivos de mediada y gran escala. Estas redes se caracterizan por presentar demandas intermedias en los nodos.

En la siguiente imagen se presenta un ejemplo de una típica red cerrada. En este caso dos tanques de nivel constante alimentan la red, la cual presenta algunos nodos con demandas y otros no. 

IMAGEN

## Planteamiento y solución de sistemas hidráulicos de redes cerradas

En un sistema hidráulico compuesto por tuberías que funcionan con flujo a presión es necesario identificar los elementos que componen el sistema (tramos de tubería, nodos, accesorios, etc.) antes de plantera cualquier ecuación o cualquier sistema de ecuaciones.

Para la solución de este tipo de redes es necesario el planteamiento de la ecuación de conservación de la masa (sumatoria de caudales) en cada nodo, considerando las demandas. Adicionalmente, deben estimarse las pérdidas de energía (fricción y por accesorios) entre los tramos que componen los circuitos o mallas.

Para la solución de los sistemas de ecuaciones que se generan en la solución de estas redes hidráulicas, convencionalmente se divide el problema en función del número de mallas (análisis individual de cada malla) y para cada malla se tienen en cuenta cada tramo de tubería que las conforma. Para el caso de mallas que tengan la misma tubería con una malla equidistante, se debe considerar el cálculo de esta tubería por aparte en cada malla y posteriormente por un proceso de ensayo y error, repartir la diferencia de los cálculos en cada malla hasta que converja el sistema.

### Ecuaciones y variables. Solución de una red cerrada

Como se mencionó, para la solución de estos problemas es necesario el planteamiento de la ecuación de conservación de la energía y las ecuaciones de las pérdidas de energía entre cada tramo de tuberías tanto localizadas como por fricción.

Con base en las actividades presentadas anteriormente en este módulo es posible plantear las pérdidas de energía totales en un tramo de la malla así:

**Nota:** Para este ejemplo conceptual se consideró que la ecuación que definen las pérdidas por fricción es la ecuación de Darcy-Weisbach. Es posible el uso de otras ecuaciones, tales como la de Haze-William o Manning, ecuaciones y conceptos fuera del alcance del presente curso. 

Para facilitar la presentación de esta ecuación es posible convertir las pérdidas de energía por accesorios en longitudes equivalentes o longitudes virtuales de tubería que, matemáticamente sean iguales a las pérdidas de fricción. Esto se logra igualando las ecuaciones así:

Por tanto, es posible plantear la ecuación de pérdidas de energía totales considerando una longitud total que corresponda a la suma de la longitud real del tramo de tubería más la longitud equivalente, lo cual permite presentar la ecuación de pérdidas totales así:

Considerando las constantes que se presentan en el problema, la ecuación puede ser transformada de manera general a:

Donde,

aij son las constantes agrupadas.

Como el lector reconocerá con la anterior ecuación, las incgnitas en cada tubería y por tanto en cada malla corresponde al caudal. Para la estimación del caudal deben cosniderarse los caudales demandas y el caudal residual o remanente que se genera en las tubrías una vez a logrado satifacer la demanda del nodo.

### Ejemplo conceptual. Método de solución de una red cerrada

En la literatura existen diferentes metodologías que permiten la estimación del caudal remanente que se distribuye por cada tubería en función de la demanda de cada nodo, del caudal inicia y de las características hidráulicas y geometrica de cada tubería. 

Entre los métodos más utilizados se destacan el método de Hardy Cross y el método de R.J. Cornish. Ambos métodos consideran una distribución inicial (que debe ser definida por lógica por el diseñador) y a partir de metodología iterativa estimar los caudales finales circulantes antes minimizando el error o diferencia de caudales entre iteraciones.

El método de Cross se basa en reducir la diferencia de caudales ($/Delta Q$) a tal punto que entre cada proceso de iteración el valor de ($/Delta Q$) sea cero. La ecuación que define el error del caudal que circula entre los tramos de tuberías en una red cerrada corresponde a:

En el caso del método de Cornish lo que se busca es minimizar la diferencia de las pérdidas ($/Delta H_t$). Al igual que con el método de Cross a partir de la suposición de datos iniciales y mediante un proceso de iteración o de tanteo debe minimizarse esta diferencia hasta encontrar la convergencia. La ecuación que define el error de las pérdidas de energía totales entre tramos de una red cerrada corresponde a:

### Ejercicio de aplicación solucionado

Para aplicar los conceptos vistos en esta actividad por favor diríjase a la sección ["Taller de aplicación de las unidades anteriores"]((Taller_aplicacion_tres_unidades_anteriores.md)) y analice los ejercicios solucionados 1F y 1G.

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.11.08 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   7   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conceptos_bombas_hidraulicas.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](Taller_aplicacion_tres_unidades_anteriores.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|