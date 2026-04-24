# Laboratorio de Adquisición de Señales EMG con BITalino


## 

## 1\. Metodología

Para garantizar una correcta adquisición de las señales y minimizar la introducción de ruido o artefactos, se establecieron las siguientes consideraciones y pasos durante la práctica:

### 1.1. Preparación del Sujeto y Colocación de Electrodos

* **Selección del sujeto:** Se escogió al integrante del grupo con menor densidad de vello en brazos y piernas para asegurar una mejor adherencia y conductividad de los electrodos.
* **Zonas de colocación:** Se evitaron las superficies con pelo y se ubicaron los electrodos en zonas distantes a las prominencias óseas para captar correctamente la señal EMG del vientre muscular.
* **Reutilización:** Se utilizaron dos electrodos de registro en el bíceps. Tras finalizar las pruebas en el brazo, estos mismos electrodos se retiraron y se reubicaron en la parte lateral del muslo. En todo momento se tuvo en cuenta que una vez colocado el electrodo para la prueba de un músculo específico, no se retiró ni reacomodó hasta finalizar todas las mediciones de esa zona.

### 1.2. Consideraciones Técnicas y de Entorno

* **Prevención de ruido:** Se mantuvo estricto cuidado con el movimiento del dispositivo BITalino y, en particular, de los cables. El movimiento de estos componentes es la principal fuente de ruido (artefactos por movimiento) que posteriormente dificultaría el filtrado de la señal.
* **Registro audiovisual:** Se grabó en video gran parte del procedimiento práctico. Esto sirve como registro audiovisual de las conexiones y como respaldo para correlacionar los movimientos físicos con la señal ploteada en caso de requerir depuración.

### 1.3. Protocolo de Medición

Cada evaluación tuvo una duración aproximada de **1 a 2 minutos** (fijado en 2 minutos para la estandarización final) y se dividió estrictamente en dos fases para cada músculo:

1. **Lectura Basal:** Toda evaluación inició obligatoriamente con una toma en silencio eléctrico (reposo total) para establecer la línea base.
2. **Lectura en Movimiento:** Posteriormente, se realizaron las contracciones correspondientes.
3. **Gestión de archivos:** Cada intento se guardó con un nombre distinto desde el software OpenSignals para diferenciar claramente los registros de reposo y movimiento de cada músculo .





## 2\. Registro Fotográfico y Audiovisual

### 2.1. Foto de conexión de electrodos en el cuerpo
<img width="968" height="577" alt="image" src="https://github.com/user-attachments/assets/82d93c61-779b-4aa5-ac4a-9b775bdc7aa9" />

### 2.2. Videos de la captura de datos
#### 2.2.1. Brazo en reposo
https://github.com/user-attachments/assets/c62726f7-ccb3-4288-a3a7-ccb89e7e1dfd

#### 2.2.2. Brazo en movimiento
https://github.com/user-attachments/assets/7661854a-ba69-45cd-9433-009c79ba6adf

#### 2.2.3. Muslo de la pierna en reposo
https://github.com/user-attachments/assets/33a9fd27-58cd-4c31-b671-2cd659c594ef

#### 2.2.4. Muslo de la pierna en movimiento
https://github.com/user-attachments/assets/4b288360-fcaa-4296-919c-e694e9ca580f


## 3\. Ploteo de Señales en OpenSignals

A continuación se presentan las gráficas obtenidas directamente de la interfaz de OpenSignals para cada una de las pruebas.

### 3.1. Pruebas en el Bíceps

* **Reposo:**
<img width="1200" height="400" alt="Brazo_reposo" src="https://github.com/user-attachments/assets/c5fd8ce4-100f-41e8-b2c7-ea2afbafd99a" />


* **Movimiento:**
<img width="1200" height="400" alt="Brazo" src="https://github.com/user-attachments/assets/eb2791fd-3bee-4435-91f7-86ae2e5e1508" />


### 3.2. Pruebas en el Muslo (Vasto Lateral)

* **Reposo:**
<img width="1200" height="400" alt="Pierna_reposo" src="https://github.com/user-attachments/assets/9742b89e-ded2-41a7-aa5f-fdd829c2124c" />

* **Movimiento:**
<img width="1200" height="400" alt="Pierna" src="https://github.com/user-attachments/assets/ce386f9e-7619-4416-a72b-51dfa0dbb4f2" />




## 4\. Análisis de la Señal

### 4.1. Señal del Brazo en reposo

La señal presenta una amplitud muy baja (cercana a 0 mV), viéndose casi plana. Esto se debe a que el músculo del brazo no realiza ningún tipo de movimiento durante la medición, lo que genera que no haya cambios de amplitud y frecuencia en la señal, y que sea el ruido electrónico del sistema lo que el BITalino llegue a medir. 

### 4.2. Señal del Brazo en movimiento

La señal muestra cambios notorios en la amplitud (cercana a +/- 1.5 V) en forma de picos, aunque se notan patrones irregulares entre éstos, porque se observan picos con amplitudes muy distintas entre etras, junto con un mayor ruido en la señal. Estas irregularidades pueden deberse a las contracciones medidas, ya que se realizaron con distintas intensidades, resultando en que la señal presente distintas amplitudes y frecuencias.

### 4.3. Señal del Muslo en reposo

Similar a la primera señal, esta señal presenta una amplitud muy baja (cercana a 0 mV), porque el muslo no realiza ningún tipo de movimiento durante la medición, evitando cambios de amplitud y frecuencia en la señal, y que el BITalino solo mida ruido electrónico. 

### 4.4. Señal del Muslo en movimiento

La señal muestra cambios notorios en la amplitud (cercana a +/- 1.5 V) en forma de picos, con patrones más periódicos o repetitivos, porque la amplitud se mantiene casi constante. Estos picos repetitivos son causados por las contracciones del muslo, las cualees fueron más coordinadas entre sí, generando amplitudes y frecuencias similares durante cada pico. 





## 5\. Datos y Procesamiento en Python

### 5.1. Archivos de Datos Crudos

Los datos exportados por OpenSignals que se utilizaron para el análisis son:

* `Prueba\\\_en\\\_reposo\\\_brazo.txt`
* `Prueba\\\_en\\\_brazo.txt`
* `Prueba\\\_en\\\_reposo\\\_pierna.txt`
* `Prueba\\\_en\\\_pierna.txt`

### 5.2. Código de Ploteo

Para la visualización de los datos mediante programación, se utilizó la librería `opensignalsreader`. El script ejecuta la lectura y ploteo de los archivos `.txt` generados.



**Script utilizado:**

\# Ejecutar este comando en la ventana de comandos para poder visualizar el ploteo de la señal EMG: pip install opensignalsreader

\# Import OpenSignalsReader

from opensignalsreader import OpenSignalsReader



\# Read OpenSignals file

acq = OpenSignalsReader('Prueba\_en\_reposo\_brazo.txt')

acq = OpenSignalsReader('Prueba\_en\_brazo.txt')

acq = OpenSignalsReader('Prueba\_en\_reposo\_pierna.txt')

acq = OpenSignalsReader('Prueba\_en\_pierna.txt')

\# Read OpenSignals file and plot all signals

acq = OpenSignalsReader('Prueba\_en\_reposo\_brazo.txt', show=True)

acq = OpenSignalsReader('Prueba\_en\_brazo.txt', show=True)

acq = OpenSignalsReader('Prueba\_en\_reposo\_pierna.txt', show=True)

acq = OpenSignalsReader('Prueba\_en\_pierna.txt', show=True)

