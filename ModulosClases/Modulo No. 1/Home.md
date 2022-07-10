# Bienvenido al curso de Epanet. Uso y aplicaciones. 
![Imagen 1](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/b30a070763c8fdd0debdf2836196f1bbc795673b/.jpg/IconoEpanetV3.png)

*Universidad Escuela Colombiana de Ingeniería Julio Garavito*

***Andrés Humberto Otálora Carmona, andres.otalora@escuelaing.edu.co***
# Introducción. 
EPANET es un software de modelación hidráulica de sistemas a presión. Corresponde a un programa de dominio
púlico, desarrollado por la Agencia de Protección Ambiental de Estados Unidos y difundido ampliamente en 
el mundo para el desarrollo de actividades de consultoría, investigación aplicada, investigación teórica y
como software de gestión para todo tipo de programas de tuberías presurizadas.Si bien fue diseñado para 
el análisis de sistemas con agua potable, también puede ser utilizado para el análisis de cualquier 
fluido no compresible con flujo a presión. 

La primera versión de EPANET fue lanzada en 1993 y posteriormente se lanzó EPANET 2, versión que dispone
de código libre en lenguaje C. 

El software permite realizar análisis hidráulicos en sistemas de tuberías presurizadas a partir de las 
características físicas de las tuberías (longitud, material, coeficiente de rugosidad, diámetro) y la 
dinámica de los nodos, los cuales puede incluir demandas de caudales (demanda constante o demanda variable).

El software permite integrar, además de las redes de tuberías y nodos, tanques de alimentación, sistemas
de bombeos y accesorios tipo válvulas a partir de la inclusión de coeficentes de pérdidas localizadas. 

Con el desarrollo de las herramientas computacionales, diseñadores y programadores de todo el mundo han
elaborado distintas aplicaciones compatibles con el software original, permitiendo una interacción entre
otros programas tales como: AutoCAD, QGis, ArcGis, SWMM, Python, R, entre otros. Esta interacción de 
software ha permitido aumentar el volumen de procesamiento, acortando los procesos de construccion de la
geometría, la inclusión de información y los análisis simultaneos para distintos escenarios. 

La versión original del programa fue desarrollada en inglés por la EPA y ha sido traducida al español por 
varias instituciones. En España y Latinoamérica una de las de mayor difusión es la desarrollada por la 
Universidad Politécnica de Valencia.

# Objetivo principal del curso. 
El objetivo general de este curso corresponde al estudio y aplicación del software de simulación hidráulica
EPANET, en su versión 2.2 en español. El curso se desarrolla a partir de la solición de diferentes ejercicios
aplicados tomando como punto de partida los fundamentos básicos de la hidráulica a presión, los conceptos de
conservación de la energía que incluyen los conceptos de pérdidas localizadas y por fricción y los fundamentos
de las redes abiertas y redes cerradas en un sistema presurizado.

# Objetivos secundarios del curso. 
**1.** Conceptualización de los fundamentos de la hidráulica a presión.

**2.** Análisis de las herramientas básicas del software de EPANET.

**3.** Aplicación del software de EPANET en problemas aplicados para la solución de probloemas en sistemas
       de flujo a presión.

**4.** Análisis de de las herramientas avanzadas del software de EPANET.

**5.** Análisis de los resultados para la toma de decisiones utilizando EPANET.

**6.** Conceptualización y aplicación de algunas herramientas complementarias para la programación de EPANET. 


# Contenido Programático

Con base en el alcance del curso y los objetivos de aprendizaje definidos en el apartado anterior se ha 
dividio el curso en tres módulo. El contenido de estos módulos permite que el estudiante aprenda de manera
gradual y escalonada el uso y aplicación de las herramientas del software. El estudiante no solo podrá
aplicar el sofwtare, sino también estará en la capacidad de analizar el orden de magnitud de los resultantes
y podrá tomar decisiones en futuros diseños o planes de gestión. 

A continuación se presentan el contenido programático, con una pequeña descripción de su temática y de las
actividades que el estudiante deberá realizar para completarlas. 

## Módulo No. 1 - Conceptos básicos de hidráulica a presión

#### **1.1 Conceptos generales de flujo a presión**
Descripción de los conceptos generales de los flujos a presión. Definiciones conceptuales de los fundamentos
de la hidráulica, descripción y detalle de las ecuaciones básicas que rigen los sistemas presurizados. 

#### **1.2 Conservación de la energía**
Análisis y aplicación de la ecuación de conservación de energía y de la ecuación de Bernoulli para sistemas
con flujos a presión. Descripción de las partes que componen las ecuaciones.

#### **1.3 Pérdidas de energía. Pérdidas localizadas y pérdidas por fricción**
Descripción de las pérdidas de energía localizadas utilizando la ecuación de Darcy - Weisbach. Revisión de
los coeficientes de rugosidad de las tuberías. Análisis de las ecuación de pérdidas localizadas. Revisión
de coeficientes de pérdidas localizadas.
Ejercicios de aplicación resueltos.

### **Taller de aplicación de las unidades 1.1, 1.2 Y 1.3** 

#### **1.4 Conceptos de bombas hidráulicas**
Descripción de los tipos de bombas hidráulicas. Bombas en serie y en paralelo.
Curvas de eficiencia de las bombas. Concepto de NPSH de las bombas. Revisión de sumergencia.

#### **1.5 Conceptos de redes abiertas**
Conceptos y aplicaciones de sistemas de tuberías denominados abiertos. Ejericios de aplicación resueltos.

#### **1.6 Conceptos de redes cerradas**
Conceptos y aplicaciones de sistemas de tuberías denominados cerrados. Ejericios de aplicación resueltos.

### **Taller de aplicación de las unidades 1.4, 1.5 Y 1.6** 


## Módulo No. 2 - Uso y aplicación básica de EPANET. Ventanas y herramientas

#### **2.1 Generalidades de Epanet**
Módulo en el que se conocerá las funcionalidades y aplicaciones del software EPANET. Se describirán las partes,
ventanas y herramientas que conforman el software.

#### **2.2 Trazado de la red. Esquelo del modelo hidráulico**
Se aprenderá a realizar el trazado de una red hidráulica a presión a partir del desarrollo de un ejercicio 
aplicado. Se revisaran varias metodologías para realizar el trazado de una red utilizando las herramientas
propias de Epanet y utilizando herramientas de otros software.

#### **2.3 Alimentación del modelo Epanet. Elementos de la red**
Un vez se tenga el esqueleto de la red se dispondrá aprender como ingresar los diferentes características 
de elementos que componen la red tales como sus diámetros, longitdunes, nodos y materiales. En este módulo se 
enseñarán las herramientas que permiten adicionar, editar y eliminar accesorios, nodos, tanques y bombas. 

### **Taller de aplicación de las unidades 2.1, 2.2 Y 2.3** 

#### **2.4 Resultados. Análisis y revisión.**
Con la red construida, los accesorios definidos y las características de la red ingresos al modelo se 
procede a realizar las simulaciones y con ello extraer y analizar los resultados. Se explicarán las diferentes
herramientas de análisis de resultados de las simulaciones. También se realizarán análisis
utilizando herramientas de Office a partir de los datos extraidos del Epanet y utilizando 
los conceptos de hidráulica a presión.


## Módulo No. 3 - Uso y aplicación intermedia de EPANET. 

#### **3.1 Demanda variable.**
Es posible definir demandas variables en cada uno de los nodos que componen una red. Este módulo pretende dar a 
conocer la aplicación de la herramienta del Epanet a partir de un ejercicio aplicado de un sistema de hidráulico
a presión con demanda variable.

#### **3.2 Ecuaciones para el cálculo de las pérdidas por fricción. Variación de los resultados.**
En este módulo se describe conceptualmente las diferentes ecuaciones que utiliza Epanet para la determinación de las 
pérdidas por fricción en los sistemas a presión. Se realizará una comparación de los resultaos evaluando, para un
mismo problema práctico, las diferentes ecuaciones de pérdidas de energía. 

#### **3.3 Inclusión de rociadores.**
A partir de un ejercicio práctico se analizan las metodologías para la definición de rociadores (emisores) 
utilizando las herramientas de Epanet.

#### **3.4 Curvas de rendimiento.**
A partir de un ejercicio práctico se incluirán curvas de rendimiento en una bomba hidráulica que alimentará
una red de drenaje a presión. Se analizarán las características de una curva de rendimiento real antes de 
aplicarlo al proyecto en Epanet.

#### **3.5 Tanque de alimentación asimétricos.**
A partir de un ejercicio práctico se incluirán tanques de alimentación con formas asimétrica (diferentes a un 
cubo o a un paralelepipedo) en un sistema hidráulico con una red de flujo a presión. Se analizarán las curvas
de alimentación a partir de las curvas de capacidad o curvas de volumen de tanques asimétricos. 

### **Taller de aplicación de la unidad 3.1, 3.2, 3.3, 3.4 y 3.5** 

#### **3.6 Programación en Epanet.**
A partir de diferentes herramientas de programación se realiza cargue de información, edición de parámetros
y análisis de información utilizando diferentes programadores de consola, entre ellos la integración de Epanet
y Python.     

### **Taller de aplicación de la unidad 2.4** 

*En la siguiente imagen se presenta el contenido pogramático resumido en un diagrama de flujo.*

![Imagen 2](https://github.com/AndresOtalora92/CursoEpanetBasico-Intermedio/blob/817dcef56340f2e95f2e3c6337da5fd4f3eaf50a/.jpg/DiagramasCursoBasico3.jpg)

# Material del curso por módulos.

Tal como se describió anteriormente, se recomienda que el estudiante revise, estudie y analice la 
información contenida en cada submódulo, siguiendo el orden definido en el contenido programático. En el 
caso que el estudiante requiera la certificación del cursos,este deberá realizar las actividades 
y presentarlas al tutor siguiendo las instrucciones del caso.
