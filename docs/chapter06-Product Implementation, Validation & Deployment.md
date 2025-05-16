# Chatper 6: Product Implementation, Validation & Deployment
 ## 6.1 Software Configuration Management
 Para gestionar la configuración del software de nuestra aplicación, abordaremos tres áreas clave: el control del código fuente, que consiste en administrar las versiones y mantener una estructura ordenada del código; la configuración del entorno de desarrollo, con el objetivo de que todos los integrantes del equipo utilicen herramientas homogéneas; y la configuración del despliegue, enfocada en la implementación en entornos productivos. Estas prácticas aseguran consistencia y eficiencia durante todo el ciclo de vida de la aplicación.

 ### 6.1.1 Software Development Environment Configuration
 1. Project Management:
Para la administración del proyecto se utilizaron herramientas de comunicación y control de versiones. Se creó una organización en GitHub para gestionar el código y las versiones del proyecto. Asimismo, se utilizaron plataformas como Google Meet y Discord para coordinar reuniones de equipo y mantener la comunicación interna.

- GitHub: https://github.com/

- Google Meet: https://meet.google.com/

- Discord: https://discord.com/download

2. Requirement Management:
La recopilación, organización y priorización de requisitos se realizó utilizando herramientas específicas. Se utilizó Trello como una solución visual para la organización de tareas mediante tableros personalizados, mientras que Pivotal Tracker se empleó para gestionar y dar seguimiento al Product Backlog del proyecto.

- Trello: https://trello.com/es

- Pivotal Tracker: https://www.pivotaltracker.com/

3. Product UX/UI Design:
Para el diseño de la experiencia de usuario (UX) y la interfaz de usuario (UI), se utilizó Figma, permitiendo la creación de wireframes, mockups y prototipos interactivos que ayudaron a validar el diseño antes de su desarrollo. Además, UXPressia se empleó para desarrollar User Personas, Empathy Maps, Journey Maps e Impact Maps, mientras que Miro fue utilizado para diseñar los escenarios As-Is y To-Be.

- Figma: https://www.figma.com/downloads/

- UXPressia: https://uxpressia.com/

- Miro: https://miro.com/es/

4. Software Development:
Para construir la Landing Page de la startup se utilizaron HTML5, CSS3 y JavaScript. En cuanto a la Web Application, se optó por Angular en el Frontend y Java Spring Boot en el Backend. Por último para el desarrollo movil se utilizó Flutter.

- Visual Studio Code: Usado principalmente para el desarrollo de la Landing Page y el desarrollo movil, con diversas extensiones que facilitaron la productividad.

- JetBrains Toolbox: Proporcionó un entorno robusto para el desarrollo web y móvil, con funcionalidades avanzadas de edición y depuración.

- Visual Studio Code: https://code.visualstudio.com/

- JetBrains Toolbox: https://www.jetbrains.com/toolbox-app/

5. Software Documentation:
La documentación técnica del proyecto se elaboró y almacenó en GitHub, aprovechando su funcionalidad como plataforma de control de versiones y alojamiento de documentación. Se crearon repositorios específicos, utilizando archivos en formato Markdown para facilitar la edición y colaboración entre los miembros del equipo.

- GitHub: https://github.com/

 ### 6.1.2 Source Code Management
 En este proyecto, emplearemos GitHub como plataforma principal y sistema de control de versiones para gestionar el código fuente de las distintas partes del proyecto dentro de una organización.

**Repositorios en GitHub**
- Organización: https://github.com/orgs/upc-Soluciones-IOT-BicasTeam/repositories
- Report: https://github.com/upc-Soluciones-IOT-BicasTeam/upc-iot-BicasTeam-report
- Landing Page: https://github.com/upc-Soluciones-IOT-BicasTeam/upc-AppWeb-BicasTeam-LandingPage.github.io  
- Backend: https://github.com/upc-Soluciones-IOT-BicasTeam/upc-OpenSource-BicasTeam-api
- ForntEnd Web: https://github.com/upc-Soluciones-IOT-BicasTeam/upc-OpenSource-BicasTeam-AppWeb
- FrontEnd Mobile:

**GitFlow Workflow**
Implementaremos el modelo GitFlow como Workflow de control de versiones, siguiendo las convenciones y prácticas establecidas para una gestión eficiente del desarrollo de software.
1. Branches Principales:
- `main`: Rama principal del repositorio, contiene el código estable y liberado.
- `develop`: Rama de desarrollo deonde se integran las nuevas características y mejoras.

2. Branches de Funcionalidades (Feature Branches):
- Para cada nueva funcionalidad, se creará una rama de funcionalidad con el prefijo `feature/`, seguido del nombre descriptivo de la función o característica. En nuestro caso, creamos 5 branches de características correspondientes a los 5 capítulos de nuestro informe, donde se realizan los commits respectivos antes de fusionarlos con la rama develop cuando estén listos.

3. Branches de Lanzamiento (Release Branches) y Branches de Corrección (Hotfix Branches):
En nuestro caso, no hicimos uso de estas branches ya que no lo vimos necesario al ser solo documentacion del reporte.

**Versionado Semántico**
Seguimos la especificación Semantic Versioning 2.0.0 para nombrar nuestras versiones, siguiendo el formato: `MAJOR.MINOR.PATCH`.

**Conventional Commits**
Aplicamos el estándar de Conventional Commits para los mensajes de commit, siguiendo un formato estructurado que describe claramente los cambios realizados. Esto nos ayudó a automatizar la generación de notas de versión y facilitar la comprensión del historial de cambos del proyecto.

Con estas prácticas y convenciones adaptadas a una organización en GitHub, buscamos mantener un flujo de desarrollo ordenado, colaborativo y bien documentado.

 ### 6.1.3 Source Code Style Guide & Conventions
En esta sección, se establece las convenciones y prácticas que seguiremos para nombrar elementos y programar en los lenguajes utilizados en la solución, que incluyen HTML, CSS, JavaScript, Angular, Java, y Gherkin para los archivos `.feature`. Todas las convenciones seguirán la nomenclatura en inglés y adoptarán convenciones estándares de codificación.
1. **HTML y CSS**:
- Basado en las recomendaciones de W3C y otras fuentes de la comunidad, se establecerán convenciones para el nombramiento de elemntos hTML y estilo de la codificación CSS.
- Se seguirán las convenciones recomendadas por Google para HTML y CSS, que incluyen el uso de identaciones de 2 espacios, el uso de comillas dobles para atributos y el uso de comentarios descriptivos.
- Se utilizará la metodologìa BEM para organizar las clases CSS en bloques, elementos y modificadores, lo que facilitará la modularidad y la reutilización del código. 
- Se debe utilizar los elementos HTML de manera semántica para una correcta descripción del contenido del sitio web, incluyendo el uso adecuado de etiquetas.
- Para el desarrollo con Vue.js, se adoptarán las convenciones recomendadas por la comunidad de Vue, que incluyen el uso de PascalCase para los nombres y componentes y el uso de camelCase para las propiedades y métodos de los componentes.

2. **JavaScript**:
- Se tomarán en cuenta las directrices proporcionadas por MDN para la escritura de JavaScript, que incluyen el uso de nombres descriptivos para variables y funciones en camelCase, el uso de declaración de variavles con `let` o `const` en lugar de `var`, y el uso de punto y coma al final de cada declaración.
- Se seguirán las convenciones de codificación recomendadas por Google para JavaScript, que incluyen el uso de comillas simples para literales de cadena, el uso de comentarios descriptivos y el uso de funciones de flecha para expresiones de función.

3. **Angular:**
- Se seguirán las convenciones de codificación recomendadas por la comunidad de Angular, que incluyen el uso de TypeScript con tipado estricto, la separación de responsabilidades mediante componentes, servicios y módulos, y el uso de decoradores como `@Component`, `@Injectable` y `@NgModule`.
- Además, se organizarán los archivos en una estructura modular, agrupando componentes, servicios y modelos según su funcionalidad, y se fomentará el uso de Observables y RxJS para la gestión de estados y eventos.

4. **Java (Spring Boot):**
- Se aplicarán las convenciones de codificación de Java, como el uso de PascalCase para clases, camelCase para métodos y variables, y documentación con comentarios Javadoc.
- En el desarrollo con Spring Boot, se adoptarán buenas prácticas como la inyección de dependencias mediante anotaciones (`@Autowired`, `@Service`, `@Repository`), la separación de capas (controladores, servicios, repositorios), y el uso de DTOs para la transferencia de datos entre las capas. También se seguirá la configuración basada en anotaciones (`@SpringBootApplication`, `@Configuration`) para facilitar el mantenimiento y la escalabilidad de la aplicación.

5. **Flutter:**
- Se adoptarán las convenciones de codificación recomendadas por la comunidad de Flutter y Dart, que incluyen el uso de camelCase para nombres de variables y métodos, PascalCase para clases y widgets, y documentación con comentarios de tipo DartDoc.
- La estructura del proyecto se organizará siguiendo el patrón recomendado por Flutter, como el uso de `lib` con subcarpetas para `models`, `views`, `widgets`, `services` y `providers`. Se fomentará el uso de widgets reutilizables, y una separación clara entre la lógica de presentación y la lógica de negocio para mantener el código modular y fácil de mantener.

6. **Gherkin**:
- Se aplicarán las convenciones recomendadas para escribir especificaciones legibles en Gherkin, que incluyen el uso de palabras clave como `Given`, `When` y `Then` para describir el comportamiento del sistema, el uso de un lenguaje sencillo y claro, y la organización de los escenarios en contextos, acciones y resultados.
- Se seguirán las mejores prácticas recomendadas por Cucumber para escribir escenarios de prueba en Gherkin, que incluyen la reutilización de pasos de prueba, la modularización de escenarios y la escritura de pruebas autoexplicativas.

Además de estas referencias, se promoverá el uso de buenas prácticas y metodologías estándar en el desarrollo de software, como la modularidad, la reutilización de código, la legibilidad del código, la optimización del rendimiento y la seguridad. 
Con estas guías de estilo y convenciones de codificación, buscamos asegurar la coherencia, la calidad y la mantenibilidad del código a lo largo de todo el proyecto.

 ### 6.1.4 Software Deployment Configuration
 En esta sección, describiremos la configuración necesaria para desplegar satisfactoriamente cada uno de los productos digitales de nuestra solución, incluyendo Landing Page, y las Frontend Web Applications.

Pasos para el despliegue

1. Landing Page:
- Clonar o descargar el repositorio desde GitHub.
- Configurar el servidore web para alojar la Landing Page.
- Copiar los archivos HTMLS, CSS y JavaScript en el directorio correspondiente del servidor.
- Configurar cualquier dependencia adicional, como bibliotecas de JavaScript o imágenes.
- Verificar quue la Landing Page se cargue correctamente en el navegador.

2. Frontend Web Applications:
- Clonar o descargar el repositorio desde GitHub.
- Instalar las dependencias.
- Construir la aplicación para producción.
- Configurar el servidor web.
- Verificar que la aplicación se cargue correctamente en el navegador
 ## 6.2 Landing Page, Service & Applications Implementation
 ### 6.2.1 Sprint 1
 En esta sección, documentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 1. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo
 #### 6.2.1.1 Sprint Planning 1
 En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.
<table>
  <tbody>
    <tr>
      <td>Sprint #</td><td>Sprint 1</td>
    </tr>
    <tr>
      <td colspan="2">Sprint Planning Background</td>
    </tr>
		<tr>
			<td>Date</td>
			<td>2025-05-04</td>
		</tr>
		<tr>
			<td>Time</td>
			<td>07:06 PM</td>
		</tr>
		<tr>
			<td>Location</td>
			<td>Google Meet</td>
		</tr>
		<tr>
			<td>Prepared by</td>
			<td>Huarcaya Chavez, Miguel Alejandro Daniel</td>
		</tr>
		<tr>
			<td>Attendees (to planning meeting)</td>
			<td>Huarcaya Chavez, Miguel Alejandro Daniel / Torres Espinoza, Elias / Tarazona Medina, Piero Abel / Chacon Martinez, Mauricio Sebastián / Donayre Peña, Moises Rodolfo / Valenzuela Huillcaya, Aldhair Johan Juan</td>
		</tr>
		<tr>
			<td>Sprint 1 Review Summary</td>
			<td>- Desplegar la landing page informativa, permitiendo a los visitantes conocer el sistema y navegar entre sus secciones básicas.

Resultados alcanzados:

Landing Page:

Se publicaron todas las secciones informativas: resumen del sistema (US01), funcionalidades clave (US02), comparativa gratuita vs PRO (US03) y video explicativo (US04).

Se validó su responsividad en desktop y móvil.

Opiniones del equipo:

Se valoró positivamente la colaboración conjunta y la resolución de problemas en equipo.

Se identificó la documentación de versiones como área de mejora para el próximo sprint.

Feedback del Product Owner:

“La información de la landing es muy clara. Antes de avanzar, validemos la usabilidad de cada sección en diferentes resoluciones.”.”</td>
		</tr>
		<tr>
			<td>Sprint 1 Retrospective Summary</td>
			<td>- Aspectos positivos:

Comunicación continua y efectiva a través de Discord, lo que facilitó resolver bloqueos en tiempo real.

Oportunidades de mejora:

Ajustar las estimaciones de esfuerzo: subestimamos la integración del video explicativo (US04), lo que provocó una demora de medio día.

Desglosar mejor las tareas de CSS responsive para reducir retrabajo.

Plan de acción:
En el próximo Sprint dedicaremos 15 min adicionales en el planning para:

Refinar las estimaciones de cada historia.

Dividir las historias grandes en subtareas de máximo 4 horas.</td>
	</tr>
		<tr>
			<td colspan="2">Sprint Goal & User Stories</td>
		</tr>
		<tr>
			<td>Sprint 1 Goal</td>
			<td>- Sprint 1 Goal
Nuestro enfoque está en entregar la experiencia pública inicial mediante la Landing Page e implementar las funcionalidades principales del rol gerente en la aplicación web.

Creemos que esto aportará visibilidad del producto y capacidades de incorporación a potenciales clientes a través de la Landing Page, así como valor de negocio para los gerentes registrados al permitirles gestionar vehículos y conductores, y acceder a estadísticas operativas relevantes.

Esto se confirmará cuando los visitantes puedan acceder y navegar correctamente por la Landing Page sin errores visuales o de diseño, y los gerentes registrados puedan iniciar sesión, registrar vehículos y conductores, y visualizar estadísticas de su operación dentro de la plataforma web.</td>
		</tr>
		<tr>
			<td>Sprint 1 Velocity</td>
			<td>- Para este primer Sprint estimamos una velocidad de 8 Story Points, basada en nuestra capacidad de equipo y en la complejidad de las historias seleccionadas.</td>
		</tr>
		<tr>
			<td>Sum of Story Points</td>
			<td>
| Orden | Story ID | Título | Story Points |
| ----- | ------- | ------ | ------------ |
| 1 | US01 | Ver descripción general del sistema | 2 |
| 2 | US02 | Ver funcionalidades clave | 2 |
| 3 | US03 | Ver comparativa de cuenta gratuita vs PRO | 1 |
| 6 | US06 | Redirigir al registro | 1 |
| Total | | | 6 |
</td>
		</tr>
  </tbody>
</table>

 #### 6.2.1.2 Aspect Leaders and Collaborators
 | Team Member | Github Username | section-header | section-hero | section-about-us | section-about-team | section-services | section-pricing | section-footer |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Huarcaya, Miguel | MiguelHuarcayaChavez | C |  | L |  | C |  |
| Torres, Elias | EliasTorresEzpinoza |  | L |  | C |  |  | L |
| Tarazona, Piero | pierotm |  |  |  | L |  | C |  |
| Chacon, Mauricio | mxuriciocm | L |  |  | C | L |  | C |
| Donayre, Moises | MoisesD19 |  |  | C |  |  | L |  |
| Valenzuela, Aldhair | AldhaValenzuelaH |  | C |  |  |  |  | C |

| Team Member | Github Username | IAM | Subscription & Payments | Profile Management | Analytics | Vehicles & Tracking | Shipment | Issues |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Huarcaya, Miguel | MiguelHuarcayaChavez | L | L |  |  | C | C |
| Torres, Elias | EliasTorresEzpinoza | C | C |  |  |  | L | L |
| Tarazona, Piero | pierotm |  |  | C | L |  |  |  |
| Chacon, Mauricio | mxuriciocm |  |  | L | C |  |  |  |
| Donayre, Moises | MoisesD19 |  |  |  |  | L |  |  |
| Valenzuela, Aldhair | AldhaValenzuelaH |  |  |  |  | C |  |  |

 #### 6.2.1.3 Sprint Backlog 1
 El Sprint 1 está centrado en la implementación de las funcionalidades clave de la landing page del sitio web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los visitantes una experiencia inicial sólida al presentar de manera clara y concisa las características y beneficios del sitio, junto con una navegación intuitiva y acceso rápido a la información relevante. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos las bases para futuras iteraciones, asegurando que la página de inicio cumpla con las expectativas de los usuarios y contribuya al éxito del proyecto.

<table border="1">
    <tbody>
        <tr>
            <td>Sprint #</td>
            <td colspan="7">Sprint 1</td>
        </tr>
        <tr>
            <td colspan="2">User Story</td>
            <td colspan="6">Work-Item / Task</td>
        </tr>
        <tr>
            <td>Id</td>
            <td>Title</td>
            <td>Id</td>
            <td>Title</td>
            <td>Description</td>
            <td>Estimation (Hours)</td>
            <td>Assigned To</td>
            <td>Status(To-do / InProcess / ToReview / Done)</td>
        </tr>
        <tr>
            <td>US01</td>
            <td>Ver descripción general del sistema</td>
            <td>T01</td>
            <td>Diseñar sección de descripción</td>
            <td>Crear el diseño visual y la estructura de la sección de la descripción general del sistema.</td>
            <td>8</td>
            <td>Aldahir Valenzuela</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US02</td>
            <td>Ver funcionalidades clave</td>
            <td>T04</td>
            <td>Identificar funcionalidades clave</td>
            <td>Definir y documentar las funcionalidades más importantes del sistema para mostrar.</td>
            <td>4</td>
            <td>Mauricio Chacon</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US03</td>
            <td>Ver comparativa de cuenta gratuita vs PRO</td>
            <td>T07</td>
            <td>Definir comparativa</td>
            <td>Especificar las características y beneficios de las cuentas gratuita y PRO para la comparación.</td>
            <td>4</td>
            <td>Moises Donayre</td>
            <td>Done</td>
        </tr>
		    <td>US04</td>
            <td>Ver video o animación explicativa</td>
            <td>T11</td>
            <td>Crear guion del video</td>
            <td>Escribir el guion detallado que se utilizará para la creación del video explicativo.</td>
            <td>5</td>
            <td>Aldahir Valenzuela</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US05</td>
            <td>Completar formulario de contacto</td>
            <td>T12</td>
            <td>Diseñar formulario de contacto</td>
            <td>Crear la interfaz de usuario para el formulario donde los interesados puedan ingresar sus datos.</td>
            <td>4</td>
            <td>Elias Torres</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US06</td>
            <td>Redirigir al registro</td>
            <td>T09</td>
            <td>Crear botón de registro</td>
            <td>Diseñar e implementar el botón o enlace que lleva a la página de registro.</td>
            <td>3</td>
            <td>Elias Torres</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US16</td>
            <td>Registrar cuenta de gerente</td>
            <td>T13</td>
            <td>Implementar formulario de registro</td>
            <td>Desarrollar el formulario para que los gerentes puedan crear sus cuentas.</td>
            <td>8</td>
            <td>Piero Tarazona</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US17</td>
            <td>Iniciar sesión como gerente</td>
            <td>T14</td>
            <td>Crear formulario de inicio de sesión</td>
            <td>Desarrollar la interfaz para que los gerentes puedan ingresar con sus credenciales.</td>
            <td>3</td>
            <td>Mauricio Chacon</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US20</td>
            <td>Ver perfil personal</td>
            <td>T15</td>
            <td>Mostrar datos del perfil</td>
            <td>Implementar la visualización de la información personal del usuario autenticado.</td>
            <td>2</td>
            <td>Miguel Huarcaya</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US23</td>
            <td>Crear vehículo</td>
            <td>T16</td>
            <td>Implementar formulario de registro de vehículo</td>
            <td>Desarrollar el formulario para que los gerentes puedan registrar nuevos vehículos.</td>
            <td>3</td>
            <td>Moises Donayre</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US24</td>
            <td>Ver listado de vehículos registrados</td>
            <td>T17</td>
            <td>Mostrar lista de vehículos</td>
            <td>Desarrollar la interfaz para visualizar todos los vehículos registrados.</td>
            <td>2</td>
            <td>Piero Tarazona</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US25</td>
            <td>Asignar un conductor a un vehículo</td>
            <td>T18</td>
            <td>Crear interfaz de asignación</td>
            <td>Desarrollar la funcionalidad para vincular un conductor a un vehículo específico.</td>
            <td>3</td>
            <td>Elias Torres</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US27</td>
            <td>Ver temperatura y humedad del vehículo</td>
            <td>T19</td>
            <td>Mostrar datos de sensor</td>
            <td>Implementar la visualización de la temperatura y humedad del vehículo.</td>
            <td>2</td>
            <td>Mauricio Chacon</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US28</td>
            <td>Ver ubicación actual del vehículo</td>
            <td>T20</td>
            <td>Integrar mapa con ubicación</td>
            <td>Implementar la visualización de la ubicación del vehículo en un mapa.</td>
            <td>3</td>
            <td>Miguel Huarcaya</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US34</td>
            <td>Crear envío</td>
            <td>T21</td>
            <td>Implementar formulario de creación de envío</td>
            <td>Desarrollar el formulario para que los gerentes puedan crear nuevos envíos.</td>
            <td>5</td>
            <td>Moises Donayre</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US35</td>
            <td>Asignar envío a un conductor</td>
            <td>T22</td>
            <td>Crear interfaz de asignación de envíos</td>
            <td>Desarrollar la funcionalidad para asignar un envío a un conductor.</td>
            <td>3</td>
            <td>Aldahir Valenzuela</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US37</td>
            <td>Ver estado del envío</td>
            <td>T23</td>
            <td>Mostrar estado del envío</td>
            <td>Implementar la visualización del estado actual del envío.</td>
            <td>1</td>
            <td>Piero Tarazona</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US44</td>
            <td>Ver reportes por conductor (como gerente)</td>
            <td>T24</td>
            <td>Generar reporte de conductor</td>
            <td>Desarrollar la funcionalidad para generar reportes basados en la actividad de cada conductor.</td>
            <td>2</td>
            <td>Elias Torres</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US46</td>
            <td>Acceder a sección de suscripción</td>
            <td>T25</td>
            <td>Crear enlace a suscripción</td>
            <td>Implementar un enlace o botón para acceder a la sección de gestión de suscripciones.</td>
            <td>2</td>
            <td>Mauricio Chacon</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US47</td>
            <td>Subir comprobante de pago</td>
            <td>T26</td>
            <td>Implementar formulario de carga</td>
            <td>Desarrollar la funcionalidad para que los gerentes puedan subir el comprobante de pago.</td>
            <td>2</td>
            <td>Miguel Huarcaya</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US53</td>
            <td>Ver condiciones ambientales por vehículo</td>
            <td>T27</td>
            <td>Mostrar condiciones por vehículo</td>
            <td>Implementar la visualización de la temperatura y humedad de cada vehículo.</td>
            <td>3</td>
            <td>Moises Donayre</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US54</td>
            <td>Mostrar color según condición ambiental</td>
            <td>T28</td>
            <td>Implementar indicadores de color</td>
            <td>Desarrollar la lógica para mostrar colores según los rangos de temperatura y humedad.</td>
            <td>3</td>
            <td>Aldahir Valenzuela</td>
            <td>Done</td>
        </tr>
    </tbody>
</table>

 #### 6.2.1.4 Development Evidence for Sprint Review
 Esta sección documenta y presenta la serie de commits realizados en el repositorio del Landing Page. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.
 | Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date)|
 | --- | --- | --- | --- | --- | --- |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | d3b094b | chore:... | initial commit | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 499f6c3 | feat:... | create structure for landing | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-header | a6fd61f | feat:... | create header section | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-us | f46c9f4 | feat:... | create about us | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 559b871 | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 320162e | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 74db128 | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 6db4844 | feat:... | delete file style | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | f80d9c2 | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 77dcfbf | feat:... | deleted style | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 57cd331 | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 2ac60ee | feat:... | deleted style | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | a89f5a6 | feat:... | add folder for organizing files | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 9c04bc0 | feat:... | create about team | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | e645b3b | feat:... | delete public directory | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-about-team | 1488c1e | feat:... | add style and images | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-hero | 09191fd | feat:... | implement hero section | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-hero | 0ba7ade | feat:... | implement footer section | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-footer | 77037f0 | feat:... | create footer section | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-pricing | 84c90ea | chore:... | created pricing and contact section | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | c3a6a0c | feat:... | merge branch 'feature/section-hero' | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | 4f4b5b7 | feat:... | merge branch 'feature/section-about-us' | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | e63214c | feat:... | merge branch 'feature/section-about-team' into develop | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | 7d5209d | feat:... | merge branch 'feature/section-services' into develop | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | 432e18e | feat:... | merge branch 'feature/section-pricing' into develop | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | develop | 9b278c2 | feat:... | merge branch 'feature/section-footer' into develop | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | fbf4690 | fix:... | fix the ubication for the code | 10-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | c6a949e | feat:... | update index.html | 30-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 2e872c2 | feat:... | update index.html | 30-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 7ca9228 | fix:... | button get star | 30-04-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 80969dc | feat:... | implement video about the product | 05-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | bd8eecb | fix:... | implement video about the product | 05-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 49e5318 | feat:... | implement video about the team | 05-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 1b50053 | fix:... | implement video about the team | 05-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 4446436 | fix:... | implement video about the team | 05-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 5396416 | fix:... | link about the team | 06-06-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 3c21c8a | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 4fd8208 | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 34ad386 | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | a689428 | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | a89718e | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 1bb2d40 | feat:... | update index.html | 28-09-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | bdc70ba | feat:... | apk download | 22-11-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 2bb167c | feat:... | update styles.css | 22-11-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | ab4cdd9 | feat:... | update styles.css | 22-11-2024 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | 8deffb7 | fix:... | servies implement | 10-05-2025 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | e9cdf14 | fix:... | the styles were modified | 11-05-2025 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | main | d588b20 | fix:... | update of the hero, pricing, header section | 15-05-2025 |
 | upc-AppWeb-BicasTeam-LandingPage.github.io | feature/section-footer | d352dd8 | feat:... | add new css style | 15-05-2025 |

 #### 6.2.1.5 Execution Evidence for Sprint Review
 Durante el Sprint 1, se logró un progreso significativo en la implementación de las características clave de la página de inicio del sitio web. El equipo completó con éxito todas las historias de usuario asignadas para este sprint, que incluyeron el desarrollo de un resumen claro de las características y beneficios del sitio web, la integración de acceso visible a información detallada de precios, la adición de un resumen conciso al final de la página de inicio, la inclusión de un llamado a la acción prominente para dirigir a los visitantes a la aplicación web principal, la presentación de contenido informativo claro y detallado, y la integración de información de contacto visible en la página de inicio. El equipo trabajó de manera colaborativa para garantizar que las características implementadas cumplan con los requisitos y contribuyan a una experiencia de usuario positiva. Capturas de pantalla:

 Header:<br>
 ![Header](/assets/chapter06/header.png)

 Hero:<br>
 ![Hero](/assets/chapter06/hero.png)
 
 About Us:<br>
 ![About-Us](/assets/chapter06/about-us.png)
 
 About The Team:<br>
 ![About-Team](/assets/chapter06/about-team.png)
 
 Services:<br>
 ![EnvironmentService](/assets/chapter06/environment-service.png)

 ![GpsService](/assets/chapter06/gps-service.png)

 ![OrganizationService](/assets/chapter06/organization-service.png)

 ![CommunicationService](/assets/chapter06/communication-service.png)

 ![VehicleStatusService](/assets/chapter06/vehicle-status-service.png)
 
 Pricing:<br>
 ![Pricing](/assets/chapter06/pricing.png)
 
 Footer:<br>
 ![Footer](/assets/chapter06/footer.png)

 APP WEB:
  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/analiticsIssues.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/analiticsShipmetns.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/analiticsTransport.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/goPro.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/home.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/issues.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/login.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/shipments.png)

  ![AppWeb](/assets/chapter06/Execution%20evidence%20for%20sprint%20review/vehicles.png)


 #### 6.2.1.6 Services Documentation Evidence for Sprint Review
 Durante este Sprint 1, hemos hecho uso de un Fake API (Beeceptor) para hacer uso de Endpoints.

 ![Beeceptor](/assets/chapter06/beeceptor%20documentation%20evidence.png)

 #### 6.2.1.8 Software Deployment Evidence for Sprint Review
 Durante el Sprint 1, llevamos a cabo el despliegue de nuestra Landing Page en GitHub Pages y el desarrollo inicial de la aplicación web enfocada en el rol de gerente. A continuación, detallamos los pasos realizados:

Creación del Repositorio en GitHub: Iniciamos creando repositorios dedicados para nuestra landing page y nuestra aplicación web.

Configuración de la Rama main: Aseguramos que la rama principal del repositorio de la landing page se llamara main, ya que GitHub Pages toma esta rama como base para el despliegue automático.

Preparación del Contenido de la Landing Page: Diseñamos y desarrollamos el contenido informativo, incluyendo secciones clave como beneficios, diferencia entre cuenta gratuita y PRO, y formulario de contacto.

Desarrollo del Frontend Web (Gerente): Implementamos funcionalidades clave para el gerente, como inicio de sesión, registro, gestión de vehículos y conductores, y visualización de estadísticas.

Generación del Enlace de GitHub Pages: Desde la sección "Pages" de configuración del repositorio, configuramos la fuente de despliegue para que tomara el contenido de la rama main.

Despliegue Automático de la Landing Page: GitHub Pages detectó los cambios y desplegó correctamente la landing en la URL proporcionada.

Despliegue local de la Aplicación Web: Para la aplicación del gerente, utilizamos entornos de desarrollo local (ej. Vite + React o Angular) y avanzamos en la integración de vistas y componentes según las historias priorizadas.

 #### 6.2.1.9 Team Collaboration Insights during Sprint

Durante este primer Sprint, hemos completado el desarrollo de la Landing Page y hemos avanzado significativamente en la implementación del frontend web del rol gerente. La colaboración entre los miembros del equipo se refleja en los múltiples commits realizados en los distintos repositorios de GitHub, los cuales han sido debidamente documentados con capturas de pantalla.

Para asegurar una colaboración efectiva, hemos adoptado GitFlow como metodología de trabajo colaborativo en Git. Esta estrategia nos permitió organizar el trabajo en ramas específicas tanto para cada sección de la landing como para cada módulo funcional del frontend del gerente (por ejemplo: vista de conductores, formulario de creación de vehículos, pantalla de login, etc.).

Además, distribuimos las tareas asignando a cada integrante una sección o funcionalidad distinta, lo que nos permitió desarrollar de forma paralela la landing y las vistas del gerente. Esta estrategia nos permitió avanzar de manera más eficiente, cumplir con las historias de usuario planificadas y completar los entregables antes de la fecha límite.