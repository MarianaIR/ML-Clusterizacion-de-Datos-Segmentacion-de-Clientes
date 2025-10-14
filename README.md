# 🛒 CLUSTERIZACIÓN DE DATOS: SEGMENTACIÓN DE CLIENTES

[![Python](https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54)](https://www.python.org/)  
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)  
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=matplotlib&logoColor=white)](https://matplotlib.org/)  
[![Seaborn](https://img.shields.io/badge/Seaborn-0099CC?style=flat&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)

Este proyecto desarrolla un análisis completo de Ciencia de Datos aplicando **Machine Learning no supervisado (Clusterización)** para la **segmentación de clientes** en un E-commerce.

---

## 🧠 Contenido del Proyecto

### 1️⃣ Preparación de Datos y Análisis RFM
- **Técnica Central:** Se emplea la técnica **RFM (Recencia, Frecuencia, y Valor Monetario)** para segmentar el comportamiento del cliente basándose en datos transaccionales.
- **Carga de Datos:** El *dataset* utilizado, `e_commerce.csv`, es una adaptación del **Brazilian E-Commerce Public Dataset by Olist**.
- **Exploración de Datos:** El conjunto de datos consta de 26 columnas, incluyendo detalles del cliente (ID, CP, Ciudad, Estado), detalles del pedido (status, horario, precio, envío, tipo de pago, valor) y la categoría del producto.

### 2️⃣ Modelado (Clusterización y Segmentación)
- **Cálculo de Variables RFM:** Creación de las métricas de Recencia, Frecuencia y Valor Monetario a partir de los datos transaccionales (Inferido del uso de RFM).
- **Clusterización:** Aplicación de un modelo de *clustering* (tipo inferido por el objetivo) sobre las variables RFM para agrupar clientes con comportamientos similares.

### 3️⃣ Generación de Insights y Estrategias
- **Identificación de Segmentos Clave:** Creación de segmentos accionables para marketing, tales como:
    * **Premium:** Clientes con baja frecuencia pero altos ingresos (requieren atención especializada).
    * **Leales:** Clientes que compran con alta frecuencia y con un valor significativo (ofrecer descuentos especiales para mantenerlos activos).
    * **Sleeping Whale (Ballena Dormida):** Clientes con alta recencia e ingresos muy altos, pero que dejaron de comprar hace mucho tiempo (prioridad para estrategias de reactivación).
- **Toma de Decisiones:** Los *insights* generados permiten a la gerencia y al equipo de marketing tomar decisiones estratégicas basadas en el comportamiento real del cliente.

---

## 🛠️ Librerías Utilizadas

| Librería       | Uso principal                               |
|----------------|---------------------------------------------|
| **Pandas**     | Carga, manipulación y preparación de datos RFM|
| **NumPy**      | Cálculos numéricos y manejo de *arrays*|
| **Matplotlib / Seaborn** | Visualización de clusters y segmentos para el análisis|
| **Datetime** | Manejo de fechas y cálculo de la **Recencia** (actualidad)|

---

## 🎯 Objetivo del Proyecto
Aplicar la metodología RFM para la segmentación de clientes de un E-commerce, utilizando Machine Learning para identificar grupos de clientes con características de compra distintivas, y así proporcionar a la empresa conocimientos valiosos que permitan la personalización de campañas de marketing y la retención de clientes clave.

---

## 📈 Resultados Esperados
- Identificación de **segmentos de clientes claramente diferenciados** (ej. Premium, Leales, Durmientes).
- Obtención de **conocimientos estratégicos (*insights*)** para definir acciones de marketing específicas para cada grupo (ej. Atención especializada a clientes Premium, descuentos a clientes Leales).
- Mejora en la retención de clientes de alto valor que muestran signos de inactividad (**Sleeping Whale**).
