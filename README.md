# Equipo 8 - Fundamentos de Diseño
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1 , conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial. 

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# DESCRIPCION DEL PROYECTO

El equipo 8 desarrollará SafeWalk AI, un sistema inteligente de alerta para peatones que previene accidentes en cruces urbanos mediante sensores, visión artificial con ESP32-CAM e IoT.

El sistema detecta peatones distraídos, evalúa su comportamiento en tiempo real y clasifica el nivel de riesgo, activando alertas visuales, sonoras y mensajes en pantalla solo cuando es necesario.

Además, registra datos en Micro SD para análisis básico de patrones.

Asimismo, el proyecto incorpora un enfoque inclusivo, ya que brinda asistencia a personas con discapacidad visual mediante alertas sonoras en el cruce peatonal(cebra), y a personas con discapacidad auditiva mediante la conexión con una aplicación móvil que envía vibraciones y notificaciones en tiempo real, permitiendo advertir situaciones de riesgo de manera accesible.

Este proyecto contribuye a los ODS 3, 9 y 11, promoviendo la seguridad vial, la innovación tecnológica y el desarrollo de ciudades más inclusivas y seguras.

---

# PROBLEMÁTICA

La movilidad urbana es fundamental para el desarrollo de las ciudades, sin embargo, en el Perú la seguridad vial continúa siendo un desafío importante, especialmente para los peatones. El alto flujo vehicular, la falta de infraestructura adecuada y el incumplimiento de normas de tránsito incrementan el riesgo de accidentes, y estudios en Lima confirman que la congestión vehicular puede inducir comportamientos más arriesgados en los peatones al momento de cruzar (10).
Esta situación se vuelve aún más crítica para personas con discapacidad o movilidad reducida. En ciudades como Trujillo, los ciudadanos con discapacidad visual, auditiva o motriz han sido históricamente invisibilizados en el espacio público, enfrentando sistemas de señalización que no consideran sus necesidades reales de accesibilidad (4). 


# PROPUESTA DE SOLUCIÓN

Por ello, nuestro proyecto propone el desarrollo de SafeWalk AI, un sistema inteligente que, mediante el uso de visión artificial con ESP32-CAM, sensores de distancia y conectividad IoT, detecta situaciones de riesgo en cruces peatonales y genera alertas accesibles para dos tipos de usuarios: peatones distraídos por el uso del celular, mediante alertas sonoras y visuales en el semáforo (11, 12), y personas con discapacidad visual o auditiva, mediante notificaciones personalizadas en aplicaciones móviles o relojes inteligentes. Dado que la exclusión de las personas con discapacidad en su libre desplazamiento conlleva que no puedan integrarse a la vida económica y social, perjudicando su calidad de vida (4), este sistema busca contribuir a una movilidad urbana más segura e inclusiva, alineándose con los Objetivos de Desarrollo Sostenible, especialmente los ODS 3, 9, 10 y 11 (1).

Su diseño compacto, basado en una estructura impresa en 3D, permite su implementación como un prototipo funcional y escalable hacia ciudades inteligentes.

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

# Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

⚕️**ODS 3: Salud y bienestar**

Este ODS busca garantizar una vida sana y promover el bienestar para todas las personas. Nuestro proyecto aborda específicamente la meta 3.6, que establece reducir a la mitad las muertes y lesiones causadas por accidentes de tráfico para el año 2030 (1).
En el Perú:

- Entre enero y julio de 2022 se registraron más de 47,000 siniestros de tránsito, con un saldo de 1,853 fallecidos y más de 30,000 lesionados (3).
- El 11% de los accidentes fatales en Lima durante 2024 fue responsabilidad directa de peatones distraídos, principalmente por el uso del celular al cruzar (11).
- Para las personas con discapacidad, las barreras físicas en el entorno urbano no solo limitan su movilidad, sino que también restringen su acceso a servicios de salud y rehabilitación (5).

SafeWalk AI contribuye a este objetivo mediante alertas personalizadas en cruces peatonales, reduciendo el riesgo de accidentes y promoviendo la seguridad, autonomía y calidad de vida de los usuarios más vulnerables.
Ejemplos de soluciones similares a nivel global:

- NaviLens — sistema de señalización accesible para personas con discapacidad visual mediante códigos QR de alta velocidad.
- Microsoft Seeing AI — aplicación que usa inteligencia artificial para describir el entorno a personas con discapacidad visual en tiempo real.


🏭**ODS 9: Industria, innovación e infraestructura**

Este ODS promueve la modernización de la infraestructura existente mediante la incorporación de nuevas tecnologías que la hagan más eficiente, segura e inclusiva (1).
En el Perú:

En 2023 se registraron aproximadamente 1,303 accidentes de tránsito solo en Lima, atribuidos principalmente a deficiencias en la señalización vial e infraestructura inadecuada (8).
El 60% de los atropellos es responsabilidad del peatón, muchos de ellos relacionados con distracciones por dispositivos móviles, evidenciando la necesidad de sistemas de alerta en tiempo real (12).
La infraestructura urbana peruana carece de tecnología adaptada a las necesidades de personas con discapacidad, quienes representan más de 3 millones de ciudadanos en el país (2).

SafeWalk AI no requiere una transformación total de la ciudad. Combinando sensores, conectividad IoT e inteligencia artificial, lleva la seguridad directamente a los objetos que las personas ya usan, como el smartwatch o el celular, tomando decisiones en tiempo real para proteger al usuario en la calle.
Ejemplos de soluciones similares a nivel global:

Smart Traffic Systems en Singapur — semáforos inteligentes que ajustan los tiempos de cruce según el flujo peatonal en tiempo real.
Waymap — app de navegación indoor y outdoor para personas con discapacidad visual usando IoT y sensores.


🏙️**ODS 11: Ciudades y comunidades sostenibles** 
Este ODS busca lograr que las ciudades sean inclusivas, seguras, resilientes y sostenibles, garantizando el acceso equitativo al espacio público para todos los ciudadanos (1).
En el Perú:

El 57.2% de las personas con discapacidad califica como mala la accesibilidad en el transporte y espacio público urbano (4).
Lima Metropolitana concentra el 65.8% de la población con discapacidad visual del país, aproximadamente 1,966,766 personas, que enfrentan barreras diarias para desplazarse con autonomía (5).
Los peatones con discapacidad han sido históricamente invisibilizados en el diseño de la infraestructura urbana, vulnerando su derecho a circular libremente por la ciudad (9).


---

## 📸 Fotografía del Equipo 
<p align="center">
<img width="1408" height="768" alt="imagen_alumnos_IA" src="Recursos/Imágenes/WhatsApp Image 2026-03-17 at 10.03.50 PM.jpeg" />
  <em>Figura 1. Fotografía del equipo 8</em>
</p>

---

## 👥 Integrantes del Equipo  

| Foto | Nombre | Rol | Intereses |
|------|--------|-----|-----------|
| <img src="/Recursos/Imágenes/655903395_943863358260627_6909408214037791066_n.jpg" width="90"/> | **Angello Areche Espeza** | Técnico en prototipado y hardware | Diseño y modulado de prototipos, emsamblaje y soldadura de componentes |
| <img src="/Recursos/Imágenes/Foto Rolando.jpeg" width="90"/> | **Rolando Ronceros Huaynapomas** | Arquitecto del sistema | Diseñar cómo se conectan todos los componentes (sensores, ESP32, app), definir la estructura general del sistema |
| <img src="/Recursos/Imágenes/leslie.foto.jpeg" width="90"/> | **Leslie Stephany Tomanguilla Huaman** | Analista de problemáticas | Identificar problemas actuales y dar soluciones |
| <img src="/Recursos/Imágenes/WhatsApp Image 2026-03-20 at 11.19.52 PM.jpeg" width="90"/> | **Daniela Mori Mendoza** |  Coordinadora de documentación | Gestión, redacción y edición de documentos |
| <img src="/Recursos/Imágenes/alex.jpeg" width="90"/> | **Alex Jhosep Ccoyllo Sotelo** | Programador del sistema | Programación, análisis de datos, desarrollo con ESP32 |

---

## 📌 Resumen Final  
El Equipo 8 está conformado por estudiantes comprometidos con generar un impacto positivo en la sociedad mediante soluciones tecnológicas innovadoras. En esta nueva propuesta, se ha decidido trabajar con los ODS 3, 9 y 11 ,los cuales abordan problemáticas relacionadas con la seguridad ciudadana, el desarrollo de ciudades seguras y la implementación de tecnología para mejorar la calidad de vida.

📑 Referencias Bibliográficas:

*1.* Organización Mundial de la Salud. Lesiones causadas por el tránsito [Internet]. Ginebra: OMS; 2023 [citado 5 abr 2026]. Disponible en: https://www.who.int/es/news-room/fact-sheets/detail/road-traffic-injuries

*2.* Gobierno del Perú. Reporte estadístico de siniestros viales 2022 [Internet]. Lima: Gobierno del Perú; 2022 [citado 5 abr 2026]. Disponible en: https://cdn.www.gob.pe/uploads/document/file/4489498/Reporte%20Estad%C3%ADstico%20de%20Siniestros%20Viales%202022.pdf

*3.* Infocop. Consecuencias psicológicas, físicas y socioeconómicas de los accidentes de tráfico [Internet]. Madrid: Infocop; 2024 [citado 5 abr 2026]. Disponible en: https://www.infocop.es/consecuencias-psicologicas-fisicas-y-socioeconomicas-de-los-accidentes-de-trafico-2/

*4.* Defensoría del Pueblo. Se debe garantizar que espacios y servicios públicos sean accesibles para personas con discapacidad [Internet]. Lima: Defensoría del Pueblo; 2023 [citado 5 abr 2026]. Disponible en: https://www.gob.pe/institucion/defensoria/noticias/685982-defensoria-del-pueblo-se-debe-garantizar-que-espacios-y-servicios-publicos-sean-accesibles-para-personas-con-discapacidad

*5.* Defensoría del Pueblo. Defensoría identifica más de 150 puntos críticos que afectan derechos de personas que transitan por el centro de Lima [Internet]. Lima: Defensoría del Pueblo; 2023 [citado 5 abr 2026]. Disponible en: https://www.defensoria.gob.pe/defensoria-del-pueblo-identifica-mas-de-150-puntos-criticos-que-afectan-derechos-de-personas-que-transitan-por-el-centro-de-lima/

*6.* Infobae. Aumentan los accidentes de tránsito en Perú: más de 1.300 incidentes reportados en 2024 [Internet]. Lima: Infobae; 2024 [citado 5 abr 2026]. Disponible en: https://www.infobae.com/peru/2024/11/03/aumentan-los-accidentes-de-transito-en-peru-mas-de-1300-incidentes-reportados-en-2024/

*7.* Infobae. Atropellos a peatones en Lima se incrementan un 37% en lo que va del 2024 [Internet]. Lima: Infobae; 2024 [citado 5 abr 2026]. Disponible en: https://www.infobae.com/peru/2024/08/17/atropellos-a-peatones-en-lima-se-incrementan-un-37-en-lo-que-va-del-2024/
