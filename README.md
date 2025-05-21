# 📊 Análisis de Factores Socioeconómicos y su Impacto en el Desempeño Académico (Saber 11)

## 🧠 Descripción del Proyecto

Este proyecto tiene como objetivo identificar y analizar cómo las condiciones socioeconómicas, familiares, tecnológicas y escolares de los estudiantes en Colombia influyen en su desempeño en las pruebas Saber 11. Utilizando un enfoque de procesamiento de datos a gran escala, el análisis combina estadística descriptiva, inferencial y técnicas de aprendizaje automático supervisado y no supervisado.

Se trabajó con más de 4.7 millones de registros del ICFES (2017–2024), y se implementaron herramientas modernas de Big Data y análisis predictivo para extraer patrones y generar recomendaciones de política educativa con base en evidencia empírica.

## 🛠 Herramientas y Tecnologías

- Python 3.10+
- Apache Spark (PySpark): procesamiento distribuido de grandes volúmenes de datos.
- Databricks: entorno colaborativo para manipulación y análisis de datos masivos.
- scikit-learn: modelado predictivo, regresiones regularizadas y clustering (K-Means).
- Pandas / NumPy: manipulación de datos.
- Matplotlib / Seaborn: visualización de datos.
- Jupyter Notebooks / Databricks Notebooks: desarrollo iterativo del análisis.

## 📌 Etapas del Proyecto (Metodología CRISP-DM)

1. Entendimiento del negocio  
   Identificación del problema educativo y definición del objetivo analítico: mejorar la comprensión de los factores que afectan el desempeño académico.

2. Entendimiento de los datos  
   Unificación de datos Saber 11 entre 2017–2024. Exploración de variables sociodemográficas, institucionales y de rendimiento.

3. Preparación de los datos  
   - Limpieza, imputación y estandarización de más de 4 millones de registros.  
   - Reducción a variables clave: 35 columnas seleccionadas.

4. Modelado predictivo (supervisado)  
   - Implementación de regresión Ridge para predecir el puntaje global.  
   - Mejores métricas obtenidas:  
     - RMSE ≈ 42  
     - R² ≈ 0.32

5. Segmentación (no supervisado)  
   - Clustering con K-Means (k=4) para agrupar estudiantes según sus patrones de desempeño.  
   - Visualización de perfiles estudiantiles diferenciados.

6. Evaluación y discusión  
   - Pruebas ANOVA unidireccionales para variables categóricas.  
   - Análisis de desigualdades por nivel socioeconómico, acceso a internet, tipo de colegio, entre otros.

## 🔍 Hallazgos clave

- Existe una brecha significativa de rendimiento académico entre estudiantes según su nivel socioeconómico.
- El acceso a internet, computadores y libros en el hogar está fuertemente relacionado con puntajes más altos.
- Las características del colegio (oficial/privado, jornada, ubicación) también influyen de forma importante.
- El modelo predictivo, aunque con capacidad moderada, permite priorizar intervenciones basadas en datos.
- El clustering reveló perfiles estudiantiles diferenciados, útiles para políticas focalizadas.



