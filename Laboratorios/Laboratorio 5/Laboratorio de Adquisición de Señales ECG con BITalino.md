# Laboratorio de Adquisición de Señales ECG con BITalino

## 1. Metodología

Para garantizar una correcta adquisición de las señales de electrocardiograma (ECG) y minimizar la introducción de ruido o artefactos, se establecieron las siguientes consideraciones y pasos durante la práctica.

### 1.1. Preparación del Sujeto y Colocación de Electrodos

*   **Selección del sujeto:** Se escogió al integrante del grupo con menor densidad de vello corporal para asegurar una mejor adherencia y conductividad de los electrodos.
*   **Zonas de colocación:** Se buscaron regiones con baja actividad muscular (huesos) para reducir el ruido de las activaciones musculares (artefactos de movimiento).
*   **Configuración de las Derivaciones de Einthoven:** Se exploraron diferentes posiciones de los electrodos para adquirir señales de ECG correspondientes a las tres derivaciones de Einthoven (I-III).
    *   **Derivación I (Lead I):** Se configuró con el electrodo positivo (IN+) en la clavícula izquierda o muñeca izquierda, el electrodo negativo (IN-) en la clavícula derecha o muñeca derecha, y el electrodo de referencia (REF) en la cresta ilíaca izquierda.
    *   **Derivación II (Lead II):** Se intercambiaron los electrodos positivo y de referencia de la configuración de la Derivación I.
    *   **Derivación III (Lead III):** Se intercambiaron los electrodos negativo y de referencia de la configuración de la Derivación II.
    *   **Reutilización:** Se recomienda cambiar los electrodos de gel por unos nuevos en cada experimento o si se nota que no están en buenas condiciones.

### 1.2. Consideraciones Técnicas y de Entorno

*   **Prevención de ruido:** Se mantuvo un control riguroso sobre los movimientos del sujeto y de los cables del dispositivo BITalino (r)evolution. El movimiento es una fuente crítica de ruido (artefactos de movimiento) que complica el análisis de las señales. Las áreas con baja actividad muscular (huesos) son preferibles.
*   **Registro audiovisual:** Se grabó el procedimiento práctico en video. Esto proporciona un registro visual de la colocación de los electrodos y del estado del sujeto durante diferentes fases del protocolo, facilitando la interpretación posterior de la señal.

### 1.3. Protocolo de Medición

Se ejecutó un protocolo específico utilizando el software OpenSignals (r)evolution, que incluyó varias fases diseñadas para observar el comportamiento de la señal bajo diferentes condiciones:

1.  **Conexión y Prueba:** Se conectó el BITalino (r)evolution Core BT y el Assembled ECG Sensor a uno de los canales analógicos. Se colocaron los electrodos de gel en los sensores y en el cuerpo del sujeto.
2.  **Línea Base Inicial:** Se registró una señal base con bajo ruido y sin movimientos (respiración normal) durante 30 segundos.
3.  **Hiperventilación (Ciclos Respiratorios):** Se repitió un ciclo de INHALACIÓN-RETENCIÓN-EXHALACIÓN-RETENCIÓN tres veces, manteniendo las fases de respiración y descanso durante cinco segundos.
4.  **Segunda Línea Base:** Se registró otra fase base de 30 segundos.
5.  **Actividad Física (Burpees):** El sujeto realizó una rutina de 2.8 minutos de burpees . Se observó la frecuencia cardíaca antes, durante y después del ejercicio.
6.  **Tercera Línea Base:** Se registró una última fase base de 30 segundos.
7.  **Hipoventilación (Respiración Larga):** El sujeto realizó una inhalación profunda y prolongada (aprox. 7 segundos) seguida de una contención de la respiración (aprox. 7 segundos).
8.  **Gestión de Archivos:** Las grabaciones se detuvieron y los datos se guardaron para su posterior análisis. Este procedimiento se repitió para las distintas derivaciones y posiciones de electrodos.

## 2. Registro Fotográfico y Audiovisual

### 2.1. Foto de conexión de electrodos en el cuerpo
<Espacio para imagen de conexión de electrodos>

### 2.2. Videos de la captura de datos
#### 2.2.1. Sujeto en reposo
<Espacio para video en reposo>

#### 2.2.2. Sujeto en hiperventilación
<Espacio para video en hiperventilación>

#### 2.2.3. Sujeto después de actividad física (burpees)
<Espacio para video después de actividad física>

#### 2.2.4. Sujeto en hipoventilación
<Espacio para video en hipoventilación>

## 3. Ploteo de Señales en OpenSignals

A continuación se presentan las gráficas obtenidas directamente de la interfaz de OpenSignals para las diferentes pruebas realizadas.

### 3.1. Señal en Reposo

<Espacio para gráfica en reposo>

### 3.2. Señal en Hiperventilación

<Espacio para gráfica en hiperventilación>

### 3.3. Señal Post-Actividad Física (Burpees)

<Espacio para gráfica post-actividad física>

### 3.4. Señal en Hipoventilación

<Espacio para gráfica en hipoventilación>

## 4. Análisis de la Señal

### 4.1. Análisis de la Señal en Reposo



### 4.2. Análisis de la Señal en Hiperventilación



### 4.3. Análisis de la Señal Post-Actividad Física



### 4.4. Análisis de la Señal en Hipoventilación



## 5. Datos y Procesamiento en Python

### 5.1. Archivos de Datos Crudos

Los datos exportados por OpenSignals que se utilizaron para el análisis son:

*   `Prueba_reposo_D1.txt`
*   `Prueba_reposo_D2.txt`
*   `Prueba_reposo_D3.txt`
*   `Prueba_hiperventilacion_D1.txt`
*   `Prueba_hiperventilacion_D2.txt`
*   `Prueba_hiperventilacion_D3.txt`
*   `Prueba_post_burpees_D1.txt`
*   `Prueba_post_burpees_D2.txt`
*   `Prueba_post_burpees_D3.txt`
*   `Prueba_hipoventilacion_D1.txt`
*   `Prueba_hipoventilacion_D2.txt`
*   `Prueba_hipoventilacion_D3.txt`

### 5.2. Código de Ploteo

Para la visualización de los datos mediante programación, se utilizó la librería `opensignalsreader`.

**Script utilizado:**
```python
# Ejecutar este comando en la ventana de comandos para poder visualizar el ploteo de la señal ECG: pip install opensignalsreader

from opensignalsreader import OpenSignalsReader

# Leer archivos OpenSignals (Ejemplo para Derivación I)
acq_reposo = OpenSignalsReader('Prueba_reposo_D1.txt')
acq_hiper = OpenSignalsReader('Prueba_hiperventilacion_D1.txt')
acq_burpees = OpenSignalsReader('Prueba_post_burpees_D1.txt')
acq_hipo = OpenSignalsReader('Prueba_hipoventilacion_D1.txt')

# Leer archivos OpenSignals y plotear las señales (Ejemplo para Derivación I)
acq_reposo = OpenSignalsReader('Prueba_reposo_D1.txt', show=True)
acq_hiper = OpenSignalsReader('Prueba_hiperventilacion_D1.txt', show=True)
acq_burpees = OpenSignalsReader('Prueba_post_burpees_D1.txt', show=True)
acq_hipo = OpenSignalsReader('Prueba_hipoventilacion_D1.txt', show=True)
