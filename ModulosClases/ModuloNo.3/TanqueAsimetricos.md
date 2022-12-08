# Curso de Epanet - Módulo 3 - Tanque de alimentación asimétricos

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>

Keywords: `Tanques` `Asimétricos` `Alimentación`

## Introducción

En esta actividad se presenta la metodología y los conceptos para trabajar con un tanque asimétrico trabajando a partir de su curva de almacenamiento o curva de capacidad.

## Objetivos

El objetivo principal de esta actividad es darle a conocer el usuario las posibilidades que tiene para incorporar tanques simétricos o asimétricos a partir del ingres de su curva de almacenamiento o capacidad. 

## Tanque asimétricos y curva de capacidad

Como su nombre lo indica, un tanque asimétrico corresponde a aquel tanque cuya geometría no es regular y por tanto, el volumen de almacenado (cuando el tanque es alimentado)  o volumen de descarga (cuando el tanque es alimentado) cambia en función del nivel del agua en dicho tanque. Los tanques irregulares son generalmente usados en viviendas, edicificaciones de poca altura, hospitales, zonas de extracción de minerales, zonas con reservorios temporales, entre otros.

A continuación se presentan algunos ejemplos de tanque asimétricos.

<div align="center">
  <img src="Imagenes/FiguraNo.2.121.PNG" width="500px">
</div>

<div align="center">
  <img src="Imagenes/FiguraNo.2.122.PNG" width="400px">
</div>



Una curva de capacidad o curva de almacenamiento corresponde al gráfico y/o función que representa el volumen acumulado para cada nivel de agua que se mida en el tanque.  

A continuación se presentan un ejemplo de una curva de capacidad o de almacenamiento.

<div align="center">
  <img src="Imagenes/FiguraNo.2.123.PNG" width="400px">
</div>

## Ejemplo de aplicación.

Utilizando la red hidráulica construida y presentada en las actividades anteriores de este módulo (módulo 3) se desarollará esta actividad. Se adicionará a la red un nuevo tramo que descargará al nodo 2 y que inicia en un tanque o reservorio asimétrico con la siguiente curva de almacenamiento o curva de capacidad:


<div align="center">
  <img src="Imagenes/FiguraNo.2.125.PNG" width="700px">
</div>

<br>

<div align="center">
  <img src="Imagenes/FiguraNo.2.124.PNG" width="380px">
</div>

Se asumirá que el nivel inicial del tanque en la modelación es de 240.8 m.s.n.m (siendo este también el nivel máximo) y con un nivel mínimo e 239.4 m.s.n.m

## Tanque asimétrico con curva de almacenamiento en EPANET

_a._

<div align="center">
  <img src="Imagenes/FiguraNo.2.126.PNG" width="700px">
</div>

_b._

<div align="center">
  <img src="Imagenes/FiguraNo.2.127.PNG" width="700px">
</div>

_c._

<div align="center">
  <img src="Imagenes/FiguraNo.2.128.PNG" width="700px">
</div>

_d._

<div align="center">
  <img src="Imagenes/FiguraNo.2.129.PNG" width="700px">
</div>

_e._

<div align="center">
  <img src="Imagenes/FiguraNo.2.130.PNG" width="700px">
</div>

_f._

<div align="center">
  <img src="Imagenes/FiguraNo.2.131.PNG" width="700px">
</div>

_g._

<div align="center">
  <img src="Imagenes/FiguraNo.2.132.PNG" width="700px">
</div>

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.08.12 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   2   |


_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._


| [Anterior](../ModuloNo.3/CurvasRendimiento.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente] |
|-------------------------------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------|
