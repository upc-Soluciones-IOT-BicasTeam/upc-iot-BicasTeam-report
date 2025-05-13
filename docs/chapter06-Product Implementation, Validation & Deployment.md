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
 ## 6.2 Landing Page, Service & Applications Implementation
 ### 6.2.1 Sprint 1
 #### 6.2.1.1 Sprint Planning 1
 #### 6.2.1.2 Aspect Leaders and Collaborators
 #### 6.2.1.3 Sprint Backlog 1
 #### 6.2.1.4 Development Evidence for Sprint Review
 #### 6.2.1.5 Testing Suite Evidence for Sprint Review
 #### 6.2.1.6 Execution Evidence for Sprint Review
 #### 6.2.1.7 Services Documentation Evidence for Sprint Review
 #### 6.2.1.8 Software Deployment Evidence for Sprint Review
 #### 6.2.1.9 Team Collaboration Insights during Sprint
 ## 6.3 Validation Interviews
 ### 6.3.1 Diseño de Entrevistas
 ### 6.3.2 Registro de Entrevistas
 ### 6.3.3 Evaluaciones según Heurísticas
 ## 6.4 Video About-the-Product
