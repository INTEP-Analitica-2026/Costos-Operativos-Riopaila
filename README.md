# Costos Operativos — Riopaila Castilla

Proyecto de Analítica Predictiva Aplicada a los Negocios
INTEP Roldanillo Valle | Postgrado Especialización en Big Data y Analítica de Datos  | 2026

## Equipo
- Cesar Augusto Tirado.
- Eliana Villanueva.
- Francisco Jaier Trejos

## Descripción
[Poner aquí Breve descripción del problema de negocio]

## Archivos
- `Notebook.ipynb` — Código Python completo
- `Presentacion.pptx` — Diapositivas de la exposición
- `Informe.docx` — Informe ejecutivo para el gerente


  

## 1. Descripción del Proyecto

El proyecto consiste en el desarrollo de un modelo de analítica predictiva y prescriptiva para el Ingenio Riopaila Castilla, analizando más de 117.000 registros históricos (2021-2025) de labores agrícolas en cultivos de caña de azúcar. Su objetivo principal es entender el comportamiento de los costos operativos, anticipar desviaciones presupuestales, identificar ineficiencias en campo y proporcionar recomendaciones basadas en datos para optimizar la asignación de recursos financieros.

## 3. Modelos Usados
   
Se implementaron algoritmos de Machine Learning enfocados en clasificación, regresión y segmentación:
•	Árbol de Decisión: Utilizado por su alta precisión y capacidad para manejar datos numéricos y categóricos. Fue clave para identificar qué variables tienen mayor peso en la desviación de costos.
•	Regresión Logística: Empleado para clasificar labores en categorías binarias (ej. "eficiente" vs. "no eficiente") y calcular la probabilidad de que una labor supere el presupuesto.
•	Regresión Lineal: Aplicado para estimar valores continuos, cuantificando el impacto directo de cada variable sobre el costo total esperado.
•	Clustering (K-Means): Utilizado para la segmentación de lotes según su perfil de eficiencia y costo por unidad.
•	SARIMA: Modelo de series de tiempo aplicado para proyectar la evolución estacional y anual de los costos hasta 2026.

## 4. Tecnologías Usadas
   
El proyecto se fundamenta en las siguientes tecnologías y disciplinas:
•	Arquitectura de Big Data: Para la limpieza, estructuración y procesamiento de un dataset masivo (más de 117.000 a 177.000 registros).
•	Machine Learning / Analítica Predictiva: Para el entrenamiento y evaluación de los modelos algorítmicos.
•	Análisis Exploratorio de Datos (EDA): Técnicas estadísticas para detectar outliers extremos, patrones de estacionalidad mensual y correlaciones de variables.

## 5. Resultado Principal y Métricas Clave

El hallazgo principal es que la ineficiencia operativa y el gasto están altamente concentrados en labores y lotes específicos, pero el gasto general es predecible en un 82% basándose únicamente en el volumen de trabajo.
Aquí tienes las métricas críticas que respaldan este resultado:
Concentración del Gasto
Indicador	Métrica Clave	Impacto en el Negocio
Top 3 Labores Costosas	65% del presupuesto total	Se concentra en: Fertilización (26.4%), Control de malezas (23.1%) y Riego (16.0%).
Gasto en Fertilización	$70.000 millones (en 5 años)	Consumidos por solo 2 materiales (Abono aporque y equipo asociado). Es el mayor potencial de ahorro.
Motor del Costo (Variable)	0.818 (Importancia)	El 82% del costo de una labor depende exclusivamente de la "Cantidad producida real" (volumen).
Outliers Detectados	> $18 millones	Labores atípicas que superan este costo y representan desviaciones no justificadas por el volumen.


