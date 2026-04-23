
# Cuestionario sobre Electromiografía (EMG)

<div align="justify">

### Q1. ¿Cuáles son las frecuencias significativas para las adquisiciones de EMG? ¿Son iguales en todas las áreas del cuerpo, como el área facial?
Las señales de electromiografía suelen tener un rango de frecuencia relevante que oscila entre los 10 Hz y los 500 Hz, concentrándose la mayor parte de la energía capturada entre los 20 Hz y 150 Hz. Por otro lado, las frecuencias no son exactamente iguales en todas las áreas del cuerpo, debido a que los músculos faciales suelen tener unidades motoras más pequeñas y rápidas en comparación con los músculos grandes de las extremidades. Esto desplaza la frecuencia hacia rangos ligeramente más altos en el área facial debido a la velocidad de activación necesaria para expresiones precisas.

### Q2. ¿Qué tipo de filtro es esencial al trabajar con señales de EMG? ¿Por qué necesitamos aplicar dicho filtro?
Es esencial aplicar un Filtro de Banda. Por un parte aplicar el Filtro Pasa-Altos se usa para eliminar el ruido de movimiento y artefactos de baja frecuencia causados por el movimiento de los cables o el contacto de los electrodos, por otro lado, aplicar el Filtro Pasa-Bajos se usa para eliminar el ruido de alta frecuencia y evitar el solapamiento, asi limitar la señal al rango fisiológico útil. 

### Q3. ¿Cómo difiere la amplitud en cada contracción muscular? ¿Existe una diferencia según la ubicación del cuerpo?
La amplitud de la señal EMG está directamente relacionada con la intensidad de la contracción. Es decir, a mayor fuerza o esfuerzo muscular, más unidades motoras se reclutan y disparan a frecuencias más altas, lo que resulta en un aumento de la amplitud de la señal. Por lo tanto, según la ubicación la amplitud va a variar ya que depende del tamaño del músculo, la densidad de fibras musculares, la profundidad del músculo respecto a la piel y la cantidad de tejido adiposo entre el músculo y el electrodo. 

### Q4. Muestre una captura de pantalla de una porción relevante de los datos de electromiografía (EMG) dentro del experimento propuesto en la sección D de un musculo facial ¿Esta señal corresponde a lo que esperaba? ¿Por qué?  ¿Qué emoción y acción realizó para activar el musculo? ¿Qué musculo activo? 
<img width="980" height="745" alt="image" src="https://github.com/user-attachments/assets/a3e1d8a1-492c-4f2a-a08d-bc22c30d7296" />

Para esta práctica, se realizó la adquisición de señales electromiográficas colocando los electrodos en la cara anterior del muslo, posicionándolos en el musculo recto femoral y el sartorio aproximadamente, y para garantizar una señal limpia se utilizó el tarso  como punto de referencia. 

Al observar las capturas de OpenSignals, la señal en reposo muestra una línea de base sumamente estable con una amplitud mínima, esto indica una correcta colocación de los electrodos y un buen contacto con la piel, confirmando que los músculos no presentan una pre-activación significativa. 
En contraste, la señal en movimiento muestra ráfagas de actividad eléctrica de gran amplitud, este cambio drástico es el resultado de realizar la extensión de la pierna, lo cual genera una señal estocástica pero proporcional al esfuerzo realizado.

Por lo tanto, la señal obtenida corresponde exactamente a lo esperado, ya que la acción que disparó esta actividad fue la extensión de la rodilla, movimientos donde el recto femoral actúa como motor principal, por ello los picos de frecuencia y amplitud observados validan que el sensor BITalino capturó con éxito el potencial de acción muscular.


### Q5. Según tus conocimientos, ¿la amplitud de la EMG es igual a la cantidad de fuerza que has generado con tu músculo?
No, la amplitud de la EMG no es una medida directa de la fuerza mecánica generada por el músculo, debido a que la fatiga muscular puede aumentar la amplitud de la EMG incluso si la fuerza producida disminuye, asimismo, el cambio en la longitud del músculo altera la amplitud detectada sin que necesariamente cambie la fuerza. Por último, el grosor del tejido subcutáneo, la posición de los electrodos y la impedancia de la piel influyen en la amplitud registrada sin que la fuerza real cambie. 
</div>
