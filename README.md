# Equipo 8 - Fundamentos de Diseño
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1 , conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial. 

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# DESCRIPCION

El equipo 8 desarrollará SafeWalk AI, un sistema inteligente de alerta para peatones que previene accidentes en cruces urbanos mediante sensores, visión artificial con ESP32-CAM e IoT.

El sistema detecta peatones distraídos, evalúa su comportamiento en tiempo real y clasifica el nivel de riesgo, activando alertas visuales, sonoras y mensajes en pantalla solo cuando es necesario.

Además, registra datos en Micro SD para análisis básico de patrones.

Asimismo, el proyecto incorpora un enfoque inclusivo, ya que brinda asistencia a personas con discapacidad visual mediante alertas sonoras en el cruce, y a personas con discapacidad auditiva mediante la conexión con una aplicación móvil que envía vibraciones y notificaciones en tiempo real, permitiendo advertir situaciones de riesgo de manera accesible.

Este proyecto contribuye a los ODS 3, 9 y 11, promoviendo la seguridad vial, la innovación tecnológica y el desarrollo de ciudades más inclusivas y seguras.

---

# PROBLEMÁTICA

En el Perú, los accidentes de tránsito constituyen una de las principales problemáticas de seguridad pública, especialmente en zonas urbanas como Lima, donde el alto flujo vehicular y peatonal incrementa el riesgo de atropellos.

Una de las causas más frecuentes es la distracción de los peatones, principalmente por el uso del celular al momento de cruzar la vía, lo que reduce su capacidad de reacción ante situaciones de peligro.

A esto se suma la falta de infraestructura tecnológica en los cruces peatonales, ya que la mayoría de semáforos son sistemas tradicionales que no responden al comportamiento en tiempo real de las personas.

Esta situación evidencia la necesidad de implementar soluciones inteligentes que permitan detectar riesgos y alertar oportunamente a los peatones, contribuyendo así a la reducción de accidentes y a la mejora de la seguridad vial en el país.

---

# PROPUESTA DE SOLUCIÓN

Como solución a esta problemática, se propone el desarrollo de SafeWalk AI, un sistema inteligente de alerta para peatones que integra sensores de movimiento, medición de distancia y visión artificial mediante ESP32-CAM, junto con conectividad IoT.

Este sistema busca prevenir accidentes en cruces urbanos, detectando situaciones de riesgo en tiempo real y generando alertas accesibles.

Además, incorpora un enfoque inclusivo al brindar asistencia tanto a peatones distraídos como a personas con discapacidad visual y auditiva, mediante alertas sonoras, visuales y notificaciones móviles.

Su diseño compacto, basado en una estructura impresa en 3D, permite su implementación como un prototipo funcional y escalable hacia ciudades inteligentes.

---

# ¿Cómo funciona el proyecto?

## Detección
Sensores (PIR y ultrasónico) identifican la presencia y proximidad de peatones.

## Análisis
La ESP32-CAM captura imágenes y evalúa el comportamiento del peatón (ej. distracción por celular).

## Clasificación
El sistema determina el nivel de riesgo: seguro, sospechoso o peligro.

## Respuesta
Se activan alertas según el nivel de riesgo:

- Luces tipo semáforo  
- Sonido (buzzer)  
- Mensajes en pantalla  

## Accesibilidad

- Alertas sonoras para personas con discapacidad visual  
- Notificaciones y vibración mediante app móvil para personas con discapacidad auditiva  

## Registro de datos

Se almacenan datos en Micro SD para análisis y mejora del sistema.

---

# Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

⚕️**ODS 3: Salud y bienestar**

Hoy en día, caminar por la ciudad supone un riesgo real para nuestra salud y tranquilidad. Los accidentes de tránsito no solo golpean nuestra integridad física, sino que nos llenan de estrés y miedo al salir a la calle. La OMS ya lo advierte: las muertes viales son una crisis global que afecta, sobre todo, a los peatones y a los más vulnerables. En el Perú esto se vive a diario. Tenemos un tránsito caótico y zonas donde la señalización brilla por su ausencia, lo que multiplica el peligro. Nuestro proyecto ataca justamente esto: queremos advertir al usuario que hay peligro a su alrededor. Al anticipar el riesgo, reducimos las cifras de lesiones y, lo más importante, le devolvemos a la gente la confianza para moverse segura por su ciudad.

 🏭**ODS 9: Industria, innovación e infraestructura**
 
La tecnología ya no tiene que ser una megaobra de infraestructura para generar impacto. En vez de sentarnos a esperar a que toda la ciudad se llene de pavimento podotáctil, creemos que la innovación debe ser personal, inmediata y caber en nuestro día a día. Nuestro proyecto lleva la seguridad directamente a los objetos que ya usamos. Combinamos sensores, conectividad e inteligencia artificial para crear algo más que un simpl; estamos diseñando tecnología que lee el entorno en tiempo real y toma decisiones rápidas para proteger al usuario en la calle.

🏙️**ODS 11: Ciudades y comunidades sostenibles**

El gran reto de nuestras ciudades es crecer sin dejar a nadie atrás. Para una persona con discapacidad visual, auditiva o con déficit de atención, cruzar una avenida transitada puede ser una verdadera odisea. En el Perú, la falta de accesibilidad en las calles es evidente y esto le roba la autonomía a miles de ciudadanos así mismo limitando su vida cotidiana. Aquí es donde nuestra tecnología actúa como un puente hacia la inclusión real. El dispositivo emite alertas a la medida de cada persona  ya sea mediante vibraciones, sonidos o mensajes visuales  para guiarla en medio del caos urbano. Al final, el objetivo de este proyecto trasciende la seguridad vial: se trata de darle a cualquier persona el mismo derecho a disfrutar, acceder y recorrer su ciudad con total libertad.


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
| <img src="/Recursos/Imágenes/655903395_943863358260627_6909408214037791066_n.jpg" width="90"/> | **Angello Areche Espeza** | Líder del equipo | Innovación social, temas ambientales, organización de proyectos |
| <img src="/Recursos/Imágenes/Foto Rolando.jpeg" width="90"/> | **Rolando Ronceros Huaynapomas** | Responsable de investigación | Medio ambiente, trabajo con comunidades, búsqueda de información |
| <img src="/Recursos/Imágenes/leslie.foto.jpeg" width="90"/> | **Leslie Stephany Tomanguilla Huaman** | Diseñadora |Diseño de prototipos, creatividad, ideas prácticas |
| <img src="/Recursos/Imágenes/WhatsApp Image 2026-03-20 at 11.19.52 PM.jpeg" width="90"/> | **Daniela Mori Mendoza** |  Encargada de la documentación | Redacción, organización de información, elaboración de informes |
| <img src="/Recursos/Imágenes/alex.jpeg" width="90"/> | **Alex Jhosep Ccoyllo Sotelo** | Programador/a - Modelador/a | Programación, análisis de datos, desarrollo con ESP32 |

---

## 📌 Resumen Final  
El Equipo 8 está conformado por estudiantes comprometidos con generar un impacto positivo en la sociedad mediante soluciones tecnológicas innovadoras. En esta nueva propuesta, se ha decidido trabajar con los ODS 3, 9 y 11 ,los cuales abordan problemáticas relacionadas con la seguridad ciudadana, el desarrollo de ciudades seguras y la implementación de tecnología para mejorar la calidad de vida.
