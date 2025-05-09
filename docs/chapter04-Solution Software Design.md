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

Link de Context Canvases: https://miro.com/welcomeonboard/aWJYTFBpYTJ0WVdEN203MzdEdk9EOXk5VGtsb09lNlFtTHEyNHkyNUZGNXhQTlkyRkNJU3NNeG14cUx5VEpKMmRoQjBBUFg1VUFyMUdEc1p1NmkrcncxL29WaGdiUGVsR1ZZb2NyRURPSjBjYnlWWExvbFR4REdqVXFZU0ZaSmd0R2lncW1vRmFBVnlLcVJzTmdFdlNRPT0hdjE=?share_link_id=517257946153 

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

## 4.2 Tactical-Level Domain-Driven Design
### 4.2.1 Bounded Context: IAM
Se encarga de gestionar la identidad digital de los usuarios y controlar su acceso a recursos del sistema. Proporciona servicios de autenticación (verificación de identidad) y autorización (control de permisos) de forma segura y escalable. Su responsabilidad es manejar usuarios, roles, permisos y sesiones de manera centralizada, siguiendo principios de seguridad.

#### 4.2.1.1 Domain Layer
Contiene la lógica de negocio pura y las entidades principales relacionadas a la identidad y gestión de accesos, encapsulando el comportamiento y las reglas de negocio.

**Agregate 1: User**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| User | Entity |Representa una identidad de usuario en el sistema IAM, incluyendo credenciales seguras, estado de verificación de email y el único rol asignado. Es la raíz de un agregado que mantiene la consistencia de los datos del usuario. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripcion |
| --- | --- | --- | --- |
| id | UUID | Private | Identificador único del usuario. |
| name | String | Private | Nombre completo del usuario. |
| email | Email | Private | Objeto de valor encapsulando la dirección de correo electrónico y su validación. |
| passwordHash | String | Private | Contraseña hasheada del usuario. |
| isEmailVerified | Boolean | Private | Estado de verificación del correo electrónico. |
| status | Enum | Private |Estado del usuario. |
| roleId | UUID | Private | Referencia al ID del único rol asignado al usuario. |
| createdAt | Date | Private | Fecha de creación. |
| updatedAt | Date | Private | Fecha de actualización.|

**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| create(...) | User | Public | Crea una nueva instancia de User, aplicando validaciones iniciales. |
| changePassword(newPassword, PasswordEncoder) | Void | Public | Actualiza la contraseña del usuario después de verificar las reglas de negocio. |
| updateProfile(newName, newEmail, emailService) | Void | Public | Actualiza el nombre y email del usuario. | 
| assignRole(UUID roleId) | Void | Public | Establece o cambia el rol asignado al usuario al roleId proporcionado. |
| removeRole(UUID roleId) | Void | Public | Remueve un rol. |
| isPasswordValid(rawPassword, passwordEncoder) | Boolean | Public | Verifica si una contraseña plana coincide con el hash almacenado. |

**Agregate 2: Role**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| Role | Entity | Define un tipo de usuario con un conjunto específico de permisos. |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripcion |
| --- | --- | --- | --- |
| id | UUID | Private | Identificador único del rol. |
| name | String | Private | Nombre único del rol asignado. |
| description | String | Private | Descripción del rol. |
| permissions | Set<Permission> | Private | Conjunto de value objects Permission asociados a este rol. |

**Methods**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| create(name, description) | Role | Public | Crea una nueva instancia de Role. |
| changeName(new Name) | Void | Public | Actualiza el nombre del rol. |
| changeDescription(new Description) | Void | Public | Actualiza la descripción del rol. |
| addPermission(Permission permission) | Void | Public | Añade un Objeto de Valor Permission al conjunto de rol. |
| removePermission(Permission permission) | Void | Public | Remueve un Objeto de Valor Permission del conjunto del rol. |
| hasPermission(String permissionName) | Boolean | Public | Verifica si el rol contiene un permiso específico. |

**Aggreate 3: Session**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| Session | Entity | Representa una sesión de usuario activa para mantener el estado de autenticación, manejar tokens (acceso y refresco) y controlar el tiempo de vida de la sesión. |


**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| id | UUID | Private | Identificador único de la sesión. |
| userId | String | Private | Identificador del usuario asociado. |
| accessToken | String | Private | Token principal usado para autenticar peticiones. |
| refreshToken | String | Private | Token usado para obtener nuevos Access Tokens sin reautenticar. |
| creationTime | Date | Private | Marca de tiempo de creación de la sesión. |
| expiresAt | Date | Private | Fecha de expiración de la sesión. |
| isValid | Boolean | Private | Indica si la sesión ha sido explícitamente invalidada. |

**Methods**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| create(userId, accessToken, refreshToken, expiresAt) | Session | Public | Crea una nueva instancia de Session. |
| invalidate() | Void | Public | Marca la sesión como inválida. |
| refresh(newAccessToken, newRefreshToken, newExpiresAt) | Void | Public | Actualiza los tokens y el tiempo de expiración de la sesión. |
| isValid(currentTime: Date) | Boolean | Public | Verifica si la sesión no está expirada y no ha sido invalidada. |
| getAccessToken() | String | Public | Retorna el Access Token actual de la sesión. |

**Value Object: Email**<br>
| Nombre | Categoría | Descripción | 
| --- | --- | ---|
| Email | Value Object | Encapsula una dirección de correo electrónico en formato string. |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción | 
| --- | --- | --- | --- |
| value | String | Private | La dirección de correo electrónico en formato string. |

**Methods**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| of(string value) | Email | Public | Crea una instancia inmutable de Email después de validar su formato. |
| getValue() | String | Public | Retorna la dirección como string. |
| equals(object other) | Boolean | Public | Compara si dos emails son iguales. |
| hashCode() | int | Public | Calcula el hashcode basado en el valor. | 
| toString() | String | Public | Retorna la representación en cadena. |

**Value Object: Permission**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| Permission | Value Object | Representa una capacidad específica dentro del sistema. Es inmutable. |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| value | String | Private | Representación única del permiso. |

**Methods**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| of(string value) | Email | Public | Crea una instancia inmutable de Permission después de validar su formato. |
| getValue() | String | Public | Retorna el valor del permiso. |
| equals(object other) | Boolean | Public | Compara si dos Permission tienen el mismo valor. |
| hashCode() | int | Public | Calcula el hashcode basado en el valor. |
| toString() | String | Public | Retorna la representación en cadena. |

#### 4.2.1.2 Interface Layer
Esta capa es responsable de la recepción y formato de peticiones/respuestas externas (API REST), validación básica del formato y los datos de entrada, manejo de errores a nivel de API y delegación de la lógica de negocio a la capa de Aplicación.

**Controller 1: AuthController**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| AuthController | Controller | Controlador para los endpoints relacionados con la autenticación de usuarios y la gestión del ciclo de vida de las sesiones (registro, login, logout, refresco). |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| authService | AuthService |Private | Servicio de la capa de Aplicación para lógica de autenticación/sesiones. |
| userMapper | UserMapper | Private | Mapper para convertir entre DTOs y objetos usados por Application/Domain. |
| sessionMapper | SessionMapper | Private | Mapper para convertir entre DTOs y objetos de Sesión. |

**Endpoints**<br>
| Ruta | Método | Descripción |
| --- | --- | --- |
| /api/iam/register | POST | Registra un nuevo usuario en el sistema. |
| /api/iam/login | POST | Autentica a un usuario con email y contraseña, creando una nueva sesión. |
| /api/iam/logout | POST | Invalida la sesión activa del usuario. |
| /api/iam/refresh-session | POST | Obtiene un nuevo access token utilizando un refresh token válido. |

**Controller 2: UserController**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| UserController | Controller | Controlador para operaciones de gestión de usuarios (CRUD). |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| userService | UserService | Private | Servicio de la capa de Aplicación para lógica de gestión de usuarios. |
| userMapper | UserMapper | Private | Mapper para convertir entre DTOs y objetos de Usuario. |

**Endpoints**<br>
| Ruta | Método | Descripción |
| --- | --- | --- |
| /api/iam/users | GET | Retorna una lista paginada o completa de usuarios existentes. |
| /api/iam/users/{id} | GET | Retorna los datos de un usuario específico por su ID. |
| /api/iam/users/{id} | PUT | Actualiza datos de un usuario existente por su ID. |
| /api/iam/users/{id} | DELETE | Elimina un usuario del sistema por su ID. |
| /api/iam/users/{id}/assign-role | POST | Asigna un rol específico a un usuario por su ID. |

**Controller 3: RoleController**<br>
Nombre | Categoría | Descripción |
| --- | --- | --- |
| RoleController | Controller | Controlador para operaciones de gestión de roles (CRUD). |

**Attributes**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| roleService | RoleService | Private | Servicio de la capa de Aplicación para lógica de gestión de roles. |
| roleMapper | RoleMapper | Private | Mapper para convertir entre DTOs y objetos de Rol. |

**Endpoints**<br>
| Ruta | Método | Descripción |
| --- | --- | --- |
| /api/iam/roles | POST | Crea un nuevo rol. |
| /api/iam/roles | GET | Lista todos los roles existentes. |
| /api/iam/roles/{id} | GET | Obtiene los datos de un rol específico por su ID. |
| /api/iam/roles/{id} | PUT | Actualiza los datos de un rol existente. |
| /api/iam/roles/{id} | DELETE | Elimina un rol existente por su ID. |

**DTOs**<br>
| Nombre | Descripción |
| --- | --- |
| RegisterRequestDto | { name: String, email: String, password: String } |
| LoginRequestDto | { email: String, password: String } |
| LoginResponseDto | { accessToken: String, refreshToken: String, expiresIn: Long, userId: UUID } |
| LogoutRequestDto | { refreshToken: String } |
| UserIdDto | { userId: UUID } |
| UserUpdateDto | { name: String, email: String, status: String, roleId: UUID } |
| UserResponseDto | { id: UUID, name: String, email: String, isEmailVerified: Boolean, status: String, roleId: UUID, createdAt: Date, updatedAt: Date } |
| AssignRoleRequestDto | { roleId: UUID } |
| RoleCreateDto | { name: String, description: String, permissions: List<String> } |
| RoleUpdateDto | { name: String, description: String, permissions: List<String> } |
| RoleResponseDto | { id: UUID, name: String, description: String, permissions: List<String> } |
| CheckPermissionResponseDto | { hasPermission: Boolean } |

#### 4.2.1.3 Application Layer
En la capa de Application Layer se ubican los servicios que contienen la lógica de negocio relacionada con usuarios y roles.

**Service 1: AuthService**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| AuthService | Service | Servicio de aplicación responsable de los casos de uso relacionados con la autenticación de usuarios y la gestión de sesiones y tokens. |

**Dependencies**<br>
| Nombre | Tipo de Objeto | Visibilidad | Descripción |
| --- | --- | --- | --- |
| userRepository | UserRepository | Private | Acceso a la persistencia de Usuarios. |
| sessionRepository | SessionRepository | Private | Acceso a la persistencia de Sesiones. |
| roleRepository | RoleRepository | Private | Necesario para obtener el rol por defecto o validar roles asignados. |
| passwordEncoder | PasswordEncoder | Private | Servicio técnico para hashear y verificar contraseñas. |
| jwtProvider | JwtProvider(Infrastructure) | Private | Servicio técnico para generar y validar JWTs. |
| emailService | EmailService | Private | Servicio técnico para enviar emails. |
| userFactory | UserFactory | Private | Ayuda a construir objetos User complejos si el constructor de User no es suficiente. |
| sessionFactory | SessionFactory | Private | Ayuda a construir objetos Session. |

**Methods**<br>
| Nombre | Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| registerUser(RegisterUserCommand command) | UserIdDto | Public | Implementa el caso de uso de registro de usuario. |
| authenticateUser(LoginQuery query) | LoginResponseDto | Public | Implementa el caso de uso de autenticación. |
| logoutUser(LogoutCommand command) | Void | Public | Implementa el caso de uso de cierre de sesión. |
| refreshSession(RefreshSessionCommand command) | LoginResponseDto | Public | Implementa el caso de uso de refresco de sesión. |
| checkUserPermission(CheckPermissionQuery query) | Boolean | Public | Implementa el caso de uso para verificar si un usuario tiene un permiso. (Podría ser también un Domain Service). |

**Service 2: UserService**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| UserService | Service | Servicio de aplicación responsable de los casos de uso de gestión de usuarios (CRUD y asignación de rol) por parte de administradores u otros procesos internos. |
	
**Dependencies**<br>
| Nombre | Tipo de Objeto | Visibilidad | Descripción |
| --- | --- | --- | --- |
| userRepository | UserRepository | Private | Acceso a la persistencia de Usuarios. |
| roleRepository | RoleRepository | Private | Necesario para validar roles o obtener sus datos. |
| passwordEncoder | PasswordEncoder | Private | Necesario si se permite cambiar contraseña vía update. |
| authenticationService | AuthenticationService | Private | Para usar el servicio de dominio de verificación de permisos. |
| userMapper | UserMapper | Private | Para mapear entre DTOs/objetos de aplicación y objetos de Dominio/respuesta. |

**Methods**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| listAllUsers(...) | List<UserResponseDto> | Public | Listar todos los usuarios (con paginación/filtros). |
| getUserById(UUID userId) | UserResponseDto | Public | Obtener un usuario por su ID. |
| updateUser(UUID userId, UserUpdateCommand command) | UserResponseDto | Public | Actualizar datos de un usuario. |
| deleteUser(UUID userId) | Void | Public | Eliminar un usuario. |
| assignRoleToUser(AssignRoleCommand command) | Void | Public | Asignar un rol a un usuario. |

**Service 3: RoleService**<br>
| Nombre | Categoría | Descripción |
| --- | --- | --- |
| RoleService | Service | Servicio de aplicación responsable de los casos de uso de gestión de roles (CRUD y manejo de permisos) por parte de administradores. |
	
**Dependencies**<br>
| Nombre | Tipo de Objeto | Visibilidad | Descripción |
| --- | --- | --- | --- |
| roleRepository | RoleRepository | Private | Acceso a la persistencia de Roles. |
| userRepository | UserRepository | Private | Necesario para verificar si un rol está en uso antes de eliminarlo. |
| authenticationService | AuthenticationService | Private | Para usar el servicio de dominio de verificación de permisos. |
| roleMapper | RoleMapper | Private | Para mapear entre DTOs/objetos de aplicación y objetos de Dominio/respuesta. |

**Methods**<br>
| Nombre | Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| createRole(CreateRoleCommand command) | RoleResponseDto | Public | Crear un nuevo rol. |
| listAllRoles(...) | List<RoleResponseDto> | Public | Listas todos los roles. |
| getRoleById(UUID roleId) | RoleResponseDto | Public | Obtener un rol por su ID. |
| updateRole(UUID roleId, UpdateRoleCommand command) | RoleResponseDto | Public | Actualizar datos de un rol. |
| deleteRole(UUID roleId) | Void | Public | Eliminar un rol. |

**Commands y Queries**<br>
- RegisterUserCommand
- LoginQuery
- LogoutCommand
- RefreshSessionCommand
- CheckPermissionQuery
- UserUpdateCommand
- AssignRoleCommand
- CreateRoleCommand
- UpdateRoleCommand

#### 4.2.1.4 Infrastructure Layer
En la capa de Infrastructure Layer, se encuentran los repositorios que permiten la persistencia de las entidades de usuarios y roles en la base de datos.

**JpaUserRepositoryImpl**<br>
| Nombre | Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| JpaUserRepositoryImpl | Repository Implementation | UserRepository | Implementación concreta de la interfaz UserRepository utilizando JPA y, típicamente, Spring Data JPA. Maneja el mapeo entre la entidad de dominio User y la tabla/colección de la base de datos subyacente. |

**Funcionalidad clave**<br>
- Busca y carga entidades User por ID, email, etc.
- Guarda (inserta/actualiza) entidades User.
- Elimina entidades User.
- Verifica la existencia de usuarios por email o ID.
- Verifica la existencia de usuarios por roleId (para validaciones al borrar roles).

**JpaRoleRepositoryImpl**<br>
| Nombre | Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| JpaRoleRepositoryImpl | Repository Implementation | RoleRepository | Implementación concreta de la interfaz RoleRepository utilizando JPA y Spring Data JPA. Maneja el mapeo entre el agregado de dominio Role y la base de datos. |

**Funcionalidad clave**<br>
- Busca y carga agregados Role por ID, nombre, etc.
- Guarda (inserta/actualiza) agregados Role.
- Elimina agregados Role.
- Verifica la existencia de roles por nombre o ID.

**JpaSessionRepositoryImpl**<br>
| Nombre | Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| JpaSessionRepositoryImpl | Repository Implementation | UserRepository | Implementación concreta de la interfaz SessionRepository utilizando JPA y Spring Data JPA. Maneja el mapeo entre el agregado de dominio Session y la base de datos. |
	
**Funcionalidad clave**<br>
- Busca y carga agregados Session por ID, refreshToken, etc.
- Guarda (inserta/actualiza) agregados Session.
- Elimina agregados Session.
- Puede tener métodos para encontrar sesiones válidas o expiradas.

**BCryptPasswordEncoderImpl**<br>
| Nombre | Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| BCryptPasswordEncoderImpl | Security Service Implementation | UserRepository | Implementación concreta de la interfaz UserRepository utilizando JPA y, típicamente, Spring Data JPA. Maneja el mapeo entre la entidad de dominio User y la tabla/colección de la base de datos subyacente. |
	
**Funcionalidad clave**<br>
- String encode(CharSequence rawPassword): Genera el hash de una contraseña plana.
- boolean matches(CharSequence rawPassword, String encodedPassword): Verifica si una contraseña plana coincide con un hash dado.

**JwtProviderImpl**<br>
| Nombre | Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| JwtProviderImpl | Repository Implementation | Password Encoder | Implementación concreta de una interfaz PasswordEncoder (definida en una capa superior o estándar de framework) que utiliza el algoritmo BCrypt para hashear y verificar contraseñas de forma segura. |

**Funcionalidad clave**<br>
- String generateAccessToken(UserDetails userDetails, ...): Crea y firma un JWT para autenticación.
- String generateRefreshToken(SessionId sessionId, ...): Crea y firma un JWT para refresco de sesión.
- Métodos para extraer información (ej. userId, sessionId, roles) de un token válido.

#### 4.2.1.5 Bounded Context Software Architecture Component Level Diagrams
![Component Level Diagrams IAM]()

##### 4.2.1.6.1 Bounded Context Domain Layer Class Diagrams
![Bounded Context Domain Layer Class Diagrams IAM]()

##### 4.2.1.6.2 Bounded Context Database Design Diagram
![Bounded Context Database Design Diagram IAM]()

### 4.2.2 Bounded Context: Vehicles & Tracking
Este bounded context centraliza la gestión de los vehículos de la flota, sus características, rutas asignadas, informes de infracciones y reportes de velocidad mediante geolocalización en tiempo real, asegurando el monitoreo y control de las unidades.

#### 4.2.2.1 Domain Layer
**Aggregate 1: Vehicles**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| Vehicles | Entity / Aggregate | Representa al vehículo en sí; es la entidad principal que gestiona sus rutas, reportes y sensores. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| vehicleId | UUID | Private | Identificador único del vehículo en el sistema. |
| vehiclePlate | String | Private | Matrícula o placa del vehículo. |
| brand | String | Private | Marca del vehículo (ej: Toyota, Volvo). |
| model | String | Private | Modelo del vehículo (ej: Corolla, FH16). |
| year | Int | Private | Año de fabricación del vehículo. |
| status | String | Private | Estado actual del vehículo (ej: activo, en mantenimiento). |
| speedSensor | SpeedSensor | Private | Objeto que almacena información del sensor de velocidad. |
| humeditySensor | HumeditySensor | Private | Objeto que almacena información del sensor de humedad. |
| gpsSensor | GPSSensor | Private | Objeto que almacena información del sensor GPS. |
| driverHistory | List<Driverhistory> | Private | Historial de conductores asociados al vehículo. |
| vehicleRoutes | List<VehicleRoute> | Private | Rutas asignadas o recorridas por el vehículo. |
| vehicleReports | List<ReportVehicle> | Private | Lista de reportes generales sobre el vehículo. |
		
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| generateVehicleReport() | ReportVehicle | Public | Genera un reporte de condiciones generales del vehículo. |
| assignDriver(DriverHistory driverHistory) | Void | Public | Asigna o actualiza el historial de conductor para el vehículo. |

**Aggregate 2: VehicleRoute**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| VehicleRoute | Entity | Representa las rutas asignadas a un vehículo, indicando su recorrido planificado o histórico. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| routeId | UUID | Private | Identificador único de la ruta. |
| vehicleId | UUID | Private | Identificador del vehículo asociado a la ruta. |
| startLocation | String | Private | Punto de partida de la ruta. |
| endLocation | String | Private | Punto de destino de la ruta. |
| waypoints | List<string> | Private | Lista de puntos intermedios o paradas durante la ruta. |
| estimatedTime | Integer | Private | Tiempo estimado en minutos para completar la ruta. |
| distance | Double | Private | Distancia total de la ruta en kilómetros. |
| status | String | Private | Estado de la ruta (Ej: "Programada", "En curso", "Completada", "Cancelada"). |
| startTime | DateTime | Private | Hora y fecha de inicio programado de la ruta. |
| endTime | DateTime | Private | Hora y fecha de finalización programada o real de la ruta. |
		
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| startRoute() | Void | Public | Inicia la ruta actualizando el estado a "En curso" y registrando la hora de inicio. |
| completeRoute() | Void | Public | Finaliza la ruta, actualizando el estado a "Completada" y registrando la hora de fin. |
| updateWaypoints(newWaypoints: List<String>) | Void | Public | Actualiza la lista de puntos intermedios de la ruta. |
| calculateDistance() | Double | Public | Calcula y devuelve la distancia total de la ruta basándose en las coordenadas. |
| getRouteDuration() | Integer | Public | Retorna la duración total (en minutos) entre el inicio y el final de la ruta. |
| isRouteActive() | Boolean | Public | Verifica si la ruta está actualmente en estado "En curso". |

**Aggregate 3: RouteTracking**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| RouteTracking | Entity | Representa la ubicación en tiempo real y el seguimiento de las rutas. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| trackingId | UUID | Private | Identificador único del seguimiento de ruta. |
| vehicleId | UUID | Private | Identificador del vehículo que está siendo rastreado. |
| currentLocation | String | Private | Ubicación actual del vehículo (puede ser en coordenadas o nombre de lugar). |
| speed | Double | Private | Velocidad actual del vehículo en km/h. |
| timestamp | DateTime | Private | Fecha y hora del último registro de seguimiento. |
| routeId | UUID | Private | Ruta asignada en la cual se está realizando el seguimiento. |
| isOverSpeeding | Boolean | Private | Indica si el vehículo está excediendo el límite de velocidad permitido |
		
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| updateLocation(newLocation: String) | Void | Public | Actualiza la ubicación actual del vehículo. |
| detectOverSpeed(limit: Double) | Boolean | Public | Detecta si la velocidad actual supera el límite establecido. |
| getTrackingSummary() | String | Public | Devuelve un resumen textual del estado actual de seguimiento. |
| isOnRoute() | Boolean | Public | Verifica si el vehículo aún sigue dentro de la ruta asignada. |
| refreshTimestamp() | Void | Public | Actualiza el timestamp al momento actual para el nuevo dato registrado. |

**Value Object: GPSSensor**<br>
| Nombre| Categoría | Descripción | 
| --- | --- | ---|
| GPSSensor | Value Object | Representa el dispositivo GPS que rastrea la localización del vehículo en tiempo real. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción | 
| --- | --- | --- | --- |
| gpsId | UUID | Private | Identificador único del sensor GPS. |
| vehicleId | UUID | Private | Identificador del vehículo que está siendo geolocalizado. |
| latitude | Double | Private | Latitud actual registrada por el GPS. |
| longitude | Double | Private | Longitud actual registrada por el GPS. |
| accuracy | Double | Private | Precisión de la ubicación registrada (en metros). |
| timestamp | DateTime | Private | Hora en la que se registró la ubicación. |
		
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| updateCoordinates(newLat: Double, newLong: Double) | Void | Public | Actualiza las coordenadas geográficas actuales. |
| getLocation() | String | Public | Devuelve la ubicación actual como un string formateado. |
| getAccuracy() | Double | Public | Obtiene la precisión del último registro de ubicación. |
| refreshTimestamp() | Void | Public | Actualiza el tiempo del último registro de datos. |

**Value Object: SpeedSensor**<br>
| Nombre| Categoría | Descripción | 
| --- | --- | ---|
| SpeedSensor | Value Object | Representa el sensor de velocidad del vehículo, almacenando datos de medición. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción | 
| --- | --- | --- | --- |
| speedSensorId | UUID | Private | Identificador único del sensor de velocidad. |
| vehicleId | UUID | Private | Identificador del vehículo que está siendo rastreado. |
| currentSpeed | Double | Private | Velocidad actual detectada por el sensor (km/h). |
| speedLimit | Double | Private | Límite de velocidad permitido. |
| timestamp | DateTime | Private | Fecha y hora del último dato registrado. |
		
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| updateSpeed(newSpeed: Double) | Void | Public | Actualiza la velocidad medida por el sensor. |
| isOverSpeeding() | Boolean | Public | Verifica si se supera el límite de velocidad. |
| setSpeedLimit(limit: Double) | Void | Public | Establece un nuevo límite de velocidad. |
| refreshTimestamp() | Void | Public | Actualiza el tiempo del último dato de velocidad. |

**Value Object: HumiditySensor**<br>
| Nombre| Categoría | Descripción | 
| --- | --- | ---|
| HumiditySensor | Value Object | Representa el sensor de humedad instalado en el vehículo. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción | 
| --- | --- | --- | --- |
| humidityId | UUID | Private | Identificador único del sensor de humedad. |
| vehicleId | UUID | Private | ID del vehículo al que está asociado el sensor. |
| humidity | Float | Private | Porcentaje de humedad relativa actual (0-100%). |
| status | String | Private | Estado del sensor ("Active", "Inactive", "Error", etc.). |
| timestamp | DateTime | Private | Hora del último registro de humedad. |
| minThreshold | Float | Private | Valor mínimo aceptable de humedad. |
| maxThreshold | Float | Private | Valor máximo aceptable de humedad. |
	
**Methods**<br>
| Nombre| Tipo de retorno | Visibilidad | Descripción |
| --- | --- | --- | --- |
| updateCoordinates(newLat: Double, newLong: Double) | Void | Public | Actualiza las coordenadas geográficas actuales. |
| getLocation() | String | Public | Devuelve la ubicación actual como un string formateado. |
| getAccuracy() | Double | Public | Obtiene la precisión del último registro de ubicación. |
| refreshTimestamp() | Void | Public | Actualiza el tiempo del último registro de datos. |

#### 4.2.2.2 Interface Layer
**Controller 1: VehicleController**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| VehicleController | Controller | Controlador para los endpoints relacionados con la gestión del ciclo de vida de vehículos y sus componentes IoT (registro, actualización, monitoreo y desactivación de vehículos). |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| vehicleService | VehicleService | Private | Servicio de la capa de Aplicación para lógica de gestión del ciclo de vida de vehículos. |
| vehicleMapper | VehicleMapper | Private | Mapper para convertir entre DTOs y objetos usados por Application/Domain |

**Endpoints**<br>
| Ruta| Método | Descripción |
| --- | --- | --- |
| /vehicles | POST | Crea un nuevo vehículo en el sistema. |
| /vehicles/{id} | PUT | Actualiza la información de un vehículo existente. |
| /vehicles/{id} | GET | Recupera la información de un vehículo usando su ID. |
| /vehicles | GET | Obtiene todos los vehículos registrados en el sistema. |

**Controller 2: RouteController**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| RouteController | Controller | Controlador para gestionar las operaciones relacionadas con las rutas de vehículos, incluyendo creación, actualización, seguimiento en tiempo real y análisis histórico de trayectorias. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| routeService | RouteService | Private | Servicio de la capa de Aplicación para las rutas de vehículos. |
| routeMapper | RouteMapper | Private | Mapper para convertir entre DTOs y objetos usados por Application/Domain |

**Endpoints**<br>
| Ruta| Método | Descripción |
| --- | --- | --- |
| /routes | POST | Crea una nueva ruta para un vehículo. |
| /routes/{id} | PUT | Actualiza la información de una ruta existente. |
| /routes/{id} | GET | Recupera los detalles de una ruta específica. |
| /routes | GET | Obtiene todas las rutas activas o completadas. |
Ruta

**Controller 3: TrackingController**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| TrackingController | Controller | Controlador encargado del monitoreo en tiempo real de vehículos, gestionando la recopilación de datos GPS, actualización continua de ubicaciones, detección de desviaciones de ruta, generación de alertas inmediatas y visualización dinámica de flotas en mapas interactivos. |

**Attributes**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| trackingService | TrackingService | Private | Servicio de la capa de Aplicación para el monitoreo en tiempo real de vehículos. |
| trackingMapper | TrackingMapper | Private | Mapper para convertir entre DTOs y objetos usados por Application/Domain |

**Endpoints**<br>
| Ruta| Método | Descripción |
| --- | --- | --- |
| /tracking/{id} | GET | Recupera el seguimiento en tiempo real de una ruta. |
| /tracking/{id}/update | POST | Actualiza la ubicación y velocidad de un vehículo en seguimiento. |
| /tracking/{id}/speed-warning | GET | Verifica si el vehículo ha superado el límite de velocidad. |

**DTOs**<br>
| Nombre| Descripción |
| --- | --- |
| RegisterVehicleRequestDto | { licensePlate: String, brand: String, model: String, status: String } |
| UpdateVehicleRequestDto | { vehicleId: UUID, licensePlate: String, brand: String, model: String, status: String } |
| VehicleResponseDto | { vehicleId: UUID, licensePlate: String, brand: String, model: String, status: String } |
| RegisterRouteRequestDto | { vehicleId: UUID, startLocation: String, endLocation: String, status: String } |
| UpdateRouteRequestDto | { routeId: UUID, vehicleId: UUID, startLocation: String, endLocation: String, status: String } |
| RouteResponseDto | { routeId: UUID, vehicleId: UUID, startLocation: String, endLocation: String, status: String } |
| TrackingRequestDto | { trackingId: UUID, vehicleId: UUID, currentLocation: String, currentSpeed: Double, overSpeeding: Boolean } |
| TrackingResponseDto | { trackingId: UUID, vehicleId: UUID, currentLocation: String, currentSpeed: Double, overSpeeding: Boolean } |
| SpeedWarningRequestDto | { vehicleId: UUID, speedLimit: Double, currentSpeed: Double } |
| SpeedWarningResponseDto | { vehicleId: UUID, speedLimit: Double, isOverSpeeding: Boolean } |

#### 4.2.2.3Application Layer

**Service 1: VehicleService**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| VehicleService | Service | Servicio que coordina la lógica relacionada con los vehículos. Maneja la creación, actualización y eliminación de vehículos. |
	
**Dependencies**<br>
| Nombre| Tipo de Objeto | Visibilidad | Descripción |
| --- | --- | --- | --- |
| vehicleRepository | VehicleRepository | Private | Repositorio que interactúa con la base de datos para persistir la información de los vehículos. |
| vehicleMapper | VehicleMapper | Private | Mapea objetos de tipo VehicleDto a entidades del dominio y viceversa. |
| notificationService | NotificationService | Private | Servicio que maneja la notificación de eventos relacionados con los vehículos, como la creación o actualización. |

**Methods**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| registerVehicle | void | Public | Registra un nuevo vehículo en el sistema. |
| updateVehicle | void | Public | Actualiza los detalles de un vehículo ya registrado. |
| deleteVehicle | void | Public | Elimina un vehículo del sistema. |

**Service 2: RouteService**<br>
| Nombre| Categoría | Descripción |
| --- | --- | --- |
| RouteService | Service | Servicio que maneja la creación, actualización y eliminación de rutas en el sistema de bicicletas y vehículos. |
	
**Dependencies**<br>
| Nombre| Tipo de Objeto | Visibilidad | Descripción |
| --- | --- | --- | --- |
| routeRepository | RouteRepository | Private | Repositorio que maneja la persistencia de datos relacionados con las rutas. |
| routeMapper | RouteMapper | Private | Mapea objetos de tipo RouteDto a entidades del dominio y viceversa. |
| auditService | AuditService | Private | Servicio que maneja el registro de auditoría para la creación y modificación de rutas. |

**Methods**<br>
| Nombre| Tipo de dato | Visibilidad | Descripción |
| --- | --- | --- | --- |
| createRoute | void | Public | Crea una nueva ruta en el sistema. |
| updateRoute | void | Public | Actualiza los detalles de una ruta existente. |
| deleteRoute | void | Public | Elimina una ruta del sistema. |

#### 4.2.2.4 Infrastructure Layer
**VehicleRepositoryImpl**<br>
| Nombre| Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| VehicleRepositoryImpl |Repositorio | VehicleRepository | Implementación del repositorio para acceder a la base de datos de vehículos. |

**Funcionalidad clave**<br>
- Busca y carga vehículos por ID, nombre, tipo, etc.
- Guarda (inserta/actualiza) vehículos.
- Elimina vehículos.
- Verifica la existencia de vehículos por ID.
- Filtra vehículos por estado o tipo.

**TrackingRepositoryImpl**<br>
| Nombre| Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| TrackingRepositoryImpl |Repositorio | TrackingRepository | Implementación del repositorio para acceder a los registros de tracking de los vehículos. |

**Funcionalidad clave**<br>
- Busca y carga datos de seguimiento por ID de vehículo.
- Guarda (inserta/actualiza) registros de tracking.
- Elimina registros de tracking.
- Verifica la existencia de registros de tracking por ID de vehículo.
- Filtra registros de tracking por rango de fecha.

**VehicleTrackingServiceImpl**<br>
| Nombre| Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| VehicleTrackingServiceImpl |Servicio | VehicleTrackingService | Servicio que maneja la lógica de negocio para gestionar vehículos y su seguimiento. |

**Funcionalidades clave**<br>
- Obtiene el historial de posiciones de un vehículo dentro de un rango de tiempo.
- Calcula la ruta recorrida por un vehículo basado en los datos de tracking.
- Actualiza la información de seguimiento de un vehículo en tiempo real.
- Verifica la disponibilidad de un vehículo para su seguimiento.
- Envía alertas relacionadas con el estado de los vehículos, como el exceso de velocidad o la detención prolongada.

**GeoLocationServiceImpl**<br>
| Nombre| Categoría | Implementa | Descripción |
| --- | --- | --- | --- |
| GeoLocationServiceImpl |Servicio | GeoLocationService | Servicio que maneja la lógica para obtener y calcular las ubicaciones geográficas de los vehículos. |

**Funcionalidades clave**<br>
- Obtiene la ubicación geográfica actual de un vehículo usando GPS.
- Calcula la distancia entre dos ubicaciones geográficas.
- Determina la ruta más corta entre dos puntos usando datos de ubicación.
- Proporciona información de tráfico en tiempo real para optimizar rutas.
- Actualiza la ubicación del vehículo en tiempo real en el sistema de seguimiento.

#### 4.2.2.5 Bounded Context Software Architecture Component Level Diagrams
![Component Level Diagrams V&T]()

#### 4.2.2.6 Bounded Context Software Architecture Code Level Diagrams

##### 4.2.2.6.1 Bounded Context Domain Layer Class Diagrams
![Bounded Context Domain Layer Class Diagrams V&T]()

##### 4.2.2.6.2 Bounded Context Database Design Diagram
![Bounded Context Database Design Diagram V&T]()

