![100 Días De Data poster](100DiasDeData.png)

Contenidos:
* [Sobre el proyecto #100DíasDeData](#sobre-el-proyecto)
* [Definiciones](#definiciones)
  - [Nomenclatura de ejercicios](#nomenclatura-de-ejercicios)
  - [Sobre los 3 dīgitos que describen el nivel del ejercicio](#sobre-los-3-dígitos-que-describen-el-nivel-del-ejercicio)
* [Reglas a seguir](#reglas-a-seguir)
* [Estructura del repositorio](#estructura-del-repositorio)


## Sobre el proyecto
**#100DíasDeData**

El proyecto #100DaysOfCode tiene la idea de que una puede aprender muchísimo si escribe código una hora diaria por 100 días.

¿Qué tal si hiciéramos algo parecido con datos? Trabajar una hora por cien días seguidos en algo relacionado a datos.

Limpieza, manipulación, lectura y escritura, visualización, presentación, aplicaciones de datos. En Python, R, d3, stata, Excel, PowerBI, Tableau, lo que quieras.

## Definiciones

El repositorio esta compuesto por <span style="background-color:#be89ff78">proyectos</span> y <span style="background-color:#c7a02278">ejercicios</span>.

Un <span style="background-color:#c7a02278">ejercicio</span> es una actividad con una meta definida que puedes lograr en menos de una hora. No todos los ejercicios van a necesitar de escribir código para lograr la meta. Por ejemplo, crear unas paletas de color divergentes y secuenciales. Esto puede lograrse programáticamente escribiendo código o también utilizando ciertos sitios web.

Un <span style="background-color:#be89ff78">proyecto</span> es un grupo de ejercicios relacionados. Estos llevan más de una hora en terminar y puede que los ejercicios que lo compongan sean secuenciales. Es decir, puede que el tercer ejercicio de un proyecto no pueda llevarse a cabo hasta que se termine el segundo ejercicio.

### Nomenclatura de ejercicios:
* Los nombres de las carpetas de cada ejercicio no llevan espacios o caracteres especiales.
* La carpeta del ejercicio tiene un código de 3 dígitos describiendo el nivel del ejercicio.
* Cada ejercicio sólo tiene una carpeta. 
* Cada carpeta tiene un mínimo de 2 archivos: `instrucciones.md` y `solucion.md`. La solución puede ser un _script_ si está bien documentado. 

### Sobre los 3 dígitos que describen el nivel del ejercicio:
El nivel de un ejercicio se describe en 3 áreas: **complejidad**, **nivel de conocimiento previo necesario**, **tiempo necesario**. 

Cada área recibe una calificación del 1 - 5. 

La **complejidad** de un ejercicio se define por el número de pasos y tecnologías necesarias para llevarlo a cabo. Por ejemplo, un ejercicio en el que aprendemos a crear un gráfico de barras con `bokeh` puede ser nivel 1 o 2 de complejidad ya que es una sola tecnología (`bokeh`) y son pocos pasos necesarios para crear un gráfico de barras. Sin embargo, si el ejercicio es personalizar un gráfico de barras con`bokeh`, puede que el nivel de complejidad suba, dependiendo en que tantos pasos requiera esta personalización. 

El **nivel de conocimiento previo necesario** depende de la cantidad de tecnologías y/o información necesaria para llevar a cabo el ejercicio sin ayuda de alguien más. Por ejemplo, un ejercicio donde aprendamos a crear buenos mapas puede que se concentre en escoger buenos colores o la proyección "correcta". Si este es el caso, el ejercicio asume que ya sabes crear un mapa (aunque sea básico). Si esto es lo único que se necesita saber previamente a comenzar el ejercicio, puede tener una calificación de 1 o 2 para esta área. (Un ejemplo de nivel 4 o 5 puede ser desplegar una aplicación shiny a un servidor, por ejemplo). 

El **tiempo necesario** depende de la cantidad mínima necesaria de tiempo para completar un ejercicio. Por ejemplo, un ejercicio rápido mostrando como hacer un `INNER JOIN` en SQL puede ser un nível 1 o 2, si el ejercicio requiere que creemos una cuenta de BigQuery para ejecutar este SQL con los datos en la nube esta área sería un 2 o 3 o 4. Si el ejercicio requiere crear y entrenar un modelo de aprendizaje automatizado con una cantidad enorme de datos puede que te tome la hora entera. Esto sería un 5. 

## Reglas a seguir
Reglas que seguir:

* Un ejercicio no puede necesitar más de una hora en completarse. 
* Un ejercicio debe tener una meta que sea
  - Específica, Medible, Lograble, Relevante y con tiempo límite (una hora) o  _SMART_ por sus siglas en inglés (**S**pecific, **M**easurable, **A**chievable, **R**elevant, **T**ime-bound) 
* La meta de un ejercicio debe estar relacionada a el manejo, distribución, análisis, visualización, creación, consumo, entre otras cosas, de los datos.
* La meta de un ejercicio también puede ser relacionada a habilidades, responsabilidades y/o actividades relacionadas a los datos. Por ejemplo, un ejercicio pidiendo que unx lea un artículo sobre ética del uso de datos personales y escriba 300-500 palabras al respecto es válido. 
* Todos los datos necesarios para cumplir un ejercicio deben ser abiertos y accesibles para el público en general.
* Se pueden escribir ejercicios para software cerrado (como `Stata` y `SAS`). No sugieras que paguen por ese software. 
* Al igual que un ejercicio, un proyecto debe tener una meta _SMART_.
* Los ejercicios que componen un proyecto deben estar relacionados a la meta del proyecto. 

## Estructura del repositorio
Para desalentar el fanatismo por las herramientas el repositorio debería estar organizado por **temas** en el mundo de los datos:
* Limpieza de datos
* Visualización de datos 
* Adquisición, Creación y Distribución de datos (Creación y consumo de APIs, publicación de datos en data.world o kaggle o github, geolocalización, etc)
* Automatización de procesos (creación de reportes, _ETL pipelines_, etc)
* Análisis de datos (estadísticas básicas, extracción de información, etc) 
* Utilización de datos (ética, decisiones basadas en datos, etc)
* Surtido (herramientas y habilidades importantes que no necesariamente tengan una asociación directa con el mundo de los datos - git, manejo de proyectos, `cookiecutter`, creación de paquetes/librerías, etc)
* Proyectos: Lo más probable es que un proyecto contenga ejercicios en más de un tema así que estos estarán bajo la categoría `proyectos` 

```
.
├── LICENSE
├── README.md
├── -plantillas                                           <- Plantillas a seguir.
│   └── <nivel-de-dificultad>-<nombre-de-ejercicio>       <- Cada ejercicio tiene una carpeta con:
|       ├── instrucciones.md                              <- Archivo markdown con las instrucciones del ejercicio
|       └── solucion.md                                   <- La solución del ejercicio. Preferiblemente en markdown pero puede ser un _script_
├── adquisicion-distribucion
│   ├── <nivel-de-dificultad>-<nombre-de-ejercicio>       
|   │   ├── instrucciones.md                              
|   │   └── solucion.md                                   
|  ...
│   └── <nivel-de-dificultad>-<nombre-de-ejercicio>       
|       ├── instrucciones.md                              
|       └── solucion.md                                  
├── analisis                                  
|  ...
├── automatizacion                                 
|  ...   
├── limpieza                                 
|  ...  
├── proyectos
|   └── <nivel-de-dificultad>-<nombre-del-proyecto>       <- Cada proyecto tiene una carpeta con varios ejercicios
|       ├── <nivel-de-dificultad>-<nombre-de-ejercicio>     
|       │   ├── instrucciones.md                            
|       │   └── solucion.md                                  
|      ...
|       └── <nivel-de-dificultad>-<nombre-de-ejercicio>       
|           ├── instrucciones.md                              
|           └── solucion.md    
├── surtido                                 
|  ...   
└── visualizacion
   ...
    └── <nivel-de-dificultad>-<nombre-de-ejercicio>       
        ├── instrucciones.md                              
        └── solucion.md    
```