# Proyecto de Aplicación: Análisis de Saber 11 y Conectividad en Colombia (2017–2024)

## 1. Objetivo
Cuantificar la relación entre el rendimiento en el examen Saber 11 (segunda aplicación, calendario A) y la cobertura de internet fijo a nivel municipal, controlando por variables socioeconómicas y de recursos TIC del hogar, para orientar decisiones de inversión en infraestructura y educación.

---

## 2. Contexto
- *Problema*: Persisten brechas significativas en puntajes del Saber 11 entre municipios con distinta conectividad y condiciones socioeconómicas.  
- *Ámbito temporal*: Segunda aplicación anual, calendario A, de 2017 a 2024.  
- *Enfoque*: Panel municipal que integra puntajes Saber 11, ISNI, recursos TIC en el hogar y penetración de internet fijo (datos.gov.co).
---

## 3. Fases del Proyecto

### 3.A Fase Inicial  
- *Selección de datos*:  
  - Archivos .txt públicos de ICFES (2017–2024, aplicación 2).    
- *Exploración preliminar*:  
  - Estadísticos básicos, histogramas y boxplots.  
  - Correlaciones bivariadas y rankings municipales.

### 3.B Preparación de Datos  
- *Filtrado*: Sólo calendario A, periodo termina en 2.  
- *Selección y renombrado*: 24 variables clave (puntajes, ISNI, TIC, colegio).  
- *Codificación*:  
  - Ordinales (horas de internet, estrato, libros).  
  - Binarias (hogar con PC/internet).  
- *Imputación*:  
  - Medianas municipales → global en dedicación internet, puntajes e ISNI.  
  - NAs en educación parental → “DESCONOCIDO”/“OTROS”.  
- *Agregación*: Panel municipio–año y merge con penetración fija.

### 3.C Implementación de Modelos  
- *Supervisado*:  
  1. *Elastic Net* 
  2. *Gradient Boosting Regressor*
  - *Métricas*: RMSE, R².  
- *No supervisado*:  
  1. *PCA* (n=2) → reducción de dimensiones y biplot.  
  2. *K-means (k=4)* → segmentos municipales; silhouette score para validación.

---

## 4. Librerías y Herramientas  
- *Pandas & NumPy*: manipulación de datos.  
- *PySpark*: lectura / procesamiento escalable.  
- *scikit-learn*: pipelines, Elastic Net, GBR, PCA, K-means.  
- *Matplotlib / Seaborn*: visualizaciones.  
- *GeoPandas / Folium* (opcional): mapas coropléticos.  
- *Airflow / Prefect* (opcional): orquestación ETL.

---


## 5. Conclusiones y Observaciones  
- *Brecha urbano-rural*:
- *Elastic Net*:
- *GBR*:
- *Clusters*:
- *Tendencia histórica*:

---

## 7. Entregables  
- *Notebooks Jupyter* (notebooks/): EDA, modelado supervisado, no supervisado y análisis temporal.  
- *Scripts Python* (src/): ingesta, limpieza, pipelines ML.  
- *Dataset procesado* (data/processed/): Parquet/CSV limpio y panel final.  
- *Presentación* (PDF) y *informe técnico* (PDF).  

---




Por ahora este readme
