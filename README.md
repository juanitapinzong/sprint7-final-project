# 📊 Análisis de Segmentación y Patrones de Uso – ConnectaTel

## 🎯 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de los usuarios de *ConnectaTel* para identificar patrones de uso, segmentar clientes y generar recomendaciones estratégicas orientadas a:

•⁠  ⁠Optimización de planes comerciales
•⁠  ⁠Identificación de usuarios de alto valor
•⁠  ⁠Detección de oportunidades de crecimiento y retención

---

## 📁 Datasets utilizados

El análisis se basa en dos conjuntos de datos:

### 👥 ⁠ users ⁠

Contiene información demográfica y de estado del cliente:

•⁠  ⁠⁠ user_id ⁠: identificador único
•⁠  ⁠⁠ age ⁠: edad del usuario
•⁠  ⁠⁠ city ⁠: ciudad
•⁠  ⁠⁠ reg_date ⁠: fecha de registro
•⁠  ⁠⁠ churn_date ⁠: fecha de cancelación (si aplica)

---

### 📱 ⁠ usage ⁠

Contiene información de uso del servicio:

•⁠  ⁠⁠ user_id ⁠: identificador del usuario
•⁠  ⁠⁠ date ⁠: fecha de actividad
•⁠  ⁠⁠ type ⁠: tipo de uso (llamada o mensaje)
•⁠  ⁠⁠ duration ⁠: duración de llamadas
•⁠  ⁠⁠ length ⁠: longitud de mensajes

---

## 🔍 Etapas del análisis

El proyecto se desarrolló en las siguientes fases:

### 1. 🧹 Limpieza de datos

•⁠  ⁠Identificación y tratamiento de valores inválidos (ej: ⁠ -999 ⁠, ⁠ "?" ⁠)
•⁠  ⁠Manejo de valores nulos (MAR vs errores reales)
•⁠  ⁠Corrección de fechas inconsistentes

---

### 2. 📊 Análisis exploratorio (EDA)

•⁠  ⁠Distribuciones de:

  * edad
  * cantidad de mensajes
  * cantidad de llamadas
  * minutos de llamadas
•⁠  ⁠Visualización mediante histogramas y boxplots

---

### 3. ⚠️ Detección de outliers

•⁠  ⁠Cálculo de límites con IQR
•⁠  ⁠Identificación de valores extremos
•⁠  ⁠Decisión de:

  * mantener outliers (usuarios reales)
  * tratar variables críticas (winsorización)

---

### 4. 👥 Segmentación de clientes

•⁠  ⁠Por edad:

  * Jóvenes
  * Adultos
  * Adultos mayores

•⁠  ⁠Por nivel de uso:

  * Bajo
  * Medio
  * Alto

---

### 5. 🧠 Análisis de patrones

•⁠  ⁠Identificación de:

  * usuarios intensivos (power users)
  * comportamiento típico
  * diferencias entre segmentos

---

### 6. 🚀 Generación de insights

•⁠  ⁠Detección de segmentos de alto valor
•⁠  ⁠Identificación de oportunidades de negocio
•⁠  ⁠Recomendaciones de:

  * nuevos planes
  * estrategias de pricing
  * retención y crecimiento

---

## ▶️ Cómo ejecutar el notebook

Puedes ejecutar este proyecto de la siguiente forma:

### 🔹 Google Colab 

1.⁠ ⁠Abre Google Colab: https://colab.research.google.com
2.⁠ ⁠Sube el notebook (⁠ .ipynb ⁠) o ábrelo desde GitHub
3.⁠ ⁠Ejecuta las celdas en orden

---


## 🔁 Guía de reproducción

Para reproducir el análisis:

1.⁠ ⁠Cargar los datasets (⁠ users ⁠ y ⁠ usage ⁠)
2.⁠ ⁠Ejecutar el preprocesamiento:

   * limpieza de datos
   * tratamiento de nulos
3.⁠ ⁠Ejecutar el análisis exploratorio:

   * histogramas
   * boxplots
4.⁠ ⁠Calcular outliers usando IQR
5.⁠ ⁠Crear variables de segmentación:

   * grupos de edad
   * niveles de uso
6.⁠ ⁠Analizar patrones y generar insights

---

## 🧠 Principales conclusiones

•⁠  ⁠La mayoría de usuarios presenta un uso moderado
•⁠  ⁠Existe un segmento pequeño pero clave de *usuarios intensivos*
•⁠  ⁠Los minutos de llamada son la variable más relevante para consumo
•⁠  ⁠Los outliers representan comportamiento real, no errores

---

## 🚀 Recomendaciones

•⁠  ⁠Diseñar planes diferenciados por segmento
•⁠  ⁠Implementar pricing basado en consumo
•⁠  ⁠Priorizar retención de usuarios intensivos
•⁠  ⁠Desarrollar ofertas específicas para usuarios jóvenes
