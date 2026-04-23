# 👥📌Equipo 8 - SafeWalk AI (Zonas de Construcción)
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1, conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial.  

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# 🧾 DESCRIPCIÓN DEL PROYECTO

El equipo 8 desarrollará SafeWalk AI, un sistema inteligente de detección y alerta instalado en **zonas de construcción urbana**, orientado a mejorar la seguridad de personas con discapacidad visual en entornos con alto riesgo.

El sistema emplea una cámara conectada directamente a una NVIDIA Jetson Nano para la captura de imágenes en tiempo real. Estas imágenes son procesadas mediante un modelo de visión artificial basado en YOLO, encargado de detectar la presencia de personas con discapacidad visual a partir de elementos característicos como el bastón blanco y las gafas oscuras.
Adicionalmente, se utiliza un microcontrolador ESP32 para la gestión de los dispositivos de salida, como el altavoz y otros elementos electrónicos del sistema.
Al identificar este elemento, el sistema reconoce a una persona con discapacidad visual y activa automáticamente una alerta sonora mediante un altavoz, con el fin de advertirle sobre la proximidad de una zona de obra o peligro.

Esta alerta cumple una doble función:  
- Advertir directamente al peatón con discapacidad visual sobre un entorno riesgoso  
- Informar a trabajadores y transeúntes cercanos sobre su presencia  

El uso combinado del ESP32-CAM y la Jetson Nano permite optimizar el sistema: el ESP32-CAM se encarga de la adquisición de imágenes de forma eficiente y económica, mientras que la Jetson Nano procesa la información utilizando su GPU, logrando una detección precisa en tiempo real.

Este proyecto surge como respuesta a la problemática de la vulnerabilidad de las personas con discapacidad visual en entornos urbanos dinámicos y peligrosos como las zonas de construcción.

SafeWalk AI contribuye a los Objetivos de Desarrollo Sostenible (ODS) 3, 9, 10 y 11, promoviendo la seguridad, la innovación tecnológica y la construcción de ciudades más inclusivas.

---

# 🌍 CONTEXTO

El crecimiento urbano en las ciudades implica una constante ejecución de obras de construcción, mantenimiento vial, instalación de servicios públicos y desarrollo de infraestructura. Estas intervenciones generan entornos dinámicos y temporales caracterizados por la presencia de maquinaria pesada, excavaciones, materiales expuestos y modificaciones en las rutas peatonales habituales (10). A diferencia de la infraestructura permanente, las zonas de construcción suelen cambiar rápidamente, lo que dificulta la adaptación de los peatones y aumenta el riesgo de accidentes (11).

En este tipo de entornos, la señalización de seguridad se basa principalmente en elementos visuales como conos, cintas de advertencia, carteles informativos y barreras físicas. Sin embargo, estos mecanismos no están diseñados considerando la accesibilidad universal, lo que representa una limitación significativa para las personas con discapacidad visual (9). La ausencia de sistemas de alerta auditiva o mecanismos inteligentes de advertencia genera una brecha importante en la seguridad de este grupo poblacional.

Diversos estudios han demostrado que las personas con discapacidad visual enfrentan mayores dificultades al desplazarse en entornos urbanos no estructurados o en constante cambio, donde la detección de obstáculos depende en gran medida de señales no visuales (3, 4). En el caso de las zonas de construcción, esta problemática se intensifica debido a la presencia de riesgos adicionales como desniveles, maquinaria en movimiento y objetos imprevistos en la vía (10).

Asimismo, la falta de infraestructura accesible en estos entornos no solo incrementa el riesgo de accidentes, sino que también limita la autonomía y la movilidad de las personas con discapacidad visual, afectando su capacidad de desplazarse de manera segura e independiente en la ciudad (9). Esta situación evidencia la necesidad de incorporar soluciones tecnológicas que permitan adaptar el entorno urbano de forma dinámica, especialmente en espacios temporales de alto riesgo.

En este contexto, el uso de sistemas basados en visión artificial y computación en el borde representa una oportunidad para mejorar la seguridad en zonas de construcción. Estas tecnologías permiten detectar en tiempo real elementos relevantes del entorno y generar alertas oportunas, como lo demuestran investigaciones recientes en detección de obstáculos mediante modelos YOLO aplicados a entornos exteriores (6, 12). De esta manera, se facilita la prevención de accidentes y se promueve el desarrollo de entornos urbanos más inclusivos y seguros.

---

# 📊 EVIDENCIA DEL PROBLEMA

En el Perú, los entornos de construcción representan un problema relevante de seguridad para la población debido a la exposición a riesgos físicos como maquinaria pesada, excavaciones y estructuras temporales. De acuerdo con la Organización Internacional del Trabajo, el sector construcción es uno de los más peligrosos a nivel mundial, concentrando un alto porcentaje de accidentes laborales y urbanos debido a las condiciones dinámicas y cambiantes de las obras (10). Asimismo, normativas internacionales de seguridad establecen que la señalización en estos espacios es frecuentemente insuficiente o inadecuada, lo que incrementa la probabilidad de accidentes tanto para trabajadores como para peatones (11).

Esta situación se vuelve aún más crítica para las personas con discapacidad visual. Según la Organización Mundial de la Salud, más de mil millones de personas en el mundo viven con algún tipo de discapacidad, de las cuales una proporción significativa presenta limitaciones visuales que afectan su capacidad de desplazarse de manera segura en entornos no adaptados (9). En el contexto peruano, esta problemática se acentúa debido a la falta de infraestructura accesible en espacios urbanos temporales como zonas de construcción.

Las personas con discapacidad visual enfrentan barreras concretas en estos entornos, ya que la señalización existente es principalmente visual y no existen mecanismos auditivos que adviertan sobre peligros inmediatos. Investigaciones recientes en sistemas de navegación asistida demuestran que la detección de obstáculos en tiempo real es fundamental para mejorar la seguridad y autonomía de este grupo poblacional (3, 4). Sin embargo, en zonas de obra, estos riesgos se incrementan debido a la presencia de elementos imprevistos como zanjas abiertas, materiales de construcción y cambios constantes en la ruta peatonal (10).

Estos datos evidencian que las zonas de construcción constituyen entornos de alto riesgo para los peatones, especialmente para aquellos con discapacidad visual. La ausencia de soluciones inclusivas en estos espacios no solo incrementa la probabilidad de accidentes, sino que también limita la movilidad y autonomía de estas personas, restringiendo su acceso seguro al entorno urbano.

La magnitud de esta problemática contrasta con la limitada implementación de tecnologías que permitan adaptar estos espacios de manera inclusiva. A pesar de los avances en visión artificial y detección de objetos en tiempo real, su aplicación en infraestructura temporal sigue siendo reducida (6, 12). Esta brecha entre el desarrollo tecnológico y su aplicación práctica refleja una problemática estructural que afecta directamente la seguridad y calidad de vida de las personas con discapacidad visual en entornos urbanos dinámicos.

# 💡 JUSTIFICACIÓN DEL PROYECTO

Frente a esta problemática, surge la necesidad de desarrollar soluciones que contribuyan a mejorar la seguridad de los peatones en entornos urbanos dinámicos, especialmente en zonas de construcción. Si bien existen normativas nacionales e internacionales orientadas a garantizar la seguridad en obras, su implementación no siempre es efectiva, ya que persisten limitaciones en la señalización, supervisión y adaptación de estos espacios para usuarios vulnerables (10, 11). En particular, las personas con discapacidad visual continúan enfrentando barreras significativas debido a la falta de mecanismos de accesibilidad adecuados en estos entornos temporales.

En este sentido, las medidas tradicionales de seguridad en zonas de construcción —como señalización visual, cintas de advertencia, barreras físicas y carteles informativos— no son suficientes para garantizar la seguridad de las personas con discapacidad visual, ya que dependen principalmente de la percepción visual (9). Esto evidencia la necesidad de incorporar soluciones complementarias que utilicen otros canales sensoriales, como el auditivo, para transmitir información de riesgo de manera efectiva.

Por ello, nuestro proyecto propone el desarrollo de SafeWalk AI, un sistema inteligente que utiliza un módulo ESP32-CAM para la captura de imágenes y una Jetson Nano para el procesamiento mediante visión artificial con el modelo YOLO. Este sistema permite detectar en tiempo real la presencia de un bastón blanco en peatones, identificando así a personas con discapacidad visual y activando una alerta sonora a través de un altavoz instalado en zonas de construcción. La aplicación de modelos de detección de objetos en tiempo real ha demostrado ser efectiva para identificar elementos relevantes del entorno y generar alertas oportunas en sistemas de asistencia (6, 12).

Este enfoque busca complementar las soluciones existentes mediante el uso de inteligencia artificial aplicada a infraestructura temporal, contribuyendo a mejorar la seguridad y la inclusión en entornos de alto riesgo. En este sentido, el proyecto se alinea con los Objetivos de Desarrollo Sostenible, especialmente los ODS 3, 9, 10 y 11, promoviendo entornos urbanos más seguros, accesibles e inclusivos para todos.

---

# ⚙️ ¿Cómo funciona el proyecto?

## Captura de imágenes
El sistema utiliza un módulo ESP32-CAM conectado a la Jetson Nano, el cual captura imágenes del entorno y las transmite para su procesamiento.

## Control del sistema
La Jetson Nano recibe y procesa las imágenes, y posteriormente envía señales a un microcontrolador que gestiona los dispositivos del sistema.

## Activación de alerta
Se activa una alerta sonora que advierte sobre peligros cercanos como excavaciones o maquinaria.

## Función del sistema
El sistema busca prevenir accidentes y mejorar la seguridad del peatón con discapacidad visual mediante alertas.

# 💡 ESTADO DEL ARTE

**Sistemas de asistencia personal para personas con discapacidad visual**

La línea de investigación más desarrollada en la literatura propone soluciones que el propio usuario porta consigo. Diversos estudios han presentado sistemas de detección de obstáculos y asistencia a la navegación implementados en dispositivos como gafas inteligentes, bastones electrónicos o sistemas portables que integran cámaras, sensores y algoritmos de machine learning (3, 4). Estos sistemas permiten identificar objetos en el entorno y generar retroalimentación auditiva o háptica en tiempo real, facilitando la movilidad de las personas con discapacidad visual.

Asimismo, investigaciones recientes han incorporado modelos de detección de objetos como YOLO en dispositivos de bajo costo, logrando altos niveles de precisión en la identificación de obstáculos tanto en entornos interiores como exteriores (6). Estos avances demuestran la madurez de la visión artificial como herramienta para la asistencia a personas con discapacidad visual.

Sin embargo, todas estas propuestas comparten una limitación estructural: dependen de que el usuario adquiera, configure y porte un dispositivo adicional. Esto representa una barrera de acceso económico y tecnológico, especialmente en contextos donde no todos los usuarios pueden acceder a este tipo de soluciones.

---

**Sistemas de detección en entornos urbanos y de riesgo**

Una segunda línea de investigación se enfoca en la implementación de sistemas de detección desde infraestructura fija, utilizando cámaras y modelos de visión artificial para monitorear entornos urbanos. Estos sistemas permiten identificar objetos, personas y condiciones de riesgo en tiempo real, siendo ampliamente utilizados en aplicaciones como videovigilancia y monitoreo de tráfico.

Estudios recientes han demostrado que es posible adaptar estos sistemas para identificar a personas con discapacidad visual mediante el reconocimiento de elementos característicos como el bastón blanco, utilizando modelos de detección de objetos entrenados en múltiples escenarios (6, 12). Este enfoque resulta especialmente relevante en entornos de alto riesgo, como zonas de construcción, donde la detección temprana puede prevenir accidentes.

A pesar de estos avances, la aplicación de estos sistemas en infraestructura temporal, como obras de construcción, sigue siendo limitada. La mayoría de implementaciones se concentran en entornos permanentes, dejando una brecha importante en espacios dinámicos donde los riesgos son mayores (10).

---

**Modelos de detección de objetos para entornos dinámicos**

Investigaciones recientes han evaluado el desempeño de modelos de detección de objetos como YOLO, Faster R-CNN y DETR en tareas de identificación de obstáculos en tiempo real. Estos estudios muestran que modelos como YOLO ofrecen un balance adecuado entre precisión y velocidad, lo que los hace ideales para aplicaciones en dispositivos de borde (6).

En entornos dinámicos como zonas de construcción, donde los obstáculos pueden cambiar constantemente, la capacidad de detección en tiempo real es fundamental. La utilización de modelos optimizados permite identificar elementos relevantes del entorno y generar alertas oportunas, contribuyendo a la prevención de accidentes.

---

**Viabilidad del sistema**

Estudios recientes han demostrado la viabilidad de implementar sistemas de visión artificial en dispositivos de edge computing como la Jetson Nano, logrando ejecutar modelos de detección de objetos en tiempo real con niveles adecuados de precisión (12). Estos resultados evidencian que es posible desarrollar soluciones eficientes utilizando hardware de bajo costo.

La aplicación de estas tecnologías en zonas de construcción permite adaptar el entorno de manera inteligente, generando alertas auditivas en función de la detección de usuarios vulnerables. Esto valida la factibilidad técnica de SafeWalk AI, ya que el sistema propuesto utiliza modelos de detección en tiempo real para mejorar la seguridad en entornos urbanos dinámicos y de alto riesgo.

---

# 🌍 OBJETIVOS DE DESARROLLO SOSTENIBLE

Los Objetivos de Desarrollo Sostenible (ODS) son un conjunto de metas globales establecidas por la Organización de las Naciones Unidas como parte de la Agenda 2030 para el Desarrollo Sostenible, adoptada en el año 2015 por los Estados miembros (9). Estos objetivos buscan orientar los esfuerzos de los países hacia un desarrollo que permita mejorar la calidad de vida de las personas, reducir las desigualdades y proteger el planeta.

# Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

⚕️**ODS 3: Salud y bienestar**

Una de las metas de este objetivo, específicamente la meta 3.6, establece la necesidad de reducir el número de muertes y lesiones causadas por accidentes en entornos de riesgo para el año 2030 (9). En el contexto urbano, esto implica desarrollar medidas que protejan a los grupos más vulnerables, especialmente en espacios como zonas de construcción, donde existen múltiples peligros asociados a maquinaria, excavaciones y cambios constantes en la infraestructura (10).

A nivel global, el sector construcción es considerado uno de los más peligrosos debido a la alta incidencia de accidentes asociados a condiciones inseguras y señalización inadecuada (10, 11). Para las personas con discapacidad visual, este riesgo se incrementa significativamente, ya que la mayoría de advertencias en estos entornos son de carácter visual y no existen mecanismos accesibles que permitan identificar peligros de manera oportuna (9).

Nuestro proyecto se relaciona con este objetivo porque busca reducir el riesgo de accidentes en zonas de construcción para personas con discapacidad visual, contribuyendo a preservar su integridad física y promover su bienestar. A través de un sistema que detecta la presencia de un bastón blanco mediante visión artificial con YOLO en una Jetson Nano, y activa una alerta sonora en tiempo real, se busca mejorar la seguridad y autonomía de estas personas en entornos de alto riesgo.

---

🏭**ODS 9: Industria, innovación e infraestructura**

Una de las metas de este objetivo plantea la necesidad de modernizar la infraestructura e incorporar tecnologías que permitan hacerla más segura, eficiente e inclusiva (9). En el contexto urbano, esto incluye la implementación de sistemas inteligentes capaces de adaptarse a entornos dinámicos como las zonas de construcción.

Nuestro proyecto se vincula con este objetivo porque propone el uso de herramientas tecnológicas como cámaras, inteligencia artificial y algoritmos de detección de objetos en tiempo real para mejorar la seguridad en estos espacios. La implementación de un sistema basado en YOLO que detecte a personas con discapacidad visual y genere alertas sonoras representa una forma concreta de innovación aplicada a infraestructura temporal (6, 12).

---

🤝 **ODS 10: Reducción de las desigualdades**

En muchos casos, las personas con discapacidad enfrentan dificultades para desplazarse en el entorno urbano debido a la falta de infraestructura accesible, especialmente en espacios temporales como zonas de obra. Estas limitaciones generan una brecha en el acceso seguro al espacio público.

De acuerdo con la Organización Mundial de la Salud, una gran proporción de la población mundial presenta algún tipo de discapacidad, lo que evidencia la necesidad de desarrollar soluciones inclusivas que mejoren su calidad de vida (9). En entornos de construcción, la ausencia de mecanismos de alerta accesibles incrementa esta desigualdad.

Nuestro proyecto se relaciona con este objetivo porque busca reducir estas barreras mediante el uso de tecnología. A través de la detección en tiempo real de personas con discapacidad visual y la generación de alertas auditivas en zonas de construcción, se busca mejorar su seguridad y facilitar su desplazamiento en entornos urbanos complejos. Investigaciones recientes demuestran que los sistemas de visión artificial permiten identificar elementos clave como el bastón blanco, lo que hace viable este tipo de soluciones (6).

---

🏙️**ODS 11: Ciudades y comunidades sostenibles**

Una de las metas de este objetivo está relacionada con mejorar la seguridad y accesibilidad de los espacios urbanos, garantizando que estos sean inclusivos para todos los ciudadanos, especialmente los grupos más vulnerables (9).

En el contexto urbano, las zonas de construcción representan un desafío importante para la seguridad peatonal debido a su carácter temporal y a la presencia de riesgos constantes. La falta de adaptación de estos espacios para personas con discapacidad visual evidencia una deficiencia en la planificación urbana inclusiva (10).

El proyecto propuesto se relaciona con este objetivo porque busca contribuir al desarrollo de ciudades más seguras mediante la incorporación de tecnología en infraestructura temporal. Al implementar un sistema que detecte en tiempo real a personas con discapacidad visual y emita alertas sonoras en zonas de construcción, se promueve una mayor accesibilidad y seguridad en el entorno urbano.

---

## 📸 Fotografía del Equipo 
<p align="center">
<img width="1408" height="768" alt="imagen_alumnos_IA" src="Recursos/Imagenes/WhatsApp Image 2026-03-17 at 10.03.50 PM.jpeg" />
  <em>Figura 1. Fotografía del equipo 8</em>
</p>

---

## 👥 Integrantes del Equipo  

| Foto | Nombre | Rol | Intereses |
|------|--------|-----|-----------|
| <img src="/Recursos/Imagenes/655903395_943863358260627_6909408214037791066_n.jpg" width="90"/> | **Angello Areche Espeza** | Técnico de Hardware y Prototipos | Diseña y construye los prototipos físicos del sistema. Se encarga de la selección de componentes, ensamblaje, pruebas de funcionamiento y conexión con la Jetson Nano. |
| <img src="/Recursos/Imagenes/Foto Rolando.jpeg" width="90"/> | **Rolando Ronceros Huaynapomas** | Diseñador de Arquitectura del Sistema | Define la estructura general del proyecto. Establece cómo se conectan y comunican los distintos componentes (hardware y software), y organiza el flujo de funcionamiento del sistema. |
| <img src="/Recursos/Imagenes/leslie.foto.jpeg" width="90"/> | **Leslie Stephany Tomanguilla Huaman** | Analista Funcional del Sistema | Se encarga de organizar y estructurar los requerimientos del sistema a partir del análisis realizado por el equipo. Define las funcionalidades y asegura que las soluciones propuestas respondan correctamente al problema identificado |
| <img src="/Recursos/Imagenes/WhatsApp Image 2026-03-20 at 11.19.52 PM.jpeg" width="90"/> | **Daniela Mori Mendoza** |  Gestora de Documentación | Organiza y redacta toda la documentación del proyecto. Mantiene actualizados los informes, descripciones técnicas y avances, asegurando claridad y orden en la información. |
| <img src="/Recursos/Imagenes/alex.jpeg" width="90"/> | **Alex Jhosep Ccoyllo Sotelo** | Desarrollador de Software | Programa el funcionamiento del sistema en la Jetson Nano. Se encarga de la lógica, procesamiento de datos y conexión con los componentes del hardware. |

---

## 📌 Resumen Final  
El Equipo 8 está conformado por estudiantes comprometidos con generar un impacto positivo en la sociedad mediante soluciones tecnológicas innovadoras. En esta nueva propuesta, se ha decidido trabajar con los ODS 3, 9, 10 y 11 ,los cuales abordan problemáticas relacionadas con la seguridad ciudadana, el desarrollo de ciudades seguras y la implementación de tecnología para mejorar la calidad de vida.


---

# 📑 Referencias Bibliográficas

**1.** Wang W, et al. YOLO-OD: Obstacle Detection for Visually Impaired Navigation Assistance. *Sensors*. 2024. https://doi.org/10.3390/s24237621 

**2.** Li J, et al. PC-CS-YOLO: High-Precision Obstacle Detection. *Sensors*. 2025. https://doi.org/10.3390/s25020534 

**3.** Elhoseny M, et al. Obstacle detection system for blind navigation. *Computer & Electrical Engineering*. 2023. https://doi.org/10.1016/j.compeleceng.2023.108714 

**4.** Hassan M, et al. Deep learning obstacle detection for blind navigation. *Alexandria Engineering Journal*. 2023. https://doi.org/10.1016/j.asej.2023.102387 

**5.** Mahapatro A, et al. Real-Time Navigation System using YOLO. 2026. https://doi.org/10.5281/zenodo.19353279 

**6.** He C, Saha P. YOLO for outdoor obstacle detection. 2023. https://arxiv.org/abs/2312.07571 

**7.** Farzaneh MJ, Mohammadi HM. YOLO and SLAM navigation. 2022. https://arxiv.org/abs/2212.12185 

**8.** Thakurdesai N, et al. Deep learning walking assistance. 2019. https://arxiv.org/abs/1911.08739 

**9.** World Health Organization. World Report on Disability. 2011. https://www.who.int/publications/i/item/9789241564182 

**10.** International Labour Organization. Safety and Health in Construction. 2022. https://www.ilo.org/global/publications/books/WCMS_159358/lang--en/index.htm 

**11.** OSHA. Construction Industry Standards. 2024. https://www.osha.gov/laws-regs/regulations/standardnumber/1926 

**12.** Huangfu Y, et al. Edge Computing for Detection. 2023. https://ieeexplore.ieee.org/document/10335960

