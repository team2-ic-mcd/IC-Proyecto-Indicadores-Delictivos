<p align="center">
    <img width="200" src="https://upload.wikimedia.org/wikipedia/commons/6/68/Escudo_Unison.png">
</p>

<h4 align="center"><b>"El saber de mis hijos hará mi grandeza"</b></h4>

<h5 align="center">Facultad de ciencias exactas y naturales</h5>
 
<h5 align="center">Departamento de matemáticas</h5>

<h5 align="center">Maestría en Ciencia de datos</h5>

<p align="center">
    <img width="150" src="https://mcd.unison.mx/wp-content/uploads/2020/02/400dpiLogoCropped-150x150.png">
</p>

<h5 align="center">Curso de Ingenería de características</h5>
 
<h5 align="center">Prof. Julio Waissman</h5>

<h5 align="center">Proyecto</h5>

<h4 align="center">Narrando una historia con datos: explorando el poder de la ciencia de datos</h4>

<h5 align="center">Tema</h5>

<h4 align="center">Análisis de la variabilidad del comportamiento delictivo en relación con factores temporales y geográficos, y su correlación con el desarrollo social y urbano para la prevención del delito</h4>

<h5 align="center">Equipo 2</h5>

<h5 align="center">Burruel Duran Luis Andres</h5>

<h5 align="center">Medina León Miguel Ernesto</h5>

<h5 align="center">Estrada Ferreira Mario</h5>

<h6 align="center">Hermosillo, Sonora, México</h6>

<br>
<br>






![](https://datascientest.com/es/wp-content/uploads/sites/7/2021/05/illu_data_cleaning_blog_2-07.png)
  
<div class="container">
    <h1>Parte 1. Descarga y limpieza de datos</h1>
    <h5>En esta fase inicial, se aborda el proceso de descarga automatizada de datos provenientes de diversas fuentes en línea. Se pone un énfasis particular en la manipulación y limpieza de los conjuntos de datos, con el objetivo de transformarlos en estructuras tabulares conformes a los principios de tablas "tidy" de acuerdo a las necesidades de nuestro proyecto.
      
  Dentro de este repositorio, se encuentran los siguientes elementos:
  <ul>
  <li>Una libreta Jupyter diseñada para la descarga automatizada de datos desde múltiples APIs y fuentes mediante la implementación de funciones especializadas y eficientes, empleando métodos que permiten la obtención de datos a gran escala.</li>
  <li>Una libreta adicional, que se encarga de la lectura de los datos descargados, su transformación en DataFrames y la ejecución de tareas de limpieza y reestructuración con el fin de obtener tablas "tidy" que faciliten el análisis subsiguiente.</li>
  <li>Un archivo en formato PDF que presenta de manera detallada el enfoque temático y la propuesta de las narrativas que serán desarrolladas utilizando los datos obtenidos.</li>
  <li>Un notebook de Jupyter diseñado para la generación de presentaciones dinámicas y visuales, con el propósito de exponer de manera efectiva y atractiva las ideas contenidas en el documento PDF mencionado anteriormente.</li>
  <li>Un diccionario de datos que establece una vinculación sistemática entre los nombres de cada variable presente en las tablas de datos y sus respectivos conceptos en el contexto de nuestro análisis. Este recurso es esencial para la clarificación y la correcta interpretación de las características y métricas que se emplean en el marco de la investigación en ciencia de datos.</li>
</ul>
</h5>
    <h3> </h3>
    <h5></h5>
</div>

## Incidencia delictiva

En el presente proyecto, se llevará a cabo la obtención de cuatro archivos en formato CSV desde la página oficial del Gobierno de México, específicamente desde la siguiente fuente: https://www.gob.mx/sesnsp/acciones-y-programas/datos-abiertos-de-incidencia-delictiva. 

Los conjuntos de datos a adquirir son los siguientes:

* Cifras de Incidencia Delictiva Estatal, 2015 - agosto  2023.
* Cifras de Incidencia Delictiva Municipal, 2015 - agosto 2023.
* Cifras de Víctimas del Fuero Común, 2015 - agosto 2023.
* Cifras de Incidencia Delictiva Federal, 2012 - agosto 2023.

Las fuentes de estos datos se encuentran alojadas en los siguientes enlaces:

- Datos estatales: https://drive.google.com/file/d/1iCY71DLzgcWtyycUlOeS6BvxARL91gf-/view?usp=sharing
-  Datos municipales: https://drive.google.com/file/d/13TjyJ9RkR49o0eWTFvhNqazeL4maORYp/view?usp=sharing
-  Datos de víctimas del fuero común: https://drive.google.com/file/d/1JsXir5EGFMcEjtJKzZSu7hSdEt5zYOX9/view?usp=sharing
-  Datos federales: https://drive.google.com/file/d/1p6ZeTkeu7UCAzyLUOnM_o-Yn_B3i89bC/view?usp=sharing

Una vez completada la adquisición de estos datos, se llevará a cabo un proceso de limpieza y transformación con el objetivo de obtener tablas en formato 'tidy'. Estas tablas limpias y organizadas serán fundamentales para la posterior comparación y correlación con otros conjuntos de datos, tales como:

1. Datos de desarrollo social y urbano.
2. Datos climáticos por municipio.
3. Datos relacionados con la creación de escuelas y graduados por año.

Estos análisis permitirán contar una narrativa basada en evidencia, explorando temas como:

* La influencia de la creación de espacios recreativos y áreas comunes en la prevención de la delincuencia.
* La relación entre el tipo de crímenes y las condiciones climáticas, incluyendo temperaturas extremas y lluvias torrenciales, así como la variación en la actividad delictiva en función de las horas de luz solar.
* La identificación de patrones de delincuencia predominantes en distintos sectores geográficos del estado de Sonora.

Este enfoque analítico nos permitirá desarrollar una narrativa robusta y fundamentada en datos que contribuirá a un mayor entendimiento de la incidencia delictiva en el contexto estudiado.

## Metereología municipal y estatal

En el contexto de este proyecto, se procederá a la obtención de un archivo CSV que contenga datos climatológicos diarios para cada municipio. Estos datos han sido adquiridos mediante el uso de la API Historical Weather. Para obtener información detallada sobre esta API, se puede consultar el siguiente sitio web: https://open-meteo.com/en/docs/historical-weather-api

El conjunto de datos que se busca adquirir es el siguiente:

* Datos climáticos municipales

Las fuentes de estos datos son accesibles a través de la API, cuya ubicación se encuentra en el siguiente enlace: https://archive-api.open-meteo.com/v1/archive

Una vez completada la obtención de estos datos en su forma original (raw), se llevará a cabo un proceso de limpieza y transformación con el propósito de estructurar los datos en tablas en conformidad con el formato 'tidy'. Este proceso de limpieza incluye la eliminación de valores NaN y la exclusión de datos correspondientes a fechas futuras.

### Tablas tidy seleccionadas

Después de adquirir los datos en su forma original y someterlos a un proceso de limpieza y transformación, se han generado seis tablas organizadas en el formato 'tidy'. Estas tablas, junto con sus respectivas descripciones, son las siguientes:

1. Incidencia_Delictiva_Estatal:

    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Entidad: entidad de registro.
    * Clasificación de delitos (primera, segunda, tercera y cuarta): categorización de los delitos en diferentes niveles.
    * Conteo de delitos: número de delitos registrados.

2. Incidencia_Delictiva_Municipal:
    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Municipio: municipio de registro.
    * Clasificación de delitos (primera, segunda, tercera y cuarta): categorización de los delitos en diferentes niveles.
    * Conteo de delitos: número de delitos registrados.
    * Región del estado de Sonora: región geográfica a la que pertenece el municipio.

3. Incidencia_Delictiva_Federal:
    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Entidad: entidad de registro.
    * Ley: ley relacionada con el delito.
    * Concepto: concepto del delito.
    * Tipo: tipo de delito.
    * Conteo de delitos: número de delitos registrados.

4. Victimas_Fuero_Comun_Estatal:
    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Entidad: entidad de registro.
    * Clasificación de delitos (primera, segunda y tercera): categorización de los delitos en diferentes niveles.

5. Meteorología_Climatología_Estatal:
    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Entidad: entidad de registro.
    * Valor promedio mensual de temperatura máxima, mínima y promedio: valores climáticos registrados a dos metros sobre el suelo.
    * Hora promedio mensual de salida y puesta de Sol: horarios en los cuales el sol aparece y desaparece del horizonte.
    * Minutos promedio de luz solar: duración promedio de la luz solar en minutos.
    * Precipitación total mensual: cantidad total de precipitación atmosférica registrada, incluyendo diversas formas de precipitación.
    * Lluvia total mensual: cantidad total de lluvia registrada.
    * Horas de precipitación mensual: suma total de horas con precipitación registrada.

6. Meteorología_Climatología_Municipal:
    * Año: año de registro de los datos.
    * Mes: mes de registro de los datos.
    * Entidad: entidad de registro.
    * Municipio: municipio de registro.
    * Región del estado de Sonora: región geográfica a la que pertenece el municipio.
    * Valores climáticos, horarios, minutos de luz solar y datos de precipitación: similar a la tabla anterior, pero a nivel municipal.

Estas tablas 'tidy' representan el resultado de una exhaustiva preparación de datos y están listas para ser utilizadas en análisis subsiguientes y en la construcción de modelos y narrativas basadas en datos.

<h2 align="center">Historias a contar</h2>

<br>
<br>

![](https://www.productosjumbo.com/wp-content/uploads/2021/07/banner-canchasc.jpg)

### Efectos del desarrollo social y urbano sobre la disminución de la delincuencia

> El paisaje urbano ha experimentado cambios notables en los últimos años, con la creación de nuevos parques, espacios verdes, canchas deportivas y áreas recreativas. Estos proyectos urbanos plantean la pregunta de su utilidad y efecto en la sociedad. Se ha formulado la hipótesis de que los espacios verdes y las áreas recreativas pueden desviar la atención de la población, en particular de los jóvenes, de actividades delictivas, como el consumo de drogas o la participación en pandillas. Sin embargo, ¿hasta qué punto esta hipótesis se sostiene? Este estudio propone una investigación que compara conjuntos de datos sobre la incidencia delictiva en municipios y colonias con datos proporcionados por la Secretaría de Desarrollo Social y Urbano. El objetivo es determinar si existe una correlación significativa entre el desarrollo social y urbano y la reducción de la delincuencia, así como analizar el impacto de las áreas recreativas en la población en términos de prevención del delito.

<br>
<br>
<br>

![](https://englishlive.ef.com/es-mx/blog/wp-content/uploads/sites/8/2018/07/Hablemos-de-las-estaciones-y-el-clima-en-ingl%C3%A9s1.jpg)

### Impacto de las estaciones en la incidencia de un tipo específico de delito

> ¿Influye la temporada en la incidencia de diferentes tipos de delitos y cuáles predominan en cada estación? Esta interrogante cobra relevancia en el contexto de Sonora, un estado caracterizado por su variabilidad climática. Por ejemplo, las elevadas temperaturas del verano o las pocas horas de sol en invierno podrían influir en el comportamiento delictivo y su distribución. Para abordar esta cuestión, se requieren dos conjuntos de datos: uno que registre los tipos de delitos cometidos a lo largo del año y otro que recoja información climática durante el mismo período.

<br>
<br>
<br>

![](https://contraloria.sonora.gob.mx/images/2023/02/10/mapa_regionalizacion_cpcem_2021_2024.jpg)

### Análisis geoespacial de la distribución de tipos de delito en el estado de Sonora: norte, centro y sur

> Este estudio tiene como objetivo investigar la incidencia de diversos tipos de delitos en diferentes zonas del estado de Sonora. Dado que Sonora es uno de los estados más extensos de México, resulta relevante comprender la distribución de estos delitos en distintas regiones, y determinar si existen correlaciones significativas tanto entre las zonas como entre los municipios. Se llevará a cabo una comparación de los delitos en las distintas regiones, con el propósito de identificar patrones y determinar cuál de estas áreas presenta una mayor conflictividad delictiva. Para llevar a cabo esta investigación, se empleará una base de datos que registra la ocurrencia de diferentes tipos de delitos en los municipios de Sonora a lo largo de un período de 5 años.

