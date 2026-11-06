# Sprint IA07 — Yarinacocha

Proyecto UNI: Sistema híbrido de aprendizaje automático y optimización combinatoria para la planificación de rutas de recolección de residuos sólidos urbanos.

## Ejecución
1. Abrir `Sprint_IA07_Hiperparametros_Yarinacocha.ipynb` en Google Colab.
2. Ejecutar las celdas en orden, incluyendo la instalación de bibliotecas.
3. Al solicitar el CSV, adjuntar `residuos_yarinacocha_2026(2).csv` (o colocarlo en la misma carpeta).
4. Esperar a que terminen los trials y consultar `artifacts/`.
5. Publicar en GitHub Notebook, configuración, logs y gráficos.

## Enfoque
Predicción de kilogramos por recorrido, Random Forest y XGBoost, RandomSampler y TPESampler de Optuna, validación cronológica 70/15/15 y 3 folds temporales para búsqueda. Objetivo: minimizar MAE; se reportan también RMSE y R².

## Datos y límites
El Notebook original describe el dataset como **simulado**. No presentar sus métricas como validación con información operacional real. El archivo incluye fechas hasta diciembre de 2026. La optimización de rutas OR-Tools queda fuera del alcance de este sprint.

## Reproducibilidad
Semilla 42, 15 trials por método/modelo de forma predeterminada. Para prueba rápida local: `N_TRIALS=2 jupyter nbconvert --to notebook --execute Sprint_IA07_Hiperparametros_Yarinacocha.ipynb --output prueba.ipynb`.
