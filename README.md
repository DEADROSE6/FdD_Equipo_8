# Equipo 8 - SafeWalk IA
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1 , conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial. 

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# 🧾 DESCRIPCION DEL PROYECTO

El equipo 8 desarrollará SafeWalk AI, un sistema inteligente de detección y alerta instalado en semáforos de cruces peatonales, orientado a mejorar la seguridad de personas con discapacidad visual en el espacio urbano.

El sistema utiliza visión artificial basada en YOLO, ejecutada sobre una Jetson Nano, para detectar en tiempo real la presencia simultánea de bastón blanco y gafas en un peatón. Al identificar ambos objetos al mismo tiempo, el sistema infiere que se trata de una persona con discapacidad visual y activa de forma automática una alerta sonora a través de un altavoz instalado en el semáforo, notificando tanto al peatón vulnerable como a los demás transeúntes cercanos, quienes al escuchar el aviso pueden brindar asistencia o actuar con mayor precaución en el cruce.

La elección de Jetson Nano responde a una necesidad técnica concreta: al contar con GPU NVIDIA integrada, permite ejecutar modelos de detección de objetos como YOLO con baja latencia y alta eficiencia en tiempo real, algo que no puede garantizarse con alternativas como el ESP32-CAM o incluso una Raspberry Pi 5, cuya arquitectura CPU no está optimizada para inferencia de imágenes con inteligencia artificial.

Este proyecto nace como propuesta de solución frente a una problemática documentada en fuentes oficiales del gobierno peruano, revistas científicas indexadas en Scielo e IEEE, que evidencian tanto la vulnerabilidad de las personas con discapacidad visual en entornos urbanos como el potencial de la visión artificial aplicada a la seguridad vial.

SafeWalk AI contribuye a los ODS 3, 9, 10 y 11, promoviendo la seguridad vial, la innovación tecnológica aplicada a infraestructura urbana y el desarrollo de ciudades más inclusivas y seguras para todos.

---

# 🌍 CONTEXTO

La movilidad urbana es un aspecto fundamental para el desarrollo de las ciudades, ya que permite el desplazamiento seguro de las personas dentro del espacio público. Sin embargo, en muchos países, incluyendo el Perú, la seguridad vial continúa siendo un desafío importante, especialmente para los peatones, quienes representan uno de los grupos más vulnerables dentro del sistema de tránsito. La interacción constante entre vehículos y peatones en las vías urbanas, sumada a factores como el alto flujo vehicular, la falta de infraestructura adecuada y el incumplimiento de normas de tránsito, incrementa el riesgo de accidentes. Estudios realizados en Lima evidencian que los peatones tienden a elegir rutas más cortas para cruzar, influenciados por la ubicación de elementos urbanos, y que la congestión vehicular puede inducir comportamientos más arriesgados que aumentan el riesgo de accidentes (1).

Esta situación se vuelve aún más crítica para las personas con discapacidad visual, quienes enfrentan mayores dificultades al momento de desplazarse de forma autónoma por el espacio público. Un estudio del Banco Interamericano de Desarrollo que evaluó la accesibilidad peatonal en rutas urbanas con participación de personas con distintos tipos de discapacidad concluyó que las personas con discapacidad visual son las más afectadas por las barreras presentes en el entorno urbano, especialmente en los recorridos asociados a cruces peatonales y paradas de transporte público (2). En muchos casos, los sistemas de señalización existentes no están diseñados considerando plenamente las necesidades de accesibilidad de estas personas, lo que limita su capacidad de desplazarse con seguridad ante situaciones de riesgo vial.

# 📊 EVIDENCIA DEL PROBLEMA

 En el Perú, los accidentes de tránsito representan un problema significativo de seguridad pública. De acuerdo con información del Ministerio de Transportes y Comunicaciones del Perú, entre enero y julio de 2022 se registraron más de 47,000 siniestros de tránsito, los cuales ocasionaron 1,853 fallecidos y más de 30,000 personas lesionadas (3). Dentro de estas cifras, los peatones constituyen uno de los grupos más afectados, representando aproximadamente el 25.7% de las personas fallecidas en accidentes de tránsito. A nivel local, según el Observatorio Nacional de Seguridad Vial, solo en el departamento de Lima se registraron aproximadamente 1,303 accidentes de tránsito en 2023, atribuidos principalmente a las malas condiciones de las carreteras y la inadecuada señalización vial (3).
 
Esta situación se agrava para las personas con discapacidad visual. Los Censos Nacionales 2017 del INEI revelaron que aproximadamente 1,966,766 personas en el Perú experimentan dificultades o limitaciones permanentes en la visión, siendo Lima Metropolitana la zona con mayor concentración de esta población, representando el 65.8% del total (4). Estas personas enfrentan barreras concretas al desplazarse por la ciudad: la ausencia de semáforos sonoros, la falta de pisos podotáctiles y la inadecuada señalización en los cruces peatonales limitan su capacidad de circular de forma segura e independiente (5).

Estos datos evidencian que el entorno vial presenta riesgos importantes para quienes se desplazan a pie, especialmente en intersecciones y cruces peatonales. Para las personas con discapacidad visual, este riesgo es aún mayor. Como señalan Seminario-Hurtado y Alfaro Torres (5), las barreras físicas en el entorno urbano no solo limitan la movilidad de estas personas, sino que también restringen su acceso a servicios esenciales, afectando directamente su calidad de vida y autonomía.

La magnitud de esta población contrasta con la precariedad de las condiciones de accesibilidad que enfrentan en el espacio público. Según el BID, las rutas peatonales asociadas al transporte urbano presentan deficiencias críticas para las personas con discapacidad visual, siendo este grupo el más perjudicado por la falta de infraestructura adaptada (2). Esta brecha entre las necesidades reales de la población y la oferta de infraestructura urbana refleja una problemática sistémica que afecta directamente la seguridad y autonomía de las personas con discapacidad visual en los espacios públicos.

# 💡 JUSTIFICACIÓN DEL PROYECTO

Frente a esta problemática, surge la necesidad de desarrollar soluciones que contribuyan a mejorar la seguridad de los peatones en los espacios urbanos. Si bien el Estado peruano ha establecido un marco legal orientado a garantizar la accesibilidad, la implementación de estas normativas no ha sido efectiva, ya que persisten barreras físicas, sociales e institucionales, entre ellas la falta de asignación de un presupuesto público razonable y la ausencia de mecanismos de fiscalización adecuados (5).

En este sentido, entre las medidas recomendadas para mejorar la accesibilidad en entornos urbanos para personas con discapacidad visual se encuentran los semáforos sonoros, los pisos podotáctiles y los carteles con información en braille; sin embargo, su aplicación no es generalizada ni adecuada en el Perú (5). Esto evidencia que las soluciones tradicionales son insuficientes y que se requiere innovar en la forma en que las alertas de riesgo llegan específicamente a las personas invidentes en los cruces peatonales.

Por ello, nuestro proyecto propone el desarrollo de SafeWalk AI, un sistema inteligente que, mediante el uso de visión artificial con YOLO implementado en una Raspberry Pi 5 y una cámara, detecta en tiempo real objetos asociados a personas con discapacidad visual —específicamente el bastón blanco y las gafas oscuras— en cruces peatonales, y genera una alerta sonora a través de un altavoz instalado en el semáforo. Este aviso busca beneficiar tanto a la persona invidente como a los demás peatones presentes, quienes al escuchar la alerta pueden brindar apoyo. Investigaciones previas han demostrado la viabilidad de sistemas similares basados en Raspberry Pi con redes neuronales convolucionales para la detección de objetos en tiempo real (6, 7, 8). Dado que la brecha de accesibilidad peatonal para personas con discapacidad visual en espacios urbanos persiste pese a la normativa existente (2), este sistema busca contribuir a una movilidad urbana más segura e inclusiva, alineándose con los Objetivos de Desarrollo Sostenible, especialmente los ODS 3, 9, 10 y 11 (9).


---


# ¿Cómo funciona el proyecto?
## Detección
Sensores PIR y ultrasónico identifican la presencia y proximidad de peatones en el cruce. La cámara ESP32-CAM detecta objetos asociados a personas con discapacidad, como bastones blancos o sillas de ruedas, reconociendo automáticamente a usuarios vulnerables.
## Análisis
La ESP32-CAM captura imágenes y evalúa el comportamiento del peatón, identificando situaciones de riesgo como el uso del celular al momento de cruzar, así como el perfil de movilidad del usuario según los objetos detectados.
##Clasificación
El sistema determina el nivel de riesgo en tres estados:

Seguro — el peatón cruza con atención y sin riesgo inmediato
Sospechoso — se detecta distracción o comportamiento de riesgo
Peligro — situación de riesgo inminente para el peatón

## Respuesta en el semáforo
Se activan alertas físicas según el nivel de riesgo detectado:

Luces tipo semáforo
Sonido mediante buzzer
Mensajes en pantalla

## Respuesta en app móvil / smartwatch
De forma simultánea, el sistema envía señales vía Bluetooth o WiFi al dispositivo personal del usuario, con alertas diferenciadas según su perfil registrado:

Discapacidad visual — alerta sonora automática al detectar bastón blanco
Discapacidad auditiva — alerta visual y patrones de vibración en smartwatch o app móvil, donde pulsos cortos indican precaución y pulsos largos indican peligro
Discapacidad motriz — tiempo extendido de cruce al detectar silla de ruedas y notificación en app móvil

## Registro de datos
Se almacenan datos en Micro SD para análisis posterior y mejora continua del sistema.

---

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
