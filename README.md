# Clasificaci-n-y-Optimizaci-n-de-Hiperpar-metros
Descripción
Este proyecto aplica técnicas de Machine Learning para clasificar pacientes según su probabilidad de generar altos costos médicos, basándose en un conjunto de datos.

Dataset
Se utilizó un dataset que contiene variables como edad, sexo, índice de masa corporal (BMI), número de hijos, hábito de fumar, región y costos médicos (charges).

Para la clasificación, se definió un objetivo binario: pacientes con costos por encima del percentil 75 fueron etiquetados como "alto costo" y el resto como "bajo costo".

Metodología
Análisis Exploratorio de Datos (EDA): Inspección inicial para entender la estructura, detectar valores faltantes y outliers.

Preprocesamiento:
Imputación (no fue necesaria en este caso por ausencia de datos faltantes).
Codificación One-Hot para variables categóricas.
Escalado de variables numéricas con StandardScaler.

Modelos Entrenados:
Regresión Logística
K-Nearest Neighbors (KNN)
Árbol de Decisión

Validación: Se utilizó validación cruzada para evaluar el rendimiento inicial de los modelos.

Optimización de Hiperparámetros: Se aplicaron GridSearchCV y RandomizedSearchCV para mejorar el desempeño.

Evaluación Final: Los modelos optimizados se evaluaron mediante métricas como accuracy, precisión, recall, F1-Score y ROC-AUC. También se analizaron matrices de confusión y curvas ROC para entender la capacidad de clasificación.

Resultados
Los tres modelos optimizados lograron altos niveles de precisión y capacidad predictiva.
El mejor rendimiento se obtuvo con los modelos optimizados por RandomizedSearchCV.
La regresión logística mostró un excelente balance entre precisión y recall.
KNN y árbol de decisión también demostraron un desempeño robusto, con diferencias mínimas.

Conclusión
El proyecto confirma que es posible predecir con buena precisión si un paciente tendrá altos costos médicos usando modelos clásicos de clasificación. La optimización de hiperparámetros y el análisis cuidadoso de métricas clave permiten seleccionar modelos confiables para aplicaciones reales.
