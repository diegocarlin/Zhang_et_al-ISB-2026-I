<div align="justify">
  
## Artículo 1
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
*   Este filtro se aplica a la señal de neumografía de impedancia para capturar una tasa respiratoria fisiológicamente plausible de entre 6 y 48 respiraciones por minuto en los rangos de 0.1 Hz a 0.8 Hz. 
*   **Referencia Visual (Figura 2):**
*   <img width="888" height="509" alt="image" src="https://github.com/user-attachments/assets/9bea192c-3ea6-4254-aab8-175f9be3762f" />

*   En el diagrama, este filtro es el punto de entrada que limpia la señal para que el siguiente bloque "Detect Breaths" pueda identificar con precisión los valles o inicios de cada respiración. Sin este filtrado específico, el algoritmo de detección de respiraciones fallaría debido a la inestabilidad de la línea base o al ruido superpuesto.

### 3. Filtro Antialiasing
*   Utilizado antes del remuestreo de las señales para evitar el solapamiento de frecuencias..

### 4. Filtro de Fase Cero
*   El artículo menciona explícitamente el uso de un filtro de fase cero para los sonidos pulmonares, esto es fundamental en el procesamiento ya que evita distorsiones de fase que podrían alterar la morfología de la señal original.


## Artículo 2
**Title**

## Referencias bibliográficas
**J. A. Sanchez-Perez et al., "A Wearable Multimodal Sensing System for Tracking Changes in Pulmonary Fluid Status, Lung Sounds, and Respiratory Markers," Sensors, vol. 22, no. 3, p. 1130, feb. 2022. doi: 10.3390/s22031130.**
</div>
