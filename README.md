<center>

![Logo Upc](https://www.upc.edu.pe/static/img/logo_upc_red.png "Logo upc")
Universidad Peruana de Ciencias Aplicadas
# Informe de Trabajo Final

</center>


### <center>Aplicaciones Web</center> 
<center>Ciclo: 2025-01</center>
<center>Carrera: Ingenieria de Software</center>  
<center>NRC: 2956</center> 
<center>Profesor: Angel Augusto Velasquez Nuñez</center> 
<center>"INFORME DE TRABAJO FINAL (TP1)"</center> 

### <center>Startup: Bicas team</center>
### <center>Producto: MoviGestion</center>
### Integrantes:

<table >
    <tr>
        <th>Nombre</th>
        <th>Codigo</th>
    </tr>
    <tr>
        <td>Huarcaya Chavez Miguel Alejandro Daniel</td>
        <td>u202116207</td>
    </tr>
    <tr>
        <td>Tarazona Medina Piero Abel</td>
        <td>u202217633</td>
    </tr>
    <tr>
        <td>Elias Torres Espinoza</td>
        <td>u20191A453</td>
    </tr>
    <tr>
        <td>Donayre Peña, Moises Rodolfo</td>
        <td>u202216021</td>
    </tr>
    <tr>
        <td>Chacon Martinez, Mauricio Sebastián</td>
        <td>u202212911</td>
    </tr>
    <tr>
        <td>Valenzuela Huillcaya, Aldhair Johan Juan</td>
        <td>u20201F572</td>
    </tr>
</table >

<center> mayo, 2025</center>

---
---
---

**Registro de Versiones del Informe:**

En esta sección se resumen todas las modificaciones relevantes que sean realizadas sobre el informe durante el ciclo de vida del proyecto.



---
---
---

# Project Report Collaboration Insights
Link de Repositorio: https://github.com/upc-Soluciones-IOT-BicasTeam/upc-iot-BicasTeam-report.git

TB1: En esta etapa, el equipo se reunió para definir el alcance y los objetivos, asignando tareas específicas a cada miembro. Comenzamos recopilando datos y revisando información relevante, con cada miembro contribuyendo con investigaciones individuales que luego compartimos y discutimos en reuniones periódicas. En GitHub, establecimos un flujo de trabajo para colaborar en la redacción del informe, creando un repositorio dedicado con secciones divididas en archivos Markdown para facilitar la colaboración y revisión

![Capturas-TB1](/assets/chapter01/Report%20collaboration/tb1%20collaborators.png)

TP1: Implementamos todo lo investigado en la anterior entrega en una aplicacion web, mas especificamente la capa de presentación. Utilizamos una "fake api" para emular un "back-end" de donde recoger datos y mostrar una simulacion realista de como se veria nuestra aplicacion.
Utilizamos GitHub Pages para desplegar el "front-end" de nuestra aplicación y "beeceptor" para la "fake api".
Po ultimo, corregimos ciertos puntos del figma de la entrega anterior

![Capturas-TP1]()


---
---
---

# Contenido

### [Capítulo I: Introducción](#capítulo-i-introducción-1)

### [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis-1)

---
---
---

# Student Outcome

**El curso contribuye al cumplimiento del Student Outcome ABET:**
**ABET – EAC - Student Outcome** 

Criterio: La capacidad de funcionar efectivamente en un equipo cuyos miembros
juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo,
establecen objetivos, planifican tareas y cumplen objetivos.
En el siguiente cuadro se describe las acciones realizadas y enunciados de
conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro
del ABET – EAC - Student Outcome 5.




---
---
---

# Capítulo I: Introducción
## 1.1 Startup Profile
### 1.1.1 Descripción de la Startup
MoviGestion transforma la gestión de flotas tradicional en una operación inteligente y conectada. Combinamos una plataforma web, una aplicación móvil intuitiva, y la integración de dispositivos IoT para el monitoreo en tiempo real de la ubicación (GPS), temperatura y humedadde la carga y/o vehículo. Maximizamos la eficiencia, aseguramos la integridad de la carga y ofrecemos control total a las empresas de transporte.

Con esta combinación, ayudamos a las empresas de transporte a maximizar la eficiencia operativa, reducir costos, prevenir pérdidas por condiciones ambientales inadecuadas y tomar decisiones basadas en datos precisos. Nuestra plataforma permite una supervisión total del estado de los envíos, vehículos y conductores, con alertas inteligentes configuradas según los requisitos específicos de cada carga, lo que asegura una trazabilidad completa y la integridad del producto en cada etapa del proceso logístico.

Además, ofrecemos un modelo freemium escalable, ideal para empresas que deseen comenzar a digitalizar sus operaciones con la posibilidad de crecer según sus necesidades. Nuestro enfoque dual –administradores y conductores– garantiza que cada usuario cuente con herramientas especializadas y eficientes adaptadas a su rol en la operación.

**Misión**: Proporcionar a las empresas de trasnporte una solución tecnológica integral e inteligente que optimice la gestión de flotas, garantice la integridad de la carga mediante el monitoreo activo y la telemetría avanzada, y mejore la eficiencia operativa y la rentabilidad de nuestros clientes.

**Visión**: Ser la platafoma líder y el socio tecnológico preferido para la gestión inteligente de flotas, impulsando la transformación digital del sector transporte a través de la innovación continua en IoT y análisis de datos para un futuro logístico más eficiente, seguro y sostenible.

### 1.1.2 Perfiles de integrantes del equipo

| Integrante                               | Información                                                                                                                                                                                              | Foto                                                                  |
| :--------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| **Piero Abel Tarazona Medina** | `Código:` U202217633  <br> `Carrera:` Ingeniería de Software <br> Estudiante de 7mo ciclo. Me caracterizo por mi pensamiento crítico y capacidad de encontrar soluciones viables para distintos problemas. Conocimientos en HTML, CSS, C++, Java, Javascript, C#. | <img src="./assets/chapter01/piero.png" alt="Piero" width="150">    |
| **Mauricio Sebastián Chacon Martinez** | `Código:` U202212911 <br> `Carrera:` Ingeniería de Software <br> Apasionado por la programación. Conocimientos en HTML, CSS, Javascript, y Astro. Persona responsable y comprometida con su desarrollo profesional. | <img src="./assets/chapter01/mauricio.png" alt="Mauricio" width="150"> |
| **Miguel Huarcaya Chavez** | `Código:` U202116207 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en JavaScript, TypeScript, HTML, CSS, Vue y Angular. Persona responsable y colaborativa.                                  | <img src="./assets/chapter01/miguel.jpg" alt="Miguel" width="150">    |
| **Elias Torres Espinoza** | `Código:` U20191A453 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en Angular, Vue, TypeScript, JavaScript, C++, C#, Python, HTML y CSS.                                                    | <img src="./assets/chapter01/elias.jpg" alt="Elias" width="150">    |
| **Moises Rodolfo Donayre Peña** | `Código:` U202216021 <br> `Carrera:` Ingeniería de Software <br> Apasionado por el desarrollo web y móvil. Conocimientos en Vue, Angular y Flutter. Persona empática y colaborativa.                     | <img src="./assets/chapter01/moises.png" alt="Moises" width="150">    |
| **Aldhair Johan Juan Valenzuela Huillcaya**| `Código:` U20201F572 <br> `Carrera:` Ingeniería de Software <br> Comunicativo y analítico. Conocimientos en Angular, Vue, React, Flutter y Kotlin.                                                  | <img src="./assets/chapter01/aldahir.png" alt="Aldahir" width="150">  |

## 1.2 Solution Profile
### 1.2.1 Antecedentes y problemática

En el sector del transporte empresarial, la gestión de flotas representa un reto creciente que va más allá de la simple asignación de vehículos y conductores. La complejidad de mantener operaciones eficientes, seguras y rentables se ve agravada por la necesidad de monitorear en tiempo real variables críticas como la ubicación, la temperatura y la humedad, especialmente en cargas sensibles. Muchos sistemas actuales de gestión de fflotas se quedan cortos: carecen de flexibilidad, no ofrecen una integración real con tecnologías IoT y presentan interfaces poco amigables que limitan su adopción por parte de usuarios clave como gerentes de flota y conductores.
Esa falta de soluciones completas genera consecuencias importantes: pérdida de productos por condiciones ambientales no controladas, falta de visibilidad operativa, toma de decisiones reactivas en lugar de proactivas, y una gestión ineficiente de recursos humanos y logísticos. Además, los empresarios y transportistas necesitan herramientas diferenciadas y especializadas que se adapten a sus roles, y que, al mismo tiempo, trabajen en conjunto dentro de un ecosistema digital centralizado.

**Objetivo Principal**:
Desarrollar una solución tecnológica integral, denominada MoviGestion, que transforme la gestión de flotas tradicionales en una operación inteligente, conectada y proactiva, incorporando monitoreo ambiental en tiempo real, analítica avanzada, y funcionalidades especializadas tanto para gerentes como para conductores.

**Objetivos Específicos**:

1. Diseñar una plataforma web robusta orientada a gerentes de flota, que centralice la planificación, seguimiento, y análisis de operaciones logísticas con foco en eficiencia y control ambiental.
2. Desarrollar una aplicación móvil intuitiva para conductores, que facilite la gestión de sus envíos, el reporte de incidentes y el monitoreo de las condiciones de la carga.
3. Integrar tecnología IoT avanzada, que permita el seguimiento en tiempo real de la ubicación GPS, temperatura y humedad de los vehículos y su carga.
4. Incorporar un sistema de alertas preventivas e informes analíticos que permitan tomar decisiones informadas basadas en datos contextuales y actualizados.

**Restricciones**:

1. La plataforma debe ser accesible desde distintos dispositivos, priorizando la experiencia de uso tanto en escritorio como en móvil.
2. Todos los datos transmitidos y almacenados deben cumplir con estándares de seguridad y privacidad.
3. El sistema debe estar preparado para escalar y soportar múltiples usuarios concurrentes sin comprometer la estabilidad ni el rendimiento.

Utilizaremos la técnica de las 5W y 2Hs para desglosar el problema y entenderlo en detalle. Esta técnica nos proporcionará respuestas claras sobre qué, cuándo, dónde, quién, por qué, cómo y cuánto, lo que nos ayudará a encontrar soluciones efectivas.

**Técnica 5Ws y 2Hs**

### Técnica 5Ws y 2Hs

| Elemento      | Pregunta                                                                 | Descripción                                                                                                                                                                                |
|---------------|--------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **What?**     | ¿Cuál es el problema?                                                    | Las empresas de transporte enfrentan una gestión ineficiente de sus flotas, especialmente en lo relacionado al monitoreo ambiental, trazabilidad de envíos y control operativo en tiempo real. |
| **When?**     | ¿Cuándo se manifiesta el problema?                                       | Durante la operación diaria, especialmente en envíos críticos que requieren control ambiental o cuando hay múltiples vehículos y conductores involucrados simultáneamente.                  |
| **Where?**    | ¿Dónde ocurre el problema?                                               | En todo el ciclo de gestión de flotas: asignación de envíos, seguimiento, monitoreo ambiental, control de recursos y comunicación entre gerentes y conductores.                            |
| **Who?**      | ¿A quién afecta el problema?                                             | A los empresarios y gerentes de flota que requieren control y eficiencia, y a los conductores que necesitan herramientas claras para gestionar sus tareas y reportar novedades.            |
| **Why?**      | ¿Por qué sucede el problema?                                             | Por la falta de soluciones integrales que combinen monitoreo ambiental, control en tiempo real, comunicación efectiva y análisis estratégico en una misma plataforma accesible.            |
| **How?**      | ¿Cómo se diferencia del estado óptimo?                                   | En el estado actual, se presentan pérdidas por fallas en el control ambiental, decisiones tardías por falta de datos, y operaciones fragmentadas. El estado óptimo implicaría control total y proactividad. |
| **How much?** | ¿Cuánto impacto genera el problema?                                      | Genera costos adicionales, riesgo de pérdida de carga sensible, baja productividad operativa y menor satisfacción del cliente. MoviGestion busca reducir significativamente ese impacto.   |


### 1.2.2 Lean UX Process

#### 1.2.2.1 Lean UX Problem Statements

El estado actual del sector de gestión de flotas y logística en el Perú se basa principalmente en procesos tradicionales, manuales y sistemas fragmentados. La mayoría de las empresas de transporte pequeñas y medianas aún dependen de herramientas básicas como el GPS o registros en papel para gestionar sus envíos, lo que limita la visibilidad en tiempo real sobre el estado de los vehículos, las condiciones de la carga y la eficiencia de las rutas.
Lo que los productos o servicios existentes no logran resolver es la integración de monitoreo ambiental en tiempo real (temperatura, humedad), coordinación con los conductores y la toma de decisiones basada en datos, todo dentro de una solución accesible, simple y adaptada a las necesidades reales del mercado local. Las soluciones actuales suelen ser costosas, complejas o poco prácticas para empresas de menor escala.
Nuestro producto abordará esta brecha mediante una plataforma integrada que combina un panel web, una aplicación móvil y dispositivos IoT, permitiendo a las empresas de transporte monitorear en tiempo real la ubicación de sus vehículos, las condiciones de la carga y el comportamiento de los conductores. Con esta información, podrán reducir pérdidas, mejorar la seguridad y optimizar su operación logística a través de alertas inteligentes y datos accionables.
Nuestro enfoque inicial será atender a las pequeñas y medianas empresas de transporte en Perú que desean comenzar a digitalizar sus operaciones, pero que no cuentan con los recursos técnicos o financieros para implementar sistemas de gestión de flotas a gran escala.
Sabremos que hemos tenido éxito cuando veamos que estas empresas utilizan activamente nuestra plataforma para monitorear al menos el 80% de su flota en tiempo real, reportan un aumento del 15% en su eficiencia operativa y una reducción en incidentes relacionados a daños en la carga o retrasos por fallas logísticas durante los primeros seis meses de uso.

#### 1.2.2.2 Lean UX Assumptions

1. Bussiness Assumptions
  - Creeemos que las empresas de transporte pequeñas y medianas estarán dispuestas a invertir en una solución digital si esta reduce sus costos logísticos.
  - Creemos que ofrecer una versión gratuita (freemiun) atraerá a empresas interesadas en digitalizar su operación sin un compromiso económico inicial.
  - Creemos que mejorar la trazabilidad y el control de flotas aumentará la reputación de nuestros clientes ante sus propios clientes finales.
2. Outcome Assumptions
  - Creemos que al usar nuestra solución, los usuarios mejorarán su eficiencia operativa al menos en un 15% en los primeros seis meses.
  - Creemos que nuestros usuarios podrán reducir la cantidad de incidencias relacionadas con mal manejo de carga sensible en un 30%.
  - Creemos que contar con monitoreo en tiempo real motivará a los usuarios a tomar decisiones más rápidas y fundamentales ante desvíos o eventos inesperados.
3. User Assumptions
  - Creemos que los administradores logísticos buscan herramientas simples, con buena visualización de datos y alertas automatizadas que les ayudan a anticiparse a problemas.
  - Creemos que los conductores valoran una app que sea intuitiva, con pocas acciones manuales, y que facilite su comunicación con la base.
  - Creemos que ambos perfiles (administradores y conductores) están abiertos a usar tecnología móvil o web siempre que no requiera conocimientos técnicos avanzados.
4. Feature Assumptions
  - Creemos que el rastreo GPS en tiempo real permitirá a los administradores mejorar la supervisión de sus unidades y prevenir desviaciones no autorizadas.
  - Creemos que el monitoreo de temperatura y humedad será especialmente valioso para empresas que transportan alimentos, medicinas u otros productos sensibles.
  - Creemos que las alertas automaticas cuando se detectan variaciones críticas (temperatura, ruta, velocidad) ayudarán a prevenir pérdidas o daños en la carga.
  - Creemos que una app para conductores que incluya geolocalización, recepción de instrucciones y registro de entregas facilitará su trabajo y reducirá errores.
  - Creemos que un panel de control web con visualización de datos en tiempo real facilitará el seguimiento de múltiples vehículos de forma simultánea.
  - Creemos que permitir a los usuarios configurar sus propios umbrales de alerta hará que la plataforma se adapte mejor a diferentes tipos de carga y necesidad operativa.
5. User Outcome Assumptions
  - Creemos que los administradores sentirán mayor control y seguridad al saber en todo momento la ubicación y estado de sus unidades y cargas.
  - Creemos que los conductores se sentirán mas respaldados y organizados al usar una app que centraliza sus instrucciones y tareas diarias.
  - Creemos que nuestros usuarios experimentarán una reducción del estrés y una mejora en la percepción de profesionalismo al digitalizar su operación logística.

#### 1.2.2.3 Lean UX Hypothesis Statements

- **Creemos que lograremos** una reducción del 15% en desvíos no autorizados y tiempos de entrega. **Sí** los administradores de flota **obtienen** un mayor control en tiempo real sobre la ubicación de sus vehículos **con** la funcionalidad de rastreo GPS en tiempo real.
- **Creemos que lograremos** reducir las pérdidas por mal estado de productos sensibles en un 30%. **Sí** las empresas que transportan alimentos, medicinas u otras cargas delicadas **obtienen** la capacidad de prevenir daños por condiciones ambientales inadecuadas **con** el monitoreo en tiempo real de temperatura y humedad.
- **Creemos que lograremos** mejorar la capacidad de reacción ante incidentes logísticos. **Sí** los administradores logísticos **obtienen** notificaciones oportunas para actuar ante desvíos de ruta o cambios críticos en las condiciones de la carga **con** la funcionalidad de alertas automáticas configurables.
- **Creemos que lograremos** una reducción de errores en la ejecución de rutas y entregas. **Sí** los conductores **obtienen** una herramienta centralizada para seguir instrucciones, registrar entregas y ubicarse **con** una aplicación movil intuitiva que incluya geolocalización y tareas asignadas.
- **Creemos que lograremos** una operación logística más ágil y organizada. **Sí** los administradores de operaciones **obtienen** una visualización clara y centralizada del estado de múltiples vehículos en tiempo real **con** un panel web interactivo y actualizado automáticamente.
- **Creemos que lograremos** mayor adopción y satisfacción de los usuarios en distintos sectores logísticos. **Sí** los administradores **obtienen** una herramienta flexible que se adapta a sus necesidades particulares de operación y tipo de carga **con** la posibilidad de configurar umbrales personalizados de alerta.

#### 1.2.2.4 Lean UX Canvas

<table>
<tr>
<td>Business Problem<br><br>El estado actual del sector de gestión de flotas y logística en el Perú se basa principalmente en procesos tradicionales, manuales y sistemas fragmentados. La mayoría de las empresas de transporte pequeñas y medianas aún dependen de herramientas básicas como el GPS o registros en papel para gestionar sus envíos, lo que limita la visibilidad en tiempo real sobre el estado de los vehículos, las condiciones de la carga y la eficiencia de las rutas.
Lo que los productos o servicios existentes no logran resolver es la integración de monitoreo ambiental en tiempo real (temperatura, humedad), coordinación con los conductores y la toma de decisiones basada en datos, todo dentro de una solución accesible, simple y adaptada a las necesidades reales del mercado local. Las soluciones actuales suelen ser costosas, complejas o poco prácticas para empresas de menor escala.
Nuestro producto abordará esta brecha mediante una plataforma integrada que combina un panel web, una aplicación móvil y dispositivos IoT, permitiendo a las empresas de transporte monitorear en tiempo real la ubicación de sus vehículos, las condiciones de la carga y el comportamiento de los conductores. Con esta información, podrán reducir pérdidas, mejorar la seguridad y optimizar su operación logística a través de alertas inteligentes y datos accionables.
Nuestro enfoque inicial será atender a las pequeñas y medianas empresas de transporte en Perú que desean comenzar a digitalizar sus operaciones, pero que no cuentan con los recursos técnicos o financieros para implementar sistemas de gestión de flotas a gran escala.
Sabremos que hemos tenido éxito cuando veamos que estas empresas utilizan activamente nuestra plataforma para monitorear al menos el 80% de su flota en tiempo real, reportan un aumento del 15% en su eficiencia operativa y una reducción en incidentes relacionados a daños en la carga o retrasos por fallas logísticas durante los primeros seis meses de uso.</td>
<td rowspan="2">Solutions<br><br>- Plataforma web modular que permita monitoreo centralizado de vehículos, condiciones de carga y rendimiento de conductores.<br>
- Aplicación móvil para conductores con geolocalización, registro de entregas, incidencias y recepción de instrucciones.<br>
- Integración con sensores IoT para medir temperatura, humedad y ubicación GPS en tiempo real.<br>
- Sistema de alertas inteligentes personalizable según tipo de carga, condiciones de ruta y criterios del usuario.<br>
- Configuración de umbrales críticos y reglas de automatización según la operación logística de cada empresa.<br>
- Visualización de reportes dinámicos y descarga de informes operativos para análisis y toma de decisiones.<br>
- Plan freemium con funcionalidades básicas y opción de escalar a planes pagos con acceso completo.</td>
<td>Business Outcomes<br><br>- Los administradores visualizan el estado de al menos el 80% de su flota en tiempo real desde el panel web.<br>
- Los usuarios configuran alertas automáticas personalizadas para monitoreo ambiental. <br>
- Los conductores registran entregas e incidencias usando la app en al menos el 70% de los trayectos. <br>
- Los usuarios responden a alertas críticas en menos de 15 minutos desde su emisión. <br>
- Los administradores descargan o revisan reportes analíticos semanalmente. <br>
- Las empresas activas registran y monitorean al menos un envío por día en la plataforma. <br>
- Usuarios en plan gratuito comienzan a usar funciones avanzadas en los primeros 10 días.</td>
</tr>
<tr>
<td>Users<br>- Administradores logísticos: Encargados de supervisar envíos, flota y eficiencia operativa.<br>
- Conductores: Ejecutores en campo que necesitan herramientas sencillas e instrucciones claras.<br>
- Empresarios/Propietarios: Tomadores de decisiones que buscan eficiencia, ahorro y trazabilidad.<br></td>
<td>User Outcomes & Benefits<br><br>- Los administradores desean sentirse en control de sus operaciones, tomar decisiones basadas en datos y reducir el riesgo de pérdida de productos.<br>- Los conductores quieren cumplir sus rutas sin complicaciones, sentirse acompañados por la empresa y no tener que depender de instrucciones confusas o procesos manuales.<br>
- Los usuarios quieren una experiencia sin fricciones: que la herramienta sea confiable, clara, y que les permita cumplir su trabajo sin estrés adicional.<br>
- Los usuarios desean ahorrar tiempo en tareas rutinarias como reportes e incidencias. <br>
- Las empresas buscan que su equipo se sienta empoderado y respaldado por la tecnología. <br>
- El uso exitoso de la plataforma debe hacer que los usuarios se sientan más seguros, profesionales y valorados dentro de su organización.</td>
</tr>
<tr>
<td>Hypotheses<br><br>- Creemos que lograremos una reducción del 15% en desvíos no autorizados y tiempos de entrega. Sí los administradores de flota obtienen un mayor control en tiempo real sobre la ubicación de sus vehículos con la funcionalidad de rastreo GPS en tiempo real.<br>
- Creemos que lograremos reducir las pérdidas por mal estado de productos sensibles en un 30%. Sí las empresas que transportan alimentos, medicinas u otras cargas delicadas obtienen la capacidad de prevenir daños por condiciones ambientales inadecuadas con el monitoreo en tiempo real de temperatura y humedad.<br>
- Creemos que lograremos mejorar la capacidad de reacción ante incidentes logísticos. Sí los administradores logísticos obtienen notificaciones oportunas para actuar ante desvíos de ruta o cambios críticos en las condiciones de la carga con la funcionalidad de alertas automáticas configurables.<br>
- Creemos que lograremos una reducción de errores en la ejecución de rutas y entregas. Sí los conductores obtienen una herramienta centralizada para seguir instrucciones, registrar entregas y ubicarse con una aplicación movil intuitiva que incluya geolocalización y tareas asignadas.<br>
- Creemos que lograremos una operación logística más ágil y organizada. Sí los administradores de operaciones obtienen una visualización clara y centralizada del estado de múltiples vehículos en tiempo real con un panel web interactivo y actualizado automáticamente.<br>
- Creemos que lograremos mayor adopción y satisfacción de los usuarios en distintos sectores logísticos. Sí los administradores obtienen una herramienta flexible que se adapta a sus necesidades particulares de operación y tipo de carga con la posibilidad de configurar umbrales personalizados de alerta.</td>
<td>What’s the most important thing we need to learn first?<br><br>- ¿Los administradores y empresarios realmente perciben valor en una solución que combina rastreo, monitoreo ambiental y alertas inteligentes?<br>
- ¿Están dispuestos a cambiar su modelo actual (basado en herramientas tradicionales) por una solución digital como MoviGestion?<br>
- ¿Consideran que este tipo de solución es suficientemente prioritaria como para adoptarla en sus operaciones dentro de los próximos seis meses?<br>
Estas preguntas nos permitirán validar si el problema identificado es realmente significativo y si nuestra solución tiene cabida real en el mercado objetivo.</td>
<td>What’s the least amount of work we need to do to learn the next most important thing?<br><br>- Realizar entrevistas cualitativas con 5–8 administradores logísticos y empresarios.<br>
- Lanzar una encuesta online validando interés y funcionalidades clave.<br>
- Construir un MVP funcional (solo panel + una función de monitoreo + alertas) para 3–5 empresas.<br>
- Medir uso, retroalimentación y percepción de valor en 2 semanas.</td>
</tr>
</table>

## 1.3 Segmento Objetivo

Los segmentos objetivos de MoviGestion son:

**Empresarios**: Este segmento está compuesto por propietarios de empresas que gestionan flotas de transporte en diversos sectores como logística, transporte de mercancías y transporte de pasajeros. Los empresarios, cuyas edades suelen oscilar entre los 30 y los 60 años, pueden ser tanto hombres como mujeres y suelen tener un alto nivel educativo, con títulos en administración de empresas o campos relacionados.

En este contexto, según un informe de Infobae, una empresa de transporte en Perú reveló que el 70% de sus ingresos corresponde a empresas y atienden alrededor de 2 mil empresas mensualmente. Además, un estudio de flotas y movilidad reveló que más de un tercio de las empresas peruanas ya han adaptado o están considerando adaptar su política de movilidad debido al teletrabajo.

<img src="./assets/chapter01/empresarios.jpg" alt="Imagen de Empresarios" width="600" height="400"> <br><br>


**Transportistas**: En el próspero mercado de transporte de carga por carretera en Perú, estimado en 8,31 mil millones de dólares en 2024 y proyectado a crecer a 10,75 mil millones en 2029 con una tasa anual del 6,5%, se encuentra un segmento fundamental: los transportistas. Este grupo, que incluye a conductores y operadores de vehículos de flota, se enfrenta a la necesidad de gestionar eficientemente sus tareas diarias de transporte. Las características demográficas de los transportistas varían ampliamente, con edades que van desde los 20 hasta los 60 años, predominantemente hombres aunque con una creciente presencia femenina. Además, todos ellos requieren licencias de conducir válidas y experiencia en la conducción de vehículos de flota.

<img src="./assets/chapter01/transportista.jpeg" alt="Imagen de Transportistas" width="600" heigth="400"><br><br>


-----
-----
-----
# Capítulo II: Requirements Elicitation & Analysis

## 2.1 Competidores
**TRACK-POD:**
Track-POD se destaca como un software de entrega avanzado que ofrece una experiencia todo en uno para el monitoreo eficiente del rendimiento del conductor y la confirmación de entrega en tiempo real. Su aplicación electrónica de prueba de entrega y su solución móvil proporcionan a los usuarios las herramientas necesarias para optimizar sus operaciones de entrega y mejorar la satisfacción del cliente. Con un enfoque en la simplicidad y la eficacia, Track-POD es una opción sólida para aquellos que buscan mejorar la eficiencia de su cadena de suministro.

**ONFLEET:**
Onfleet ofrece un moderno software de gestión de entregas diseñado para simplificar y optimizar las operaciones de mensajería local. Su plataforma incluye intuitivas aplicaciones de teléfonos inteligentes para conductores, un panel web en tiempo real para distribuidores y notificaciones automáticas por mensajes SMS para mantener a los clientes informados sobre el estado de sus entregas. Con características centradas en la eficiencia y el análisis, Onfleet es una opción confiable para aquellos que buscan una solución completa y fácil de usar para la gestión de entregas. 

**DISPATCH SCIENCE:**
Dispatch Science ofrece un sistema de gestión de entregas integral diseñado para satisfacer las necesidades de expedidores, transportistas y empresas de mensajería. Su plataforma administra, optimiza y automatiza una amplia gama de procesos, incluidos precios, facturación, distribución, enrutamiento y seguimiento en tiempo real. Con un enfoque en la personalización y la escalabilidad, Dispatch Science es una opción ideal para aquellos que buscan una solución flexible y adaptable para la gestión de entregas en constante evolución.

### 2.1.1 Análisis competitivo
**Tabla 3.**<br>
*Análisis Comeptitivo organizado para todos los competidores potenciales de MoviGestion.*
<table border="1">
	<tbody>
		<tr>
			<td colspan="6">Competitive Analysis Landscape</td>
		</tr>
		<tr>
			<td>¿Por qué llevar a cabo este análisis?</td>
			<td colspan="5">El objetivo de este análisis es investigar a detalle las características principales y las propuestas de valor que ofrecen otras empresas que tienen el objetivo de brindar una solución a nuestra misma problemática. Así, podremos encontrar una forma viable y consistente con la que podremos diferenciarnos de ellos.</td>
		</tr>
		<tr>
			<td colspan="2">Empresas</td>
			<td>MoviGestion</td>
			<td>Onfleet</td>
			<td>Track-POD</td>
			<td>Dispatch Science</td>
		</tr>
		<tr>
			<td rowspan="2">Perfil</td>
			<td>Overview</td>
			<td>MoviGestion es una aplicación diseñada específicamente para la gestión eficiente de flotas de transporte en diversos sectores empresariales. Proporciona una amplia gama de herramientas y características para optimizar la operación y el rendimiento de las flotas.</td>
			<td>Onfleet es una plataforma SaaS líder en la gestión de entregas de última milla. Ofrece una solución integral para ayudar a las empresas a gestionar eficientemente sus operaciones de flota.</td>
			<td>Track-POD es un software especializado en la planificación de rutas y recorridos de vehículos, diseñado para maximizar la eficiencia de las entregas y la logística.</td>
			<td>Dispatch Science es un sistema completo de gestión de entregas diseñado para cargadores y transportistas. Simplifica y automatiza la gestión de pedidos, el transporte y el seguimiento en tiempo real.</td>
		</tr>
		<tr>
			<td>Ventaja competitiva</td>
			<td>Se destaca por ofrecer una información detallada sobre la flota, lo que permite un seguimiento preciso del rendimiento a lo largo del tiempo.</td>
			<td>Ofrece a los mensajeros una gestión y análisis eficientes de sus entregas locales, lo que aumenta la eficiencia operativa y la satisfacción del cliente.</td>
			<td>Proporciona una herramienta avanzada de planificación de rutas que simplifica la organización de múltiples entregas y ofrece una aplicación de comprobante de entrega electrónica para los conductores.</td>
			<td>Brinda una solución completa para la gestión de entregas, desde la planificación hasta el seguimiento en tiempo real, lo que optimiza la eficiencia operativa y reduce los costos.</td>
		</tr>
		<tr>
			<td rowspan="2">Perfil de Marketing</td>
			<td>Mercado objetivo</td>
			<td>Se dirige a conductores y empresas que gestionan flotas de transporte en una variedad de sectores empresariales.</td>
			<td>Se enfoca en conductores y empresas involucradas en operaciones de entrega de última milla.</td>
			<td>Está dirigido a conductores y empresas que requieren una planificación eficiente de rutas y logística para sus operaciones de transporte.</td>
			<td>Se centra en cargadores y transportistas que necesitan una solución completa para la gestión de entregas y la logística.</td>
		</tr>
		<tr>
			<td>Estrategias de marketing</td>
			<td>Las estrategias de marketing de MoviGestion incluyen contenido relevante, presencia en el website y en redes sociales, promociones, así como publicidad dirigida para aumentar la visibilidad y la adopción de la aplicación.</td>
			<td>Utiliza estrategias de marketing de contenido, publicidad en línea y redes sociales para promocionar suplataforma y llegar a nuevos clientes.</td>
			<td>Se promociona a través de marketing de contenido, presencia en la web y publicidad en línea para atraer a conductores y empresas interesados en optimizar su logística de entrega.</td>
			<td>Emplea marketing de contenido, publicidad en línea y relaciones públicas para llegar a cargadores y transportistas y demostrar el valor de su plataforma.</td>
		</tr>
		<tr>
			<td rowspan="3">Perfil de Producto</td>
			<td>Productos & Servicios</td>
			<td>MoviGestion ofrece una Aplicación móvil completa para la gestión de flotas, que incluye seguimiento en tiempo real, informes detallados y herramientas de análisis.</td>
			<td>Proporciona una aplicación móvil robusta y una plataforma web para la gestión de entregas, que incluye funciones de seguimiento, notificaciones y análisis.</td>
			<td>Ofrece una aplicación móvil especializada en la planificación de rutas y entregas, junto con una plataforma web para la gestión logística.</td>
			<td>Ofrece una aplicación móvil y una plataforma web integral para la gestión de entregas, que incluye planificación de rutas, seguimiento en tiempo real y generación de informes.</td>
		</tr>
		<tr>
			<td>Precios y Costos</td>
			<td>Presenta distintos planes de pago con distintas funcionalidades para cada versión de pago.</td>
			<td>Ofrece un modelo de precios transparente con una opción gratuita y una versión de pago para empresas con necesidades más avanzadas.</td>
			<td>Proporciona una opción gratuita con funciones básicas y una suscripción premium para acceder a características adicionales y soporte prioritario.</td>
			<td>Ofrece una opción gratuita limitada y una suscripción premium con características completas y soporte dedicado.</td>
		</tr>
		<tr>
			<td>Canales de distribución</td>
			<td>Se distribuye a través de su sitio web oficial.</td>
			<td>Se distribuye mediante plataformas de aplicaciones móviles y su sitio web, garantizando la accesibilidad para los usuarios en diferentes dispositivos.</td>
			<td>Está disponible en plataformas de aplicaciones móviles y en la web, lo que permite a los usuarios acceder desde cualquier dispositivo.</td>
			<td>Se distribuye a través de plataformas de aplicaciones móviles y en la web, asegurando una amplia disponibilidad para los usuarios.</td>
		</tr>
		<tr>
			<td rowspan="4">Análisis SWOT</td>
			<td>Fortalezas</td>
			<td>- Actualizaciones continuas para mejorar la funcionalidad y seguridad.</td>
			<td>- Transparente en cuanto a precios y características
            - Facilita la comunicación entre conductores y despachadores</td>
			<td>- Optimiza las rutas cada día siendo más eficiente
            - Aplicación móvil y plataforma web de fácil uso.</td>
			<td>- Brinda capacidad de administrar todos los aspectos
            - Tiene un valor incomparable</td>
		</tr>
		<tr>
			<td>Debilidades</td>
			<td>- Carece de ciertas características específicas que pueden ser necesarias para algunos usuarios.</td>
			<td>- La optimización de rutas se limita a entregas de última milla y no es adecuada para todos los tipos de transporte.</td>
			<td>- Limitaciones en la cantidad de rutas que pueden ser agregadas simultáneamente.
            - Algunas características pueden ser difíciles de usar para usuarios no técnicos.</td>
			<td>- Algunas características pueden ser difíciles de usar para usuarios no técnicos.
            - Puede ser abrumador para usuarios nuevos debido a la amplia gama de características.</td>
		</tr>
		<tr>
			<td>Oportunidades</td>
			<td>- Expansión hacia áreas adicionales de gestión empresarial, como la gestión de activos y la logística de almacenes.</td>
			<td>- Mejora continua de la experiencia del usuario y la funcionalidad de la plataforma.</td>
			<td>- Crecimiento del mercado de entregas y logística debido al aumento del comercio electrónico y la demanda de servicios de entrega rápida.</td>
			<td>- Oportunidad de expandirse a nuevos mercados verticales y regionales, aprovechando la versatilidad de la plataforma.</td>
		</tr>
		<tr>
			<td>Amenazas</td>
			<td>- Presencia de competidores establecidos con mayor cuota de mercado y recursos. 
            - Rápida evolución de la tecnología que puede requerir actualizaciones frecuentes para mantenerse relevante</td>
			<td>- Competencia de otras plataformas de gestión de entregas establecidas y emergentes. 
            - Otras aplicaciones son más baratas.</td>
			<td>- Posible competencia de soluciones de logística integradas ofrecidas por grandes empresas tecnológicas.</td>
			<td>- Riesgo de imitación por parte de competidores más pequeños y ágiles. 
            - Posible cambio en las regulaciones que afectan el transporte y la entrega.</td>
		</tr>
	</tbody>
</table>

### 2.1.2 Estrategias y tácticas frente a competidores
Se presenta un análisis del panorama competitivo en el que opera MoviGestion, junto con una serie de estrategias y tácticas preliminares diseñadas para enfrentar a los competidores, maximizar el valor para los clientes y posicionar a la startup para el éxito a largo plazo. Al centrarse en la diferenciación, la adaptabilidad, la penetración en el mercado y la colaboración estratégica, MoviGestion puede consolidar su posición como líder innovador en el sector de la gestión de flotas de transporte. 

**1. Diferenciación de Producto:**<br>
**Estrategia:** Destacar las características únicas de la aplicación MoviGestion que la diferencian de la competencia, como la información detallada de la flota y las actualizaciones continuas. <br>
**Tácticas:** Desarrollar campañas de marketing centradas en las características distintivas de MoviGestion. Realizar demostraciones en vivo y ofrecer pruebas gratuitas para mostrar el valor añadido a los clientes potenciales.<br><br>
**2. Mejora Continua y Adaptación:**<br>
**Estrategia:** Mantenerse ágil y adaptable a través de actualizaciones frecuentes y mejoras continuas en la aplicación. <br>
**Tácticas:** Establecer un canal de retroalimentación con los usuarios para recopilar comentarios y sugerencias de mejora. Utilizar métricas de uso y análisis de usuarios para identificar áreas de oportunidad y realizar ajustes rápidos. <br><br>
**3. Penetración de Mercado:**<br>
**Estrategia:** Expandir la base de clientes y aumentar la cuota de mercado a través de una mayor visibilidad y alcance. <br>
**Tácticas:** Implementar campañas de marketing digital dirigidas a sectores específicos, como empresas de logística y transporte. Colaborar con asociaciones y eventos de la industria para aumentar la exposición y el reconocimiento de la marca. <br><br>
**4. Colaboración y Alianzas Estratégicas:**<br>
**Estrategia:** Establecer colaboraciones y alianzas con empresas complementarias para ampliar el alcance y la oferta de servicios. <br>
**Tácticas:** Explorar asociaciones con proveedores de tecnología de la información y servicios de logística para integrar soluciones y ofrecer paquetes combinados. Identificar oportunidades de co-marketing y co-branding para aprovechar la base de clientes existente de los socios. <br><br>
**5. Optimización de Costos y Valor Percibido:**<br> 
**Estrategia:** Ofrecer una propuesta de valor clara y competitiva que combina funcionalidades avanzadas con precios atractivos. <br>
**Tácticas:** Realizar análisis de precios comparativos con la competencia para garantizar que MoviGestion ofrezca un valor superior por el precio. Ofrecer opciones de precios flexibles y descuentos para atraer a nuevos clientes y fomentar la retención de clientes existentes. <br><br>
**6. Desarrollo de Nuevas Funcionalidades y Servicios:** <br>
**Estrategia:** Mantenerse a la vanguardia de la innovación mediante el desarrollo continuo de nuevas funcionalidades y servicios. <br>
**Tácticas:** Realizar investigaciones de mercado y análisis de tendencias para identificar las necesidades emergentes de los clientes. Priorizar el desarrollo de características clave que aborden estas necesidades y proporcionen una ventaja competitiva.

## 2.2 Entrevistas
Según lo aclarado por Folgueiras (2016), la entrevista es un tipo y/o modelo de técnica de recopilación de información, con la cual se busca obtener datos de forma oral y personalizada sobre opiniones, acontecimientos, ideas, experiencias y cualquier otro tipo de información relevante para un objetivo especial, el cual normalmente es para un caso de estudio o para el proyecto de solución de alguna problemática presentada.. Tanto si se elabora dentro de una investigación, como si se diseña al margen de un estudio sistematizado, tiene unas mismas características y pasos a seguir para mantener la base primordial de obtención de información relevante y utilizable para el trabajo.

### 2.2.1 Diseño de entrevistas
Con el fin de obtener y separar correctamente toda la información obtenida durante las entrevistas, se optó por definir un banco de preguntas según nuestro segmento de mercado identificado anteriormente. Este grupo de preguntas está especializado para la obtención de información específica según la persona entrevistada y según la problemática investigada para el proyecto y la posible solución en la forma de nuestro producto. 

**EMPRESARIOS:**
1. ¿Cuál es su nombre y qué edad tiene? ¿En qué distrito vive? 
2. ¿Cuál es su estado civil? Indicar si tienes hijos. 
3. ¿Cuánto tiempo de experiencia tiene en esa función? 
4. ¿Cómo realiza actualmente la gestión de vehículos, conductores y rutas en su	empresa? 
5. ¿Qué herramientas o sistemas utiliza actualmente para administrar su flota de transporte? 
6. ¿Qué funcionalidades le gustaría ver en una herramienta de gestión de flotas ideal?
7. ¿Cómo cree que una solución tecnológica podría mejorar la eficiencia operativa de su empresa en términos de gestión de flotas? 
8. ¿Cuáles son sus preocupaciones principales en cuanto a seguridad y cumplimiento normativo en la gestión de flotas? 
9. ¿Qué impacto cree que tendría una solución de gestión de flotas eficiente en la rentabilidad de su empresa? 
10. ¿Qué tan dispuesto estaría a adoptar una nueva solución tecnológica para la gestión de flotas en su empresa? 
11. ¿Qué características específicas le resultarían más útiles para mejorar la gestión de su flota? 
12. ¿Cómo evaluaría el éxito de una solución de gestión de flotas una vez implementada en su empresa? 
13. ¿Tiene alguna experiencia previa con soluciones similares? ¿Qué lecciones ha aprendido de esa experiencia? 

**TRANSPORTISTAS:**
1. ¿Cuál es su nombre y qué edad tiene? ¿En qué distrito vive? 
2. ¿Cuál es su estado civil? Indicar si tienes hijos. 
3. ¿Para qué empresa trabaja? ¿Y a qué se dedica dentro de la empresa? 
4. ¿Cuánto tiempo de experiencia tiene en esa función? 
5. ¿Qué requisitos pide la empresa para que puedan trabajar en ella? 
6. ¿Cuántos viajes al día realiza un vehículo de la empresa? 
7. ¿Cómo recibe el conductor la información de los viajes que tiene que realizar? 
8. ¿Cómo se comunica la empresa con los conductores de los buses en cualquier momento? 
9. ¿Cómo gestionan los viajes y las rutas que deben realizar los buses? 
10. ¿Cómo gestiona el mantenimiento de los buses y con qué frecuencia se hace dicho proceso? 
11. ¿Qué aspectos cambiaria de la empresa donde trabaja para hacerla más eficiente? 
12. ¿Esta usted familiarizado con el manejo de aplicaciones móviles para el rubro transporte? 
13. ¿Estaría dispuesto a usar alternativas tecnológicas como aplicaciones que le faciliten la gestión de su trabajo? 
14. ¿Qué dispositivos tecnológicos usan en su vida diaria y para el trabajo? 
15. ¿Qué medios (tv, redes sociales, chats con amigos) utiliza para enterarse de nuevas noticias (problemas sociales, oportunidades de negocio, paro de transporte, etc.)? 
16. A lo largo de su experiencia, ¿Cuáles son los principales problemas o dificultades que encuentra en el país que perjudican su trabajo? 
17. Finalmente, ¿En qué planes o proyectos personales se visualiza en el futuro? 

### 2.2.2 Registro de entrevistas
**Segmento 1: EMPRESARIOS**<br>
**Entrevista N°1:**<br>
**Figura 1.**<br>
*Imagen de presentación de la primera entrevista realizada a nuestro primer segmento objetivo.*
![Imagen de presentación de la primera entrevista realizada a nuestro primer segmento objetivo.](/assets/chapter02/entrevista_empresario1.png)
*Nota.* La persona que se encuentra a la derecha es el entrevistador, integrante del grupo, mientras que la persona a la izquierda es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Marco Tarazona
- **Edad:** 57 años
- **Distrito:** Puente Piedra
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
- **Inicio de la entrevista:** 0:00
- **Duración:** 2:10 min
- **RESUMEN:**
- **Demografía (Edad, lugar):** 57 años, Puente Piedra, Lima.  
- **Rol & Experiencia:** Gestor de camiones dedicado al transporte de materiales de construcción; más de 15 años coordinando flotas.  
- **Objetivos / “Jobs”:** Asignar entregas a cada conductor de forma ágil y documentada; minimizar el tiempo invertido en llamadas o mensajes dispersos.  
- **Motivaciones / Valores:** Eficiencia operativa y control transparente de las tareas diarias; disposición a modernizar el negocio si la solución simplifica procesos.  
- **Frustraciones (“Pains”):** La asignación es verbal o por WhatsApp, lo que provoca desorden y poca trazabilidad.  
- **Habilidades (Skills):** Liderazgo operativo, conocimiento de logística de materiales y coordinación básica con herramientas móviles.  
- **Tecnología & Canales:** Smartphone con WhatsApp (principal), sin software formal de gestión aún.  

**Entrevista N°2:**<br>
**Figura 2.**<br>
*Imagen de presentación de la segunda entrevista realizada a nuestro primer segmento objetivo.*
![Imagen de presentación de la segunda entrevista realizada a nuestro primer segmento objetivo.](/assets/chapter02/entrevista_empresario2.png)
*Nota.* La persona que se muestra en la grabación es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Gilver Flores
- **Edad:** 48 años
- **Distrito:** Villa El Salvador
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
- **Inicio de la entrevista:** 2:10 min
- **Duración:** 7:53 min
- **RESUMEN:**
- **Demografía (Edad, lugar):** 48 años, Villa El Salvador, Lima.  
- **Rol & Experiencia:** Empresario; una década gestionando flotas de transporte mixto.  
- **Objetivos / “Jobs”:** Optimizar asignación de rutas, garantizar puntualidad y mantener los buses en óptimas condiciones.  
- **Motivaciones / Valores:** Competitividad, seguridad de pasajeros y reputación corporativa; ve la tecnología como ventaja estratégica.  
- **Frustraciones (“Pains”):** Procesos manuales y falta de visibilidad integral sobre mantenimiento y desempeño.  
- **Habilidades (Skills):** Toma de decisiones basada en KPI, manejo de GPS básico, gestión de personal.  
- **Tecnología & Canales:** WhatsApp para coordinación diaria; rastreo GPS para monitoreo; abierto a apps SaaS de flota.  

**Entrevista N°3:**<br>
**Figura 3.**<br>
*Imagen de presentación de la tercera entrevista realizada a nuestro primer segmento objetivo.*
![Imagen de presentación de la tercera entrevista realizada a nuestro primer segmento objetivo.](/assets/chapter02/entrevista_empresario3.png)
*Nota.* La persona que se muestra en la grabación es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Abraham Quenta
- **Edad:** 28 años
- **Provincia:** Tacna
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
-**Inicio de la entrevista:** 7:53 min
- **Duración:** 16:21 min
- **RESUMEN:**
## Abraham Quenta
- **Demografía (Edad, lugar):** 28 años, Tacna.  
- **Rol & Experiencia:** Emprendedor del rubro transporte; 6 años dirigiendo su propia empresa.  
- **Objetivos / “Jobs”:** Habilitar reservas de asientos en línea y rastrear a conductores en tiempo real.  
- **Motivaciones / Valores:** Cumplir regulaciones de ATU y MTC; ofrecer un servicio moderno y conveniente a los pasajeros.  
- **Frustraciones (“Pains”):** Dependencia de Excel y WhatsApp para operaciones críticas; información dispersa sobre mantenimiento.  
- **Habilidades (Skills):** Gestión básica de datos en Excel, administración de pequeñas operaciones logísticas.  
- **Tecnología & Canales:** Excel para emisión de billetes, WhatsApp para comunicación interna; busca plataforma unificada.

**Segmento 2: TRANSPORTISTAS**<br>
**Entrevista N°1:**<br>
**Figura 4.**<br>
*Imagen de presentación de la primera entrevista realizada a nuestro segundo segmento objetivo.*
![Imagen de presentación de la primera entrevista realizada a nuestro segundo segmento objetivo.](/assets/chapter02/entrevista_transportista1.png)
*Nota.* La persona que se encuentra a la izquierda es el entrevistador, integrante del grupo, mientras que la persona a la derecha es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Ricardo Chate Flores
- **Edad:** 45 años
- **Distrito:** Cercado de Lima
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
- **Inicio de entrevista:** 16:21 min
- **Duración:** 26:26 min
- **RESUMEN:**
- **Demografía (Edad, lugar):** 45 años, Cercado de Lima.  
- **Rol & Experiencia:** Conductor y supervisor de flota en Arellanos; más de 25 años en transporte de personal y turismo.  
- **Objetivos / “Jobs”:** Recibir rutas claras y reportar incidencias sin demora; supervisar cumplimiento de otros conductores.  
- **Motivaciones / Valores:** Orden, puntualidad y buena comunicación con la central.  
- **Frustraciones (“Pains”):** Las rutas le llegan vía secretaria y hay retrasos; coordinar sólo por WhatsApp limita la trazabilidad.  
- **Habilidades (Skills):** Conducción segura, supervisión de flota, uso básico de apps móviles para rutas.  
- **Tecnología & Canales:** Smartphone con WhatsApp y aplicación interna para visualizar rutas asignadas.

**Entrevista N°2:**<br>
**Figura 5.**<br>
*Imagen de presentación de la segunda entrevista realizada a nuestro segundo segmento objetivo.*
![Imagen de presentación de la segunda entrevista realizada a nuestro segundo segmento objetivo.](/assets/chapter02/entrevista_transportista2.png)
*Nota.* La persona que se encuentra a la izquierda es el entrevistador, integrante del grupo, mientras que la persona a la derecha es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Víctor Cuba Bautista
- **Edad:** 42 años
- **Distrito:** Villa el Salvador
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
- **Inicio de entrevista:** 26:26 min
- **Duración:** 31:37 min
- **RESUMEN:**
- **Demografía (Edad, lugar):** 42 años, Villa El Salvador, Lima.  
- **Rol & Experiencia:** Conductor con 25 años en servicio de transporte grupal.  
- **Objetivos / “Jobs”:** Cumplir itinerarios y mantener el bus conforme al calendario de kilometraje.  
- **Motivaciones / Valores:** Calidad de servicio y seguridad de los pasajeros.  
- **Frustraciones (“Pains”):** Comunicación fragmentada; mantenimiento reactivo genera imprevistos.  
- **Habilidades (Skills):** Amplia pericia en conducción, familiaridad con apps de navegación.  
- **Tecnología & Canales:** WhatsApp, GPS integrado, aplicaciones como Uber y Waze para referencias de tráfico. 

**Entrevista N°3:**<br>
**Figura 6.**<br>
*Imagen de presentación de la tercera entrevista realizada a nuestro segundo segmento objetivo.*
![Imagen de presentación de la tercera entrevista realizada a nuestro segundo segmento objetivo.](/assets/chapter02/entrevista_transportista3.png)
*Nota.* La persona que se muestra en la grabación es el entrevistado.

**Datos principales:**
- **Nombre completo del entrevistado:** Martín Merino Ávila
- **Edad:** 50 años
- **Distrito:** Villa el Salvador
- **Link:** https://upcedupe-my.sharepoint.com/entrevistas
- **Inicio de entrevista:** 31:37 min
- **Duración:** 39:39 min
- **RESUMEN:**
- **Demografía (Edad, lugar):** 50 años, Villa El Salvador, Lima.  
- **Rol & Experiencia:** Conductor con 35 años en transporte de personal.  
- **Objetivos / “Jobs”:** Ejecutar rutas programadas con puntualidad y participar en mejoras de flota.  
- **Motivaciones / Valores:** Servicio eficiente y trato cordial al cliente; aspiración a formar su propia flotilla de taxis.  
- **Frustraciones (“Pains”):** Buses antiguos y procesos de comunicación poco ágiles; desea mejor infraestructura para el pasajero.  
- **Habilidades (Skills):** Conducción de larga data, uso práctico de GPS y seguimiento de incidencias.  
- **Tecnología & Canales:** WhatsApp y GPS como herramientas diarias; predispuesto a probar nuevas apps de gestión.  


### 2.2.3 Análisis de entrevistas
**EMPRESARIOS** 
Para el análisis de las entrevistas, se pueden identificar varias características comunes entre los entrevistados que son relevantes para la construcción de los arquetipos de usuarios en el segmento objetivo de empresarios. A continuación, se presenta un análisis de estas características: 
- Todos los entrevistados llevan una media de aproximadamente de 25 años de experiencia. 
- Los entrevistados tienen empresas de transporte que ofrecen servicios tanto para el transporte personal como para el turismo.
- El WhatsApp es el medio de comunicación más utilizado por los empresarios para comunicar a sus trabajadores las rutas y envíos que fueron asignados. 
- Algunos empresarios también utilizan aplicaciones móviles para confirmar que llegó la entrega. 
- El mantenimiento de los buses se realiza de manera preventiva, basado en un calendario establecido por kilometraje. 
- La empresa gestiona el mantenimiento en coordinación con los conductores y el personal de mecánica. 
- Los empresarios están dispuestos a utilizar aplicaciones móviles para mejorar la gestión de su trabajo. 
- Los empresarios están en busca de mejoras en la comunicación dentro de la empresa. 
- La edad de los entrevistados se encuentra en el rango de 30 a 55 años. <br>

**TRANSPORTISTAS** 
Para el análisis de las entrevistas, se pueden identificar varias características comunes entre los entrevistados que son relevantes para la construcción de los arquetipos de usuarios en el segmento objetivo de transportistas. A continuación, se presenta un análisis de estas características: 
- Todos los entrevistados tienen una amplia experiencia como conductores de autobuses, con una media de aproximadamente 28.3 años de experiencia. 
- Los entrevistados trabajan para empresas de transporte que ofrecen servicios tanto para el transporte personal como para el turismo. 
- Además de conducir, algunos entrevistados también tienen roles de supervisión dentro de la empresa. 
- El WhatsApp es el medio de comunicación más utilizado por los conductores para comunicarse tanto entre ellos como con la empresa. 
- Algunos conductores también utilizan aplicaciones móviles para controlar el tiempo de salida y la ubicación de los buses en tiempo real. 
- Los viajes y las rutas son asignados por la empresa, generalmente a través de un programador o una secretaria. 
- Las rutas pueden ser fijas o rotativas, dependiendo de la empresa y las necesidades del servicio. 
- El mantenimiento de los buses se realiza de manera preventiva, basado en un calendario establecido por kilometraje. 
- La empresa gestiona el mantenimiento en coordinación con los conductores y el personal de mecánica. 
- Los conductores están familiarizados y dispuestos a utilizar aplicaciones móviles para mejorar la gestión de su trabajo. 
- Los conductores sugieren mejoras en la comunicación dentro de la empresa y en la calidad del servicio prestado, destacando la importancia del trato al cliente. 
- La implementación de nuevas tecnologías, como aplicaciones que faciliten la gestión de rutas y mantenimiento, es vista como una oportunidad para mejorar la eficiencia en el trabajo. 
- La edad de los entrevistados se encuentra en el rango de 40 a 50 años. 
- La mayoría de nuestros entrevistados reside en el distrito de Villa el Salvador, como también en el Cercado de Lima. Además, el 100% de nuestros entrevistados vive con su familia. 
- El 100% de entrevistados cree que la comunicación debe ser mejorada dentro de la empresa y la consideran vital para un buen desempeño.

## 2.3 Needfinding
Según lo señalado por Patnaik (2017), la metodología del Needfinding se concentra principalmente en la acción de descubrir las necesidades, tanto explícitas como implícitas, de los segmentos objetivos seleccionados con el fin de poder crear soluciones adecuadas. Para esto, es necesario ver más allá de todo lo tangible y concentrarse en ideas más abstractas y conceptos más amigables para todos los usuarios.

Para reconocer las demandas de los usuarios, empleamos diversos enfoques. Primero, segmentamos a los usuarios en diferentes categorías y generamos perfiles que representan a nuestro público objetivo, mediante la creación de User Persona. Esto nos permitió agrupar las necesidades específicas de cada tipo de usuario. Luego, para corroborar y validar las necesidades que habíamos determinado previamente para cada categoría de usuario, realizamos entrevistas con representantes de los dos conjuntos de usuarios que habíamos identificado utilizando los User Persona.

### 2.3.1 User Personas
El proceso de creación de user personas es esencial para comprender las necesidades, desafíos y expectativas de los diferentes segmentos de usuarios en el contexto de nuestra aplicación MoviGestion, que se enfoca en brindar soluciones tecnológicas a academias deportivas. Estas user personas sirven como representaciones ficticias pero realistas de los usuarios reales con los que interactuamos en el ámbito empresarial.

Las fichas de User Persona son herramientas fundamentales para comprender las necesidades, comportamientos y características de los usuarios en un segmento objetivo específico. Estas fichas se basan en el análisis de entrevistas realizadas a conductores de autobuses, así como en la identificación de patrones comunes y aspectos relevantes para la construcción de arquetipos. A través de estas fichas, se representan de manera visual y detallada las características clave de cada User Persona, lo que facilita la comprensión y empatía con los usuarios por parte del equipo de desarrollo y diseño.

**Figura 7.**<br>
*User Persona del primer segmento objetivo: Conductor.*
![User Persona del primer segmento objetivo: Conductor.](/assets/chapter02/user_persona_conductor.png)

**Figura 8.**<br>
*User Persona del segundo segmento objetivo: Empresario.*
![User Persona del segundo segmento objetivo: Empresario.](/assets/chapter02/user_persona_empresario.png)


### 2.3.2 User Task Matrix
Según lo señalado por Patnaik Una Matriz de Tareas de Usuario es una herramienta utilizada en el diseño de experiencia de usuario (UX) y desarrollo de productos para organizar y visualizar las tareas que los usuarios realizan en un sistema o plataforma. Esta matriz ayuda a identificar las diversas acciones que los usuarios llevarán a cabo en el producto, así como la frecuencia y la importancia de cada una de estas tareas (Patnaik, 2017).

**Figura 9.**<br>
*User Task Matrix para el primer y segundo User Persona.*
![User Task Matrix para el primer y segundo User Persona.](/assets/chapter02/user_task_matrix.png)


**Diferencias:** Los empresarios se centran más en tareas relacionadas con la gestión general de la flota, como monitoreo del rendimiento, registro de incidencias y planificación de rutas. 
Los transportistas, por otro lado, se centran en tareas más operativas, como seguimiento de envíos, mantenimiento de vehículos y comunicación con conductores. 
Coincidencias: Ambos grupos reconocen la importancia de la seguridad en la gestión de flotas, lo que se refleja en tareas como el registro de incidencias y la implementación de medidas de seguridad. Tanto los empresarios como los transportistas valoran la eficiencia operativa, como se evidencia en tareas como el monitoreo del rendimiento y la planificación de rutas.

### 2.3.3 User Journey Mapping
Según Patnaik (2017), un Mapeo de Viaje es una técnica utilizada en el diseño de experiencia de usuario (UX) para visualizar y comprender la experiencia que tiene un usuario al interactuar con un producto o servicio a lo largo del tiempo. El proceso de creación de un Journey Map implica mapear los diferentes puntos de contacto entre el usuario y el producto o servicio, desde el inicio hasta la finalización de su interacción. Esto puede incluir todas las etapas del viaje del usuario, desde el descubrimiento inicial del producto hasta la compra, el uso continuo y el soporte posterior a la venta.

**Figura 10.**<br>
*User Journey Map para el primer User Persona.*
![User Journey Map para el primer User Persona.](/assets/chapter02/user_journey_map_conductor.png)

**Figura 11.**<br>
*User Journey Map para el segundo User Persona.*
![User Journey Map para el segundo User Persona.](/assets/chapter02/user_journey_map_empresario.png)

### 2.3.4 Empathy Mapping
Un Mapeo de Empatía es una herramienta utilizada en el diseño de experiencia de usuario (UX) y el desarrollo de productos para comprender mejor las necesidades, deseos, emociones y comportamientos de los usuarios. El objetivo principal del Empathy Mapping es fomentar la empatía entre los miembros del equipo de diseño y los usuarios finales del producto o servicio (Patnaik, 2017).

**Figura 12.**<br>
*User Empathy Map del primer User Persona.*
![User Empathy Map del primer User Persona.](/assets/chapter02/user_empathy_map_conductor.png)

**Figura 13.**<br>
*User Empathy Map del segundo User Persona.*
![User Empathy Map del segundo User Persona.](/assets/chapter02/user_empathy_map_empresario.png)


### 2.3.5 As-is Scenario Mapping
**Figura 14.**<br>
*As-is Scenario Mapping del primer User Persona.*
![As-is Scenario Mapping del primer User Persona.](/assets/chapter02/as_is_scenario_map_conductor.png)

**Figura 15.**<br>
*As-is Scenario Mapping del segundo User Persona.*
![As-is Scenario Mapping del segundo User Persona.](/assets/chapter02/as_is_scenario_map_empresario.png)


## 2.4 Ubiquitous Language
Ubiquitous Language (o Lenguaje Ubicuo) es un conjunto de términos compartidos y consistentes que se utilizan en todo un equipo de desarrollo (diseñadores, programadores, analistas, stakeholders, etc.) para describir el dominio del problema. Es muy común en metodologías como Domain-Driven Design (DDD).

| Término | Definición |
| --- | --- |
| Administrador | Persona encargada de gestionar la academia y supervisar la flota de transporte. |
| Transportista | Encargado de operar los vehículos, realizar rutas y reportar incidencias. |
| Conductor | Persona que conduce los autobuses y está en contacto directo con los atletas. |
| Unidad (Vehículo) | Autobús o transporte asignado para movilizar a los atletas. |
| Ruta | Trayecto predefinido que sigue una unidad para trasladar usuarios. |
| Incidencia | Evento anómalo o problema reportado durante el servicio de transporte. |
| Planificación de Rutas | Proceso de definir y optimizar los recorridos de los vehículos. |
| Panel de Control | Interfaz dentro de la aplicación que muestra métricas y estado de la flota. |