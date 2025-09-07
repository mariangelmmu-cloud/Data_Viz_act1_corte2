#  **Taller de Imputación de Datos**

##  Objetivo
Aprender a:
1. Identificar valores faltantes en un conjunto de datos mixto.
2. Clasificar los tipos de ausencia (MCAR, MAR, MNAR).
3. Definir si se deben imputar o no.
4. Aplicar técnicas de imputación apropiadas.
5. Representar los datos antes y después de imputar.
6. Evaluar si la imputación preserva las características de la variable.



##  Lineamientos de trabajo

### 1. Exploración inicial de las variables
- Cargar el dataset `base_imputacion_mixta_1000.csv` https://github.com/Kalbam/Datos/blob/main/base_imputacion_mixta_1000.csv.
- Identificar las variables **cualitativas** y **cuantitativas**.
- Observar la estructura general de la base de datos (`.head()`, `.info()`, `.describe()`).



### 2. Detección de valores faltantes
- Calcular el número y porcentaje de valores faltantes por variable.
- Representar gráficamente los nulos:
  - **Gráfico de barras** con el porcentaje de nulos por variable.
  - **Mapa de calor** que muestre la distribución de los faltantes por fila y columna.



### 3. Clasificación del tipo de faltante
- Clasificar los faltantes en **MCAR**, **MAR** o **MNAR** según patrones observados.
- Justificar por qué una variable cae en cada categoría.



### 4. Discusión sobre imputabilidad
- Responder para cada variable:
  - ¿Se justifica imputar o dejar los nulos?
  - ¿Qué riesgo tendría imputar esta variable?
  - ¿Qué técnica sería más adecuada (media, mediana, moda, interpolación, etc.)?



### 5. Representación de la imputación
- Aplicar al menos **tres técnicas distintas de imputación** según el tipo de variable:
  - Numéricas: media, mediana, KNN, regresión.
  - Categóricas: moda, hot-deck, KNN.
  - Series temporales: forward fill, backward fill, interpolación.
- Generar **gráficos comparativos antes y después de imputar**:
  - Histogramas y boxplots para numéricas.
  - Gráficos de barras para categóricas.
  - Líneas para series temporales.



### 6. Evaluación de la imputación
- Validar si la imputación alteró la variable:
  - **Normalidad**: prueba de Shapiro–Wilk.
  - **Igualdad de distribuciones**: Kolmogorov–Smirnov.
  - **Comparación de medias o rangos**:
    - t de Student (si es normal).
    - Mann–Whitney U (si no es normal).
- Concluir si la técnica de imputación **preserva o distorsiona** los datos originales.
- Comparar entre las distintas técnicas aplicadas.



### 7. Conclusión preliminar
- Elaborar una **tabla resumen** con:
  - Nombre de la variable.
  - Porcentaje de nulos.
  - Tipo de ausencia (MCAR, MAR, MNAR).
  - Método sugerido de imputación.
  - Evidencia de que la imputación mantiene o no la distribución.

