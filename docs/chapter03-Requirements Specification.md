# Capítulo 3: Requirements Specification
## 3.1 To-Be Scenario Mapping

CONDUCTOR:

![To-Be Conductor](/assets/chapter03/to-be%20scenario%20conductor.png)

EMPRESARIO:

![To-Be Empresario](/assets/chapter03/to-be%20scenario%20empresario.png)

## 3.2 User Stories

USER STORIES 
<table>
<tr>
        <th>Epic ID</th>
        <th>Titulo</th>
        <th>Descripcion</th>
    </tr>
    <tr>
        <td>EP01</td>
        <td>Technical Histories</td>
        <td>Como desarrollador quiero manejar la aplicación mediante APIrest para controlar los datos y el flujo de este por toda la solución.</td>
    </tr>
    <tr>
        <td>EP02</td>
        <td>Información del sitio web</td>
        <td>Como visitante quiero información detallada y precisa de lo que ofrece el sitio web para tomar mejores decisiones.</td>
    </tr>
    <tr>
        <td>EP03</td>
        <td> Navegación de sitio web</td>
        <td>Como visitante quiero una navegación fluida y detallada para tomar una desicion a conciencia</td>
    </tr>
    <tr>
        <td>EP04</td>
        <td> Visualización de estadísticas de transportistas</td>
        <td>Como gerente quiero tener un registro de actividades hechas por todos los transportistas para tener un control y seguimiento del rendimiento general de mis empleados.</td>
    </tr>
    <tr>
        <td>EP05</td>
        <td>Visualización de estadísticas propias</td>
        <td>Como transportista quiero ver las acciones hechas durante mi trabajo para tener un registro de las actividades hechas en mi labor.</td>
    </tr>
    <tr>
        <td>EP06</td>
        <td>Gestión de envíos</td>
        <td>Como gerente quiero un registrar envíos a mis transportistas y tener un control de ello a través del tiempo para mejorar el rendimiento de los envíos de mi empresa.</td>
    </tr>
    <tr>
        <td>EP07</td>
        <td>Gestión de vehículos</td>
        <td>Como gerente quiero un registro de mis vehículos a si como quien esta a cargo de ellos para tener un seguimiento de su estado a través del tiempo.</td>
    </tr>
    <tr>
        <td>EP08</td>
        <td>Gestión de datos personales</td>
        <td>Como usuario quiero manejar mi información personal para tenerla actualizada en todo momento.</td>
    </tr>
    <tr>
        <td>EP09</td>
        <td>Reporte de problemas</td>
        <td>Como transportista quiero reportar problemas que puedan suceder en mi labor para que se tomen las medidas necesarias.</td>
    </tr>
    <tr>
        <th>Epic Id</th>
        <th>Story Id</th>
        <th>Titulo</th>
        <th>Descripcion</th>
        <th>Criterios de aceptacion</th>
    </tr>
    <!-- SEPARACION DE ENCABEZADOS -->
    <tr>
        <td rowspan="6">EP04</td>
        <td rowspan="2">US01</td>
        <td rowspan="2">Visualización de paquetes entregados por un transportista</td>
        <td rowspan="2">Como gerente quiero visualizar el registro de paquetes entregados por un transportista para medir rendimiento del transportista</td>
        <td>Visualización del Registro de Paquetes Entregados - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente accede al perfil del transportista cuyo rendimiento desea medir. Entonces se muestra un registro claro y detallado de todos los paquetes entregados por el transportista, incluyendo la fecha y hora de entrega, la descripción del paquete y cualquier otra información relevante.</td>
    </tr>
    <tr>
        <td>Filtrado y Ordenación de Registros - Dado el gerente está visualizando el registro de paquetes entregados por el transportista. Cuando el gerente necesita analizar los datos de manera específica. Entonces se proporcionan opciones para filtrar y ordenar los registros según diferentes criterios, como la fecha de entrega, el estado del paquete o el cliente, lo que permite al gerente acceder a la información relevante de manera rápida y eficiente.</td>
    </tr>
    <tr>
        <td rowspan="2">US02</td>
        <td rowspan="2">Visualización de reportes de un transportista</td>
        <td rowspan="2">Como gerente quiero ver los reportes hechos por mis transportistas para tomar decisiones estratégicas en los próximos envíos.</td>
        <td>Visualización de reportes - Dado el gerente esta autenticado en la aplicación. Cuando el gerente accede a la sección de reportes de la aplicación. Entonces se muestra un resumen claro y detallado de todos los reportes realizados por los transportistas.</td>
    </tr>
    <tr>
        <td>Análisis para Decisiones Estratégicas - Dado el gerente está visualizando los reportes de los transportistas. Cuando el gerente revisa los reportes de manera detallada. Entonces el gerente utiliza la información de los reportes para tomar decisiones estratégicas en cuanto a la asignación de rutas, la mejora de los procesos operativos y la implementación de medidas correctivas, con el objetivo de optimizar el rendimiento y la eficiencia en los próximos envíos.</td>
    </tr>
    <tr>
        <td rowspan="2">US03</td>
        <td rowspan="2">Visualización de envíos asignados a un transportista</td>
        <td rowspan="2">Como gerente quiero ver los envíos asignados de un transportista para poder medir el rendimiento de mis empleados.</td>
        <td>Visualización de Envíos Asignados - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente accede al perfil del transportista cuyo rendimiento desea medir. Entonces se muestra un listado claro y completo de todos los envíos asignados al transportista, incluyendo detalles como el origen, destino, fecha de entrega programada y estado actual de cada envío.</td>
    </tr>
    <tr>
        <td>Acceso a Detalles de Envíos - Dado el gerente está visualizando los envíos asignados de un transportista. Cuando el gerente selecciona un envío específico de la lista. Entonces se despliegan los detalles completos del envío seleccionado, incluyendo información detallada sobre la carga, instrucciones especiales del cliente y cualquier otra información relevante para la entrega.</td>
    </tr>
    <!-- SEPARACION DE EPIC 4 -->
    <tr>
        <td rowspan="8">EP05</td>
        <td rowspan="3">US04</td>
        <td rowspan="3">Visualización de envíos asignados</td>
        <td rowspan="3">Como transportista, quiero poder ver los envíos que me han sido asignados, incluyendo detalles sobre los envíos y destinos correspondientes para poder organizar mejor el orden de mis tareas.</td>
        <td>Visualización de Envíos Asignados - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista accede a la sección de "Mis Envíos" en la aplicación. Entonces el transportista puede ver una lista clara y actualizada de todos los envíos que le han sido asignados, con detalles completos sobre cada envío.</td>
    </tr>
    <tr>
        <td>Detalles Claros y Accesibles - Dado el transportista está viendo los envíos asignados. Cuando el transportista selecciona un envío específico de la lista. Entonces se muestran los detalles detallados del envío de manera clara y accesible, incluyendo la dirección de recogida, la dirección de entrega, la fecha límite de entrega y cualquier instrucción especial asociada con el envío.</td>
    </tr>
    <tr>
        <td>Facilidad de Organización - Dado el transportista está viendo los envíos asignados. Cuando el transportista necesita organizar el orden de sus tareas. Entonces se proporcionan opciones para que el transportista organice los envíos según su conveniencia, ya sea por fecha de entrega o proximidad geográfica.</td>
    </tr>
    <tr>
        <td rowspan="2">US05</td>
        <td rowspan="2">Visualización de paquetes entregados</td>
        <td rowspan="2">Como transportista quiero visualizar los paquetes que he entregado para tener un comprobante de trabajo realizado</td>
        <td>Visualización de Paquetes Entregados - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista accede a su perfil o panel de control. Entonces se muestra un registro claro y detallado de todos los paquetes que ha entregado.</td>
    </tr>
    <tr>
        <td>Acceso Fácil y Rápido a los Registros - Dado el transportista está visualizando sus paquetes entregados. Cuando el transportista necesita acceder a registros específicos. Entonces se proporcionan opciones de búsqueda y filtrado para que el transportista pueda encontrar rápidamente los paquetes entregados en función de diferentes criterios, como la fecha de entrega o el estado del paquete.</td>
    </tr>
    <tr>
        <td rowspan="3">US06</td>
        <td rowspan="3">Visualización de reportes realizados</td>
        <td rowspan="3">Como transportista quiero visualizar los reportes que hice en mi labor para tener un historial de incidencia en mi trabajo.</td>
        <td>Visualización de Reportes Realizados - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista accede a la sección de "Mis Reportes" o "Historial de Incidencias". Entonces se muestra una lista completa y organizada de todos los reportes que el transportista ha realizado durante su labor, incluyendo problemas técnicos, infracciones vehiculares, accidentes en la carretera y problemas con los paquetes.</td>
    </tr>
    <tr>
        <td>Detalles Claros y Accesibles - Dado el transportista está visualizando sus reportes realizados. Cuando el transportista selecciona un reporte específico de la lista. Entonces se muestran los detalles detallados del reporte de manera clara y accesible, incluyendo la fecha y hora del reporte, la descripción del incidente y cualquier otra información relevante asociada al reporte.</td>
    </tr>
    <tr>
        <td>Funcionalidad de Búsqueda y Filtrado - Dado el transportista está visualizando sus reportes realizados. Cuando el transportista necesita encontrar un reporte específico en su historial. Entonces se proporcionan opciones de búsqueda y filtrado para que el transportista pueda buscar y acceder rápidamente a un reporte específico utilizando diferentes criterios, como la fecha del reporte o el tipo de incidencia, facilitando la navegación y la gestión del historial de incidencias.</td>
    </tr>
    <!-- SEPARACION DE EPIC 5-->
    <tr>
        <td rowspan="4">EP06</td>
        <td rowspan="2">US07</td>
        <td rowspan="2">Asignación de envíos</td>
        <td rowspan="2">Como gerente, quiero poder asignar envíos a mis transportistas para distribuir eficientemente los envíos.</td>
        <td>Asignación Exitosa de Envíos - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente selecciona un envío para asignarlo a un transportista específico. Entonces el envío se asigna correctamente al transportista seleccionado en la aplicación.</td>
    </tr>
    <tr>
        <td>Asignación sin éxito de envío - Dado el gerente registra un envío sin éxito. Cuando el gerente completa el formulario de envío. Entonces se muestra un mensaje de error y es dirigido a la pagina principal.</td>
    </tr>
    <tr>
        <td rowspan="2">US08</td>
        <td rowspan="2">Visualización de historial de envíos</td>
        <td rowspan="2">Como gerente quiero ver el historial de envíos realizado para saber cuantos de estos fueron exitosos</td>
        <td>Visualización del Historial de Envíos - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente accede a la sección de historial de envíos. Entonces se muestra un registro completo y detallado de todos los envíos realizados, incluyendo información como la fecha de envío, origen, destino y estado de entrega de cada envío.</td>
    </tr>
    <tr>
        <td>Filtrado por Envíos Exitosos - Dado el gerente está visualizando el historial de envíos. Cuando el gerente selecciona la opción para filtrar por envíos exitosos. Entonces se muestran únicamente los envíos que han sido completados con éxito, lo que permite al gerente identificar rápidamente la cantidad y los detalles de los envíos exitosos realizados en un período específico.</td>
    </tr>
    <!-- SEPARACION DE EPIC 6-->
    <tr>
        <td rowspan="7">EP07</td>
        <td rowspan="3">US09</td>
        <td rowspan="3">Asignación de flotas </td>
        <td rowspan="3">Como gerente, quiero asignar flotas a mis transportistas para que puedan realizar encargos.</td>
        <td>Asignación Exitosa de Flotas - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente selecciona una flota para asignarla a un transportista específico. Entonces la flota se asigna correctamente al transportista seleccionado en la aplicación.</td>
    </tr>
    <tr>
        <td>Asignación de flotas sin éxito - Dado el gerente asigna una flota para un transportista. Cuando el gerente registra el proceso. Entonces se muestra un mensaje de error y se redirige a la pagina principal.</td>
    </tr>
    <tr>
        <td>Asignación de flota a transportista con flota ya existente: Dado el gerente asigna una flota a un transportista. Cuando el transportista ya tiene asignado una flota ya existente. Entonces se reemplaza la flota del transportista con la actual registrada.</td>
    </tr>
    <tr>
        <td rowspan="4">US10</td>
        <td rowspan="4">Gestión de inventario de flotas </td>
        <td rowspan="4">Como gerente, quiero añadir nuevas flotas a mi negocio para tener un control activo de mis flotas.</td>
        <td>Añadir Nuevas Flotas - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente accede a la sección de gestión de flotas y selecciona la opción para añadir una nueva flota. Entonces se presenta un formulario claro y completo donde el gerente puede ingresar todos los detalles relevantes de la nueva flota como placa, modelo y numero de serie del vehículo.</td>
    </tr>
    <tr>
        <td>Confirmación de Añadido Exitoso - Dado el gerente ha añadido una nueva flota con éxito. Cuando la operación de añadir la nueva flota se completa. Entonces se muestra un mensaje de confirmación claro y visible en la aplicación, informando al gerente que la nueva flota ha sido añadida con éxito a su negocio, lo que le permite tener un control activo y actualizado de todas sus flotas.</td>
    </tr>
    <tr>
        <td>Añadido fallido - Dado el gerente ha completado el formulario de añadido de flota. Cuando envíe el formulario. Entonces se mostrara un mensaje de error y será redirigido a la pagina principal</td>
    </tr>
    <tr>
        <td>Añadir flota existente: Dado el gerente añade una flota. Cuando el gerente añada una flota con un numero de serie ya existente. Entonces se mostrara un mensaje de error Y no se registrara la nueva flota.</td>
    </tr>
    <!-- SEPARACION DE EPIC 7-->
    <tr>
        <td rowspan="6">EP08</td>
        <td rowspan="3">US11</td>
        <td rowspan="3">Modificar perfil de gerente</td>
        <td rowspan="3">Como gerente quiero gestionar mis datos para que estén actualizados</td>
        <td>Acceso a la Gestión de Datos - Dado el gerente está autenticado en la aplicación MoviGestion. Cuando el gerente accede a su perfil personal. Entonces se muestra la opción clara y accesible para gestionar sus datos personales.</td>
    </tr>
    <tr>
        <td>Modificación de Datos - Dado el gerente está en la sección de gestión de datos de su perfil. Cuando el gerente realiza cambios en sus datos, como nombre, número de contacto o dirección de correo electrónico. Entonces los cambios se reflejan de manera inmediata y precisa en su perfil, asegurando que la información esté actualizada.</td>
    </tr>
    <tr>
        <td>Confirmación de Actualización Exitosa - Dado el gerente ha modificado sus datos. Cuando la modificación se completa. Entonces se muestra un mensaje de confirmación que indica que los datos se han actualizado correctamente, proporcionando retroalimentación al gerente sobre el éxito de la operación.</td>
    </tr>
    <tr>
        <td rowspan="3">US12</td>
        <td rowspan="3">Modificar perfil de transportistas</td>
        <td rowspan="3">Acceso a la Gestión de Datos Personales - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista accede a su perfil personal. Entonces se muestra la opción clara y accesible para gestionar sus datos personales.</td>
    </tr>
    <tr>
        <td>Modificación de Datos Personales - Dado el transportista está en la sección de gestión de datos personales de su perfil. Cuando el transportista realiza cambios en sus datos personales, como nombre, número de contacto o dirección de correo electrónico. Entonces los cambios se reflejan de manera inmediata y precisa en su perfil, asegurando que la información esté actualizada.</td>
    </tr>
    <tr>
        <td>Confirmación de Actualización Exitosa - Dado el transportista ha modificado sus datos personales. Cuando la modificación se completa. Entonces se muestra un mensaje de confirmación que indica que los datos personales se han actualizado correctamente, proporcionando retroalimentación al transportista sobre el éxito de la operación</td>
    </tr>
    <!-- SEPARACION DE EPIC 8-->
    <tr>
        <td rowspan="9">EP09</td>
        <td rowspan="2">US13</td>
        <td rowspan="2">Reporte de infracciones</td>
        <td rowspan="2">Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes para que el gerente pueda tomar las medidas del caso.</td>
        <td>Registro de Infracciones Vehiculares - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista identifica una infracción vehicular durante su viaje. Entonces el transportista puede acceder a la función de reporte de infracciones vehiculares, proporcionar detalles sobre la infracción observada y enviar el reporte con éxito a la plataforma para su registro.</td>
    </tr>
    <tr>
        <td>Registro fallido de infracciones - Dado el transportista envía un reporte de infracción . Cuando hay algún error en el envío. Entonces se muestra un mensaje de error y se redirige a la pagina principal.</td>
    </tr>
    <tr>
        <td rowspan="2">US14</td>
        <td rowspan="2">Reporte de accidentes en la carretera</td>
        <td rowspan="2">Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes para que el gerente pueda organizar las futuras rutas.</td>
        <td>Registro de Accidentes en la Carretera - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista se encuentra con un accidente en la carretera durante su viaje. Entonces el transportista puede acceder a la función de reporte de accidentes en la carretera, proporcionar detalles sobre el accidente presenciado y enviar el reporte con éxito a la plataforma para su registro</td>
    </tr>
    <tr>
        <td>Error en registro de accidentes - Dado el transportista completa el formulario de accidentes. Cuando envía el formulario y hay problemas. Entonces se muestra un mensaje de error y se redirige a la pagina principal.</td>
    </tr>
    <tr>
        <td rowspan="2">US15</td>
        <td rowspan="2">Reporte de problemas con el paquete</td>
        <td rowspan="2">Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes para que el gerente pueda reportarlo al cliente.</td>
        <td>Registro de Problemas con los Paquetes - Dado el transportista está autenticado en la aplicación MoviGestion. Cuando el transportista detecta un problema con uno de los paquetes que está transportando durante su viaje. Entonces el transportista puede acceder a la función de reporte de problemas con los paquetes, proporcionar detalles sobre el problema encontrado y enviar el reporte con éxito a la plataforma para su registro.</td>
    </tr>
    <tr>
        <td>Registro fallido de problema con el paquete - Dado el transportista envío un reporte de problema con el paquete. Cuando el registro presente algún error. Entonces se mostrara un mensaje de error y se redirigirá ala página principal.</td>
    </tr>
    <tr>
        <td rowspan="3">US16</td>
        <td rowspan="3">Reporte de problemas técnicos</td>
        <td rowspan="3">Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes para que el gerente pueda resolverlo lo antes posible.</td>
        <td>Registro exitoso de problemas técnicos - Dado el transportista esta autenticado en la aplicación. Cuando el transportista encuentre un problema técnico durante su viaje. Entonces el transportista completa el formulario de reporte de problemas técnicos en la aplicación, proporcionando detalles sobre el problema y enviándolo con éxito para su registro.</td>
    </tr>
    <tr>
        <td>Registro sin éxito de problemas técnicos - Dado que el transportista esta autenticado en la aplicación. Cuando el transportista envía un registro de reporte no exitoso. Entonces se muestra un mensaje de "error" Y el transportista es enviado a la pagina principal.</td>
    </tr>
    <tr>
        <td>Seguimiento y Resolución Oportuna del Problema - Dado el gerente recibe la notificación sobre un problema técnico reportado por un transportista. Cuando el gerente revisa el reporte del problema técnico. Entonces el gerente realiza un seguimiento oportuno del problema reportado, toma las medidas necesarias para resolverlo lo antes posible y proporciona retroalimentación al transportista sobre las acciones tomadas para abordar el problema.</td>
    </tr>
    <!-- SEPARACION DE EPIC 9-->
    <!-- SEPARACION ENCABEZADOS -->
    <tr>
        <td rowspan="6">EP02</td>
        <td rowspan="2">US17</td>
        <td rowspan="2">Presentación de sitio web</td>
        <td rowspan="2">Como visitante del segmento gerente quiero un resumen rápido y asertivo sobre lo que ofrece el sitio web para tener una idea rápida sobre lo que ofrece el sitio web.</td>
        <td>Visualización del Resumen en el Landing Page - Dado el visitante accede al landing page del sitio web. Cuando el visitante visualiza la sección de resumen rápido.Entonces se presenta un resumen claro y conciso de las principales características y beneficios del sitio web, destacando los puntos más relevantes de manera atractiva y fácil de entender.</td>
    </tr>
    <tr>
        <td>Información Asertiva y Relevante - Dado el visitante está leyendo el resumen en el landing page. Cuando el visitante revisa la información presentada. Entonces la información proporcionada se centra en los aspectos más importantes y distintivos del sitio web, ofreciendo una visión rápida y clara de lo que ofrece y cómo puede beneficiar al usuario.</td>
    </tr>
    <tr>
        <td rowspan="2">US18</td>
        <td rowspan="2">Resumen de precios</td>
        <td rowspan="2">Como visitante del segmento gerente quiero una vista detallada del plan ofrecido por el sitio web para tomar una desicion de compra a conciencia.</td>
        <td>Acceso a la Información del Plan - Dado el visitante del segmento gerente está en el sitio web. Cuando el visitante busca información detallada sobre el plan ofrecido. Entonces se proporciona un acceso claro y visible a la página o sección que describe en detalle el plan ofrecido, ya sea a través del menú de navegación, enlaces destacados o botones de llamada a la acción</td>
    </tr>
    <tr>
        <td>Descripción Completa y Clara del Plan - Dado el visitante está en la página de información del plan. Cuando el visitante lee la descripción del plan. Entonces se presenta una descripción completa y clara del plan ofrecido, incluyendo características, beneficios, limitaciones, términos y condiciones, precio y cualquier otra información relevante que permita al visitante entender completamente lo que está incluido en el plan.</td>
    </tr>
    <tr>
        <td rowspan="2">US19</td>
        <td rowspan="2">Información a pie de pagina</td>
        <td rowspan="2">Como visitante del segmento gerente quiero un resumen del sitio web al final de este para no perder tiempo buscando algún apartado de mi interés.</td>
        <td>Resumen Claro y Conciso - Dado el visitante del segmento gerente está en el landing page del sitio web. Cuando el visitante llega al final de la página. Entonces se presenta un resumen claro y conciso del sitio web, destacando los aspectos más relevantes, como las características principales, los servicios ofrecidos, la información de contacto y cualquier otra información importante para el visitante.</td>
    </tr>
    <tr>
        <td>Navegación Rápida a Secciones Clave - Dado el visitante está revisando el resumen al final del landing page. Cuando el visitante busca acceder rápidamente a una sección específica del sitio web. Entonces se incluyen enlaces o botones que permiten al visitante navegar rápidamente a secciones clave del sitio web, como servicios, precios, testimonios, preguntas frecuentes o información de contacto, facilitando la exploración y la búsqueda de información relevante.</td>
    </tr>
    <!-- SEPARACION EPIC 2 -->
    <tr>
        <td rowspan="6">EP03</td>
        <td rowspan="2">US20</td>
        <td rowspan="2">Ir a aplicación web directamente</td>
        <td rowspan="2">Como visitante del segmento gerente quiero que la pagina me permita dirigirme directamente a la aplicación web principal para ahorrar tiempo.</td>
        <td>Llamado a la Acción Claro - Dado el visitante ha revisado el resumen en el landing page. Cuando el visitante desea obtener más información o realizar una acción específica. Entonces se presenta un llamado a la acción claro y visible que guía al visitante a explorar más a fondo el sitio web o tomar la acción deseada, como registrarse, suscribirse o contactar al equipo.</td>
    </tr>
    <tr>
        <td>Facilidad de Acceso desde Dispositivos Móviles - Dado el visitante del segmento gerente accede al sitio web desde un dispositivo móvil. Cuando el visitante desea dirigirse a la aplicación web principal. Entonces el enlace o botón para acceder a la aplicación web principal está optimizado para dispositivos móviles y es fácilmente accesible y usable en pantallas más pequeñas, asegurando una experiencia de usuario fluida y sin inconvenientes.</td>
    </tr>
    <tr>
        <td rowspan="2">US21</td>
        <td rowspan="2">Navegación de información</td>
        <td rowspan="2">Como visitante del segmento gerente quiero información precisa sobre lo que ofrece el sitio web para tomar una desicion mejor informada.</td>
        <td>Contenido Informativo Claro y Detallado -Dado el visitante del segmento gerente está en el sitio web. Cuando el visitante busca información sobre lo que ofrece el sitio web. Entonces se presenta contenido claro, detallado y preciso que describe las características, funcionalidades y beneficios del sitio web de manera comprensible y convincente.</td>
    </tr>
    <tr>
        <td>Descripción de Características Destacadas - Dado el visitante del segmento gerente está revisando la información del sitio web. Cuando el visitante busca comprender las características más destacadas. Entonces se proporciona una descripción específica de las características clave del sitio web, resaltando sus puntos fuertes y ventajas competitivas de manera clara y concisa.</td>
    </tr>
    <tr>
        <td rowspan="2">US22</td>
        <td rowspan="2">Navegación de contacto</td>
        <td rowspan="2">Como visitante del segmento gerente quiero ver información de contacto del sitio creado para sentir mas confianza del sitio web.</td>
        <td>Visible y Accesible en el Sitio Web - Dado el visitante del segmento gerente está en el sitio web. Cuando el visitante busca información de contacto. Entonces la información de contacto, como dirección de correo electrónico, número de teléfono y/o dirección física, se muestra claramente y de manera destacada en una sección visible del sitio web, como en el encabezado, pie de página o una sección dedicada específicamente a la información de contacto.</td>
    </tr>
    <tr>
        <td>Completa y Actualizada - Dado el visitante busca información de contacto. Cuando el visitante revisa la información proporcionada. Entonces la información de contacto es completa y precisa, incluyendo todos los detalles necesarios para que el visitante pueda comunicarse con el sitio web de manera efectiva. Además, se asegura de que la información esté actualizada y corresponda a la ubicación y horario de operación vigentes.</td>
    </tr>
    <!-- SEPARACION EPIC 3 -->
    <!-- SEPARACION ENCABEZADOS -->
    <tr>
        <td rowspan="6">EP01</td>
        <td rowspan="2">US23</td>
        <td rowspan="2">Technical - eliminar transportista</td>
        <td rowspan="2">Como desarrollador, quiero poder eliminar un transportista existente a través del API para mantener la integridad de la base de datos desde otras aplicaciones.</td>
        <td>Eliminar transportista exitosamente - Dado que el endpoint '/transportistas/{id}' está disponible Y un transportista con el ID proporcionado está almacenado en la base de datos. Cuando se envía una solicitud DELETE. Entonces se recibe una respuesta con estado 204. Y el transportista se elimina correctamente de la base de datos.</td>
    </tr>
    <tr>
        <td>Intentar eliminar un transportista inexistente - Dado que el endpoint '/transportistas/{id}' está disponible Y no hay ningún transportista con el ID proporcionado almacenado en la base de datos. Cuando se envía una solicitud DELETE. Entonces se recibe una respuesta con estado 404 Y se incluye un mensaje en el cuerpo de la respuesta con el valor "Transportista no encontrado".</td>
    </tr>
    <tr>
        <td rowspan="2">US24</td>
        <td rowspan="2">Technical - Agregar transportista</td>
        <td rowspan="2">Como desarrollador, quiero poder agregar un nuevo transportista a través del API para gestionar la base de datos de transportistas desde otras aplicaciones</td>
        <td>Agregar transportista exitosamente - Dado que el endpoint '/transportistas' está disponible. Cuando se envía una solicitud POST con los valores de nombre, número de contacto y correo electrónico. Entonces se recibe una respuesta con estado 201 Y se incluye un recurso de transportista en el cuerpo de la respuesta con un nuevo ID asignado y los valores registrados.</td>
    </tr>
    <tr>
        <td>Agregar transportista con nombre existente - Dado que el endpoint '/transportistas' está disponible Y un transportista con el mismo nombre ya está almacenado. Cuando se envía una solicitud POST con valores de nombre, número de contacto y correo electrónico idénticos. Entonces se recibe una respuesta con estado 400 Y se incluye un mensaje en el cuerpo de la respuesta con el valor "No se cumplen todas las restricciones".</td>
    </tr>
    <tr>
        <td rowspan="2">US25</td>
        <td rowspan="2">Technical - Actualizar informacion</td>
        <td rowspan="2">Como desarrollador, quiero poder actualizar la información de un transportista existente a través del API para mantener los datos actualizados desde otras aplicaciones.</td>
        <td>Actualizar información de transportista exitosamente - Dado que el endpoint '/transportistas/{id}' está disponible Y un transportista con el ID proporcionado está almacenado en la base de datos. Cuando se envía una solicitud PUT con valores actualizados para nombre, número de contacto o correo electrónico. Entonces se recibe una respuesta con estado 200 Y se incluye un recurso de transportista actualizado en el cuerpo de la respuesta.</td>
    </tr>
    <tr>
        <td>Intentar actualizar un transportista inexistente - Dado que el endpoint '/transportistas/{id}' está disponible Y no hay ningún transportista con el ID proporcionado almacenado en la base de datos. Cuando se envía una solicitud PUT con valores actualizados para nombre, número de contacto o correo electrónico. Entonces se recibe una respuesta con estado 404 Y se incluye un mensaje en el cuerpo de la respuesta con el valor "Transportista no encontrado".</td>
    </tr>
    <!-- SEPARACION EPIC 1 -->
</table>

Link Pivotal Tracker:https://www.pivotaltracker.com/projects/2700650

## 3.3 Impact Mapping
EMPRESARIO
![Impact Mapping Empresario 1](/assets/chapter03/ImpactMapGerente1.png)

![Impact Mapping Empresario 2](/assets/chapter03/ImpactMapGerente2.png)

![Impact Mapping Empresario 3](/assets/chapter03/ImpactMapGerente3.png)

TRANSPORTISTA
![Impact Maapping Transportista 1](/assets/chapter03/ImpactMapTrans1.png)

![Impact Maapping Transportista 2](/assets/chapter03/ImpactMapTrans2.png)

![Impact Maapping Transportista 3](/assets/chapter03/ImpactMapTrans3.png)

## 3.4 Product Backlog

| #Orden | User Story ID | Titulo | Descripcion | Story Points (1/2/3/5/8) |
|--------|---------------|--------|-------------|--------------------------|
| 1 | US17 | Presentación de sitio web | Como visitante del segmento gerente quiero un resumen rápido y asertivo sobre lo que ofrece el sitio web para tener una idea rápida sobre lo que ofrece el sitio web. | 1 |
| 2 | US20 | Ir a aplicación web directamente | Como visitante del segmento gerente quiero que la pagina me permita dirigirme directamente a la aplicación web principal para ahorrar tiempo. | 1 |
| 3 | US21 | Navegación de información | Como visitante del segmento gerente quiero información precisa sobre lo que ofrece el sitio web para tomar una desicion mejor informada. | 1 |
| 4 | US22 | Navegación de contacto | Como visitante del segmento gerente quiero ver información de contacto del sitio creado para sentir mas confianza del sitio web. | 1 |
| 5 | US18 | Resumen de precios | Como visitante del segmento gerente quiero una vista detallada del plan ofrecido por el sitio web para tomar una desicion de compra a conciencia. | 1 |
| 6 | US19 | Información a pie de pagina |Como visitante del segmento gerente quiero un resumen del sitio web al final de este para no perder tiempo buscando algún apartado de mi interés. | 1 |
| 7 | US07 | Asignación de envíos | Como gerente, quiero poder asignar envíos a mis transportistas para distribuir eficientemente los envíos. | 3 |
| 8 | US09 | Asignación de flotas | Como gerente, quiero asignar flotas a mis transportistas para que puedan realizar encargos. | 3 |
| 9 | US23 | Technical - eliminar transportista | Como desarrollador, quiero poder eliminar un transportista existente a través del API para mantener la integridad de la base de datos desde otras aplicaciones. | 3 |
| 10 | US24 | Technical - Agregar transportista | Como desarrollador, quiero poder agregar un nuevo transportista a través del API para gestionar la base de datos de transportistas desde otras aplicaciones. | 3 |
| 11 | US25 | Technical - Actualizar informacion | Como desarrollador, quiero poder actualizar la información de un transportista existente a través del API para mantener los datos actualizados desde otras aplicaciones | 3 |
| 12 | US11 | Modificar perfil de gerente | Como gerente quiero gestionar mis datos para que estén actualizados | 3 |
| 13 | US04 | Visualización de envíos asignados | Como transportista, quiero poder ver los envíos que me han sido asignados, incluyendo detalles sobre los envíos y destinos correspondientes para poder organizar mejor el orden de mis tareas. | 2 |
| 14 | US10 | Gestión de inventario de flotas | Como gerente, quiero añadir nuevas flotas a mi negocio para tener un control activo de mis flotas. | 2 |
| 15 | US01 | Visualización de paquetes entregados por un transportista | Como gerente quiero visualizar el registro de paquetes entregados por un transportista para medir rendimiento del transportista | 2 |
| 16 | US05 | Visualización de paquetes entregados | Como transportista quiero visualizar los paquetes que he entregado para tener un comprobante de trabajo realizado | 2 |
| 17 | US13 | Reporte de infracciones | Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes para que el gerente pueda tomar las medidas del caso. | 3 |
| 18 | US14 | Reporte de accidentes en la carretera | Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes para que el gerente pueda organizar las futuras rutas. | 3 |
| 19 | US15 |Reporte de problemas con el paquete | Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes para que el gerente pueda reportarlo al cliente. | 3 |
| 20 | US16 | Reporte de problemas técnicos | Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes para que el gerente pueda resolverlo lo antes posible. | 3 |
| 21 | US02 | Visualización de reportes de un transportista | Como gerente quiero ver los reportes hechos por mis transportistas para tomar decisiones estratégicas en los próximos envíos. | 2 |
| 22 | US06 | Visualización de reportes realizados | Como transportista quiero visualizar los reportes que hice en mi labor para tener un historial de incidencia en mi trabajo. | 2 |
| 23 | US03 | Visualización de envíos asignados a un transportista | Como gerente quiero ver los envíos asignados de un transportista para poder medir el rendimiento de mis empleados. | 2 |
| 24 | US08 | Visualización de historial de envíos | Como gerente quiero ver el historial de envíos realizado para saber cuantos de estos fueron exitosos | 2 |
| 25 | US12 | Modificar perfil de transportistas | Como transportista quiero gestionar mis datos personales para que estén actualizados | 3 |


Product Backlog Pivotal tracker:

![Product Backlog](/assets/chapter03/Product%20backlog.png)

LINK Pivotal Tracker:https://www.pivotaltracker.com/projects/2700650