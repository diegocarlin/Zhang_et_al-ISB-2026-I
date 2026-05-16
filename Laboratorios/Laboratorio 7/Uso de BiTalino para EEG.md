# Laboratorio de Adquisición de Señales EEG con BITalino

## 1. Metodología

### 1.1. Materiales y Equipos
Para la adquisición de las señales electroencefalográficas (EEG) se emplearon los siguientes recursos:
* **Hardware:** Módulo BITalino (r)evolution Board Kit con conexión Bluetooth.
* **Sensores:** 3 electrodos superficiales desechables de Ag/AgCl con gel conductor.
* **Software:** OpenSignals (r)evolution (para la visualización y registro en tiempo real).
* **Accesorios adicionales:** Audífonos de aislamiento acústico pasivo (estrictamente sin tecnología de cancelación activa de ruido, para evitar interferencias electromagnéticas en la señal), una prenda (polo) para oclusión visual y un dispositivo de reproducción de audio.

### 1.2. Preparación del Sujeto y Posicionamiento de Electrodos
Previo al inicio de las mediciones, se preparó la piel del participante para garantizar una baja impedancia en la interfaz electrodo-piel:
1.  **Electrodos de Medición (IN+ e IN-):** Se colocaron dos electrodos en la región frontal del sujeto (posiciones aproximadas a **Fp1** y **Fp2**).
2.  **Electrodo de Referencia (REF):** Se ubicó en la región retroauricular, específicamente sobre la apófisis mastoides (detrás de la oreja).

Una vez adheridos, los electrodos se conectaron a los terminales del BiTalino, vinculando el dispositivo vía Bluetooth a la computadora para visualizar la señal en la interfaz de OpenSignals.

### 1.3. Protocolo de Adquisición de Datos
El registro de la señal EEG se dividió en seis fases continuas, diseñadas para evaluar la actividad cerebral ante diferentes estímulos y aislar los artefactos fisiológicos. El sujeto fue ubicado en un entorno aislado y libre de contacto con superficies vibratorias para mitigar el ruido mecánico.

* **Fase 1: Línea Basal con Privación Sensorial (1 minuto)**
    Se buscó registrar la actividad cerebral en el estado más neutro posible (predominancia esperada de ritmos Alfa).Para ello, el participante se colocó los audífonos para aislar el sonido externo de forma puramente pasiva, se cubrió la vista completamente con un polo y se le indicó mantener una postura estática, evitando cualquier movimiento facial. Además se apagaron las luces del salón y se procuraba hablar en un tono de voz bajo para evitar el menor número de estimulaciones posible.

https://github.com/user-attachments/assets/ba2e23e3-fee6-4d0a-800b-c7fae714dbc6


* **Fase 2: Apertura Ocular y Fijación Visual (1 a 1.5 minutos)**
    Se retiró la oclusión visual. El sujeto abrió los ojos y mantuvo la mirada fija en un punto específico frente a él, con el objetivo de observar la atenuación del ritmo Alfa y la transición hacia el ritmo Beta.
* **Fase 3: Recuperación de Línea Basal (30 segundos)**
    El sujeto retomó las condiciones de la Fase 1(ojos cerrados y aislamiento sonoro)para restablecer la señal a su estado basal.
* **Fase 4: Inducción de Artefactos (30 segundos)**
    Se le solicitó al participante realizar movimientos faciales controlados para registrar la interferencia electromiográfica (EMG) y electrooculográfica (EOG) sobre el EEG. El protocolo consistió en parpadear de manera exagerada cada 2 segundos y realizar movimientos de masticación continuo.
* **Fase 5: Segunda Recuperación Basal (30 segundos)**
    Nuevamente, el sujeto regresó al estado de relajación total con los ojos cerrados para estabilizar la señal post artefactos.
* **Fase 6: Protocolo de Diseño Libre (Cognitivo y Auditivo)**
    Se evaluó la modulación de las ondas cerebrales ante carga cognitiva y estímulos emocionales sonoros. Esta fase se subdividió en cuatro etapas, con la instrucción estricta de **no vocalizar ni hablar** en ningún momento para evitar contaminación por ruido muscular (EMG):
    1.  **Carga Cognitiva Simple (20 segundos):** Se le plantearon tres preguntas matemáticas/lógicas sencillas en voz baja. El sujeto las resolvió mentalmente.
    2.  **Carga Cognitiva Compleja (20 segundos):** Se le plantearon tres preguntas de mayor dificultad analítica, resolviéndolas también de forma exclusivamente mental.
    3.  **Estímulo Auditivo Relajante (1 minuto):** Se reprodujo una pista musical con una melodía rítmica, suave y constante.
    4.  **Estímulo Auditivo Estresante (1 minuto):** Se cambió a una pista musical caótica, densa y con múltiples instrumentos superpuestos para evaluar los cambios en la actividad cerebral ante estrés acústico.

## 2. Registro Fotográfico y Audiovisual
**Colocación de los electrodos para EEG en la frente
<img width="1200" height="1600" alt="6dd7f591-f8f1-4d76-abe2-727578f20378" src="https://github.com/user-attachments/assets/072b77f8-53b9-4cfa-a081-372777ed394e" />
**Toma de la señal basal
<img width="1200" height="1600" alt="176af3bb-8c24-49e5-8c65-b49d9010ad2b" src="https://github.com/user-attachments/assets/7a975b13-7927-4d7c-bd79-cfc6fd35e362" />
**Mirar a un punto fijo (parte superior de la botella)
<img width="1200" height="1600" alt="f46bc9ea-8f44-4438-8d72-2d5aa71a88e8" src="https://github.com/user-attachments/assets/c7b65fbd-7fd5-46fd-af5a-d9624a3b201c" />
https://github.com/user-attachments/assets/ccd4e420-aa25-4d37-9421-2466a58a2533
**Parpadeo y masticación al mismo tiempo para instroducir artefactos a la señal
<img width="1200" height="1600" alt="8ca64ae7-a8e3-485d-9119-ac9d5827b709" src="https://github.com/user-attachments/assets/289cb435-e074-4d34-a433-0abf8b3bd3b6" />
https://github.com/user-attachments/assets/63f8198b-ca66-4fcb-93f2-448bb02d0c3d
**Carga cognitiva simple
https://github.com/user-attachments/assets/6c3c8f59-f2f5-4690-9470-78111f866208
**Carga cognitiva compleja
https://github.com/user-attachments/assets/48c3e65f-57c3-4521-84bc-708396b41eb1
**Estímulo auditivo relajante
https://github.com/user-attachments/assets/c3692684-2ea0-470e-94db-d687b33352b5
**Estímulo auditivo estresante
https://github.com/user-attachments/assets/22c315e5-5c30-4a24-a6e8-971ae2248be3
<img width="1200" height="1600" alt="ef708ae6-6eba-4b84-b850-8175cf871f68" src="https://github.com/user-attachments/assets/a7d90e3b-ee98-4db7-97fd-151a9e7f45ff" />

## 3. Ploteo de Señales en OpenSignals

A continuación se presentan las gráficas obtenidas directamente de la interfaz de OpenSignals para las diferentes pruebas realizadas.



## 4. Análisis de la Señal


## 5. Datos y Procesamiento en Python

### 5.1. Archivos de Datos Crudos



### 5.2. Código de Ploteo

