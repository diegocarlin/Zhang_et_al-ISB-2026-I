# Zhang_et_al-ISB-2026-I
Repositorio perteneciente al grupo 3 de Introducción a Señales Biomédicas

# Análisis Neuromuscular del Control Postural: Y-Balance Test + EMG

## 📝 Descripción
Este proyecto integra el **Y-Balance Test** con **Electromiografía de Superficie (sEMG)** para evaluar la estabilidad dinámica en estudiantes universitarios (18-25 años). El enfoque principal es analizar el **Índice de Co-activación (CCI)** para descubrir las estrategias neuromusculares ocultas tras el rendimiento físico observable y mitigar el riesgo de lesiones por sedentarismo.

## 🎯 Objetivo
Identificar si diferentes perfiles corporales (**delgado, sobrepeso y atlético**) utilizan estrategias de activación muscular distintas para lograr el equilibrio, permitiendo fundamentar programas de **fisioterapia preventiva personalizada**.

## ⚙️ Metodología
El flujo de trabajo técnico se divide en tres fases críticas:

1.  **Captura Biomecánica:** 
    *   Ejecución del Y-Balance Test.
    *   Registro simultáneo de 8 músculos de la extremidad inferior.
2.  **Procesamiento de Señal (DSP):** 
    *   **Filtrado:** Eliminación de artefactos de movimiento y ruido de red (60 Hz).
    *   **Métricas:** Cálculo de amplitud (**RMS**) y **Frecuencia Mediana**.
3.  **Análisis Funcional:** 
    *   Cálculo del **CCI** entre pares agonista-antagonista.
    *   Diferenciación entre eficiencia neuromuscular vs. rigidez articular.

## 👥 Integrantes

| Nombre                 | Rol                          |
|----------------------|------------------------------|
| Rodrigo Zubiate      | Líder de proyecto            |
| Juan Raúl Ramírez    | Procesamiento de señales     |
| Diego Carlín         | Desarrollo de algoritmos     |
| David Aguilar        | Análisis de datos            |
| Davidt Fernández     | Documentación y testing      |
