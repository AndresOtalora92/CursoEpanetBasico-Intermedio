# Curso de Epanet - Módulo 1 - Taller de aplicación de las actividades anteriores. 

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br><i>Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co </i>
</div>


Keywords: `Hidráulica a Presión` `Conceptos de hidráulica a presión` `Taller de práctica`

## Problema 1A - Conceptos generales de los flujos a presión.

Una tubería circular de 10 cm de radio con flujo a presión transporta agua a 20°C. Si la tubería tiene una longitud total de 100 m y la diferencia de presión entre el punto inicial y el punto final de la tubería es de 10 kPa, determine:

**a)** La velocidad máxima a la que debe fluir el agua para que el flujo sea laminar.

**b)** El caudal máximo a la que debe fluir el agua para que el flujo sea laminar.

**c)** El gradiente hidráulico.

**d)** El esfuerzo cortante total que el flujo le genera a la tubería.

### Solución Problema 1A

#### a) Para la determinación de los demás numerales es necesario conocer la densidad y la viscosidad del agua a 20°C. Revisando las tablas se tiene que:

<div align="center">
  $\rho=998.0 \frac{Kg}{m^3}$
</div>

<div align="center">
  $\mu=1.003*10^{-3}\frac{kg}{m*s}$
</div>

Con estos valores y sabiendo que se requiere que el Número de Reynolds (Re) a lo sumo sea 2000 (para condición máximo de flujo laminar), es posible despejar la velocidad media del flujo así:

<div align="center">
  $Re=\frac{\rho*V*D}{\mu}$
</div>

<div align="center">
  $2000=\frac{998*V*(2*0.10)}{1.003*10^{-3}}$
</div>

<div align="center">
  <b> V =0.10 m/s </b> 
</div>



#### b) A partir de la velocidad media y utilizando el concepto de caudal se tiene que:

<div align="center">
  $Q = V*(\frac{\pi}{4}*D^2)$
</div>

<div align="center">
  <b> Q = 0.00031 m³/s </b> 
</div>

#### c) Conocida la longitud y la diferencia de presión entre los puntos extremos se tiene que:

<div align="center">
  $Gradiente =\frac{\Delta P}{L}$
</div>

<div align="center">
  <b> Gradiente = 100 Pa/m </b>
</div>


#### d) A partir del gradiente hidráulico y asumiendo que es igual a la pendiente de la línea de energía (Sf) es posible estimar el esfuerzo cortante así:

<div align="center">
  $\tau=\gamma*R*S_f$
</div>

<div align="center">
  $\tau=\rho*g*R*S_f$
</div>

<div align="center">
  $\tau=\rho*g*A/P*S_f$
</div>

<div align="center">
  $\tau=998*9.81*0.0314/0.628*100=48951.9 Pa$
</div>

<div align="center">
  $\tau=48951.9 Pa$
</div>

Este ejercicio también se encuentra resuelto en código de Wolfram Mathematica, código que puede ser descargado en el [link de descarga](Soluciones/Solucion1A.nb) o directamente el archivo en el siguiente [link de descarga](https://pruebacorreoescuelaingeduco-my.sharepoint.com/:u:/g/personal/andres_otalora_escuelaing_edu_co/EaT58Xbtpd9Og6eR72h8eBMBTGkl9Qn3bXSop4VVugQi5w?e=LkGyPO)

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.11.09 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   1   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conceptos_redes_abiertas%20y%20redes_cerradas.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | 
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|