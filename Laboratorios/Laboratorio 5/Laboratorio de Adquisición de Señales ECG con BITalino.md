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
<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/1a98e9b1-fba5-4f1a-983d-daacd6c750e8" />

### 2.2. Videos de la captura de datos
#### 2.2.1. Sujeto en reposo
https://github.com/user-attachments/assets/b443ec53-4550-473f-a133-59003dc12691

#### 2.2.2. Sujeto en hiperventilación
<Espacio para video en hiperventilación>

#### 2.2.3. Sujeto después de actividad física (burpees)
<Espacio para video después de actividad física>

#### 2.2.4. Sujeto en hipoventilación
<Espacio para video en hipoventilación>

## 3. Ploteo de Señales en OpenSignals

A continuación se presentan las gráficas obtenidas directamente de la interfaz de OpenSignals para las diferentes pruebas realizadas.

### 3.1. Señal en Reposo

<img width="1012" height="411" alt="ECG-I_derivada_basal" src="https://github.com/user-attachments/assets/f8afeb4a-db21-40c3-915e-d4dc19c2de08" />
<img width="1012" height="411" alt="ECG-II_derivada_basal" src="https://github.com/user-attachments/assets/a497dd51-cdca-43ac-9c23-43d0e0d2a799" />
<img width="1012" height="411" alt="ECG-III_derivada_basal" src="https://github.com/user-attachments/assets/c5f50a90-23fe-44da-b0be-9f10e405d49b" />

Aquí se muestran las señales en reposo después de la actividad física (Basal 2):
<img width="1012" height="411" alt="ECG-II_derivada_basal2" src="https://github.com/user-attachments/assets/00e69d23-d50c-4db1-9fc8-3ce657ba6794" />
<img width="1012" height="411" alt="ECG-I_derivada_basal2" src="https://github.com/user-attachments/assets/d892b0a3-12b1-469c-9c22-f4f7e50e6cb8" />

### 3.2. Señal en Hiperventilación

<img width="1012" height="411" alt="ECG-II_derivada_CR" src="https://github.com/user-attachments/assets/d02e763c-03ec-4fac-9394-97626dcf813e" />
<img width="1012" height="411" alt="ECG-I_derivada_CR" src="https://github.com/user-attachments/assets/e9809a28-5981-4663-bded-9cfc1803fc7b" />


### 3.3. Señal Post-Actividad Física (Burpees)

<img width="1012" height="411" alt="Burpee-III_derivada" src="https://github.com/user-attachments/assets/137c74b0-1df1-4d56-8026-86b1f01831ec" />
<img width="1017" height="411" alt="Burpee-I_derivada" src="https://github.com/user-attachments/assets/2606ecb3-6e89-4620-bc4d-b39d0059cc02" />
<img width="1012" height="411" alt="Burpee-II_derivada" src="https://github.com/user-attachments/assets/33acb041-5d76-4ab6-b21d-dd34d678683c" />


### 3.4. Señal en Hipoventilación

<img width="1012" height="411" alt="Hipoventilación_III_derivada" src="https://github.com/user-attachments/assets/b99c4ca3-1c76-4faf-bf85-a0ec78051686" />
<img width="1012" height="411" alt="Hipoventilación_I_derivada" src="https://github.com/user-attachments/assets/8fe540f5-759c-492b-8bad-2eac411ab1c0" />
<img width="1012" height="411" alt="Hipoventilación_II_derivada" src="https://github.com/user-attachments/assets/a0d8efc7-9800-4918-b2c7-7cd910b9b60a" />


## 4. Análisis de la Señal

### 4.1. Análisis de la Señal en Reposo

Al observar las señales capturadas, se identifican las siguientes características clave:
- Derivación I: Presenta la menor amplitud de voltaje (picos R cercanos a 0.2mV). Esto es coherente con la teoría, ya que el vector de despolarización ventricular suele ser casi perpendicular a la línea que une ambos brazos, proyectando una magnitud menor sobre este eje.
- Derivación II: Es la señal más clara y con mayor amplitud, alcanzando picos R de aproximadamente 1.0mV. Esto sucede porque el eje eléctrico del corazón está casi alineado con el vector de esta derivación, lo que la convierte en la mejor opción para identificar ondas P y complejos QRS.
- Derivación III: Muestra una amplitud intermedia (alrededor de 0.8 mV). La señal es nítida, permitiendo una visualización adecuada de la repolarización (onda T), aunque con una relación señal-ruido ligeramente menor que la DII en este registro particular.

### 4.2. Análisis de la Señal en Hiperventilación

- Derivación I: No hubo cambios visibles comparándola con la señal en reposo . Esto ocurre porque esta señal observa el corazón de manera horizontal (los electrodos - y + están ubicados en la clavícula izquierda y la clavícula derecha, respectivamente), por lo que no puede detectar los cambios generados por la hiperventilación, ya que son más notorios en el eje vertical.
- Derivación II: Presenta una menor longitud de sus intervalos R-R y una mayor frecuencia cardiaca, eventos causados por una taquicardia leve producto de una rápida respiración.

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
