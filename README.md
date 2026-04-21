#  👥📌Equipo 8 - SafeWalk IA
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1 , conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial. 

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# 🧾 DESCRIPCION DEL PROYECTO

El equipo 8 desarrollará SafeWalk AI, un sistema inteligente de detección y alerta instalado en semáforos de cruces peatonales, orientado a mejorar la seguridad de personas con discapacidad visual en el entorno urbano.

El sistema emplea un módulo ESP32-CAM para la captura de imágenes en tiempo real. Estas imágenes son enviadas a una Jetson Nano, donde se ejecuta un modelo de visión artificial basado en YOLO, encargado de detectar la presencia de un bastón blanco en los peatones.

Al identificar este elemento, el sistema reconoce a una persona con discapacidad visual y activa automáticamente una alerta sonora mediante un altavoz instalado en el semáforo, con el fin de advertir a las personas cercanas y fomentar un cruce más seguro.

Esta alerta cumple una doble función: orientar al peatón con discapacidad visual durante el cruce y advertir a los demás transeúntes sobre su presencia, fomentando una mayor atención y apoyo en el entorno.

El uso combinado del ESP32-CAM y la Jetson Nano permite optimizar el sistema: el ESP32-CAM se encarga de la adquisición de imágenes de forma eficiente y económica, mientras que la Jetson Nano procesa la información utilizando su GPU, logrando una detección precisa en tiempo real.

Este proyecto surge como respuesta a la problemática de la vulnerabilidad de las personas con discapacidad visual en espacios urbanos, respaldada por estudios de fuentes oficiales y literatura científica.

SafeWalk AI contribuye a los Objetivos de Desarrollo Sostenible (ODS) 3, 9, 10 y 11, promoviendo la seguridad, la innovación tecnológica y la construcción de ciudades más inclusivas.

---

# 🌍 CONTEXTO

La movilidad urbana es un aspecto fundamental para el desarrollo de las ciudades, ya que permite el desplazamiento seguro de las personas dentro del espacio público. Sin embargo, en muchos países, incluyendo el Perú, la seguridad vial continúa siendo un desafío importante, especialmente para los peatones, quienes representan uno de los grupos más vulnerables dentro del sistema de tránsito. La interacción constante entre vehículos y peatones en las vías urbanas, sumada a factores como el alto flujo vehicular, la falta de infraestructura adecuada y el incumplimiento de normas de tránsito, incrementa el riesgo de accidentes. Estudios realizados en Lima evidencian que los peatones tienden a elegir rutas más corNo tas para cruzar, influenciados por la ubicación de elementos urbanos, y que la congestión vehicular puede inducir comportamientos más arriesgados que aumentan el riesgo de accidentes (1).

Esta situación se vuelve aún más crítica para las personas con discapacidad visual, quienes enfrentan mayores dificultades al momento de desplazarse de forma autónoma por el espacio público. Un estudio del Banco Interamericano de Desarrollo que evaluó la accesibilidad peatonal en rutas urbanas con participación de personas con distintos tipos de discapacidad concluyó que las personas con discapacidad visual son las más afectadas por las barreras presentes en el entorno urbano, especialmente en los recorridos asociados a cruces peatonales y paradas de transporte público (2). En muchos casos, los sistemas de señalización existentes no están diseñados considerando plenamente las necesidades de accesibilidad de estas personas, lo que limita su capacidad de desplazarse con seguridad ante situaciones de riesgo vial.

# 📊 EVIDENCIA DEL PROBLEMA

 En el Perú, los accidentes de tránsito representan un problema significativo de seguridad pública. De acuerdo con información del Ministerio de Transportes y Comunicaciones del Perú, entre enero y julio de 2022 se registraron más de 47,000 siniestros de tránsito, los cuales ocasionaron 1,853 fallecidos y más de 30,000 personas lesionadas (3). Dentro de estas cifras, los peatones constituyen uno de los grupos más afectados, representando aproximadamente el 25.7% de las personas fallecidas en accidentes de tránsito. A nivel local, según el Observatorio Nacional de Seguridad Vial, solo en el departamento de Lima se registraron aproximadamente 1,303 accidentes de tránsito en 2023, atribuidos principalmente a las malas condiciones de las carreteras y la inadecuada señalización vial (3).
 
Esta situación se agrava para las personas con discapacidad visual. Los Censos Nacionales 2017 del INEI revelaron que aproximadamente 1,966,766 personas en el Perú experimentan dificultades o limitaciones permanentes en la visión, siendo Lima Metropolitana la zona con mayor concentración de esta población, representando el 65.8% del total (4). Estas personas enfrentan barreras concretas al desplazarse por la ciudad: la ausencia de semáforos sonoros, la falta de pisos podotáctiles y la inadecuada señalización en los cruces peatonales limitan su capacidad de circular de forma segura e independiente (5).

Estos datos evidencian que el entorno vial presenta riesgos importantes para quienes se desplazan a pie, especialmente en intersecciones y cruces peatonales. Para las personas con discapacidad visual, este riesgo es aún mayor. Como señalan Seminario-Hurtado y Alfaro Torres (5), las barreras físicas en el entorno urbano no solo limitan la movilidad de estas personas, sino que también restringen su acceso a servicios esenciales, afectando directamente su calidad de vida y autonomía.

La magnitud de esta población contrasta con la precariedad de las condiciones de accesibilidad que enfrentan en el espacio público. Según el BID, las rutas peatonales asociadas al transporte urbano presentan deficiencias críticas para las personas con discapacidad visual, siendo este grupo el más perjudicado por la falta de infraestructura adaptada (2). Esta brecha entre las necesidades reales de la población y la oferta de infraestructura urbana refleja una problemática sistémica que afecta directamente la seguridad y autonomía de las personas con discapacidad visual en los espacios públicos.

# 💡 JUSTIFICACIÓN DEL PROYECTO

Frente a esta problemática, surge la necesidad de desarrollar soluciones que contribuyan a mejorar la seguridad de los peatones en los espacios urbanos. Si bien el Estado peruano ha establecido un marco legal orientado a garantizar la accesibilidad, la implementación de estas normativas no ha sido efectiva, ya que persisten barreras físicas, sociales e institucionales, entre ellas la falta de asignación de un presupuesto público razonable y la ausencia de mecanismos de fiscalización adecuados (5).

En este sentido, entre las medidas recomendadas para mejorar la accesibilidad en entornos urbanos para personas con discapacidad visual se encuentran los semáforos sonoros, los pisos podotáctiles y los carteles con información en braille; sin embargo, su aplicación no es generalizada ni adecuada en el Perú (5). Esto evidencia que las soluciones tradicionales son insuficientes y que se requiere innovar en la forma en que las alertas de riesgo llegan específicamente a las personas invidentes en los cruces peatonales.

Por ello, nuestro proyecto propone el desarrollo de SafeWalk AI, un sistema inteligente que utiliza un módulo ESP32-CAM para la captura de imágenes y una Jetson Nano para el procesamiento mediante visión artificial con el modelo YOLO. Este sistema permite detectar en tiempo real la presencia de un bastón blanco en peatones, identificando así a personas con discapacidad visual y activando una alerta sonora a través de un altavoz instalado en el semáforo. 

Este enfoque busca complementar las soluciones existentes mediante el uso de inteligencia artificial, contribuyendo a mejorar la seguridad y la inclusión en los entornos urbanos. En este sentido, el proyecto se alinea con los Objetivos de Desarrollo Sostenible, especialmente los ODS 3, 9, 10 y 11, promoviendo una movilidad más segura, accesible e inclusiva.


---


# ¿Cómo funciona el proyecto?
## Captura de imágenes
El sistema utiliza un módulo ESP32-CAM para capturar imágenes en tiempo real del entorno del cruce peatonal.
## Procesamiento y detección
Las imágenes son enviadas a una Jetson Nano, donde se ejecuta un modelo de visión artificial basado en YOLO para detectar la presencia de un bastón blanco en los peatones.
## Control del sistema
Una vez realizada la detección, la Jetson Nano envía una señal a un microcontrolador (ESP32 o Arduino), encargado de gestionar los dispositivos electrónicos del sistema.
## Activación de alerta
El microcontrolador activa una alerta sonora mediante un altavoz instalado en el semáforo, con el fin de advertir a las personas cercanas.

## Función del sistema
La alerta busca mejorar la seguridad en el cruce peatonal, facilitando la identificación de personas con discapacidad visual y promoviendo una mayor atención por parte del entorno.

---
# 💡 ESTADO DEL ARTE

**Sistemas de asistencia personal para personas con discapacidad visual**

La línea de investigación más desarrollada en la literatura propone soluciones que el propio usuario porta consigo.Leong y Kanesaraj Ramasamy (7) propusieron un sistema de detección de obstáculos y estimación de distancia para personas con discapacidad visual implementado en gafas inteligentes con Raspberry Pi, cámara y algoritmos de machine learning, que genera retroalimentación auditiva o háptica en tiempo real según la proximidad de los objetos detectados. Este sistema está diseñado para identificar objetos y estimar sus distancias, proporcionando retroalimentación auditiva o háptica en tiempo real al usuario. 
Ferreira et al. (8) diseñaron un sistema modular de gafas inteligentes para detección de obstáculos en navegación de personas invidentes, validando la viabilidad de integrar procesamiento de visión artificial en objetos cotidianos del usuario con alertas sonoras como salida principal.
Okolo et al. propusieron un sistema de navegación asistida inteligente que combina YOLOv8 implementado sobre Raspberry Pi con sensores ultrasónicos, cámara, altavoz y sensor de humedad, alcanzando una precisión promedio del 91.70% en la detección de nueve tipos de obstáculos en entornos interiores y exteriores, con tiempos de detección de apenas 0.001 segundos para personas y vehículos.Este resultado confirma que YOLO es un algoritmo maduro y eficiente para aplicaciones de detección en tiempo real orientadas a personas con discapacidad visual.
Sin embargo, todas estas propuestas comparten una limitación estructural: dependen de que el usuario adquiera, configure y porte un dispositivo adicional, lo que representa una barrera de acceso económico y tecnológico que excluye precisamente a quienes más necesitan la solución.

**Sistemas de detección en cruces peatonales para personas con discapacidad visual**

Una segunda línea de investigación se enfoca específicamente en el desafío del cruce de calles, que representa uno de los mayores riesgos para las personas invidentes en el espacio urbano. 
Chang et al. propusieron un sistema wearable basado en edge computing con inteligencia artificial que combina gafas inteligentes, un dispositivo de cintura y un bastón inteligente para asistir a personas con discapacidad visual en el uso seguro de cruces cebra, adoptando deep learning para el reconocimiento en tiempo real de la señalización peatonal y alcanzando una precisión del 90% en la detección del cruce cebra. Este trabajo evidencia que la combinación de bastón y gafas como objetos de referencia es un enfoque válido para identificar al usuario invidente en el contexto del cruce peatonal, lo que directamente sustenta la estrategia de detección de SafeWalk AI.
Ji H et al. (8, 6) desarrollaron un dataset multi-escena y un detector de objetos específicamente diseñado para identificar a personas invidentes en espacios públicos exteriores, demostrando que los sistemas de videovigilancia existentes pueden adaptarse para reconocer a este grupo de usuarios mediante visión artificial. Su trabajo es especialmente relevante para SafeWalk AI porque establece la viabilidad técnica de detectar personas invidentes desde cámaras fijas instaladas en infraestructura pública, no desde dispositivos portados por el usuario.

**Modelos de detección de objetos para personas con discapacidad visual**

Investigaciones recientes en IEEE Access han realizado evaluaciones comparativas entre YOLOv8, Faster R-CNN y DETR para sistemas de detección de obstáculos orientados a personas con discapacidad visual, encontrando que DETR logra una puntuación de confianza del 99%, precisión del 98% y velocidad de procesamiento de 40 ms por fotograma, mientras que YOLOv8 ofrece resultados competitivos con mayor eficiencia computacional, representando un balance adecuado entre precisión y velocidad para dispositivos de borde. Estos resultados son directamente aplicables a SafeWalk AI, donde la velocidad de inferencia en la Jetson Nano es un factor crítico.

**Viabilidad del sistema**

Estudios recientes han demostrado la viabilidad de implementar sistemas de monitoreo de tráfico en tiempo real utilizando dispositivos de edge computing. En particular, se ha logrado ejecutar modelos de detección de objetos como YOLOv4 en una Jetson Nano, alcanzando aproximadamente 7.8 FPS y una precisión cercana al 90% en detección de vehículos (12).
Estos resultados evidencian que es posible ejecutar modelos de deep learning en dispositivos de bajo costo y recursos limitados, aplicando técnicas como transfer learning y cuantización de modelos.
Esto valida directamente la factibilidad técnica de SafeWalk AI, ya que el sistema propuesto también utiliza YOLO en una Jetson Nano para realizar detección en tiempo real desde infraestructura urbana.


# 🌍 OBJETIVOS DE DESARROLLO SOSTENIBLE

Los Objetivos de Desarrollo Sostenible (ODS) son un conjunto de metas globales establecidas por la Organización de las Naciones Unidas como parte de la Agenda 2030 para el Desarrollo Sostenible, adoptada en el año 2015 por los Estados miembros (9). Estos objetivos buscan orientar los esfuerzos de los países hacia un desarrollo que permita mejorar la calidad de vida de las personas, reducir las desigualdades y proteger el planeta.

# Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

⚕️**ODS 3: Salud y bienestar**

Una de las metas de este objetivo, específicamente la meta 3.6, establece la necesidad de reducir a la mitad el número de muertes y lesiones causadas por accidentes de tráfico en el mundo para el año 2030 (10). En el contexto urbano, esto implica desarrollar medidas que protejan a los grupos más expuestos a estos riesgos, entre ellos los peatones con discapacidad, cuya seguridad física al desplazarse por la vía pública está directamente vinculada con su bienestar y su capacidad de acceder a servicios de salud y rehabilitación.

En el Perú, esta problemática tiene una dimensión concreta. Entre enero y julio de 2022, los accidentes de tránsito ocasionaron 1,853 fallecidos y más de 30,000 personas lesionadas (3), cifras que evidencian el impacto que la inseguridad vial tiene sobre la salud pública. Para las personas con discapacidad visual, este riesgo se agrava debido a la ausencia de infraestructura accesible en los cruces peatonales. Como señalan Seminario-Hurtado y Alfaro Torres (5), las barreras físicas en el entorno urbano no solo limitan la movilidad de estas personas, sino que también restringen su acceso a servicios esenciales, afectando directamente su calidad de vida.

Nuestro proyecto se relaciona con este objetivo porque busca reducir el riesgo de accidentes en cruces peatonales para personas con discapacidad visual, contribuyendo así a preservar su integridad física y promover su bienestar. A través de un sistema que detecta objetos asociados a peatones invidentes —el bastón blanco y las gafas oscuras— mediante YOLO en una Jetson Nano instalada en semáforos, y emite una alerta sonora para avisar a los demás peatones presentes, se busca que estas personas puedan desplazarse con mayor seguridad y autonomía, lo cual representa una mejora directa en su salud y calidad de vida.

🏭**ODS 9: Industria, innovación e infraestructura**

Una de las metas de este objetivo plantea la necesidad de modernizar la infraestructura existente e incorporar nuevas tecnologías que permitan hacerla más eficiente y segura (9). En el caso de las ciudades, esto se relaciona con el desarrollo de sistemas inteligentes que ayuden a mejorar la movilidad urbana y la seguridad vial.
Nuestro proyecto se vincula con este objetivo porque propone el uso de herramientas tecnológicas como cámaras, inteligencia artificial y algoritmos de detección de objetos en tiempo real para mejorar la seguridad de las personas invidentes en los cruces peatonales. La implementación de un sistema que detecte el bastón blanco y las gafas oscuras mediante YOLO en una Jetson Nano, y que emita una alerta sonora desde el semáforo, representa una forma concreta de innovación aplicada a la infraestructura urbana (6, 7, 8).

🤝 **ODS 10: Reducción de las desigualdades**

En muchos casos, las personas con discapacidad enfrentan dificultades para desplazarse en el entorno urbano debido a la falta de infraestructura accesible o a la ausencia de sistemas que les brinden apoyo en situaciones de riesgo. De acuerdo con datos del Instituto Nacional de Estadística e Informática, en el Perú más de tres millones de personas presentan algún tipo de discapacidad (10), lo que representa una parte importante de la población. Esto evidencia la necesidad de desarrollar soluciones que contribuyan a mejorar su acceso y movilidad en los espacios públicos.

Nuestro proyecto se relaciona con este objetivo porque busca contribuir a la reducción de estas barreras mediante el uso de tecnología. A través del desarrollo de un sistema que pueda detectar en tiempo real objetos asociados a personas invidentes en cruces peatonales y emitir alertas sonoras, se busca brindar una herramienta que facilite el desplazamiento de estas personas y mejore su seguridad al momento de cruzar la vía pública. En ese sentido, investigaciones recientes demuestran que la detección automática del bastón blanco mediante sistemas de visión artificial instalados en infraestructura pública constituye una solución viable y escalable para identificar a personas invidentes en espacios exteriores (6), lo que refuerza la urgencia de propuestas tecnológicas que cierren esta brecha.



🏙️**ODS 11: Ciudades y comunidades sostenibles**

Una de las metas de este objetivo está relacionada con mejorar la seguridad de los sistemas de transporte y garantizar que estos sean accesibles, especialmente para los grupos más vulnerables de la población, como niños, adultos mayores y personas con discapacidad (9).

En el Perú, los accidentes de tránsito continúan siendo un problema importante. Según información del Ministerio de Transportes y Comunicaciones del Perú, entre enero y julio del año 2022 se registraron más de 47,000 siniestros de tránsito en el país, lo que ocasionó miles de personas fallecidas y lesionadas (3). Dentro de estas cifras, los peatones se encuentran entre los grupos más afectados.

El proyecto propuesto se relaciona con este objetivo porque busca aportar a la construcción de ciudades más seguras mediante el uso de tecnología. Al desarrollar un sistema que permita detectar en tiempo real a personas con discapacidad visual a través de sus objetos distintivos —el bastón blanco y las gafas oscuras— y emitir una alerta sonora en el semáforo, se busca contribuir a mejorar la seguridad vial y la accesibilidad en los espacios urbanos, con especial énfasis en los cruces peatonales.



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

## 📑 Referencias Bibliográficas:

**1.** Huamaní Meza A, et al. Seguridad vial y peatones en Lima Metropolitana [Internet]. Lima: Editorial Innova; 2023 [citado 2025]. Disponible en: https://www.editorialinnova.com/index.php/nrj/article/view/323  

**2.** Rodríguez Porcel M, Lee S, Sandoval D, Tascón Valencia J, Jaramillo PJ, Pedraza L. Auditoría georreferenciada y diagnóstico de accesibilidad peatonal de personas con discapacidad en la primera y última milla de un viaje [Internet]. Washington D.C.: Banco Interamericano de Desarrollo; 2023 [citado 2025]. Disponible en: https://publications.iadb.org/es/auditoria-georreferenciada-y-diagnostico-de-accesibilidad-peatonal-de-personas-con-discapacidad-en 
 
**3.** Ministerio de Transportes y Comunicaciones del Perú. De enero a julio del 2022 ocurrieron más de 47 mil siniestros de tránsito en el Perú [Internet]. Lima: MTC; 2022 [citado 2025]. Disponible en: https://www.gob.pe/institucion/mtc/noticias/647689-de-enero-a-julio-del-2022-ocurrieron-mas-de-47-mil-siniestros-de-transito-en-el-peru/

**4.** Instituto Nacional de Estadística e Informática. Perfiles sociodemográficos de la población con discapacidad [Internet]. Lima: INEI; 2019 [citado 2025]. Disponible en: https://www.inei.gob.pe/media/MenuRecursivo/publicaciones_digitales/Est/Lib1675/libro.pdf  

**5.** Seminario-Hurtado N, Alfaro Torres HM. Accesibilidad en entornos urbanos para personas con discapacidad visual en el Perú: un análisis normativo. Cuadernos de Vivienda y Urbanismo [Internet]. 2025 [citado 2025]; 18. Disponible en: https://revistas.javeriana.edu.co/index.php/cvyu/article/view/41190/

**6.** Ji H, Mendonça I, Aritsugi M. Multi-Scene Dataset and Object Detector for Outside Blind Individual Identification. IEEE Access [Internet]. 2026 [citado 2026]; 14: 1423-1438. Disponible en: https://ieeexplore.ieee.org/document/11317963  

**7.** Leong X, Kanesaraj Ramasamy R. Obstacle Detection and Distance Estimation for Visually Impaired People. IEEE Access [Internet]. 2023 [citado 2025]; 11: 136609-136629. Disponible en: https://ieeexplore.ieee.org/document/10336791 

**8.** Ferreira AA, Barros CAL, Pereira TEB, Santana MFA, Silva IDS, Oliveira FS. Modular Smart Glasses for Real-Time Obstacle Detection in Blind Navigation. IEEE [Internet]. 2025 [citado 2025]. Disponible en: https://ieeexplore.ieee.org/document/11334173 

**9.**  Organización de las Naciones Unidas. Objetivos de Desarrollo Sostenible [Internet]. Nueva York: ONU; 2015 [citado 2025]. Disponible en: https://www.un.org/sustainabledevelopment/es/sustainable-development-goals/ 

**10.**  PROTRÁNSITO – Municipalidad Metropolitana de Lima. Centro de Control y Gestión de Tránsito (CCGT) [Internet]. Lima: PROTRÁNSITO; s.f. [citado 2025]. Disponible en: http://protransito.munlima.gob.pe/index.php/es-es/monitoreo/ccgt

**11.**  ITS Perú. ¿Quién o qué decide el ritmo de los semáforos en Lima? [Internet]. Lima: ITS Perú; 2024 [citado 2025]. Disponible en: https://itsperu.org/articulos/quien-o-que-decide-el-ritmo-de-los-semaforos-en-lima/ 

**12.**  Huangfu Y, Ahrabi M, Tahal R, Huang J, Mohammad-Alikhani A, Reymann S. Efficient Edge Computing Device for Traffic Monitoring Using Deep Learning Detectors. IEEE [Internet]. 2023 [citado 2025]. Disponible en: https://ieeexplore.ieee.org/document/10335960

