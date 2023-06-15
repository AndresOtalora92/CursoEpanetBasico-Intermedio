<div align="center"><a href="https://enlace-academico.escuelaing.edu.co/psc/FORMULARIO/EMPLOYEE/SA/c/LC_SA_MN.LC_FRM_ADM_EC_CMP.GBL" target="_blank"><img src="https://github.com/rcfdtools/R.TeachingResearchGuide/blob/main/CaseUse/.icons/IconCEHBannerCertificado.jpg" alt="R.LTWB" width="100%" border="0" /></a></div>

# Curso de Epanet - Módulo 1 - Conservación de la masa. Caudal en flujos a presión. 

<div align="center">
  <img src="../../.icons/IconoEpanetV3.png" width="600px">
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br></div>

<div align="center">
Andrés Humberto Otálora Carmona
<br></div>

<div align="center">
Profesor del Centro de Estudios Hidráulicos
<br></div>

<div align="center">
andres.otalora@escuelaing.edu.co
<br></div>




<br>

<br>

<div align="center">
       <a href="https://youtu.be/JAfoS4p42Ro">
        <img src="../../.icons/INICIO_OBJETIVOS.PNG" width="800px">
    </a>
</div>

Keywords: `Energía` `Bernoulli` `Flujo` `Flujo másico` `masa`

## Introducción

En este módulo se presenta de manera general los conceptos básicos y las ecuaciones que definen la conservación de la masa en un sistema hidráulico a presión. También se definirán las ecuaciones empíricas más utilizadas para la determinación del caudal en una tubería circular con flujo a presión a partir de las propiedades hidráulicas del sistema, las características del fluido y a parti del gradiente de energía.

## Objetivos

El objetivo principal de esta actividad es introducir al estudiante en los conceptos relacionados con la conservación de la masa y el repaso de algunas ecuaciones para la estimación de los caudales en un sistema a presión. 

<br>

<br>

<div align="center">
       <a href="https://youtu.be/GhabhrhwI7U">
        <img src="../../.icons/INICIO_ACTIVIDAD.PNG" width="800px">
    </a>
</div>


## Conservación de la masa. Definiciones

La ley de conservación de la masa o ley de continuidad versa que en un sistema cerrado, la diferencia entre todas las entradas y todas las salidas son iguales al cambio del volumen con respecto al tiempo.

En la siguiente expresión se presenta la ecuación de continuidad para un flujo laminar e incompresible.

<div align="center">
  <img src="ecuaciones/Ecuacion7.PNG" width="300px">
</div>

Para sistemas hidráulicos donde no existe acumulación temporal del fluido y también cuando el flujo está en condiciones permanentes, la ecuación de continuidad se puede presentar así:

<div align="center">
  <img src="ecuaciones/Ecuacion8.PNG" width="300px">
</div>

Esta es una de las ecuaciones que el software EPANET resuelve en cada uno de los nodos que componen una red. Para el uso de los signos de estas ecuaciones, se utiliza un sistema nemotécnico en el cual se asume que los caudales que ingresan al volumen de control son negativos y los caudales que salen del volumen de control son negativos. 

En la siguiente figura se muestra una representación del volumen de control de una tubería que trabaja con flujo a presión. En esta figura se detallan las fronteras en las cuales se definen los caudales de entrada y los caudales de salida.

<div align="center">
  <img src="Imagenes/FiguraNo.1.9.PNG" width="300px">
</div>

En algunos casos particulares, cuando la densidad del fluido que ingresa a un volumen de control es diferente a la densidad del fluido que sale, la ecuación de continuidad debe expresarse en función del flujo másico. 

El flujo másico corresponde a la cantidad de masa que atraviesa una sección transversal. 

El flujo másico se puede expresar como:

<div align="center">
  <img src="ecuaciones/Ecuacion10.PNG" width="150px">
</div>

Con base en lo anterior, la ecuación de continuidad para un sistema permanente y sin acumulación corresponde a:

<div align="center">
  <img src="ecuaciones/Ecuacion11.PNG" width="300px">
</div>

Esta última ecuación es utilizada por EPANET para la aplicación de su módulo de "simulación de calidad del agua".

## Ecuaciones experimentales para la estimación de los caudales en tuberías a presión 

Existen diferentes ecuaciones empíricas para la estimación del caudal en una tubería a presión. Estas ecuaciones en general depende de las propiedades del fluido transportado y del gradiente hidráulico. 

A continuación se presentan dos de las ecuaciones más utilizadas para la estimación del caudal en un sistema a presión.

###  Ecuación de Hagen-Poiseuille

Para la estimación de un flujo laminar incompresible en una tubería a presión de sección circular y en condiciones de régimen permanente para flujos con números de Reynolds menores a 2000, es posible utilizar la ecuación Hagen - Poiseuille.

<div align="center">
  <img src="ecuaciones/Ecuacion12.PNG" width="250px">
</div>


Donde,
<br> Q= Caudal de la tubería (m³/s)
<br> g = aceleración de la gravedad (m/s²)
<br> D = Diámetro (m)
<br> $\Delta(P/\gamma)$: Pendiente de la línea piezométrica (m/m)
<br> $\vartheta$: Viscosidad cinemática del fluido (m²/s)


###  Ecuación de Hazen - William 

Otra ecuación muy utilizada para la estimación del caudal en tuberías con flujos a presión es la ecuación de Hazen - William. Esta ecuación es ampliamente aplicada para el diseño de redes de acueductos.,

La ecuación en unidades del sistema internacional se expresa de la siguiente manera.:

<div align="center">
  <img src="ecuaciones/Ecuacion13.PNG" width="350px">
</div>


Donde,

<br> Q= Caudal de la tubería (m³/s)
<br> A= Área Hidráulica (m²)
<br> R = Radio Hidráulico (m). Para tuberías circular D/4
<br> D = Diámetro (m)
<br> C = Coeficiente de rugosidad de Hazen - William
<br> Sf = Pendiente de la línea de energía (m/m)

Para nuestro curso, estas ecuaciones pueden ser utilizadas para comparar y analizar los resultados en tramos de tuberías una vez se ejecute el programa. También pueden ser aplicadas en el proceso de pre-dimensionamiento de las tuberías (definición de un primer diámetro) que componen el sistema antes de cargar la geometría definitiva al programa. 

### Ejercicio de aplicación solucionado

Para aplicar los conceptos vistos en esta actividad por favor diríjase a la sección ["Taller de aplicación de las unidades anteriores"]((Taller_aplicacion_tres_unidades_anteriores.md)) y analice el ejercicio solucionado 1B.

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2022.08.30 | Versión No. 1 | [AndresOtalora92](https://github.com/AndresOtalora92)  |   5   |

_CursoEpanetBasico-Intermedio es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [AndresOtalora92](https://github.com/AndresOtalora92?tab=repositories) en GitHub._

| [Anterior](Conceptos_generales_flujo_a_presion.md) | [:house: Inicio](../../README.md) | [:beginner: Ayuda / Colabora] | [Siguiente](Conservacion_de_energia.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|

<div align="center"><a href="https://enlace-academico.escuelaing.edu.co/psc/FORMULARIO/EMPLOYEE/SA/c/LC_SA_MN.LC_FRM_ADM_EC_CMP.GBL" target="_blank"><img src="https://github.com/rcfdtools/R.TeachingResearchGuide/blob/main/CaseUse/.icons/IconCEHBotonCertificado.png" alt="R.LTWB" width="260" border="0" /></a></div>

##


<div align="center"><a href="http://www.escuelaing.edu.co" target="_blank"><img src="../../.icons/Banner1.svg" alt="Support by" width="100%" border="0" /></a><sub><br>Este curso guía ha sido desarrollado con el apoyo de la Escuela Colombiana de Ingeniería - Julio Garavito. Encuentra más contenidos en https://github.com/uescuelaing</sub><br><br></div>