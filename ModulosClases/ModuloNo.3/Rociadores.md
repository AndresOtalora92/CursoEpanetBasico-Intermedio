# Curso de Epanet - Módulo 3 - Inclusión de rociadores

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

Keywords: `Rociadores` `Válvulas` `Coeficiente de Caudal` `Nodos`

## Introducción

En esta actividad se presenta de manera general el concepto general de un rociador, las ecuaciones que rigen su comportamiento y el procedimiento sugerido para ingresarse un rociador en una red hidráulica a presión utilizando las herramientas de EPANET en los nodos o uniones.

## Objetivos

El objetivo principal de esta actividad es darle a conocer al usuario las metodologías sugeridas por EPANET para tener en cuenta el comportamiento hidráulico de un rociador en una red hidráulica a presión. Como se verá más adelante los rociadores descarga un caudal en función de la variación de la presión en su salida.


## Rociadores
Un rociador corresponde a un accesorio tipo válvula con una boquilla que permite dispersar el fluido (agua-espuma) de manera controlada en un radio de influencia definido por la presión y el caudal. Generalmente, este tipo de accesorios son utilizados en las redes contra-incendios en las edificaciones, oficinas, bodegas entre otros. 

A manera de contexto a continuación se presenta algunas imágenes de los diferentes disposiciones y diseños de geometrías:

<div align="center">
  <img src="Imagenes/FiguraNo.2.107.PNG" width="400px">
</div>

<div align="center">
  <img src="Imagenes/FiguraNo.2.108.PNG" width="400px">
</div>

Epanet define los rociadores a partir de la implementación de una ecuación genérica la cual depende de la relación del caudal con la presión. La ecuación se presentan a continuación:

<div align="center">
  <img src="ecuaciones/Ecuacion97.PNG" width="300px">
</div>

El exponente, para la mayoría de los rociadores (depende del diseño y el proveedor) corresponde a 0.5. El coeficiente C, también llamado el coeficiente de gasto, corresponde a la relación del caudal descargado por el rociador sobre la presión del rociador. En pocas palabras, el caudal descargado está condicionado a la presión ejercida sobre el nodo donde se instala el rociador. 

## Ejemplo de aplicación.

Utilizando la red hidráulica construida y presentada en las actividades anteriores de este módulo (módulo 3) se asumirá que existe un rociador en el nodo 6 con un exponente de 0.5 y un coeficiente de caudal o de gasto de 0.70 LPS/m.c.a



### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.07.12 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   1   |


_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._


| [Anterior](../ModuloNo.2/AnalisisResultados.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](../ModuloNo.3/ComparacionMetodos.md) |
|--------------------------------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|---------------|
