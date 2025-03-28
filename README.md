# Se-alesEMG-Fatiga
En el siguiente repositorio se mostrará una adquisición de señal electromiográfica (EMG) del músculo de un usuario el cual está realizando una contracción muscular hasta la fatiga, se aplicará un filtrado usando un filto pasa altas y un filtro pasa bajas.
El repositorio cuenta con el código, la documentación, implementación y diseño de un filtro Butterworth, el cuál recibe y filtra las señales del dispositivo AD8232.

## Descripción del Proyecto

El **AD8232** es un bloque integrado especializado para el monitoreo de señales biológicas como el ECG, diseñado para extraer, amplificar y filtrar señales de baja amplitud. Para mejorar la calidad de las señales y eliminar el ruido, se utiliza un filtro Butterworth que se ajusta de pasabanda a pasabajo. En esta implementación, se permite inicialmente el paso de señales dentro de un rango de frecuencias (filtro pasabanda), pero se ajusta para permitir solo el paso de frecuencias bajas (filtro pasabajo), eliminando así las frecuencias más altas no deseadas.

## Adquisición de la señal EMG
La señal se adquirió principalmente de tres músculos: el flexor ulnar del carpo, el flexor radial del carpo y el flexor profundo de los dedos. A continuación, se detallará la ubicación de los electrodos como la señal adquirida originalmente sin filtros:

<img src="https://github.com/user-attachments/assets/a4c3d7df-bed1-4b32-b198-4145f54d3630" width="700" alt="Imagen 2" style="display: inline-block;"/>

-<img src="https://github.com/user-attachments/assets/cf881c67-99cb-4407-b10a-79112734a435" width="200" alt="Imagen 1" style="display: inline-block;"/>

La señal original capturada presenta las siguientes características:
- *Frecuencia de muestreo*: 3000 Hz
- *Tiempo de muestreo*: 333.33 µs. Este valor se calculó a partir de la siguiente fórmula:
