<div align="justify">
  
## Artículo 1 
**A Wearable Multimodal Sensing System for Tracking Changes in Pulmonary Fluid Status, Lung Sounds, and Respiratory Markers [1]**

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

*   En el diagrama, este filtro es el punto de entrada que limpia la señal para que el siguiente bloque "Detect Breaths" pueda identificar con precisión los valles o inicios de cada respiración. Sin este filtrado específico, el algoritmo de detección de respiraciones fallaría debido a la inestabilidad de la linea base o al ruido superpuesto.

### 3. Filtro Antialiasing
*   Utilizado antes del remuestreo de las señales para evitar el solapamiento de frecuencias..

### 4. Filtro de Fase Cero
*   El artículo menciona explícitamente el uso de un filtro de fase cero para los sonidos pulmonares, esto es fundamental en el procesamiento ya que evita distorsiones de fase que podrían alterar la morfología de la señal original.


## Artículo 2
**Diagnosis of insomnia sleep disorder using short time frequency analysis of PSD approach applied on EEG signal using channel ROC-LOC [2]**

---

## Objetivo
El objetivo principal de este trabajo es desarrollar y evaluar un método para diagnosticar el insomnio usando señales del EEG analizadas mediante el análisis de frecuencia de tiempo reducido y la densidad espectral de potencia (PSD), enfocándose principalmente en el canal ROC-LOC de EEG**.

---

## Filtro Utilizado
El artículo menciona que se realiza una etapa de preprocesamiento de las señales adquiridas antes de ser analizadas en distintas bandas de frecuencia, el filtro de preprocesamiento que se usó es el siguiente:

### Filtro FIR Pasa-baja con ventana Hanning
*   Se usó este filtro con la finalidad de eliminar 2 principales tipos de ruidos: el ruido eléctrico que aparece en altos valores de frecuencia y los artefactos causados por el movimiento corporal durante la etapa de sueño. Por ello, este filtro usa una frecuencia de corte de 25 Hz, asegurando la atenuación de altas frecuencias causadas por ruido, y permitiendo enfocarse en las frecuencias del EEG que mejor resaltan la actividad del sueño.

## Artículo 3
**Design of Simulink Model to denoise ECG signal using various IIR & FIR filters [3]**

---

## Objetivo
El objetivo principal de este artículo es el diseño y la implementación de modelos de simulación para eliminar el ruido de las señales de electrocardiograma (ECG) utilizando diversas técnicas de filtrado digital. El estudio busca identificar qué configuración de filtros (FIR vs. IIR) y qué tipos de ventanas (Hamming, Kaiser, etc.) ofrecen la mejor relación señal-ruido (SNR) para obtener un diagnóstico clínico preciso sin distorsionar la morfología del complejo QRS.

---

## Tipos de Filtros Utilizados
El estudio detalla el uso de los siguientes filtros, los cuales son fundamentales en el procesamiento de señales biomédicas:

### 1. Filtro Notch (Rechaza-banda) IIR
* **Ruido que elimina:** Interferencia de la red eléctrica (Power Line Interference - PLI).
* **Frecuencia del ruido:** Se sintoniza exactamente a **50 Hz o 60 Hz**. Es un ruido provocado por el acoplamiento electromagnético de los cables de alimentación del entorno hospitalario y los equipos de monitoreo cercanos.

### 2. Filtro Pasa-alto FIR (Método de enventanado)
* **Ruido que elimina:** Fluctuación de la línea base (Baseline Wander).
* **Frecuencia del ruido:** Ruido de muy baja frecuencia, generalmente entre **0.05 Hz y 0.8 Hz**. Este ruido es causado por la mecánica de la respiración del paciente, el movimiento del cuerpo y las variaciones en la impedancia de la interfaz electrodo-piel.

### 3. Filtro Pasa-bajo IIR Butterworth
* **Ruido que elimina:** Ruido electromiográfico (EMG) y ruido térmico de alta frecuencia.
* **Frecuencia del ruido:** Frecuencias por encima de los **100 Hz**. Proviene de la actividad eléctrica de los músculos esqueléticos cercanos al corazón. Se utiliza la aproximación Butterworth porque ofrece una banda de paso máximamente plana, evitando oscilaciones artificiales en la señal.

### 4. Filtro FIR con Ventana de Kaiser
* **Ruido que elimina:** Ruido de instrumentación y ruido de banda ancha.
* **Frecuencia del ruido:** Elimina componentes fuera de la banda diagnóstica (típicamente **>150 Hz**). La ventana de Kaiser permite un ajuste fino entre el ancho del lóbulo principal y la atenuación de los lóbulos laterales, optimizando el rechazo del ruido sin perder nitidez en la señal.

### 5. Filtro Pasa-banda FIR
* **Ruido que elimina:** Artefactos simultáneos fuera de la banda de interés clínica del ECG.
* **Frecuencia del ruido:** Se configura para dejar pasar exclusivamente el rango de **0.5 Hz a 45 Hz** (banda diagnóstica estándar), atenuando todo lo que esté por debajo (Baseline Wander) y por encima (ruido muscular) en una sola etapa de filtrado.

---
## Artículo 4
**Performance Analysis of Digital Notch Filters for Eliminating Power Line Interference from EMG Signals [4]**

---
## Objetivo
El objetivo principal de este trabajo es evaluar el desempeño de diferentes configuraciones de filtros Notch (Rechaza-banda) para la eliminación de la interferencia de la línea eléctrica (PLI) en señales de electromiografía de superficie (sEMG). El estudio busca mitigar el ruido ambiental sin comprometer la integridad de la información espectral de la contracción muscular.
## Artículo 5

---
## Filtro Utilizado
El artículo destaca el uso de filtros digitales específicos para la limpieza de la señal muscular:

### Filtro Notch IIR (Infinite Impulse Response)
* **Ruido que elimina: Interferencia de la red eléctrica (Power Line Interference - PLI).

* **Frecuencia del ruido: Se sintoniza específicamente a 50 Hz (o 60 Hz dependiendo de la región). Este ruido es particularmente crítico en EMG porque el espectro de potencia de la señal muscular útil se solapa significativamente con esta frecuencia (el rango de la señal EMG suele estar entre 20 Hz y 500 Hz).

* **Sustento Técnico: Se prefiere el uso de un filtro Notch de segundo orden debido a su alta selectividad (factor Q elevado). Esto permite crear una "muesca" muy estrecha en la respuesta en frecuencia, eliminando el armónico de la red eléctrica mientras se preservan las frecuencias adyacentes que contienen información sobre el reclutamiento de unidades motoras. El artículo menciona que, a diferencia de los filtros FIR, los IIR logran esta selectividad con un orden computacional mucho menor, lo que facilita el procesamiento en tiempo real.
**Title**

## Referencias bibliográficas
**[1] J. A. Sanchez-Perez et al., "A Wearable Multimodal Sensing System for Tracking Changes in Pulmonary Fluid Status, Lung Sounds, and Respiratory Markers," Sensors, vol. 22, no. 3, p. 1130, feb. 2022. doi: 10.3390/s22031130.**

**[2] M. M. Siddiqui, G. Srivastava, and S. H. Saeed, “Diagnosis of insomnia sleep disorder using short time frequency analysis of PSD approach applied on EEG signal using channel ROC-LOC,” Sleep Science, vol. 9, no. 3, pp. 186–191, Jul. 2016, doi: 10.1016/j.slsci.2016.07.002.**
</div>
**[3] C. Chandrakar y M. Kowar, "Design of Simulink Model to denoise ECG signal using various IIR & FIR filters," *International Journal of Advanced Research in Computer Science and Software Engineering*, vol. 2, no. 1, 2012.
**[4] A. Kumar and R. P. Tewari, "Performance Analysis of Digital Notch Filters for Eliminating Power Line Interference from EMG Signals," International Journal of Biomedical Engineering and Technology, vol. 14, no. 1, pp. 22-34, 2014.
