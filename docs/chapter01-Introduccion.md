# Chapter 1
## 1.1 Startup Profile
### 1.1.1 Descripción de la Startup
MoviGestion transforma la gestión de flotas tradicional en una operación inteligente y conectada. Combinamos una plataforma web, una aplicación móvil intuitiva, y la integración de dispositivos IoT para el monitoreo en tiempo real de la ubicación (GPS), temperatura y humedadde la carga y/o vehículo. Maximizamos la eficiencia, aseguramos la integridad de la carga y ofrecemos control total a las empresas de transporte.

Con esta combinación, ayudamos a las empresas de transporte a maximizar la eficiencia operativa, reducir costos, prevenir pérdidas por condiciones ambientales inadecuadas y tomar decisiones basadas en datos precisos. Nuestra plataforma permite una supervisión total del estado de los envíos, vehículos y conductores, con alertas inteligentes configuradas según los requisitos específicos de cada carga, lo que asegura una trazabilidad completa y la integridad del producto en cada etapa del proceso logístico.

Además, ofrecemos un modelo freemium escalable, ideal para empresas que deseen comenzar a digitalizar sus operaciones con la posibilidad de crecer según sus necesidades. Nuestro enfoque dual –administradores y conductores– garantiza que cada usuario cuente con herramientas especializadas y eficientes adaptadas a su rol en la operación.

**Misión**: Proporcionar a las empresas de trasnporte una solución tecnológica integral e inteligente que optimice la gestión de flotas, garantice la integridad de la carga mediante el monitoreo activo y la telemetría avanzada, y mejore la eficiencia operativa y la rentabilidad de nuestros clientes.

**Visión**: Ser la platafoma líder y el socio tecnológico preferido para la gestión inteligente de flotas, impulsando la transformación digital del sector transporte a través de la innovación continua en IoT y análisis de datos para un futuro logístico más eficiente, seguro y sostenible.

### 1.1.2 Perfiles de integrantes del equipo

| Integrante | Información | Foto |
|------------|-------------|------|
| **Piero Abel Tarazona Medina** | `Código:` U202217633  <br> `Carrera:` Ingeniería de Software <br> Estudiante de 7mo ciclo. Me caracterizo por mi pensamiento crítico y capacidad de encontrar soluciones viables para distintos problemas. Conocimientos en HTML, CSS, C++, Java, Javascript, C#. | ![Piero](/assets/chapter01/piero.png) |
| **Mauricio Sebastián Chacon Martinez** | `Código:` U202212911 <br> `Carrera:` Ingeniería de Software <br> Apasionado por la programación. Conocimientos en HTML, CSS, Javascript, y Astro. Persona responsable y comprometida con su desarrollo profesional. | ![Mauricio](/assets/chapter01/mauricio.png) |
| **Miguel Huarcaya Chavez** | `Código:` U202116207 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en JavaScript, TypeScript, HTML, CSS, Vue y Angular. Persona responsable y colaborativa. | ![Miguel](/assets/chapter01/miguel.jpg) |
| **Elias Torres Espinoza** | `Código:` U20191A453 <br> `Carrera:` Ingeniería de Software <br> Conocimientos en Angular, Vue, TypeScript, JavaScript, C++, C#, Python, HTML y CSS. | ![Elias](/assets/chapter01/elias.jpg) |
| **Moises Rodolfo Donayre Peña** | `Código:` U202216021 <br> `Carrera:` Ingeniería de Software <br> Apasionado por el desarrollo web y móvil. Conocimientos en Vue, Angular y Flutter. Persona empática y colaborativa. | ![Moises](/assets/chapter01/moises.png) |
| **Aldhair Johan Juan Valenzuela Huillcaya** | `Código:` U20201F572 <br> `Carrera:` Ingeniería de Software <br> Comunicativo y analítico. Conocimientos en Angular, Vue, React, Flutter y Kotlin. | ![Aldahir](/assets/chapter01/aldahir.png) |



## 1.2 Solution Profile
### 1.2.1 Antecedentes y problemática

En el sector del transporte empresarial, la gestión eficiente de las flotas es un desafío constante. Los empresarios y transportistas se enfrentan a dificultades como la planificación de rutas, el seguimiento de vehículos, la programación de viajes y la gestión de costos. Aunque existen soluciones de software para la gestión de flotas, muchas de ellas no son lo suficientemente flexibles o integrales para satisfacer todas las necesidades de los usuarios.
La falta de una solución de gestión de flotas integral y fácil de usar está afectando la eficiencia operativa, aumentando los costos y reduciendo la satisfacción del cliente en el sector del transporte empresarial.

**Objetivo Principal**:
Desarrollar una plataforma web integral, MoviGestion, que simplifique y optimice la gestión de flotas de transporte para empresarios y transportistas.

**Objetivos Específicos**:

1. Interfaz de Usuario Amigable: Proporcionar una interfaz de usuario intuitiva que facilite la navegación y el uso de la plataforma.
2. Funcionalidades Complejas: Ofrecer una variedad de características útiles para la gestión de flotas, incluyendo estadísticas de rendimiento, reporte de infracciones, registro de incidencias, seguimiento de envíos exitosos y control de sitios enviados.
3. Informes Detallados: Proporcionar informes detallados que ayuden a los empresarios a tomar decisiones informadas.

**Restricciones**:

1. La plataforma debe ser desarrollada como una aplicación web para garantizar la accesibilidad en diferentes dispositivos.
2. Todos los datos de los usuarios deben ser almacenados de manera segura para proteger su privacidad.
3. La plataforma debe ser capaz de manejar un gran número de usuarios simultáneamente sin afectar su rendimiento.

Utilizaremos la técnica de las 5W y 2Hs para desglosar el problema y entenderlo en detalle. Esta técnica nos proporcionará respuestas claras sobre qué, cuándo, dónde, quién, por qué, cómo y cuánto, lo que nos ayudará a encontrar soluciones efectivas.

**Técnica 5Ws y 2Hs**

| Las 5Ws y 2Hs | Pregunta                                                    | Descripción                                                                                                                                                                       |
| ------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| What?         | ¿Cuál es el problema?                                       | Existe una falta de eficiencia en la gestión de flotas de transporte empresarial, lo que resulta en costos elevados y disminución de la satisfacción del cliente.                 |
| When?         | ¿Cuándo estamos viendo el problema?                         | Este problema se observa principalmente durante las horas pico de operación, cuando la demanda de transporte es alta y la planificación de rutas se vuelve más compleja.          |
| Where?        | ¿Dónde estamos viendo los problemas?                        | El problema se presenta en todo el proceso de gestión de flotas, desde la planificación de rutas hasta el seguimiento de vehículos y la programación de viajes.                   |
| Who?          | ¿A quién le sucede?                                         | Este problema afecta tanto a los empresarios que necesitan administrar sistemas de transporte como a los transportistas que buscan una organización eficiente en sus operaciones. |
| Why?          | ¿Por qué sucede el problema?                                | El problema surge debido a la falta de una solución de gestión de flotas integral y fácil de usar que pueda satisfacer todas las necesidades de los usuarios.                     |
| How?          | ¿Cómo se diferencia el problema del estado normal (óptimo)? | El problema se manifiesta en forma de costos operativos elevados, retrasos en las entregas, insatisfacción del cliente y dificultades en la planificación de rutas.               |
| How much?     | ¿Cuánto es el impacto financiero?                           | El problema podría estar costando a las empresas miles de dólares cada mes en costos operativos adicionales y pérdida de clientes debido a la insatisfacción.                     |

### 1.2.2 Lean UX Process

#### 1.2.2.1 Lean UX Problem Statements

A pesar de la existencia de soluciones de software para la gestión de flotas, muchas de ellas no satisfacen todas las necesidades de los usuarios en el sector del transporte empresarial. Los empresarios y transportistas se enfrentan a una brecha en el mercado: la falta de una solución de gestión de flotas integral, flexible y fácil de usar. Esta brecha está afectando la eficiencia operativa, aumentando los costos y reduciendo la satisfacción del cliente.

En MoviGestion, nuestra visión es llenar esta brecha proporcionando una solución tecnológica integral que simplifique y optimice la gestión de flotas de transporte. Nos comprometemos a ofrecer herramientas innovadoras y servicios de alta calidad que ayuden a nuestros usuarios a mejorar la eficiencia operativa, reducir costos y garantizar la satisfacción del cliente. Nuestro objetivo inicial es servir a los empresarios y transportistas que buscan una solución integral para la gestión de flotas de transporte.

#### 1.2.2.2 Lean UX Assumptions

1. Contexto: Los empresarios y transportistas a menudo utilizan múltiples herramientas y procesos manuales para gestionar sus flotas debido a la falta de soluciones integradas.
   Assumption: Dado que muchos usuarios enfrentan dificultades con la gestión descentralizada de flotas, creemos que existe una necesidad de una plataforma integral que unifique todas las funciones de gestión de flotas en una sola solución.
2. Contexto: Los empresarios a menudo luchan por controlar los costos operativos y reducir los gastos innecesarios en la gestión de flotas.
   Assumption: Dado que el control de costos es una prioridad para los usuarios, creemos que una solución que ofrezca herramientas de análisis de costos y optimización de recursos será altamente valorada.
3. Contexto: La falta de informes detallados y análisis de datos dificulta la identificación de áreas de mejora en la gestión de flotas.
   Assumption: Dado que los usuarios necesitan información precisa y detallada sobre el rendimiento de sus flotas, creemos que una solución que proporcione informes personalizables y análisis avanzados será fundamental para la toma de decisiones informadas.
4. Contexto: La seguridad y privacidad de los datos son preocupaciones críticas para los usuarios al adoptar nuevas soluciones tecnológicas.
   Assumption: Dado que los usuarios son sensibles a la seguridad de los datos, creemos que una solución que garantice la protección y privacidad de la información del cliente será fundamental para generar confianza y adopción.
5. Contexto: Los usuarios a menudo enfrentan dificultades para adaptarse a nuevas tecnologías y plataformas debido a la complejidad y la curva de aprendizaje.
   Assumption: Dado que la facilidad de uso es crucial para la adopción de la plataforma, creemos que una solución intuitiva y fácil de usar será fundamental para la aceptación y satisfacción del usuario.

#### 1.2.2.3 Lean UX Hypothesis Statements

- **Creemos que** al ofrecer una plataforma integral que unifique todas las funciones de gestión de flotas en una sola solución, aumentaremos la eficiencia y la productividad de los empresarios y transportistas al reducir la complejidad y la fragmentación en sus procesos de gestión, **sabremos que** estamos en lo correcto **cuando** veamos un aumento en el número de usuarios que reportan una reducción significativa en el tiempo dedicado a la gestión de flotas, así como una disminución en los errores asociados con la gestión descentralizada.
- **Creemos que** el control de costos es una prioridad para los usuarios, por lo tanto, cuando proporcionemos herramientas de análisis de costos y optimización de recursos, aumentaremos la capacidad de los empresarios para controlar los gastos operativos y reducir los costos innecesarios en la gestión de flotas **sabremos que** estamos en lo correcto **cuando** observemos un aumento en la adopción de las herramientas de análisis de costos, así como una disminución en los costos operativos reportados por los usuarios.
- **Creemos que** al proporcionar informes personalizables y análisis avanzados sobre el rendimiento de las flotas, permitiremos a los usuarios identificar áreas de mejora y tomar decisiones informadas para optimizar sus operaciones y aumentar la eficiencia de sus flotas **sabremos que** estamos en lo correcto **cuando** recibamos comentarios positivos de los usuarios sobre la utilidad de los informes y análisis proporcionados, así como cuando observemos una mejora en los indicadores clave de rendimiento de las flotas gestionadas a través de nuestra plataforma.
- **Creemos que** al garantizar la protección y privacidad de la información del cliente en nuestra plataforma, generaremos confianza en los usuarios y promoveremos una mayor adopción de nuestra solución de gestión de flotas **sabremos que** estamos en lo correcto **cuando** observemos un aumento en la confianza y la satisfacción del usuario, así como una disminución en las preocupaciones relacionadas con la seguridad de los datos expresadas por los usuarios.
- **Creemos que** al ofrecer una solución intuitiva y fácil de usar, aumentaremos la aceptación y satisfacción del usuario al reducir la curva de aprendizaje y facilitar la adaptación a nuevas tecnologías y plataformas en el sector del transporte empresarial **sabremos que** estamos en lo correcto **cuando** observemos una disminución en las tasas de abandono del producto, así como un aumento en la tasa de retención de usuarios y una mayor participación en las funciones ofrecidas por la plataforma.

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
