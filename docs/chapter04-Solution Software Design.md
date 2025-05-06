# Chapter 04: Solution Software Design
## 4.1 Strategic-Level Domain-Driven Design
### 4.1.1 EventStorming
Event Storming es una herramienta que nos permite descubrir el comportamiento de un negocio, recopilando eventos importantes del negocio, los actores principales, servicios de terceros y otros. Para la implementación de esta sección se realizaron entrevistas correspondientes a los segmentos objetivos, de esta manera pudimos identificar los eventos principales y desarrollar un entendimiento común

Aquí mostramos los pasos respectivos para la elaboración correcta del Event Storming realizada en la herramienta Lucidchart:

**Paso 1: Unstructured Exploration**
En esta sección se realizó una lluvia de ideas de los eventos del dominio relacionados con el dominio empresarial que se está explorando. Nos permitió identificar los eventos clave y las interacciones entre ellos.

![Paso1](/assets/chapter04/unstructured_exploration.png)

**Paso 2: Timelines**
En esta sección, los eventos identificados previamente, son agrupados en subgrupos lo cual tiene como líder al evento principal (es quien encapsula la funcionalidad principal del grupo). Estos eventos comienzan con el flujo que describe el escenario empresarial exitoso (Happy path) y también escenarios alternativos.

![Paso2](/assets/chapter04/timelines.png)

**Paso 3: Paint Points**
Durante esta fase, identificamos puntos problemáticos o (Pair Points) que son áreas donde los usuarios pueden tener dificultades al momento de realizar una respectiva funcionalidad en la aplicación. Estos puntos son importantes para mejorar la experiencia de usuario e implementar una aplicación eficiente

![Paso3](/assets/chapter04/paint_points.png)

**Paso 4: Pivotal Points**
En esta fase, nos enfocamos en identificar los puntos cruciales dentro del flujo del negocio, los cuales tienen un impacto significativo en la operatividad del sistema o el comportamiento del usuario. Estos puntos nos ayudan a priorizar qué áreas deben ser optimizadas o revisadas con mayor detalle, ya que pueden afectar el éxito de los procesos empresariales críticos.

![Paso4](/assets/chapter04/pivotal_points.png)

**Paso 5: Commands**
Los comandos representan acciones que los actores del sistema pueden ejecutar. Durante este paso, mapeamos qué acciones desencadenan los eventos clave dentro del sistema y qué actores son responsables de ejecutarlas. Esto nos ayuda a estructurar la lógica de negocio alrededor de acciones claras y específicas, facilitando la implementación de las reglas del negocio

![Paso5](/assets/chapter04/commands.png)

**Paso 6: Policies**
En este paso, se identifican las políticas, que son reglas de negocio o condiciones que deben cumplirse para que un comando pueda ser ejecutado o un evento pueda suceder. Las políticas son esenciales para definir las restricciones del sistema y asegurar que el flujo de eventos sea coherente con las reglas del negocio.

![Paso6](/assets/chapter04/policies.png)

**Paso 7: Read Models**
Los Read Models son vistas del estado del sistema, generalmente optimizadas para la consulta por parte de los usuarios o procesos. Durante este paso, definimos qué información necesita ser accesible en ciertos momentos y cómo debería ser presentada, asegurando que los actores puedan visualizar el estado del sistema de manera eficiente.

![Paso7](/assets/chapter04/read_models.png)

**Paso 8: External Systems**
En esta fase, identificamos los sistemas externos que interactúan con nuestro dominio. Aquí mapeamos las conexiones con servicios de terceros o sistemas independientes que influyen en los eventos del negocio. Es crucial entender cómo estos sistemas externos afectan los flujos y asegurar que las integraciones sean correctas.

![Paso8](/assets/chapter04/external_systems.png)

**Paso 9: Aggregates**
En este último paso, agrupamos los eventos y comandos que pertenecen a un agregado específico para garantizar que todas las operaciones dentro de un contexto estén alineadas y mantengan la consistencia del sistema.

![Paso9](/assets/chapter04/aggregates.png)

#### 4.1.1.1 Candidate Context Discovery
Nuestro equipo decidió usar la técnica “start-with-simple” ya que empezamos a observar que esta técnica se enfoca en identificar partes del sistema que claramente pertenecen juntas desde el punto de vista funcional, de usuario o de infraestructura. Ideal para sistemas bien entendidos

Hemos identificado 4 Bounded Context.

- IAM:
![IAM](/assets/chapter04/IAM.png)

- Vehicles & Tracking:
![Vehicles & Tracking](/assets/chapter04/vehicles_tracking.png)

- Shipment:
![Shipment](/assets/chapter04/shipment.png)

- Analytics:
![Analytics](/assets/chapter04/analytics.png)

Link de Lucidchart:
https://lucid.app/lucidchart/c3a56cf0-cb3f-4aa2-a9fb-b84400e5ec12/edit?viewport_loc=-11645%2C-2705%2C13687%2C7929%2C0_0&invitationId=inv_c09779ac-741d-4f3e-9d56-15a2f9117ad9

#### 4.1.1.2 Domain Message Flows Modeling
En esta sección, se describe el proceso utilizado para visualizar la interacción entre los diferentes bounded contexts que conforman el sistema. El objetivo principal es entender cómo estos contextos colaboran para resolver los casos de uso del negocio y satisfacer las necesidades de los usuarios. Para lograr esto, se aplicó la técnica de Domain Storytelling, que facilita la representación gráfica de los flujos de mensajes entre actores, contextos y sistemas, permitiendo identificar claramente las responsabilidades y los puntos de comunicación entre cada componente del dominio

- IAM -> Vehicles & Tracking
![IAM -> Vehicles & Tracking](/assets/chapter04/IAM_to_vehicles_tracking.png)

- IAM -> Analytics
![IAM -> Analytics](/assets/chapter04/IAM_to_analytics.png)

- IAM -> Shipment
![IAM -> Shipment](/assets/chapter04/IAM_to_shipment.png)

#### 4.1.1.3 Bounded Context Canvases
En esta parte del documento se describen las acciones realizadas por el equipo para estructurar los bounded contexts que fueron reconocidos a lo largo del proceso. El desarrollo de estos contextos fue llevado a cabo de forma iterativa, garantizando que cada uno representa fielmente los principios de diseño y el conocimiento del dominio. Para cada bounded context, se llevaron a cabo los siguientes pasos principales:

- Definición General del Contexto: Se establecieron tanto el propósito como los límites de cada contexto, asegurando su coherencia con el ámbito del negocio.
- Identificación de Reglas de Negocio y Lenguaje Común: Se extrajeron las principales reglas de negocio y se documentó el lenguaje compartido, con el objetivo de facilitar la comunicación entre los miembros del equipo.
- Análisis de Capacidades: Se examinaron las funcionalidades que debía ofrecer cada contexto.
- Organización por Capas: Cuando fue necesario, se implementó una estructura por capas para las capacidades definidas.
- Identificación de Dependencias: Se detectaron las relaciones y conexiones con otros contextos y sistemas externos.
- Revisión del Diseño: Se evaluó la arquitectura propuesta para garantizar un bajo acoplamiento y su alineación con los objetivos estratégicos del negocio.

Gracias a este enfoque, el equipo pudo construir los bounded contexts de forma sólida, asegurando que cada uno cumpliera con su función dentro del sistema global.

- Bounded Context Canvases IAM:
![Bounded Context Canvases IAM](/assets/chapter04/canvases_IAM.png)

- Bounded Context Canvases Vehicles & Tracking:
![Bounded Context Canvases Vehicles & Tracking](/assets/chapter04/canvases_vehicles_tracking.png)

- Bounded Context Canvases Shipment:
![Bounded Context Canvases Shipment](/assets/chapter04/canvases_shipment.png)

### 4.1.2 Context Mapping
En esta sección, se analizan las relaciones entre los bounded contexts identificados y se asignan patrones de context mapping adecuados para cada uno:

**IAM ➔ Vehicles & Tracking / Shipment**<br>
**Descripción:** IAM actúa como Proveedor de identidad y permisos. Ambos contextos consumen esta información para garantizar seguridad antes de realizar acciones operativas.

**Vehicles & Tracking ➔ Shipment**<br>
**Descripción:** Shipment necesita saber la ubicación en tiempo real del vehículo asignado para monitorear el progreso del despacho.

**Vehicles & Tracking y Shipment ➔ Analytics**<br>
**Descripción:** Ambos publican eventos relevantes (movimientos, estados de envío) que Analytics recolecta para construir reportes operativos y dashboards de rendimiento.

**IAM ➔ Analytics**<br>
**Descripción:** Los eventos de autenticación, creación o actualización de usuarios también son capturados por Analytics para rastrear actividad en el sistema.

**Preguntas estratégicas de reflexión:**

- **¿Qué pasaría si movemos capacidades de gestión de usuarios fuera de IAM?**
Se evaluó separar Registro de Usuarios en un contexto independiente. Sin embargo, se descartó para no complicar el flujo de autenticación y autorización, que debe ser centralizado.

- **¿Qué pasaría si descomponemos Vehicles & Tracking en dos contextos: gestión de vehículos vs. tracking?**
Se consideró dividirlo, pero el tracking está intrínsecamente vinculado a la entidad Vehículo, y separarlos aumentaría latencia y complejidad de sincronización. Se decidió mantenerlos juntos.

- **¿Qué pasaría si partimos Analytics en un contexto de "Reportes" y otro de "Dashboards"?**
Se analizó, pero dada la escala actual del sistema, dividir Analytics complicaría innecesariamente los flujos de eventos. Se mantiene un solo contexto por ahora.

- **¿Qué pasaría si tomamos el manejo de asignaciones (usuarios a vehículos/envíos) en un contexto separado?**
Se pensó en un "Contexto de Asignaciones", pero resultaría en dependencias redundantes entre IAM, Vehicles & Tracking y Shipment. Se decidió que cada contexto maneje sus propias asignaciones.

- **¿Qué pasaría si creamos un shared service para usuarios entre IAM y Shipment?**
Se descartó porque IAM ya es el proveedor centralizado de identidad y permisos, y mover lógica fuera de él introduciría inconsistencias.

- **¿Qué pasaría si aislamos los core capabilities de IAM en un nuevo contexto?**
Se concluyó que IAM ya está correctamente enfocado en su Core Capability (Identity Management), por lo que no se fragmenta más.

**Conclusion del analisis:**<br>
- No se crean nuevos bounded contexts adicionales.
- Se mantienen 4 bounded contexts.
- Se refuerza que IAM actúa como Supplier para Vehicles & Tracking y Shipment.
- Analytics actúa como Subscriber de eventos generados por los otros contextos.

![Context Mapping](/assets/chapter04/context_mapping.png)

#### 4.1.3.1 Software Architecture System Lanscape Diagram

![Software Architecture System Lanscape Diagram]()

#### 4.1.3.2 Software Architecture Context Level Diagram

![Software Architecture Context Level Diagram]()

#### 4.1.3.3 Software Architecture Container Level Diagrams

![Software Architecture Container Level Diagrams]()

#### 4.1.3.4 Software Architecture Deployment Diagrams

![Software Architecture Deployment Diagrams]()