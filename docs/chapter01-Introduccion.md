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

MoviGestión fue diseñada para optimizar la gestión de flotas de transporte mediante una plataforma web y una aplicación móvil que permita a gerentes y conductores gestionar envíos, monitorear condiciones ambientales y mejorar la eficiencia operativa.
Hemos observado que muchas empresas de transporte en Perú aún no han adoptado tecnologías avanzadas de monitoreo en tiempo real, lo que provoca ineficiencias operativas y mayores costos. Por ejemplo, en 2023, la Cámara de Comercio de Lima reportó que las pérdidas por robos y la ineficiencia en las rutas logísticas superaron los 70 millones de dólares, destacando la necesidad de implementar tecnologías como la telemetría y el GPS para mitigar riesgos y mejorar la seguridad en la cadena de suministro.(Cámara de Comercio de Lima, reportado por Business Empresarial, 2023). 
Actualmente, solo un porcentaje limitado de envíos se gestionan con datos precisos en tiempo real sobre la temperatura y humedad, lo que limita la capacidad de tomar decisiones informadas a tiempo.
¿Cómo podemos mejorar la visibilidad y el control de las condiciones ambientales en tiempo real para aumentar en un 15% la eficiencia operativa de las flotas durante los próximos seis meses?

#### 1.2.2.2 Lean UX Assumptions

1. Creo que mis clientes necesitan ________. <br>
**Assumtpion**: Los gerentes de flotas y empresas de transporte en Perú (especialmente aquellos que transportan carga sensible a temperatura/humedad) necesitan una forma más efectiva y accesible de monitorear en tiempo real la ubicación y las condiciones ambientales (temperatura y humedad) de sus envíos y vehículos para reducir pérdidas e ineficiencias.
2. Estas necesidades se pueden resolver con ________ . <br>
**Assumtpion**: Las necesidades identificadas (monitoreo en tiempo real de ubicación y ambiente, gestión de envíos/recursos, reportes, alertas) pueden resolverse eficazmente mediante una combinación de una plataforma web robusta para gerentes, una aplicación móvil intuitiva para conductores y dispositivos IoT instalados en vehículos y/o carga.
3. Mis clientes iniciales son (o serán) _______. <br>
**Assumtpion**: Nuestros clientes iniciales serán principalmente pequeñas y medianas empresas de transporte en Perú que actualmente no usan soluciones integrales de monitoreo ambiental o usan métodos manuales/ineficientes, y que transportan carga donde las condiciones ambientales son un factor crítico.
4. El valor # 1 que un cliente quiere de mi servicio es _______. <br>
**Assumtpion**: El valor principal que buscan nuestros clientes es la reducción de pérdidas de carga sensible y la mejora de la eficiencia operativa a través de la visibilidad y el control proactivo en tiempo real sobre las condiciones ambientales y la ubicación de sus envíos.
5. El cliente también puede obtener estos beneficios adicionales _______ . <br>
**Assumtpion**: Los clientes también valorarán y utilizarán beneficios adicionales como:
- Mejora en la comunicación y organización de los conductores.
- Toma de decisiones más informada basada en datos y estadísticas.
- Reducción de riesgos generales (no solo ambientales, también por ubicación).
- Transparencia y mejor colaboración dentro de la flota (reportes compartidos).
- Gestión centralizada y simplificada de sus recursos (conductores, vehículos, envíos).
6. Voy a adquirir la mayoría de mis clientes a través de _______. <br>
**Assumtpion**: Adquiriremos clientes principalmente a través de estrategias de marketing digital dirigidas al sector logístico en Perú, ventas directas a empresas de transporte, y la tracción generada por el modelo Freemium que permitirá probar la solución.
7. Haré dinero a través de _______. <br>
**Assumtpion**: Generaremos ingresos a través de un modelo de suscripción (PRO), donde los clientes que necesiten más conductores/vehículos o funcionalidades avanzadas pasarán del plan gratuito al de pago.
8. Mi competencia principal en el mercado será _______. <br>
**Assumtpion**: Nuestra competencia principal estará compuesta por proveedores existentes de sistemas de gestión de flotas (TMS) y monitoreo GPS en Perú (que quizás no tengan un enfoque ambiental tan fuerte), empresas que ofrecen soluciones de cadena de frío más tradicionales o puntuales, y el status quo (empresas que usan procesos manuales o básicos).
9. Los venceremos debido a _______. <br>
**Assumtpion**: Venceremos a la competencia debido a nuestra combinación única de monitoreo ambiental por envío, alertas proactivas e inteligentes, una plataforma dual optimizada para gerentes y conductores, un modelo de negocio Freemium accesible, y un enfoque integral que va más allá del simple GPS.
10. Mi mayor riesgo de producto es _______. <br>
**Assumtpion**: Nuestro mayor riesgo de producto es que los dispositivos IoT (sensores de temperatura/humedad) no sean lo suficientemente fiables, precisos o fáciles de instalar/mantener en las condiciones reales del transporte en Perú, o que su costo operativo sea prohibitivo para el cliente objetivo.
11. Resolveremos esto a través de _______. <br>
**Assumtpion**: Resolveremos el problema y construiremos el producto exitosamente a través de un proceso iterativo de desarrollo basado en hipótesis y validación constante con usuarios reales (enfoque Lean Startup / Lean UX).
12. ¿Qué otras suposiciones tenemos? Eso, si se prueba que es falso, causará que nuestro negocio / proyecto no funcione? <br>
- **Assumtpion de Riesgo Crítico #1 (Problema/Valor)**: Las empresas de transporte en Perú realmente perciben la pérdida/daño de carga por variaciones ambientales como un problema lo suficientemente COSTOSO y FRECUENTE como para justificar el pago por una solución de monitoreo en tiempo real como MoviGestion.
- **Assumtpion de Riesgo Crítico #2 (Solución/Usabilidad)**: Los conductores adoptarán y usarán la aplicación móvil de forma consistente para actualizar estados y reportar novedades, y los gerentes encontrarán la plataforma web intuitiva y útil en su operación diaria, a pesar de la posible baja alfabetización digital en algunos segmentos.
- **Assumtpion de Riesgo Crítico #3 (Mercado/Adquisición)**: Podemos alcanzar, convencer y convertir a nuestro cliente objetivo (PYMEs de transporte en Perú) de forma económicamente viable.
- **Assumtpion de Riesgo Crítico #4 (Tecnología/Operación)**: La tecnología IoT (sensores, conectividad, batería) funcionará de manera fiable y a un costo operativo (comunicaciones, mantenimiento) que permita un modelo de suscripción rentable para nosotros y asequible para el cliente.
- **Assumtpion de Riesgo Crítico #5 (Monetización)**: Un porcentaje suficiente de usuarios del plan gratuito migrará al plan PRO.

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
