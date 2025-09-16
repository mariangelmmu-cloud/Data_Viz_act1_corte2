# **Taller #2 Georreferenciación con Datos Abiertos de Colombia**

Mariangel Mercado


# **Objetivo del taller**
Aprender a integrar datos abiertos de salud, economía, combustibles o ambiente con los **shapefiles oficiales del DANE** para construir mapas temáticos (coropléticos) que permitan analizar fenómenos sociales en Colombia.

1. Selecciona uno de los **enlaces de datos abiertos** que se presentan a continuación.  
2. Descarga un dataset que contenga información a nivel **departamental** o **municipal**.  
3. Verifica que tu dataset incluya el **código DANE** (2 dígitos para departamentos, 5 dígitos para municipios).  
   - Si no aparece, deberás empatarlo usando el nombre oficial del territorio según el DANE.  
4. Une tu dataset con el **shapefile de departamentos del DANE** (`MGN2021_DPTO_POLITICO.shp`).  
5. Construye al menos **dos mapas coropléticos** en Python usando **GeoPandas**.  
6. Redacta un breve análisis interpretando los resultados de tus mapas.  



## ***Descripción del Dataset:*** 

El conjunto de datos contiene los principales indicadores de los niveles preescolar, básica y media discriminados por Departamento desde el año 2011 hasta 2023.

Este conjunto de datos se puede relacionar con el de matrícula en educación preescolar, básica y media donde se presenta la caracterización de los estudiantes que permiten obtener información para comprender el comportamiento de los indicadores.

A continuación, se muestra una breve descripción de las variables a usar en la actividad.

| Variable | Tipo de dato | Descripción |
|----------|--------------|-------------|
| AÑO | Categórico | Vigencia del indicador. |
| CÓDIGO_DEPARTAMENTO | Categórico | Código DANE del departamento. |
| DEPARTAMENTO | Categórico | Nombre del Departamento. |
| POBLACIÓN_5_16 | Numérico | Población en edad teórica de estudiar (5 a 16 años) según proyecciones de población del DANE. |
| DESERCIÓN | Numérico | Tasa de deserción intra - anual del sector oficial. Identifica la proporción de alumnos matriculados que por factores culturales, coyunturales o de prestación del servicio educativo, abandonan sus estudios durante el año lectivo. |
| DESERCIÓN_TRANSICIÓN | Numérico | Tasa de deserción intra - anual del sector oficial en transición. Identifica la proporción de alumnos matriculados que por factores culturales, coyunturales o de prestación del servicio educativo, abandonan sus estudios durante el año lectivo. |
| DESERCIÓN_PRIMARIA | Numérico | Tasa de deserción intra - anual del sector oficial en primaria. Identifica la proporción de alumnos matriculados que por factores culturales, coyunturales o de prestación del servicio educativo, abandonan sus estudios durante el año lectivo. |
| DESERCIÓN_SECUNDARIA | Numérico | Tasa de deserción intra - anual del sector oficial en secundaria. Identifica la proporción de alumnos matriculados que por factores culturales, coyunturales o de prestación del servicio educativo, abandonan sus estudios durante el año lectivo. |
| DESERCIÓN_MEDIA | Numérico | Tasa de deserción intra - anual del sector oficial en media. Identifica la proporción de alumnos matriculados que por factores culturales, coyunturales o de prestación del servicio educativo, abandonan sus estudios durante el año lectivo. |