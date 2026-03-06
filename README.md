# 📁 Challenge Telecom X: Predicción de Churn en Telecomunicaciones

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Finalizado-success?style=for-the-badge)

## 📝 Descripción del Proyecto
Este proyecto forma parte de un desafío de **Machine Learning** enfocado en el análisis de retención de clientes para la empresa Telecom X. El objetivo principal es predecir la probabilidad de que un cliente cancele su suscripción (Churn) utilizando datos demográficos, de servicios y financieros.

---

## 🛠️ Herramientas y Tecnologías
* **Python** (Google Colab)
* **Pandas / Numpy** (Procesamiento de datos)
* **Seaborn / Matplotlib** (Visualización estadística)
* **Scikit-Learn** (Modelado predictivo)

---

## 🔍 Etapas del Desarrollo

### 1. Limpieza y Preprocesamiento
* **Tratamiento de Datos:** Eliminación de duplicados y columnas no informativas (`id`).
* **Refactorización:** Simplificación de variables categóricas para mejorar la señal del modelo.
* **Codificación:** Transformación de datos de texto a formato numérico (0 y 1) mediante `LabelEncoder`.

### 2. Análisis Exploratorio (EDA)
Realizamos un análisis profundo para entender el comportamiento de los clientes:
* **Matriz de Correlación:** Identificamos que el tipo de contrato y los cargos mensuales tienen el impacto más directo en la cancelación.
* **Análisis Dirigido:** Visualizamos mediante Boxplots y KDE Plots cómo los clientes nuevos y con facturas altas son los más propensos a abandonar el servicio.



### 3. Modelado de Machine Learning
Entrenamos y comparamos dos modelos con diferentes naturalezas matemáticas:
1. **Regresión Logística:** Implementada con un *Pipeline* de estandarización (`StandardScaler`) para manejar variables de diferentes escalas.
2. **Random Forest:** Un modelo de ensamble basado en árboles que permitió capturar relaciones no lineales sin necesidad de escalamiento previo.

---

## 📊 Resultados y Evaluación
Evaluamos los modelos utilizando métricas de clasificación, priorizando el **Recall** para minimizar los falsos negativos (clientes que se van sin ser detectados).

* **Hallazgo Clave 1:** El contrato "Mes a mes" es el principal detonante de cancelación.
* **Hallazgo Clave 2:** La antigüedad del cliente actúa como un factor protector; el riesgo disminuye drásticamente tras los primeros 12 meses.
* **Hallazgo Clave 3:** El servicio de fibra óptica muestra una tasa de Churn superior a otros servicios, posiblemente asociada a la sensibilidad al precio.



---

## 💡 Estrategias de Negocio Sugeridas
Basándonos en los modelos, se proponen las siguientes acciones:
* **Fidelización Temprana:** Implementar programas de acompañamiento durante los primeros 6 meses de contrato.
* **Incentivos de Migración:** Campañas para convertir contratos mensuales en contratos anuales mediante descuentos.
* **Añadir Valor Percebido:** Ofrecer servicios gratuitos de seguridad o streaming para clientes de alto consumo y mitigar la fuga por precio.

---

## 🚀 Cómo ejecutar el proyecto
1. Clona este repositorio: `git clone https://github.com/Vitoro42/TelecomX_LATAM_Parte2`
2. Instala las dependencias: `pip install pandas requests matplotlib seaborn`
3. Ejecuta el Jupyter Notebook o el script principal.

---
**Análisis realizado por:** Victor Rubilar  
**LinkedIn:** www.linkedin.com/in/victor-rubilar-inostroza
---
