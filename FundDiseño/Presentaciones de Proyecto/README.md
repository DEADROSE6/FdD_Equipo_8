# SafeWalk AI

**Curso:** Fundamentos de Diseño  
**Grupo:** 08

---

> *"Imagina que memorizaste cada paso de tu camino al trabajo. Sabes exactamente cuántos pasos hay hasta la esquina, la textura del piso, los sonidos del entorno. Un día, una obra de construcción cambia todo eso... y nadie te avisa."*

---

## Problema

En el Perú, más de 1.9 millones de personas tienen limitaciones permanentes en la visión, y más de la mitad vive en zonas urbanas [1]. Cuando una obra altera una vereda, sus rutas memorizadas dejan de coincidir con la realidad, exponiéndolas a accidentes. La señalización actual es insuficiente y poco accesible [2]. Nadie las avisa sobre los riesgos en su camino.

**¿Cómo podemos advertir de manera oportuna a una persona con discapacidad visual cuando se aproxima a una zona de construcción que representa un riesgo para su seguridad?**

---

## Solución

SafeWalk AI detecta en tiempo real a personas con bastón blanco en zonas de construcción y les emite una alerta sonora automática antes de que lleguen al peligro.

| Característica | Descripción |
|---|---|
| **Accesible** | Utiliza alertas sonoras, un medio de comunicación adecuado para usuarios con limitaciones visuales. |
| **Autónomo** | Funciona de manera automática sin requerir intervención de operadores o personal de la obra. |
| **Eficiente** | Detecta en tiempo real la presencia de personas con discapacidad visual y genera alertas oportunas. |
| **Asequible** | Emplea hardware embebido de bajo costo, facilitando su implementación en diferentes zonas de construcción. |

---

## Propuesta de Valor

### ¿Por qué SafeWalk AI es mejor que los competidores existentes?

No existe un sistema equivalente en el mercado peruano para obras urbanas.

Los sistemas de asistencia para invidentes que existen (apps como BlindSquare, bastones inteligentes) están orientados al usuario individual, no al entorno.

**¿Cómo se está abordando el problema ahora?**
- Conos y cachacos
- Cintas de advertencia
- Vigilantes humanos

**¿Qué ofrecemos nosotros?**

SafeWalk AI les da a las empresas constructoras una herramienta concreta, portátil y de bajo costo para cumplir con su obligación legal de garantizar entornos accesibles [5], protegiendo al mismo tiempo al más de un millón de personas con discapacidad visual que viven en zonas urbanas del Perú.

### Análisis de la competencia

| Competidor | Geografía | Orientado al público | Precios | Usabilidad |
|---|---|---|---|---|
| *(Competidor 1)* | Países de Asia, Medio Oriente y Europa | Alto | — | 4/5 |
| *(Competidor 2)* | Nivel mundial | Medio | — | 4.5/5 |

---

## Modelo de Negocio

### ¿Cómo generamos ingresos?

Nuestro modelo se basa en el **alquiler por obra**. SafeWalk AI se instala directamente sobre el cachaco existente y se cobra por el tiempo que dura la construcción. Esto lo hace accesible para cualquier obra, grande o pequeña, y nos permite escalar rápidamente.

### Monetización, precio y canales

- **Precio:** S/. 300 a S/. 500 mensuales por dispositivo, incluyendo inversión, mano de obra, traslado y mantenimiento.
- **Validación:** Buscaremos el respaldo de CONADIS para abrir puertas con empresas constructoras.
- **Sostenibilidad:** El dispositivo se reutilizará en cada obra, haciendo el modelo sostenible y escalable.

---

## Estrategia

### ¿Quiénes son nuestros clientes?

- **Corto plazo:** Empresas constructoras
- **Largo plazo:** Municipalidades / Empresas de señalización vial

### ¿Cómo llegaríamos a ellos?

1. Llegamos a la empresa constructora mediante una **prueba piloto gratuita** en una obra real de Lima a cambio de retroalimentación, validando el sistema en el campo.
2. Presentamos SafeWalk AI a **CONADIS** para obtener su aval como herramienta de accesibilidad.

---

## Tracción

### ¿Qué hemos logrado?

- **Carcasa en PLA** diseñada e impresa en 3D con sistema de montaje para cachacos.
- **Modelo entrenado** con 500 imágenes con 2 clases de detección.
- **Prototipo funcional** del sistema de detección con XIAO ESP32S3 y Roboflow.

---

## Equipo

Un equipo con habilidades complementarias: desde el componente físico hasta el software, pasando por el análisis y la documentación. Todo cubierto internamente.

| Integrante | Rol |
|---|---|
| Areche Espeza, Angello | Construye y ensambla el hardware del sistema |
| Ronceros Huaynapomas, Rolando | Diseña cómo se conecta todo: hardware, software y flujo de datos |
| Tomanguilla Huaman, Leslie | Asegura que las soluciones respondan al problema real |
| Mori Mendoza, Daniela | Mantiene toda la documentación clara y organizada |
| Ccoyllo Sotelo, Alex | Programa la lógica e inteligencia del sistema |

---

## Pedido

### ¿Qué necesitamos para dar el siguiente paso?

1. **Acceso a una obra real en Lima** para validar el sistema en el campo.
2. **Apoyo para ampliar nuestro dataset** a 2,000 imágenes y superar el 80% de precisión.
3. **Alianzas con empresas de señalización vial o municipalidades** para una prueba piloto oficial.

---

## Referencias

1. Instituto Nacional de Estadística e Informática. Perfiles sociodemográficos de la población con discapacidad [Internet]. Lima: INEI; 2019 [citado 2026]. Disponible en: https://www.inei.gob.pe/media/MenuRecursivo/publicaciones_digitales/Est/Lib1675/libro.pdf

2. Organización Internacional del Trabajo. Seguridad y salud en la construcción. Edición revisada [Internet]. Ginebra: OIT; 2022 [citado 2026]. Disponible en: https://www.ilo.org/es/resource/otros/seguridad-y-salud-en-la-construccion-edicion-revisada

3. Congreso de la República del Perú. Ley N° 29973: Ley General de la Persona con Discapacidad [Internet]. Lima: Congreso de la República; 2012 [citado 2026 jun 26]. Disponible en: https://www.gob.pe/institucion/conadis/informes-publicaciones/223512-ley-general-de-la-persona-con-discapacidad-y-su-reglamento


