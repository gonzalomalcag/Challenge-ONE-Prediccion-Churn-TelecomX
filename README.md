# **Proyecto Predictivo de Churn - Challenge Alura ONE (Parte 2)**

¡Bienvenido a la culminación de mi viaje en el análisis de datos de Telecom X! Este repositorio documenta el desarrollo de un modelo de Machine Learning, la continuación de un proyecto de ETL y análisis exploratorio.

- **Autor:** Gonzalo Malca Garcia
- **Programa:** Oracle Next Education (ONE) + Alura Latam
- **Tecnologías Clave:** Python, Pandas, Scikit-learn, Seaborn, Google Colab

---

### **🎯 El Reto: De Analista a Científico de Datos**

En la primera fase de este desafío, realicé un profundo análisis exploratorio que reveló una preocupante **tasa de cancelación de clientes (Churn) del 26.58%**. Mi misión para esta segunda parte fue dar un paso más allá: utilizar esos hallazgos para construir un **modelo predictivo**.

El objetivo es dotar a Telecom X de una herramienta que permita **anticipar qué clientes están en riesgo de irse**, permitiendo así una estrategia de retención proactiva y basada en datos.

*   ➡️ *(Aquí Gonzalo puede poner el enlace a su repositorio de la Parte 1)*

---

### **🛠️ Mi Metodología: Un Pipeline de Machine Learning de Extremo a Extremo**

Para asegurar la calidad y fiabilidad de la predicción, seguí un riguroso pipeline de trabajo:

1.  **Preparación de los Datos (`Preprocessing`):**
    *   Utilicé el dataset de **7,032 clientes** previamente limpiado.
    *   Transformé todas las variables de texto a un formato numérico mediante **One-Hot Encoding**.
    *   **Estandaricé** las características numéricas para que el modelo pudiera aprender de manera justa y eficiente.

2.  **Modelado y Competencia (`Training & Selection`):**
    *   Dividí los datos en un 70% para **entrenamiento** y un 30% para **pruebas**, simulando un escenario real.
    *   Entrené dos modelos distintos para que compitieran: una **Regresión Logística** y un **Árbol de Decisión**.

3.  **Evaluación y Veredicto (`Evaluation`):**
    *   Medí el rendimiento de ambos modelos utilizando métricas clave como la **Precisión** y el **Recall**. La **Regresión Logística** demostró ser superior, especialmente en su capacidad para identificar a los clientes que realmente cancelaron.

---

### **🏆 Resultados del Modelo Campeón (Regresión Logística)**

El modelo final es capaz de predecir el Churn con un alto grado de confianza. Sus calificaciones en el conjunto de datos de prueba fueron:

| Métrica de Rendimiento     | Calificación |
| :------------------------- | :----------: |
| **Exactitud General**      |   **80%**    |
| **Recall (Sensibilidad)**  |   **57%**    |
| **Precisión**              |   **64%**    |
| **F1-Score (Balance)**     |   **0.60**   |

> **Conclusión Práctica:** Este modelo nos permite **identificar correctamente a casi 6 de cada 10 clientes** que están a punto de abandonar el servicio, dándonos una valiosa oportunidad para actuar.

---

### **💡 ¿Qué Aprendió el Modelo? Los Factores Clave del Churn**

El análisis del modelo nos reveló qué características son las más importantes para predecir la cancelación:

#### **🔴 Señales de Alerta (Aumentan el riesgo de Churn):**
*   **Servicio de Fibra Óptica:** Es el principal predictor de que un cliente podría irse.
*   **Facturas Mensuales Altas:** La sensibilidad al precio es un factor importante.
*   **Contratos Mes a Mes:** La falta de un compromiso a largo plazo aumenta la vulnerabilidad.

#### **🟢 Señales de Lealtad (Disminuyen el riesgo de Churn):**
*   **Antigüedad (Tenure):** Es, por mucho, el factor de protección más fuerte. Un cliente que supera los primeros meses es muy probable que se quede.
*   **Contratos de Larga Duración (1 o 2 años):** Generan una fuerte barrera de salida.

---

### **🚀 Cómo Usar Este Proyecto**

1.  **Clona o descarga** este repositorio.
2.  **Abre el notebook** `Solucion_Challenge_ML_GMG.ipynb` en Google Colab.
3.  **Sube el archivo** `telecom_x_datos_limpios.csv` a tu sesión.
4.  **Ejecuta todas las celdas** para ver el proceso completo.
