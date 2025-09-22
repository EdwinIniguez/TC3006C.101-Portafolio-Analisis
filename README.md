# Portafolio de Análisis

Este repositorio integra las evidencias de análisis de datos y modelado desarrolladas en los diferentes módulos de la asignatura. Cada sección contiene enlaces específicos a los repositorios y archivos que contienen las evidencias requeridas para cada indicador de competencia.

## Evidencias por Subcompetencia

### 1. Técnicas Analíticas (SMA0102A)

#### **Indicador 1:** Utiliza al menos 2 técnicas de preprocesamiento de acuerdo al problema
- **Repositorio Principal:** [TC3006C.101 - Bank Account Fraud Challenge](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - **Imputación de valores faltantes:** En `preprocess_all_datasets.py` - tratamiento de valores `-1` como datos faltantes
  - **Escalamiento de variables:** Normalización de variables numéricas para evitar sesgos por diferencias de escala
  - **Manejo de outliers:** Técnica de recorte con IQR implementada en los notebooks de EDA
  - **Balanceo de clases:** Uso de SMOTE (oversampling) y undersampling documentado en README del repo
  - **Reporte escrito:** Respote escrito con detalles sobre esto en la carpeta de reporte/
- **Repositorio Complementario:** [Aprendizaje - California Housing](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - **Escalamiento:** En `Aprendizaje/codes/preprocess/` - normalización de datos California Housing
  - **Detección de anomalías:** Análisis de outliers en dataset de regresión

#### **Indicador 2:** Explica claramente el uso de cada técnica de análisis utilizada y su relevancia en el set de datos
- **Repositorio Principal:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - `EDA.ipynb`, `EDA_1.ipynb` a `EDA_5.ipynb` - Análisis exploratorio detallado con justificación de técnicas
  - `EDA_actualizado.ipynb` - Versión consolidada del análisis exploratorio
  - README completo del repositorio explica el uso y relevancia de cada técnica de preprocesamiento
- **Repositorio Complementario:** [MODELADO](https://github.com/EdwinIniguez/MODELADO)
- **Evidencias específicas:**
  - `MODELADO/1/Exploracion_Datos.ipynb` - Análisis exploratorio con justificación de técnicas
  - `MODELADO/1/Diccionario_Simple_VisualizacionAonline.xlsx` - Documentación detallada de variables y técnicas aplicadas


### 2. Análisis de Información (SMA0104A)

#### **Indicador 1:** Evalúa el modelo con un conjunto de prueba y un conjunto de validación
- **Repositorio Principal:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - `regressionLogistica.ipynb` - Evaluación con train/test/validation splits
  - `MLP_BASE.ipynb` - Validación de red neuronal con múltiples conjuntos
  - `SVM_MLP_BASE.ipynb` - Comparación de modelos con validación rigurosa
- **Repositorio Complementario:** [Aprendizaje](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - `Aprendizaje/codes/performanceAnalysis.py` - Script completo de evaluación con train/test
  - Curvas de aprendizaje en `Aprendizaje/resources/learning_curve_*.png`

#### **Indicador 2:** Detecta correctamente el grado de bias o sesgo: bajo/medio/alto
- **Repositorio Principal:** [Aprendizaje](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - `Aprendizaje/codes/performanceAnalysis.py` - Diagnóstico automático de bias
  - `Aprendizaje/Reporte_Desempeño_modelos_aprendizaje.pdf` - Análisis detallado de bias por modelo
  - Gráficas de diagnóstico: `pred_vs_real_*.png`, `boxplot_metricas_*.png`
- **Repositorio Complementario:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - README sección "7. Resultados y Hallazgos" - Análisis de bias por tipo de modelo

#### **Indicador 3:** Detecta correctamente el grado de varianza: bajo/medio/alto
- **Repositorio Principal:** [Aprendizaje](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - `Aprendizaje/codes/performanceAnalysis.py` - Cálculo y diagnóstico de varianza
  - Curvas de aprendizaje en `Aprendizaje/resources/learning_curve_*.png` - Visualización de varianza
  - `Aprendizaje/Reporte_Desempeño_modelos_aprendizaje.pdf` - Análisis comparativo de varianza
- **Repositorio Complementario:** [MODELADO](https://github.com/EdwinIniguez/MODELADO)
- **Evidencias específicas:**
  - `MODELADO/3/actividad_curvas_aprendizaje_validacion.ipynb` - Análisis de bias-variance tradeoff

#### **Indicador 4:** Explica el nivel de ajuste del modelo: underfit, fit, overfit
- **Repositorio Principal:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - README sección "7. Resultados y Hallazgos" con subsecciones por modelo explicando nivel de ajuste
  - `regressionLogistica.ipynb` - Análisis de overfitting en regresión logística
  - `MLP_BASE.ipynb` - Diagnóstico de ajuste en redes neuronales
- **Repositorio Complementario:** [Aprendizaje](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - `Aprendizaje/codes/performanceAnalysis.py` - Diagnóstico automático de nivel de ajuste
  - `Aprendizaje/Reporte_Desempeño_modelos_aprendizaje.pdf` - Explicación detallada del ajuste por modelo

#### **Indicador 5:** Utiliza técnicas de regularización para mejorar el desempeño del modelo
- **Repositorio Principal:** [Aprendizaje](https://github.com/EdwinIniguez/Aprendizaje)
- **Evidencias específicas:**
  - `Aprendizaje/codes/models/elasticNet_framework.py` - Implementación de ElasticNet con regularización L1 y L2
  - `Aprendizaje/codes/models/elasticNet_manual.py` - Implementación manual de regularización
  - `Aprendizaje/models/elasticnet_california.joblib` - Modelo entrenado con regularización
- **Repositorio Complementario:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - README sección "9. Supuestos y Regularización" - Uso de regularización L2
  - `regressionLogistica.ipynb` - Aplicación de regularización en regresión logística


### 3. Integridad Resuelve (SEG0403A)

#### **Indicador 1:** Explica cómo la solución cumple leyes, normas y principios éticos de la industria o el contexto profesional
- **Repositorio Principal:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - README sección "10. Aspectos Éticos y Normativos" - Análisis completo de cumplimiento ético
  - Subsecciones específicas:
    - **Privacidad y protección de datos:** Uso de datos sintéticos CTGAN
    - **Equidad y no discriminación:** Métricas de fairness implementadas
    - **Transparencia y explicabilidad:** Modelos interpretables y documentación completa
    - **Cumplimiento normativo:** Principios de IA Responsable y Fair ML

#### **Indicador 2:** Explica en su repositorio cuál es la normatividad correspondiente del reto o socio formador
- **Repositorio Principal:** [TC3006C.101](https://github.com/EdwinIniguez/TC3006C.101)
- **Evidencias específicas:**
  - README sección "10. Aspectos Éticos y Normativos" - Normatividad específica:
    - **GDPR:** Regulaciones de privacidad internacional
    - **Regulaciones financieras:** Normativas para sistemas de detección de fraude
    - **NeurIPS 2022 Challenge:** Regulaciones del reto académico
  - README sección "8. Fairness en el Reto" - Normativas de equidad:
    - **Predictive Equality:** Métricas de falsos positivos por grupo
    - **Equal Opportunity:** Métricas de verdaderos positivos por grupo

---

## Repositorios de Evidencias

1. **[TC3006C.101 - Bank Account Fraud Challenge](https://github.com/EdwinIniguez/TC3006C.101)**
   - Proyecto principal de detección de fraude
   - Evidencias completas de preprocesamiento, análisis y ética
   - Documentación de normatividad y cumplimiento

2. **[Aprendizaje - Análisis Comparativo de Modelos](https://github.com/EdwinIniguez/Aprendizaje)**
   - Análisis sistemático de bias, varianza y regularización
   - Implementaciones manuales y con framework
   - Diagnósticos automáticos de ajuste de modelos

3. **[MODELADO - Proyecto de Modelado Predictivo](https://github.com/EdwinIniguez/MODELADO)**
   - Construcción manual de modelos
   - Análisis exploratorio detallado
   - Validación de supuestos estadísticos

4. **[Data Science - Proyectos de Ciencia de Datos](https://github.com/EdwinIniguez/Data-Science)**
   - Notebooks complementarios de análisis estadístico
   - Técnicas de bootstrapping y pruebas de hipótesis
   - Proyectos de regresión lineal y logística
---

**Autor:** Edwin Iñiguez Moncada  
**Fecha:** Septiembre 2025  
**Curso:** TC3006C - Inteligencia Artificial Avanzada para la Ciencia de Datos