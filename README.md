# Zhang_et_al-ISB-2026-I
Repositorio perteneciente al grupo 3 de Introducción a Señales Biomédicas
🫀 Detección de Arritmias en Señales ECG

Proyecto de nivel intermedio para el curso de Introducción a Señales Biomédicas, enfocado en el procesamiento y clasificación de señales ECG.

📌 Descripción

Se desarrolla un sistema básico para analizar señales electrocardiográficas (ECG) con el fin de detectar arritmias. El flujo incluye filtrado, detección de complejos QRS, extracción de características y clasificación de latidos.

🎯 Objetivo

Implementar un algoritmo que permita identificar latidos normales y anormales a partir de señales ECG.

🧠 Metodología
Preprocesamiento: filtrado pasa banda (0.5–40 Hz)
Detección QRS: algoritmo de Pan-Tompkins
Características: intervalo RR, duración QRS, amplitud
Clasificación: modelos básicos como KNN o SVM
💻 Implementación

Herramientas:

Python, NumPy, SciPy
Matplotlib, Scikit-learn, WFDB

Dataset recomendado:

MIT-BIH Arrhythmia Database
https://physionet.org/content/mitdb/
▶️ Uso
git clone https://github.com/tuusuario/ecg-arrhythmia-detection.git
cd ecg-arrhythmia-detection
pip install -r requirements.txt
python main.py
📊 Resultados

Se espera detectar correctamente picos R y clasificar arritmias básicas, evaluando con métricas como accuracy y recall.

📚 Referencias
Pan & Tompkins (1985) – QRS Detection
PhysioNet – MIT-BIH Database
Clifford et al. (2006) – ECG Analysis
Acharya et al. (2017) – Deep Learning en ECG
🚀 Mejora futura

Extender a modelos de deep learning y clasificación multiclase.
## 👥 Integrantes

| Nombre                 | Rol                          |
|----------------------|------------------------------|
| Rodrigo Zubiate      | Líder de proyecto            |
| Juan Raúl Ramírez    | Procesamiento de señales     |
| Diego Carlín         | Desarrollo de algoritmos     |
| David Aguilar        | Análisis de datos            |
| Davidt Fernández     | Documentación y testing      |
