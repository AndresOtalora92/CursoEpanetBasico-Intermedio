# Curso de Epanet - Módulo 3 - Inclusión de demanda variable en los nodos(análisis de periodo extendido)

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

Keywords: `Demanda` `Consumo` `Caudal` `Nodos`

## Introducción

En esta actividad se presentan los conceptos generales de una demanda variable en un nodo en una red y se presenta la metodología sugerida para su incorporación en una red previamente construida y modelada en EPANET. Se presentan un ejemplo utilizando el archivo previamente creado en las diferentes actividades que componen el módulo 2.

## Objetivos

El objetivo principal de esta actividad es darle a conocer al usuario las herramientas que tiene el software EPANET para permitir agregar una demanda variable en los nodos de un sistema de tuberías.
 
## Caudales variables o demanda variable. Conceptos
Como se mencionó a lo largo del curso, especialmente en el módulo 2, en un nodo es posible definir el consumo o demanda de caudal o en pocas palabras el caudal extraído de la red en un punto.

En caso teórico es posible definir de manera simplificada el consumo como un valor permanente o constante en el tiempo. En la ingeniería aplicada los consumo en las redes de drenaje presentan diferentes patrones de demanda, los cuales pueden ser representados como un porcentaje o factor menor o mayor a la unidad del caudal medio de consumo. 

## Ejemplo de aplicación.

Utilizando la red hidráulica construida y presentada en las diferentes actividades del módulo 2, se definirá un patron de demanda (o como lo llama EPANET, un análisis de tiempo extendido) utilizando como demanda media los caudales de demanda definidos en los nodos 3 y 6 de la red mencionada. Los patrones de demanda se presentan a continuación en forma de histogramas:

<div align="center">
  <img src="Imagenes/FiguraNo.2.85.PNG" width="500px">
</div>

<div align="center">
  <img src="Imagenes/FiguraNo.2.86.PNG" width="500px">
</div>

## Asignación y uso de la demanda variable o Análisis extendido en el tiempo

Con el concepto de caudal o demanda variable definido ya es posible definir esta característica en la red que se elaboró en el módulo 2. A continuación se presentan los pasos recomendados para realizar el análisis extendido en el tiempo:

_a._

<div align="center">
  <img src="Imagenes/FiguraNo.2.85a.PNG" width="700px">
</div>

_b._

<div align="center">
  <img src="Imagenes/FiguraNo.2.86a.PNG" width="700px">
</div>

_c._

<div align="center">
  <img src="Imagenes/FiguraNo.2.87.PNG" width="700px">
</div>

_d._

<div align="center">
  <img src="Imagenes/FiguraNo.2.88.PNG" width="700px">
</div>

_e._

<div align="center">
  <img src="Imagenes/FiguraNo.2.89.PNG" width="700px">
</div>

_f._

<div align="center">
  <img src="Imagenes/FiguraNo.2.90.PNG" width="700px">
</div>

_g._

<div align="center">
  <img src="Imagenes/FiguraNo.2.91.PNG" width="700px">
</div>

_h._

<div align="center">
  <img src="Imagenes/FiguraNo.2.92.PNG" width="700px">
</div>


_i._

<div align="center">
  <img src="Imagenes/FiguraNo.2.93.PNG" width="700px">
</div>

_j._

<div align="center">
  <img src="Imagenes/FiguraNo.2.94.PNG" width="700px">
</div>

_k._

<div align="center">
  <img src="Imagenes/FiguraNo.2.95.PNG" width="150px">
</div>

_l._

<div align="center">
  <img src="Imagenes/FiguraNo.2.96.PNG" width="700px">
</div>

_m._

<div align="center">
  <img src="Imagenes/FiguraNo.2.97.PNG" width="700px">
</div>

_n._

<div align="center">
  <img src="Imagenes/FiguraNo.2.98.PNG" width="700px">
</div>

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.06.12 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   3   |


_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._


| [Anterior](../ModuloNo.2/AnalisisResultados.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente] |
|--------------------------------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|---------------|
