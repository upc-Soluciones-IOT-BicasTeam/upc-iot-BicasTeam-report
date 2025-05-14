# Chapter 1
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
| **Piero Abel Tarazona Medina** | `Código:` U202217633  <br> `Carrera:` Ingeniería de Software <br> Estudiante de 7mo ciclo. Me caracterizo por mi pensamiento crítico y capacidad de encontrar soluciones viables para distintos problemas. Conocimientos en HTML, CSS, C++, Java, Javascript, C#. | <img src="../assets/chapter01/piero.png" alt="Piero" width="150">    |
| **Mauricio Sebastián Chacon Martinez** | `Código:` U202212911 <br> `Carrera:` Ingeniería de Software <br> Apasionado por la programación. Conocimientos en HTML, CSS, Javascript, y Astro. Persona responsable y comprometida con su desarrollo profesional. | <img src="../assets/chapter01/mauricio.png" alt="Mauricio" width="150"> |
| **Miguel Huarcaya Chavez** | `Código:` U202116207 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en JavaScript, TypeScript, HTML, CSS, Vue y Angular. Persona responsable y colaborativa.                                  | <img src="../assets/chapter01/miguel.jpg" alt="Miguel" width="150">    |
| **Elias Torres Espinoza** | `Código:` U20191A453 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en Angular, Vue, TypeScript, JavaScript, C++, C#, Python, HTML y CSS.                                                    | <img src="../assets/chapter01/elias.jpg" alt="Elias" width="150">    |
| **Moises Rodolfo Donayre Peña** | `Código:` U202216021 <br> `Carrera:` Ingeniería de Software <br> Apasionado por el desarrollo web y móvil. Conocimientos en Vue, Angular y Flutter. Persona empática y colaborativa.                     | <img src="../assets/chapter01/moises.png" alt="Moises" width="150">    |
| **Aldhair Johan Juan Valenzuela Huillcaya**| `Código:` U20201F572 <br> `Carrera:` Ingeniería de Software <br> Comunicativo y analítico. Conocimientos en Angular, Vue, React, Flutter y Kotlin.                                                  | <img src="../assets/chapter01/aldahir.png" alt="Aldahir" width="150">  |

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
Nuestro producto/servicio abordará esta brecha mediante una plataforma integrada que combina un panel web, una aplicación móvil y dispositivos IoT, permitiendo a las empresas de transporte monitorear en tiempo real la ubicación de sus vehículos, las condiciones de la carga y el comportamiento de los conductores. Con esta información, podrán reducir pérdidas, mejorar la seguridad y optimizar su operación logística a través de alertas inteligentes y datos accionables.
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
<td>Business Problem<br><br>En el sector del transporte empresarial, la gestión eficiente de las flotas es un desafío constante. Los empresarios y transportistas a menudo utilizan múltiples herramientas y procesos manuales para gestionar sus flotas debido a la falta de soluciones integradas. Esta gestión descentralizada de flotas puede llevar a ineficiencias operativas, aumento de costos y reducción de la satisfacción del cliente.
Además, los cambios en el mercado y el comportamiento del cliente están aumentando la demanda de soluciones de gestión de flotas más eficientes y fáciles de usar. Los empresarios y transportistas necesitan una solución que les permita tener una visibilidad completa de sus flotas, controlar los costos operativos, identificar áreas de mejora y adaptarse rápidamente a los cambios.
Sin embargo, muchas de las soluciones de software existentes para la gestión de flotas no satisfacen todas estas necesidades. Pueden ser difíciles de usar, no ofrecer todas las funciones necesarias o no ser lo suficientemente flexibles para adaptarse a las necesidades específicas de cada empresa.
Por lo tanto, el problema empresarial que MoviGestion está tratando de resolver es la falta de una solución de gestión de flotas integral, flexible y fácil de usar que pueda satisfacer todas las necesidades de los empresarios y transportistas en el sector del transporte empresarial. MoviGestion aspira a llenar esta brecha en el mercado proporcionando una solución tecnológica que simplifique y optimice la gestión de flotas de transporte.</td>
<td rowspan="2">Solutions<br><br>Algunas soluciones que podrían resolver el problema comercial y satisfacer las necesidades de los clientes al mismo tiempo: <br>
1. Interfaz de Usuario Intuitiva: Desarrollar una interfaz de usuario que sea fácil de navegar y usar. Esto puede incluir tutoriales interactivos, asistencia en la aplicación y una interfaz de usuario limpia y minimalista.<br>
2. Funcionalidades Avanzadas de Gestión de Flotas: Implementar una variedad de características para la gestión de flotas, como estadísticas de rendimiento, reporte de infracciones, registro de incidencias, seguimiento de envíos exitosos y control de sitios enviados. Estas características deben ser personalizables para adaptarse a las necesidades específicas de cada empresa.<br>
3. Informes Personalizables: Proporcionar informes detallados y personalizables que ayuden a los empresarios a tomar decisiones informadas. Esto puede incluir análisis de costos, informes de rendimiento y análisis de tendencias.<br>
4. Seguridad de Datos: Garantizar la seguridad y privacidad de los datos de los usuarios. Esto puede incluir el uso de encriptación de datos, autenticación de dos factores y políticas de privacidad claras.<br>
5. Soporte al Cliente: Ofrecer soporte al cliente de alta calidad para ayudar a los usuarios a resolver problemas y responder a preguntas. Esto puede incluir chat en vivo, soporte por correo electrónico y una base de conocimientos en línea.<br>
6. Integraciones con Otras Plataformas: Permitir la integración con otras plataformas y herramientas que los usuarios ya estén utilizando. Esto puede facilitar la adopción de la plataforma y mejorar la eficiencia operativa.<br>
7. Planes de Suscripción Flexibles: Ofrecer planes de suscripción flexibles que se adapten a las necesidades y al tamaño de cada empresa. Esto puede incluir planes gratuitos, planes premium y opciones de personalización.</td>
<td>Business Outcomes<br>Para MoviGestion, los resultados comerciales pueden ser medidos a través de varias métricas clave que indican el éxito del cliente y la resolución del problema comercial.
1. Eficiencia Operativa: Medir la mejora en la eficiencia operativa de las flotas de transporte de los usuarios. Esto podría ser a través de la reducción en el tiempo de inactividad de los vehículos, el aumento en el número de envíos exitosos, o la disminución en el tiempo necesario para planificar y programar los viajes.<br>
2. Reducción de Costos: Medir la reducción en los costos operativos de los usuarios. Esto podría ser a través de la disminución en los costos de combustible, mantenimiento, o infracciones.<br>
3. Satisfacción del Cliente: Medir la satisfacción del cliente a través de encuestas y comentarios. Esto podría incluir la facilidad de uso de la plataforma, la utilidad de las características ofrecidas, y la calidad del soporte al cliente.<br>
4. Retención de Usuarios: Medir la tasa de retención de usuarios. Un aumento en la retención de usuarios indica que los usuarios encuentran valor en la plataforma y continúan utilizándola a largo plazo.<br>
5. Crecimiento de Usuarios: Medir el crecimiento en el número de usuarios o empresas que utilizan la plataforma. Esto indica que la plataforma está ganando tracción en el mercado.<br>
6. Uso de la Plataforma: Medir el uso de las diferentes características de la plataforma. Esto puede ayudar a identificar qué características son más valiosas para los usuarios y dónde se pueden hacer mejoras.</td>
</tr>
<tr>
<td>Users<br><br>Para MoviGestion, los usuarios y clientes pueden ser categorizados de la siguiente manera:<br>
1. Empresarios: Son los que probablemente comprarán el servicio. Son los propietarios de empresas que necesitan administrar sistemas de transporte. Estos usuarios estarán interesados en las capacidades de gestión de flotas de la plataforma, así como en las estadísticas de rendimiento y los informes detallados que pueden ayudarles a tomar decisiones informadas.<br>
2. Transportistas: Son los usuarios finales que utilizarán la plataforma a diario. Estos usuarios buscan eficiencia y organización en sus operaciones de transporte. Necesitarán funciones como el registro de incidencias, el seguimiento de envíos exitosos y el control de sitios enviados.<br>
3. Administradores de sistemas: Son los que configuran y mantienen la plataforma. Estos usuarios necesitarán acceso a funciones de administración y configuración para asegurarse de que la plataforma se adapta a las necesidades específicas de su empresa.<br>
4. Analistas de datos: Estos usuarios podrían estar interesados en los datos recopilados por la plataforma para realizar análisis y generar informes que ayuden a la empresa a tomar decisiones estratégicas.</td>
<td>User Outcomes & Benefits<br><br>1.Eficiencia Operativa Mejorada: Al utilizar MoviGestion, los usuarios pueden mejorar la eficiencia de sus operaciones de transporte. Esto se traduce en un mejor uso de los recursos, menos tiempo perdido en tareas administrativas y más tiempo para centrarse en el crecimiento del negocio.<br>
2. Reducción de Costos: MoviGestion puede ayudar a los usuarios a reducir costos al proporcionar herramientas para optimizar el uso de la flota, reducir el tiempo de inactividad y minimizar las infracciones.<br>
3. Toma de Decisiones Informada: Con los informes detallados y las estadísticas de rendimiento que ofrece MoviGestion, los usuarios pueden tomar decisiones más informadas sobre la gestión de su flota.<br>
4. Satisfacción del Cliente Mejorada: Al mejorar la eficiencia y la fiabilidad de las operaciones de transporte, los usuarios pueden mejorar la satisfacción de sus propios clientes.</td>
</tr>
<tr>
<td>Hypotheses<br><br>1. Creemos que la eficiencia operativa se logrará si los empresarios obtienen una mejor visibilidad y control de sus flotas con la funcionalidad avanzada de gestión de flotas.<br>
2. Creemos que la reducción de costos se logrará si los transportistas obtienen una mayor eficiencia en sus operaciones de transporte con el registro de incidencias y el seguimiento de envíos exitosos.<br>
3. Creemos que la satisfacción del cliente se logrará si los desarrolladores obtienen una plataforma adaptable a las necesidades específicas de su empresa con las funciones de administración y configuración.<br>
4. Creemos que la retención de usuarios se logrará si los desarolladores, analistas de datos obtienen informes detallados y personalizables con la función de informes personalizables.<br>
5. Creemos que el crecimiento de usuarios se logrará si los empresarios obtienen una plataforma fácil de adoptar y que mejora la eficiencia operativa con la integración con otras plataformas.<br>
6. Creemos que el uso de la plataforma se incrementará si los usuarios obtienen un soporte al cliente de alta calidad con el soporte al cliente ofrecido.<br>
7. Creemos que la mejora en la eficiencia operativa se conseguirá si los empresarios obtienen una toma de decisiones más informada con la función de informes detallados y estadísticas de rendimiento ofrecidos en los planes de suscripción flexibles de MoviGestion.</td>
<td>What’s the most important thing we need to learn first?<br><br>En las etapas iniciales de nuestro proyecto, es crucial identificar los supuestos más riesgosos en nuestras hipótesis. Esto nos permite enfocarnos en mitigar esos riesgos y validar nuestras ideas de manera efectiva.<br>1.El supuesto más riesgoso asociado con la Hipótesis 1 es que los empresarios realmente necesiten y valoren una funcionalidad avanzada de gestión de flotas.<br>
2. El supuesto más riesgoso asociado con la Hipótesis 2 es que los transportistas encuentren útil y mejoren su eficiencia con el registro de incidencias y el seguimiento de envíos exitosos.<br>
3. El supuesto más riesgoso asociado con la Hipótesis 3 es que los administradores de sistemas necesiten y utilicen funciones de administración y configuración.<br>
4. El supuesto más riesgoso asociado con la Hipótesis 4 es que los analistas de datos necesiten y utilicen informes detallados y personalizables.<br>
5. El supuesto más riesgoso asociado con la Hipótesis 5 es que los empresarios estén dispuestos a adoptar una nueva plataforma y que esta mejore su eficiencia operativa.<br>
6. El supuesto más riesgoso asociado con la Hipótesis 6 es que los usuarios valoren y utilicen el soporte al cliente ofrecido.<br>En esta etapa inicial del proyecto, nuestro enfoque se centra en identificar y mitigar los riesgos para valorar en lugar de en la viabilidad absoluta de cada hipótesis. Esto nos permite abordar los desafíos más críticos y validar nuestras ideas de manera efectiva.El supuesto más riesgoso en este momento se relaciona con la Hipótesis 1, donde la necesidad y valoración real de una funcionalidad avanzada de gestión de flotas por parte de los empresarios podrían determinar el éxito o el fracaso de nuestra solución. Si este supuesto resulta ser incorrecto, nuestra idea principal de proporcionar una solución de gestión de flotas integral, flexible y fácil de usar podría fracasar.</td>
<td>What’s the least amount of work we need to do to learn the next most important thing?<br><br>Para validar nuestra suposición más arriesgada, que los empresarios realmente necesitan y valoran una funcionalidad avanzada de gestión de flotas, proponemos los siguientes experimentos con la menor cantidad de trabajo posible:<br>
1. Entrevistas con Empresarios: Realizaremos entrevistas con un pequeño grupo de empresarios en el sector del transporte. Durante estas entrevistas, preguntaremos sobre sus necesidades actuales, los desafíos que enfrentan con las soluciones existentes y qué características valorarían en una nueva solución. Esto nos permitirá validar si realmente necesitan y valorarían una funcionalidad avanzada de gestión de flotas.<br>
2. Encuestas: Diseñaremos una encuesta corta y la enviaremos a un grupo más amplio de empresarios. La encuesta incluirá preguntas sobre sus necesidades actuales, los desafíos que enfrentan y qué características les gustaría ver en una nueva solución de gestión de flotas.<br>
3. Producto Mínimo Viable (MVP): Desarrollaremos un MVP que incluya la funcionalidad avanzada de gestión de flotas y lo proporcionaremos a un pequeño grupo de empresarios para que lo prueben. Recogeremos sus comentarios y observaremos cómo utilizan el MVP para validar nuestra suposición.<br>
El objetivo de estos experimentos es aprender lo más rápido posible con la menor cantidad de trabajo. Por lo tanto, hemos diseñado nuestros experimentos de manera que podamos obtener resultados rápidamente y hacer ajustes según sea necesario."</td>
</tr>

</table>

## 1.3 Segmento Objetivo

Los segmentos objetivos de MoviGestion son:

**Empresarios**: Este segmento está compuesto por propietarios de empresas que gestionan flotas de transporte en diversos sectores como logística, transporte de mercancías y transporte de pasajeros. Los empresarios, cuyas edades suelen oscilar entre los 30 y los 60 años, pueden ser tanto hombres como mujeres y suelen tener un alto nivel educativo, con títulos en administración de empresas o campos relacionados.

En este contexto, según un informe de Infobae, una empresa de transporte en Perú reveló que el 70% de sus ingresos corresponde a empresas y atienden alrededor de 2 mil empresas mensualmente. Además, un estudio de flotas y movilidad reveló que más de un tercio de las empresas peruanas ya han adaptado o están considerando adaptar su política de movilidad debido al teletrabajo.

![Imagen de Empresarios](/assets/chapter01/empresarios.jpg)

<!-- CÓDIGO PARA MODIFICAR EL TAMAÑO <img src="https://delcorp.pe/wp-content/uploads/2017/07/motorizado_inhousev2.jpg" alt="Imagen de Empresarios" width="400" height="350"> -->

**Transportistas**: En el próspero mercado de transporte de carga por carretera en Perú, estimado en 8,31 mil millones de dólares en 2024 y proyectado a crecer a 10,75 mil millones en 2029 con una tasa anual del 6,5%, se encuentra un segmento fundamental: los transportistas. Este grupo, que incluye a conductores y operadores de vehículos de flota, se enfrenta a la necesidad de gestionar eficientemente sus tareas diarias de transporte. Las características demográficas de los transportistas varían ampliamente, con edades que van desde los 20 hasta los 60 años, predominantemente hombres aunque con una creciente presencia femenina. Además, todos ellos requieren licencias de conducir válidas y experiencia en la conducción de vehículos de flota.

![Imagen de Transportistas](/assets/chapter01/transportista.jpeg)
