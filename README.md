# 👥📌Equipo 8 - SafeWalk AI (Zonas de Construcción)
### Carrera de Ingeniería Ambiental / Informática / Industrial  
**Universidad Peruana Cayetano Heredia**

---

## 🌍 Descripción del Equipo 👥

Somos el Equipo 8 del curso Fundamentos de Diseño 2026-1, conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial.  

Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

---

# 🧾 DESCRIPCIÓN DEL PROYECTO

El equipo 8 desarrollará SafeWalk AI, este sistema emplea un módulo de captura visual conectado a una plataforma de procesamiento embebido para la adquisición y análisis de imágenes en tiempo real, sin conexión a internet. Estas imágenes son procesadas mediante un modelo de visión artificial encargado de detectar la presencia de personas con discapacidad visual a partir de elementos característicos como el bastón blanco y las gafas oscuras. Al identificar estos elementos, el sistema activa automáticamente una alerta sonora mediante un altavoz, con el fin de advertir sobre la proximidad de una zona de obra o peligro.

Este proyecto surge como respuesta a la vulnerabilidad de las personas con discapacidad visual en entornos urbanos dinámicos como las zonas de construcción, y contribuye a los Objetivos de Desarrollo Sostenible 3, 9, 10 y 11, promoviendo la seguridad, la innovación tecnológica y la construcción de ciudades más inclusivas.

---

# 🌍 CONTEXTO

El crecimiento de las ciudades peruanas conlleva una ejecución constante de obras de construcción, mantenimiento vial e instalación de servicios públicos que modifican de forma temporal el espacio urbano.En el Perú, la Contraloría General de la República ha identificado que a diciembre de 2025 existen 2,416 obras públicas paralizadas a nivel nacional, siendo Lima uno de los departamentos con mayor número de obras detenidas con 167 proyectos paralizados [1].

Esta situación representa un riesgo especialmente grave para las personas con discapacidad visual. A diferencia del resto de peatones, estas personas se orientan en la ciudad mediante rutas memorizadas, apoyándose en referencias como la cantidad de pasos, la textura del suelo y los sonidos del entorno. Cuando una obra clausura o modifica una vereda, esa ruta memorizada deja de coincidir con la realidad, exponiéndose a caídas. Un estudio del Banco Interamericano de Desarrollo concluyó que las personas con discapacidad visual son las más afectadas por las barreras presentes en el entorno urbano, especialmente en espacios donde la infraestructura cambia de forma temporal e imprevista [2]. 

---

# 📊 EVIDENCIA DEL PROBLEMA

En el Perú, las obras de construcción en espacios urbanos representan un riesgo concreto para los peatones. Según la Organización Internacional del Trabajo, el sector construcción concentra un alto porcentaje de accidentes a nivel mundial, en parte por las condiciones dinámicas y cambiantes de las obras, y por la señalización frecuentemente insuficiente o inadecuada en estos espacios [3].

Esta problemática se vuelve crítica para las personas con discapacidad visual. Los Censos Nacionales 2017 del INEI revelaron que aproximadamente 1,966,766 personas en el Perú experimentan limitaciones permanentes en la visión, de las cuales el 52.6% reside en zonas urbanas [4]. Estas personas se desplazan guiándose por referencias espaciales memorizadas (cantidad de pasos, texturas del suelo, sonidos del entorno) que les permiten construir rutas mentales conocidas. Cuando una obra clausura o modifica temporalmente una vereda, esa ruta memorizada deja de coincidir con la realidad física, exponiéndolas a caídas, colisiones con materiales de construcción o desvíos involuntarios hacia la calzada vehicular.  

Esta realidad no es abstracta. Roxana, una mujer de 56 años con discapacidad visual residente en Arequipa que utiliza el bastón blanco desde hace más de una década, describe con precisión el impacto que tienen las obras en su desplazamiento diario: "Cada vez que se realizan obras en Arequipa, abren el pavimento y lo dejan amontonado: escombros, arena, tierra, ladrillos y cascajos ocupan las veredas. Todo eso representa un obstáculo para desplazarnos. El bastón se nos atasca en esos huecos". Este testimonio refleja una problemática extendida en las ciudades peruanas, donde las intervenciones en la infraestructura urbana no contemplan mecanismos de aviso accesibles para personas invidentes [5]. 


# 💡 JUSTIFICACIÓN DEL PROYECTO

Frente a esta problemática, surge la necesidad de desarrollar soluciones tecnológicas que protejan a las personas con discapacidad visual en zonas de obra. En el Perú, la Norma Técnica A.120 de Accesibilidad Universal del Reglamento Nacional de Edificaciones establece la obligatoriedad de señalización accesible en espacios de construcción, incluyendo señalización podotáctil y auditiva en zonas de riesgo [6]. Sin embargo, su implementación es deficiente: en 2026, el 85% de las inspecciones de CONADIS reportaron incumplimientos en señalética, evidenciando que las normas existentes no se traducen en acciones concretas en los espacios de obra [6]. 

Las medidas tradicionales de seguridad en zonas de obra  (cintas de advertencia, conos de señalización, carteles informativos y barreras físicas) dependen exclusivamente de la percepción visual y no ofrecen ningún tipo de alerta para quienes no pueden verlas. Esta brecha evidencia la necesidad de incorporar soluciones complementarias que utilicen el canal auditivo para transmitir información de riesgo de manera efectiva a las personas invidentes que se aproximan a una zona de obra.

---

# ⚙️ ¿Cómo funciona el proyecto?

## Captura de imágenes
El sistema utiliza un módulo de captura visual integrado en la plataforma de procesamiento embebido, el cual adquiere imágenes del entorno en tiempo real para su análisis inmediato.

## Procesamiento e inferencia
La plataforma embebida recibe y procesa las imágenes mediante un modelo de visión artificial ligero, capaz de detectar elementos característicos de personas con discapacidad visual como el bastón blanco y las gafas oscuras, operando de forma local sin depender de conexión a internet.

## Control del sistema
Una vez procesada la imagen, la plataforma envía señales a una unidad de control que gestiona los dispositivos de salida del sistema, garantizando una respuesta rápida y coordinada.

## Activación de alerta
Al confirmar la detección, se activa automáticamente una alerta sonora que advierte sobre la proximidad de zonas de riesgo.

## Función del sistema
SafeWalk AI busca prevenir accidentes y mejorar la seguridad del peatón con discapacidad visual mediante alertas oportunas, contribuyendo a entornos urbanos más inclusivos y accesibles.


---

# 🌍 OBJETIVOS DE DESARROLLO SOSTENIBLE

Los Objetivos de Desarrollo Sostenible (ODS) son un conjunto de metas globales establecidas por la Organización de las Naciones Unidas como parte de la Agenda 2030 para el Desarrollo Sostenible, adoptada en el año 2015 por los Estados miembros [7]. Estos objetivos buscan orientar los esfuerzos de los países hacia un desarrollo que permita mejorar la calidad de vida de las personas, reducir las desigualdades y proteger el planeta.

# Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

⚕️**ODS 3: Salud y bienestar**

Una de las metas de este objetivo, específicamente la meta 3.6, establece la necesidad de reducir el número de muertes y lesiones causadas por accidentes en entornos de riesgo para el año 2030 [7]. En el contexto urbano, esto implica desarrollar medidas que protejan a los grupos más vulnerables, especialmente en espacios como zonas de construcción, donde existen múltiples peligros asociados a maquinaria, excavaciones y cambios constantes en la infraestructura [8].

Nuestro proyecto se relaciona con este objetivo porque busca reducir el riesgo de accidentes en zonas de construcción para personas con discapacidad visual, contribuyendo a preservar su integridad física y promover su bienestar. 

---

🏭**ODS 9: Industria, innovación e infraestructura**

Una de las metas de este objetivo plantea la necesidad de modernizar la infraestructura e incorporar tecnologías que permitan hacerla más segura, eficiente e inclusiva (9). En el contexto urbano, esto incluye la implementación de sistemas inteligentes capaces de adaptarse a entornos dinámicos como las zonas de construcción.

Nuestro proyecto se vincula con este objetivo porque propone el uso de herramientas tecnológicas como cámaras, inteligencia artificial y algoritmos de detección de objetos en tiempo real para mejorar la seguridad en estos espacios.

---

🤝 **ODS 10: Reducción de las desigualdades**

En muchos casos, las personas con discapacidad enfrentan dificultades para desplazarse en el entorno urbano debido a la falta de infraestructura accesible, especialmente en espacios temporales como zonas de obra. Estas limitaciones generan una brecha en el acceso seguro al espacio público.

De acuerdo con la Organización Mundial de la Salud, una gran proporción de la población mundial presenta algún tipo de discapacidad, lo que evidencia la necesidad de desarrollar soluciones inclusivas que mejoren su calidad de vida [7].
Nuestro proyecto se relaciona con este objetivo porque busca reducir estas barreras mediante el uso de tecnología. A través de la detección en tiempo real de personas con discapacidad visual y la generación de alertas auditivas en zonas de construcción.

---

🏙️**ODS 11: Ciudades y comunidades sostenibles**

Una de las metas de este objetivo está relacionada con mejorar la seguridad y accesibilidad de los espacios urbanos, garantizando que estos sean inclusivos para todos los ciudadanos, especialmente los grupos más vulnerables [7].

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

**1.** Contraloría General de la República del Perú. Informe de obras públicas paralizadas en el territorio nacional a diciembre 2025. https://cdn.www.gob.pe/uploads/document/file/9416533/7715417-informe-de-obras-publicas-paralizadas-en-el-territorio-nacional-a-diciembre-2025f.PDF  

**2.** Rodríguez Porcel M, Lee S, Sandoval D, Tascón Valencia J, Jaramillo PJ, Pedraza L. Auditoría georreferenciada y diagnóstico de accesibilidad peatonal de personas con discapacidad en la primera y última milla de un viaje. https://publications.iadb.org/es/auditoria-georreferenciada-y-diagnostico-de-accesibilidad-peatonal-de-personas-con-discapacidad-en  

**3.** Organización Internacional del Trabajo. Seguridad y salud en la construcción. https://www.ilo.org/es/resource/otros/seguridad-y-salud-en-la-construccion-edicion-revisada  

**4.** Instituto Nacional de Estadística e Informática. Perfiles sociodemográficos de la población con discapacidad https://www.inei.gob.pe/media/MenuRecursivo/publicaciones_digitales/Est/Lib1675/libro.pdf  

**5.** Radio Yaráví Arequipa. Personas con discapacidad visual enfrentan desafíos en calles de Arequipa. https://radioyaravi.org.pe/noticia/informes-especiales/personas-con-discapacidad-visual-enfrentan-desafios-en-calles-de-arequipa/  

**6.** Seminario-Hurtado N, Alfaro Torres HM. Accesibilidad en entornos urbanos para personas con discapacidad visual en el Perú: un análisis normativo. https://revistas.javeriana.edu.co/index.php/cvyu/article/view/41190/ 

**7.** World Health Organization. World Report on Disability. 2011. https://www.who.int/publications/i/item/9789241564182 

**8.** International Labour Organization. Safety and Health in Construction. 2022. https://www.ilo.org/global/publications/books/WCMS_159358/lang--en/index.htm 

**9.** OSHA. Construction Industry Standards. 2024. https://www.osha.gov/laws-regs/regulations/standardnumber/1926 


