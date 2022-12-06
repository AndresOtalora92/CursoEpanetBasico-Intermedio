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

## Ejemplo aplicado

Utilizando la red hidráulica construida y presentada en las diferentes actividades del módulo 2, se definirá un patron de demanda (o como lo llama EPANET, un análisis de tiempo extendido) utilizando como demanda media los caudales de demanda definidos en los nodos 3 y 6 de la red mencionada. Los patrones de demanda se presentan a continuación en forma de histogramas:

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.05.12 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   1   |


_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._


| [Anterior](../ModuloNo.2/AnalisisResultados.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente] |
|--------------------------------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|---------------|
