# Curso de Epanet - Módulo 1 - Conservación de la energía
<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>


Keywords: `Energía` `Bernoulli` `Línea de Corriente` `Conservación de la energía`

<br>

<br>

<div align="center">
    <b>PIQUE LA IMAGEN PARA VER EL VIDEO DE INTRODUCCIÓN </b>
    <a href="https://pruebacorreoescuelaingeduco-my.sharepoint.com/:v:/g/personal/andres_otalora_escuelaing_edu_co/ERjexa1U1iZNpHhm_8vCb5MBXP0wCzpyHXzs59Nu2On_ag?e=rBHC3F">
        <img src="Imagenes/INTRODUCCION_MOD1_ACT3.PNG" width="800px">
    </a>
</div>



## Introducción

En este módulo se presentan de manera general los conceptos básicos y las ecuaciones que definen la conservación de la energía en sistemas hidráulicos a presión. Se definirá de manera general los conceptos básicos de la energía cinética, energía potencial y energía de presión. Se describirá de manera general las pérdidas de energía en un sistema a presión y se conceptualizará el uso de la ecuación de Bernoulli para la solución de problemas aplicados. 

## Objetivos

El objetivo principal de esta actividad es introducir al estudiante en los conceptos relacionados con la conservación de la energía y su aplicación en la cinemática de los fluidos utilizando la ecuación de Bernoulli. Se espera que el estudiante tenga la capacidad de comprender las definiciones y pueda aplicarlas en la solución de problemas relacionados con los flujos a presión. Estos conceptos le permitirán al estudiante comprender la forma que el software EPANET y otros software, determinan las diferentes variables hidráulicas en los sistemas planteados.

<br>

<br>

<div align="center">
    <b>PIQUE LA IMAGEN PARA VER EL VIDEO DE LA ACTIVIDAD </b>
    <a href="https://pruebacorreoescuelaingeduco-my.sharepoint.com/:v:/g/personal/andres_otalora_escuelaing_edu_co/ETIIN4sIB2tErf4Nd_qajhwBboVcME000xEF7a6xzUWLSA?e=qKhu6v">
        <img src="Imagenes/CLASE_MOD1_ACT3.PNG" width="800px">
    </a>
</div>

### Conservación de la energía total. Ecuación de Bernoulli

- <b>Conservación de la energía: </b> En un volumen de control, la energía total en un sistema es igual a la diferencia entre el calor interno y el cambio del trabajo. La primera ley de la termodinámica indica que el trabajo y el calor transferido o intercambiado en un sistema, no se crea ni se destruye, solo se transforma. 

En la siguiente expresión se presenta la ecuación que define de manera simplificada la primera ley de la termodinámica.

<div align="center">
  <img src="ecuaciones/Ecuacion9.PNG" width="200px">
</div>

Donde,

<br>Q= Calor [J]</b>
<br>W= Trabajo [J]</b>
<br>E= Energía total en el sistema [J]</b>

En la siguiente figura se aprecia de manera simplificada este concepto.

<div align="center">
  <img src="Imagenes/FiguraNo.1.10.PNG" width="300px">
</div>

- <b> Ecuación de Bernoulli: </b> Daniel Bernoulli en 1738 en su obra "Hidrodinámica" determinó, a partir de un análisis diferencial en un volumen de control, una ecuación que permite determinar la transformación de la energía en un fluido en movimiento equivalente a la ecuación que define el cambio de la energía en un sistema termodinámico. 

Esta ecuación, coloquialmente denominada "Ecuación de Bernoulli", es la base de la hidráulica moderna y el pilar de los software de modelación de sistemas a presión. Esta ecuación utilizada en todo el mundo permite la estimación de las diferentes variables hidráulicas que definen un sistema de un fluido en movimiento.

Esta ecuación permite estimar, en unidades de metros columna de agua (m.c.a) la energía en un punto en un sistema hidráulico a presión. Es posible aplicar esta ecuación para dos puntos distintos del sistema, a lo largo de una misma línea de corriente. 

Definiendo el punto 1, como el punto de inicio del volumen de control y el punto 2 como el punto al final del volumen de control, es posible escribir la ecuación de bernoulli, sin considerar pérdidas de energía así:

<div align="center">
  <img src="ecuaciones/Ecuacion14.PNG" width="350px">
</div>

Donde, 

 
<br> $\frac{V^{2}}{2g}$: corresponde a la columna de energía cinética.
<br> $\frac{P}{\gamma}$: corresponde a la columna de energía de presión.
<br> $Z$: corresponde a la columna de energía de posición o potencial.

Tal como en cualquier sistema físico, en los sistemas hidráulicos existen pérdidas de energía. En el caso particular de sistemas con flujo a presión, se pueden identificar dos tipos de pérdidas de energía: Las pérdidas de energía generadas por accesorios y las pérdidas de energía por la fricción o el rozamiento del fluido en las paredes de la tubería.

Con estas consideraciones, la ecuación de Bernoulli se puede escribir como:

<div align="center">
  <img src="ecuaciones/Ecuacion15.PNG" width="350px">
</div>

Donde,

 
<br> $\sum_{}^{}\Delta h_f $: Pérdidas de energía debido a la fricción.
<br> $\sum_{}^{}\Delta h_k$: Pérdidas de energía debido a los accesorios.

Nota: El detalle de las pérdidas de energía por accesorios y por fricción se describe en la actividad "Pérdidas de energía. Pérdidas localizadas y pérdidas por fricción"
 
- Máquinas hidráulicas. Bombas Hidráulicas

Tal como se describirá con más detalle en el apartado "Bombas hidráulicas" una bomba hidráulica corresponde a una máquina hidráulica que proporciona energía al sistema a partir de una diferencia de presión y un aumento de la velocidad. 

En general la energía como columna de agua es función de la potencia hidráulica de la bomba (potencia mecánica por la eficiencia de la bomba), el caudal y el peso específico del fluido. A continuación se presenta la potencial de una bomba como metros columna de agua (m.c.a.)

<div align="center">
  <img src="ecuaciones/Ecuacion16.PNG" width="250px">
</div>


Nota: El detalle de los sistemas de bombeo y de la ecuación que define la energía generada por la potencia de una bomba en m.c.a se presenta en la actividad "Conceptos de bombas hidráulicas"

### - Línea de energía 

La línea de energía corresponde a la línea que une la energía total en un sistema. Para un sistema hidráulico a presión, la línea de energía une suma de la columna de velocidad, la columna de posición y la columna de presión.

### - Linea piezométrica

La línea piezométrica corresponde a la línea que une la suma de la columna de posición y la columna de presión. Es posible la visualización de esta línea en un sistema a presión si se instalan tubos piezométricos (piezómetros) a lo largo de la tubería. La altura a la cual se eleva el fluido por el tubo corresponderá a la altura piezométrica. La unión de estos puntos corresponde a la línea piezométrica.

En la siguiente figura se presenta un esquema general de la línea de energía y la línea piezométrica en un sistema a presión en el cual se han considerado las pérdidas de energía debido a la fricción y debido a los accesorios.

<div align="center">
  <img src="Imagenes/FiguraNo.1.11.PNG" width="400px">
</div>

### Ejercicio de aplicación solucionado

Para aplicar los conceptos vistos en esta actividad por favor diríjase a la sección ["Taller de aplicación de las unidades anteriores"]((Taller_aplicacion_tres_unidades_anteriores.md)) y analice el ejercicio solucionado 1C.

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.08.30 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   5   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conservacion_masa.Caudal_flujos_presion.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](Perdidas_energia.%20Perdida_localizadas_perdidas_friccion.md) |
|-------------------------------------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------|
