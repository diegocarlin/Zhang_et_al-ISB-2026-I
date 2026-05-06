## Artículo
**A Wearable Multimodal Sensing System for Tracking Changes in Pulmonary Fluid Status, Lung Sounds, and Respiratory Markers**

---

## Objetivo
El objetivo principal de este trabajo es presentar y evaluar la viabilidad de un **sistema de detección multimodal portátil**. Este dispositivo está diseñado para el monitoreo continuo y holístico del estado cardiopulmonar, específicamente en pacientes con **insuficiencia cardíaca**.

---

## Tipos de Filtros Utilizados
El artículo emplea principalmente filtros de respuesta finita al impulso (FIR) para el procesamiento de las señales. A continuación, se detallan los filtros mencionados:

### 1. Filtro Pasa-banda
*   Se aplica para sonidos pulmonares (100 Hz a 1000 Hz) el articulo especifica que se usa un filtro para aislar las frecuencias de interés, suprimiendo la interferencia de sonidos cardíacos por debajo de 100Hz y ruidos ambientales del hospital por encima de 1000 Hz

### 2. Filtro FIR con Ventana Kaiser
*   **Aplicación:** Señal de neumografía de impedancia.
*   **Rango:** 0.1 Hz a 0.8 Hz.
*   **Función:** Capturar una tasa respiratoria fisiológicamente plausible (entre 6 y 48 respiraciones por minuto).
*   **Referencia Visual (Figura 2):** 
    *   Este filtro actúa como el punto de entrada que limpia la señal.
    *   Permite que el bloque *"Detect Breaths"* identifique con precisión los valles o inicios de cada respiración.
    *   **Importancia:** Evita fallos en el algoritmo de detección causados por la inestabilidad de la línea base o el ruido superpuesto.

### 3. Filtro Antialiasing
*   **Aplicación:** Previo al remuestreo de las señales.
*   **Función:** Evitar el solapamiento de frecuencias (aliasing) durante el procesamiento digital.

### 4. Filtro de Fase Cero
*   **Aplicación:** Sonidos pulmonares.
*   **Función:** Procesar la señal sin introducir distorsiones de fase.
*   **Importancia:** Crucial para mantener la morfología original de la señal, asegurando que los datos analizados sean una representación fiel de la actividad pulmonar.
