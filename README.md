🚗 Clasificación de Autos con Machine Learning

![Car Evaluation Project](https://cdn.pixabay.com/photo/2020/04/07/15/20/volvo-5013806_1280.png)


Este proyecto implementa un modelo de **clasificación supervisada** para predecir la **categoría de aceptación de un automóvil** (Car Evaluation Dataset) utilizando **Regresión Logística** y **SVM**, con un enfoque en la **optimización de hiperparámetros** mediante **GridSearchCV**.

---

## 📊 Objetivos del Proyecto

- Aplicar técnicas de **preprocesamiento de datos categóricos** usando `ColumnTransformer` y `OneHotEncoder`.  
- Entrenar modelos base (**baseline**) con **Logistic Regression** y **SVM**.  
- Mejorar el rendimiento mediante **búsqueda en malla (GridSearchCV)**.  
- Evaluar los modelos usando métricas **Macro-Precision**, **Macro-Recall** y **Macro-F1**.  
- Determinar cuál modelo logra la mejor generalización en el conjunto de datos.

---

## 🧠 Tecnologías y Librerías Usadas

- **Python 3.x**
- **scikit-learn**
- **pandas**
- **numpy**
- **matplotlib**

---

## ⚙️ Flujo del Proyecto

1. **Importación y exploración del dataset**  
   Se carga el conjunto *Car Evaluation* (atributos como `buying`, `maint`, `doors`, `persons`, `lug_boot`, `safety`, `class`).

2. **Preprocesamiento**  
   Se aplican transformaciones para convertir variables categóricas en numéricas mediante **OneHotEncoder** y **LabelEnconder** para la variable objetivo, adicionalmente, un **Pipeline** que automatiza el flujo.

3. **Entrenamiento de modelos base (baseline)**  
   Se entrenan dos modelos iniciales:  
   - Regresión Logística  
   - SVM (Support Vector Machine)

4. **Optimización con GridSearchCV**  
   Se realiza búsqueda exhaustiva de hiperparámetros para ambos modelos con **validación cruzada (Cross-Validation)**.

5. **Comparación y selección del mejor modelo**  
   Se elige el modelo con mejor puntaje **Macro-F1**, y se genera un **informe de clasificación** y **matriz de confusión**.

---

---

## 🚀 Cómo Ejecutarlo

1. Clona el repositorio  
   ```bash
   git clone https://github.com/tuusuario/Car-Evaluation-Machine-Learning-Model-Comparison.git
   cd CarEvaluation

