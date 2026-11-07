
# Sprint IA07 — Yarinacocha

## Descripción del trabajo realizado

En este sprint desarrollamos la optimización de hiperparámetros de los modelos Random Forest y XGBoost, con el objetivo de mejorar la predicción de la cantidad de residuos sólidos urbanos, expresada en kilogramos por recorrido, en el distrito de Yarinacocha.

Para ello, trabajamos en Google Colab utilizando un conjunto de datos simulado, que dividimos cronológicamente en 70 % para entrenamiento, 15 % para validación y 15 % para prueba. Asimismo, implementamos Optuna con los métodos RandomSampler y TPESampler, estableciendo 15 pruebas por cada combinación de modelo y método, con tres particiones temporales.

Para evaluar el desempeño predictivo, consideramos las métricas MAE, RMSE y R², priorizando la minimización del error absoluto medio. También organizamos los registros, configuraciones y gráficos de los experimentos para facilitar su reproducibilidad.

Finalmente, este sprint nos permitió avanzar en el componente de aprendizaje automático de nuestro sistema híbrido. Los resultados corresponden a una evaluación experimental con datos simulados, mientras que la optimización de rutas mediante OR-Tools se desarrollará en una etapa posterior.
