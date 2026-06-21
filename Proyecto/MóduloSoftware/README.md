El sistema recopila variables ambientales en tiempo real, procesa los datos localmente y los transmite para su visualización remota.



\---



\## 🛠️ Hardware y Pinout



\### Componentes Principales

\* \*\*Microcontrolador\*\* compatible con Arduino IoT Cloud.

\* \*\*SparkFun Weather Meter Kit\*\* (Anemómetro, Veleta y Pluviómetro).

\* \*\*Sensor BME280\*\* (Temperatura, Humedad y Presión).

\* \*\*Sensor VEML6075\*\* (Luz UVA, UVB e Índice UV).

\* \*\*Sensor AS3935\*\* (Detección de Rayos y Tormentas).

\* \*\*Sensor Higrómetro\*\* (Humedad del Suelo).



\### Asignación de Pines

| Componente / Función | Pin Digital/Analógico |

| :--- | :--- |

| \*\*Dirección del Viento (Veleta)\*\* | Pin 35 |

| \*\*Velocidad del Viento (Anemómetro)\*\* | Pin 14 |

| \*\*Pluviómetro (Lluvia)\*\* | Pin 27 |

| \*\*Interrupción AS3935 (Rayos)\*\* | Pin 17 |

| \*\*Chip Select (CS) AS3935\*\* | Pin 25 |

| \*\*Señal de Humedad de Suelo\*\* | Pin 34 |

| \*\*Alimentación Humedad de Suelo\*\* | Pin 15 |



\---



\## 💻 Configuración del Software



\### Librerías Requeridas

\* `Wire.h` y `SPI.h` (Comunicación nativa).

\* `SparkFun\_Weather\_Meter\_Kit\_Arduino\_Library.h`.

\* `SparkFunBME280.h`.

\* `SparkFun\_VEML6075\_Arduino\_Library.h`.

\* `SparkFun\_AS3935.h`.



