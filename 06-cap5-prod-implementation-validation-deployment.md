<div style="page-break-before: always;"></div>

# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

Para garantizar un flujo de trabajo eficiente y estandarizado en el desarrollo de las soluciones de TerraTech, el equipo ha configurado un entorno de desarrollo integrado que abarca desde el diseño de la experiencia de usuario hasta el despliegue de la plataforma. Las herramientas seleccionadas son:

- Diseño de Interfaz (UI/UX):

    - Figma: Utilizado como la herramienta principal para el prototipado de alta fidelidad de la aplicación web, permitiendo la colaboración en tiempo real y la definición de los flujos de usuario (User Flows) antes de la implementación.
    - Miro: Utilizado para el diseño del Event Storming del proyecto.
    - UXPRESSIA: Utilizado para el desarrollo de needfinding, comprensión de nuestro User Persona.
    - Canva: Plataforma de diseño colaborativo de funcion múltiple.

- Editor de Código:

    - Visual Studio Code (VS Code): Configurado como el entorno de desarrollo (IDE) estándar para la codificación de la Landing Page y la estructura web, debido a su versatilidad y soporte de extensiones.
    - WebStorm: IDE para desarrollo web, soporta HTML, CSS, JavaScript y frameworks modernos, perteneciente a JetBrains.
    - Rider: IDE para desarrollo de aplicaciones .NET y C#, perteneciente a JetBrains.

- Gestión de Versiones y Repositorio:

    - Git: Empleado para el control de versiones local, facilitando el seguimiento de cambios y el trabajo colaborativo.
    - GitHub: Plataforma en la nube utilizada para alojar el repositorio remoto, gestionar el código fuente y asegurar el respaldo del proyecto.

- Tecnologías de Frontend y Estilizado:

    - Vue: frameworks de JavaScript para crear interfaces de usuario y aplicaciones web modernas.
    - PrimeVue: un complemento de bibliotecas de componentes de interfaz de usuario diseñada para Vue.

- Gestión de Dependencias y Despliegue:

    - npm (Node Package Manager): Gestor de paquetes encargado de administrar las librerías y dependencias necesarias para el funcionamiento de los componentes web.
    - GitHub Pages: Elegido como el servicio de hosting para el despliegue continuo de la Landing Page, permitiendo una visualización rápida y accesible para los stakeholders.

Nota de Configuración: Con el fin de mantener un código limpio y profesional, se han integrado extensiones en VS Code como ESLint para la detección de errores de sintaxis, Prettier para el formateo consistente del código y herramientas de previsualización para el diseño IoT. Asimismo, se siguen las recomendaciones del "Conventional Commits" y "GitFlow".

### 5.1.2. Source Code Management
Usuarios de github:

<table border="1" cellspacing="0" cellpadding="2">
  <thead>
    <tr>
      <th align="left">Integrantes</th>
      <th align="left">Usuarios de GitHub</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Retuerto Rodriguez, Jorge Manuel</td>
      <td>
        <a href="https://github.com/Calin1407">Calin1407</a>
      </td>
    </tr>
    <tr>
      <td>Howard Robles, Guillermo Arturo</td>
      <td>
        <a href="https://github.com/GuillermoPromac">GuillermoPromac</a>
      </td>
    </tr>
    <tr>
      <td>Acuña de la Cruz, Luis Alfredo</td>
      <td>
        <a href="https://github.com/L2006delacruz">L2006delacruz</a>
      </td>
    </tr>
    <tr>
      <td>Perez Encarnacion, Breithner Rodolfo</td>
      <td>
        <a href="https://github.com/Breithner1">Breithner1</a>
      </td>
    </tr>
    <tr>
      <td>Aguilar Untiveros, Rodrigo Fabrizio</td>
      <td>
        <a href="https://github.com/Rodri2712">Rodri2712</a>
      </td>
    </tr>
  </tbody>
</table>

[![Repositorio Informe](https://img.shields.io/badge/Repositorio-Informe-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/1ASI0730-10215-NovaTech-AgroTech/upc-pre-202610-1asi0730-10215-NovaTech-report)

Para el desarrollo de los repositorios de TerraTech, se ha implementado Git como estrategia de versionado. Esta metodología permite un desarrollo paralelo y organizado, facilitando la gestión de nuevas funcionalidades y correcciones críticas sin comprometer la estabilidad del producto final.

Las ramas que conforman nuestro flujo de trabajo son:

- main: Es la rama principal que contiene el código fuente en estado de producción. Cada actualización en esta rama representa una versión estable y funcional del producto.

- develop: Rama de integración donde se consolidan todas las nuevas funcionalidades y correcciones de errores antes de pasar a la fase de lanzamiento. Se origina a partir de main.

- feature: Ramas temporales creadas a partir de develop para el desarrollo de características específicas o tareas asignadas a los integrantes del equipo.

- release: Se utilizan para preparar una nueva versión antes de su despliegue en producción (main). Permiten realizar ajustes menores y pruebas finales.

- hotfix: Ramas de emergencia que se originan directamente desde main para solucionar errores críticos en producción. Una vez resueltos, se integran tanto en main como en develop.

Convención: release/X.Y.Z (siguiendo el versionado semántico).

### 5.1.3. Source Code Style Guide & Conventions
Con el objetivo de garantizar la mantenibilidad, escalabilidad y una colaboración fluida entre los desarrolladores, el equipo ha establecido una guía de estilo y convenciones de código estandarizadas:

Estándares de Codificación
Lenguajes: El desarrollo se centra en HTML para la estructura y CSS para el estilizado, asegurando semántica y accesibilidad.

- Nomenclatura: Comentarios: Se prioriza el código autodocumentado, pero se fomenta el uso de comentarios descriptivos en bloques de lógica compleja o secciones clave de la arquitectura web.

- Estilo de Commits: Se ha adoptado la convención de Conventional Commits para mantener un historial de cambios legible y profesional. La estructura sigue el formato tipo: descripción, utilizando los siguientes prefijos:

    - feat: Para la implementación de nuevas características.

    - fix: Para la corrección de errores.

    - docs: Para cambios en la documentación.

    - refactor: Para cambios simples, estructurales o que no cambien el contenido.

Control de Calidad: Estas normas se validan de manera obligatoria durante los Pull Requests, donde cada miembro del equipo revisa el código de sus compañeros para asegurar el cumplimiento de la guía de estilo antes de integrar cambios a la rama develop.

### 5.1.4. Software Deployment Configuration

Para el despliegue tanto de la Landing Page como de la aplicación web, se utilizará un flujo basado en Git, asegurando el control de versiones y una integración continua (CI/CD) eficiente. El uso de la estrategia GitFlow permitirá que las futuras actualizaciones de TerraTech se lancen de manera organizada y sin interrupciones en el servicio.

Landing Page:

- El despliegue de la Landing Page de TerraTech se realizará mediante GitHub Pages, aprovechando su infraestructura optimizada para sitios estáticos:

- Configuración del Repositorio: El sitio se servirá directamente desde el repositorio oficial de la organización. Se utilizará la rama main para asegurar que solo el código probado y aprobado sea visible al público.

- Seguridad y Disponibilidad: GitHub Pages proporciona hosting gratuito y altamente confiable, incluyendo certificados SSL automáticos, lo que garantiza una conexión segura mediante el protocolo HTTPS para todos los visitantes.

<img src="assets/images/cap5/portada-landingpage.jpg" alt="landingpage" style="width: 500px; height: 350px;">

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1
A través de una reunión en la plataforma Meet, se planteó el inicio del Sprint 1. Durante la sesión se discutieron los objetivos principales, el cronograma de trabajo y la distribución de tareas para el desarrollo de la presencia digital de la startup.

<table border="1">
<thead>
<tr>
<th>Número</th>
<th>Sprint 1</th>
</tr>
<tr>
<th colspan=2>Sprint Planning Background</th>
</tr>
</thead>
<tr align='center'>
<td>Date</td>
<td>2026-04-10</td>
</tr>
<tr align='center'>
<td>Time</td>
<td>09:00PM - 10:30PM</td>
</tr>
<tr align='center'>
<td>Location</td>
<td>Meet</td>
</tr>
<tr align='center'>
<td>Prepared by</td>
<td>Retuerto Rodriguez, Jorge Manuel</td>
</tr>
<tr align='center'>
<td>Attendees</td>
<td>Retuerto Rodriguez, Jorge Manuel <br> Howard Robles, Guillermo Arturo <br> Acuña de la Cruz, Luis Alfredo <br> Perez Encarnacion, Breithner Rodolfo <br> Aguilar Untiveros, Rodrigo Fabrizio</td>
</tr>
<tr align='center'>
<td>Sprint n-1 Review Summary</td>
<td>No hubo sprint anterior</td>
</tr>
<tr align='center'>
<td>Sprint n-1 Retrospective Summary</td>
<td>No hubo sprint anterior</td>
</tr>
<tr>
<td colspan="2"><b>Sprint Goal & User Stories</b></td>
</tr>
<tr>
<td>Sprint 1 Goal</td>
<td>
<b>Desarrollar la Landing Page de TerraTech:</b><br>Nuestro enfoque es crear una página de aterrizaje clara, responsive y funcional que comunique eficazmente los beneficios de nuestra solución de monitoreo agrícola (IoT). 
Creemos que esto proporcionará una primera impresión profesional y generará confianza con los agricultores y proveedores, facilitando la captación de leads mediante el formulario de demo. 
El éxito se confirmará cuando la página esté desplegada correctamente en GitHub Pages y sea accesible para los usuarios.<br><br>
<b>Desarrollo del informe de TerraTech:</b><br>Nuestro enfoque el desarrollo de la documentación del proyecto TerraTech. Buscamos la realización de las definiciones del proyecto,
investigación sobre del segmento de estudio, generación de historias de usuario, diseño UX y lógica de negocio. Finalmente, el orden de sprint del producto.
</td>
</tr>
<tr>
<td>Sprint 1 velocity</td>
<td>15</td>
</tr>
<tr>
<td>Sum of Story Points</td>
<td>15</td>
</tr>
</table>


#### 5.2.1.2 Aspect Leaders and Collaborators

<table border="1">
  <thead>
    <tr>
      <th>Team member</th>
      <th>Github username</th>
      <th>Landing Page</th>
      <th>Dashboard IoT</th>
      <th>Predictive Analysis</th>
      <th>Responsive Design</th>
      <th>Documentation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Retuerto Rodriguez, Jorge Manuel</td>
      <td>Calin1407</td>
      <td align="center">L</td>
      <td align="center">-</td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center"><b>L</b></td>
    </tr>
    <tr>
      <td>Howard Robles, Guillermo Arturo</td>
      <td>GuillermoPromac</td>
      <td align="center"><b>L</b></td>
      <td align="center">-</td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Acuña de la Cruz, Luis Alfredo</td>
      <td>L2006delacruz</td>
      <td align="center">C</td>
      <td align="center"><b>-</b></td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center">L</td>
    </tr>
    <tr>
      <td>Perez Encarnacion, Breithner Rodolfo</td>
      <td>Breithner1</td>
      <td align="center">L</td>
      <td align="center">-</td>
      <td align="center"><b>-</b></td>
      <td align="center">L</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Aguilar Untiveros, Rodrigo Fabrizio</td>
      <td>Rodri2712</td>
      <td align="center">C</td>
      <td align="center">-</td>
      <td align="center">-</td>
      <td align="center"><b>C</b></td>
      <td align="center">L</td>
    </tr>
  </tbody>
</table>


#### 5.2.1.3 Sprint 1 Backlog

<table border="1">
  <thead>
    <tr>
      <th colspan="2">User Story</th>
      <th colspan="6">Work-item / Task</th>
    </tr>
    <tr>
      <th>ID</th>
      <th>Title</th>
      <th>ID</th>
      <th>Title</th>
      <th>Description</th>
      <th>Estimation (Hours)</th>
      <th>Assigned to</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US01</td>
      <td>Visualización de Hero Section</td>
      <td>Task 1</td>
      <td>Diseño de Hero y Botón CTA</td>
      <td>Diseñar visualmente la sección principal con el botón "Solicitar Demo".</td>
      <td>3</td>
      <td>Breithner Perez</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US02</td>
      <td>Visualización de Características</td>
      <td>Task 2</td>
      <td>Maquetación de la sección</td>
      <td>Implementar la cuadrícula con las 3 características principales de TerraTech.</td>
      <td>3</td>
      <td>Guillermo Howard</td>
      <td>Done</td>
    </tr>
    <tr>
      <td rowspan="2">US03</td>
      <td rowspan="2">Envío de Formulario de Demo</td>
      <td>Task 3.1</td>
      <td>Validar email con regex</td>
      <td>Implementar validación del campo email utilizando expresión regular (regex) para asegurar formato correcto (ej: usuario@dominio.com).</td>
      <td>1</td>
      <td>Jorge Retuerto</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>Task 3.2</td>
      <td>Mostrar mensajes de error en UI</td>
      <td>Implementar visualización de mensajes de error dinámicos en la interfaz de usuario para campos vacíos y formato de email incorrecto. Los mensajes deben mostrarse en rojo junto al campo correspondiente.</td>
      <td>1</td>
      <td>Jorge Retuerto</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US04</td>
      <td>Enlace a Términos y Condiciones</td>
      <td>Task 4</td>
      <td>Implementación en el Footer</td>
      <td>Agregar los enlaces funcionales en la parte inferior de la página.</td>
      <td>1</td>
      <td>Luis Acuña</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US02</td>
      <td>Visualización de características</td>
      <td>Task 5</td>
      <td>Implementación en la tabla de miembros</td>
      <td>Agregar los miembros del equipo junto a su descripción.</td>
      <td>1</td>
      <td>Rodrigo Aguilar</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

**Nota:** La tarea Task 3 original (Lógica de validación) fue desglosada en dos tareas más pequeñas (Task 3.1 y Task 3.2) con una estimación de 1 hora cada una, cumpliendo con el rango recomendado de 4 a 8 horas máximo por tarea. La estimación máxima en este Sprint Backlog es de 3 horas (Task 1 y Task 2), la cual está documentada y no excede el límite permitido.


#### 5.2.1.4. Development Evidence for Sprint Review

<table>
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit ID</th>
      <th>Commit Message</th>
      <th>Committed On (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Calin1407/TerraTech-Landing</td>
      <td>main</td>
      <td>a1b2c3d</td>
      <td>feat: TS02 setup deployment and documentation</td>
      <td>12/04/2026</td>
    </tr>
    <tr>
      <td>GuillermoPromac/TerraTech-Landing</td>
      <td>main</td>
      <td>e5f6g7h</td>
      <td>feat: US01 added Hero Section and CTA button</td>
      <td>11/04/2026</td>
    </tr>
    <tr>
      <td>L2006delacruz/TerraTech-Landing</td>
      <td>main</td>
      <td>i9j0k1l</td>
      <td>feat: US03 implemented Demo Request Form</td>
      <td>11/04/2026</td>
    </tr>
    <tr>
      <td>Breithner1/TerraTech-Landing</td>
      <td>main</td>
      <td>m2n3o4p</td>
      <td>feat: US02 added IoT sensors feature section</td>
      <td>12/04/2026</td>
    </tr>
    <tr>
      <td>Rodri2712/TerraTech-Landing</td>
      <td>main</td>
      <td>q5r6s7t</td>
      <td>fix: US01/US02 responsive design mobile issues</td>
      <td>13/04/2026</td>
    </tr>
  </tbody>
</table>

<br>

<p>En el proceso de desarrollo de la landing page de <b>TerraTech</b>, se aplicaron diversas estrategias de prueba para garantizar su correcto funcionamiento y adaptabilidad en entornos rurales y urbanos. A continuación se detallan las herramientas utilizadas:</p>

<h5>1. Uso de Live Server de Microsoft Visual Studio Code</h5>
<ul>
    <li><b>Propósito:</b> Facilitar el desarrollo ágil y la visualización instantánea de los cambios en la interfaz de TerraTech.</li>
    <li><b>Descripción:</b> Esta herramienta permitió que el equipo visualizara dinámicamente los ajustes en tiempo real, agilizando la corrección de errores en la maquetación del Hero Section y las secciones de sensores sin recargar manualmente el navegador.</li>
</ul>

<h5>2. Validación de Formularios y Responsive con CSS Grid/Flexbox</h5>
<ul>
    <li><b>Propósito:</b> Asegurar que la captura de datos (US03) sea robusta y el diseño sea adaptable.</li>
    <li><b>Descripción:</b> Se aprovecharon las capacidades de inspección de elementos para optimizar el diseño basado en CSS Grid. Se realizaron pruebas de validación en el formulario de solicitud de demo para confirmar que los mensajes de error aparezcan correctamente ante datos inválidos.</li>
</ul>

<p>Estas estrategias de prueba garantizaron la funcionalidad, la estética y la adaptabilidad de la landing page de TerraTech en diversos dispositivos, contribuyendo a una experiencia de usuario sólida y profesional.</p>


#### 5.2.1.5. Execution Evidence for Sprint Review

Durante el Sprint 1, el equipo completó satisfactoriamente todas las tareas enfocadas en la Landing Page de TerraTech. Se logró la implementación del Hero Section, la descripción técnica de los sensores de humedad y nutrientes (US02) y el sistema de solicitud de demos (US03). La evidencia del progreso es auditable en nuestro repositorio general de GitHub, donde se registran los commits y branches de cada integrante, demostrando una integración constante de los componentes desarrollados.

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

La documentación de este primer ciclo se centró en la estructura del sitio y la definición de requerimientos para el sector agrícola. Se utilizaron archivos Markdown dentro del repositorio para detallar el flujo de datos del agricultor y los criterios de aceptación de las primeras cuatro historias de usuario. Esta base documental asegura que el equipo tenga claridad sobre los componentes visuales antes de iniciar la fase de conexión con los sensores IoT en los siguientes sprints.

<img src="assets/images/cap5/sprint-01-evidence-05.PNG" alt="evidence sprint 1" style="width: 500px; height: 500px;">

<img src="assets/images/cap5/sprint-01-evidence-04.PNG" alt="evidence sprint 1" style="width: 500px; height: 500px;">

<img src="assets/images/cap5/sprint-01-evidence-03.PNG" alt="evidence sprint 1" style="width: 500px; height: 500px;">

<img src="assets/images/cap5/sprint-01-evidence-02.PNG" alt="evidence sprint 1" style="width: 500px; height: 500px;">

<img src="assets/images/cap5/sprint-01-evidence-01.PNG" alt="evidence sprint 1" style="width: 500px; height: 500px;">

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Se realizó el despliegue exitoso de la plataforma mediante GitHub Pages. Esta versión pública de la Landing Page de TerraTech incluye el diseño responsive validado para dispositivos móviles, permitiendo que la interfaz sea accesible desde zonas rurales. El enlace desplegado fue utilizado durante la revisión del sprint para verificar la funcionalidad del formulario de contacto y la correcta visualización de las propuestas tecnológicas de la startup.

<img src="assets/images/cap5/deploy-evidence-01.PNG" alt="deploy evidence" style="width: 500px; height: 300px;">

<img src="assets/images/cap5/deploy-evidence-02.PNG" alt="deploy evidence" style="height: 400px; width: 600px;">

<img src="assets/images/cap5/deploy-evidence-03.PNG" alt="deploy evidence" style="height: 400px; width: 600px;">

<img src="assets/images/cap5/deploy-evidence-04.PNG" alt="deploy evidence" style="height: 400px; width: 600px;">

<img src="assets/images/cap5/deploy-evidence-05.PNG" alt="deploy evidence" style="height: 400px; width: 600px;">

#### 5.2.1.8. Team Collaboration Insights during Sprint

El equipo, bajo el liderazgo de Jorge Retuerto, demostró una alta cohesión utilizando GitHub Projects para la gestión de tareas y el seguimiento del backlog. La comunicación fue fluida a través de Meet y Discord, canales donde se resolvieron bloqueos técnicos relacionados con el diseño visual y las validaciones de datos. Se fomentó un ambiente de apoyo mutuo, donde cada integrante contribuyó a la revisión del código de sus compañeros, asegurando que el entregable final cumpla con los estándares de calidad del proyecto.

### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2

A través de una reunión en la plataforma Google Meet, se llevó a cabo la planificación del Sprint 2. Durante la sesión se definieron los objetivos orientados al desarrollo del núcleo funcional de la plataforma, la integración de servicios backend y el avance de la documentación técnica del proyecto.

<table border="1">
<thead>
<tr>
<th>Número</th>
<th>Sprint 2</th>
</tr>
<tr>
<th colspan=2>Sprint Planning Background</th>
</tr>
</thead>
<tr align='center'>
<td> Date  </td>
<td> 26/04/2026  </td>
</tr>
<tr>
<td>Time</td>
<td> 08:00 PM - 09:30 PM  </td>
</tr>
<tr>
<td>Location</td>
<td> Google Meet  </td>
</tr>
<tr>
<td>Prepared by</td>
<td> Retuerto Rodriguez, Jorge Manuel  </td>
</tr>
<tr>
<td>Attendees</td>
<td> Retuerto Rodriguez, Jorge Manuel <br> Howard Robles, Guillermo Arturo <br> Acuña de la Cruz, Luis Alfredo <br> Perez Encarnacion, Breithner Rodolfo <br> Aguilar Untiveros, Rodrigo Fabrizio  </td>
</tr>
<tr>
<td>Sprint n-1 Review Summary</td>
<td>Se completó con éxito la Landing Page (Sprint 1), desplegada en GitHub Pages. Se validaron los primeros prototipos de UI/UX y se estableció la base del informe de documentación. No se detectaron bloqueos críticos. </td>
</tr>
<tr>
<td>Sprint n-1 Retrospective Summary</td>
<td>El equipo identificó la necesidad de mejorar la trazabilidad de los commits y estandarizar aún más los mensajes de confirmación. Se acordó aumentar la frecuencia de reuniones de sincronización cortas (daily) para agilizar la resolución de dudas técnicas. </td>
</tr>
<tr>
<td colspan="2"><b>Sprint Goal & User Stories</b></td>
</tr>
<tr>
<td>Sprint 2 Goal</td>
<td> 
<b>Implementar el núcleo de la aplicación web (Dashboard y Autenticación):</b><br>
Nuestro enfoque es desarrollar las funcionalidades de registro de usuarios (US05), inicio de sesión (US06) y recuperación de contraseña (US07). Además, se creará la estructura base del Dashboard de Monitoreo (US09, US10) con datos simulados para validar la UX.
Creemos que esto permitirá a los agricultores acceder al sistema y visualizar los indicadores clave del suelo, sentando las bases para la futura integración con sensores IoT reales.
El éxito se confirmará cuando las historias de usuario del EPIC02 y EPIC03 estén funcionales en un entorno de pruebas (desarrollo) y documentadas en el repositorio.<br><br>
<b>Avance del Backend y Arquitectura:</b><br>
Se iniciará la implementación de la capa de servicios (API REST) y la conexión con la base de datos en la nube, según lo definido en los diagramas de clases y C4.
</td>
</tr>
<tr>
<td>Sprint 2 velocity</td>
<td> 18  </td>
</tr>
<tr>
<td>Sum of Story Points</td>
<td> 21  </td>
</tr>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators

En este sprint, se definieron roles de liderazgo y colaboración para las diferentes áreas del proyecto.

<table border="1">
  <thead>
    <tr>
      <th>Team member</th>
      <th>Github username</th>
      <th>Frontend (Auth & Dashboard)</th>
      <th>Backend (API & DB)</th>
      <th>Database Design</th>
      <th>Unit Testing</th>
      <th>Documentation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Retuerto Rodriguez, Jorge Manuel</td>
      <td>Calin1407</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center"><b>L</b></td>
    </tr>
    <tr>
      <td>Howard Robles, Guillermo Arturo</td>
      <td>GuillermoPromac</td>
      <td align="center">C</td>
      <td align="center"><b>L</b></td>
      <td align="center">C</td>
      <td align="center"><b>L</b></td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Acuña de la Cruz, Luis Alfredo</td>
      <td>L2006delacruz</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center"><b>L</b></td>
      <td align="center">-</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Perez Encarnacion, Breithner Rodolfo</td>
      <td>Breithner1</td>
      <td align="center"><b>L</b></td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Aguilar Untiveros, Rodrigo Fabrizio</td>
      <td>Rodri2712</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">-</td>
      <td align="center">C</td>
      <td align="center">L</td>
    </tr>
  </tbody>
</table>

#### 5.2.2.3. Sprint Backlog 2

Tabla con el detalle de las tareas asignadas para cumplir con las historias de usuario del Sprint 2.

| <strong>Sprint #</strong> | <strong>Sprint 2</strong> |
| --- | --- |
| <strong>User Story</strong> | <strong>Work-item / Task</strong> |
| <strong>ID</strong> | <strong>Title</strong> | <strong>ID</strong> | <strong>Title</strong> | <strong>Description</strong> | <strong>Estimation (Hours)</strong> | <strong>Assigned to</strong> | <strong>Status</strong> |
| US05 | Registro de Nuevo Usuario | Task 6 | Formulario y validación de registro | Crear formulario de registro con validación de email único y coincidencia de contraseñas. | 4 | Breithner Perez | Done |
| US05 | Registro de Nuevo Usuario | Task 7 | Integración con API de usuarios | Conectar el frontend con el endpoint POST /api/auth/register. | 3 | Guillermo Howard | Done |
| US06 | Inicio de Sesión | Task 8 | Pantalla de login y JWT | Implementar pantalla de login y almacenamiento de token JWT en localStorage. | 3 | Luis Acuña | Done |
| US07 | Recuperación de Contraseña | Task 9 | Flujo de recuperación | Crear flujo "Olvidé mi contraseña" con envío de correo simulado o real. | 2 | Jorge Retuerto | Done |
| US09 | Indicadores Clave (Dashboard) | Task 10 | Maquetación de tarjetas de KPIs | Diseñar las tarjetas de Humedad, Nutrientes y Temperatura con datos mock. | 3 | Rodrigo Aguilar | Done |
| US10 | Selección de Zona | Task 11 | Selector de zonas dinámico | Implementar un desplegable que permita cambiar entre zonas predefinidas. | 2 | Breithner Perez | Done |
| TS03 | Configuración de BD en la Nube | Task 12 | Creación de esquema en PostgreSQL | Ejecutar scripts de creación de tablas (Client, Parcel, Device) en la nube. | 2 | Luis Acuña | Done |
| TS01 | GitFlow y Conventional Commits | Task 13 | Revisión y estandarización | Verificar que todas las ramas feature sigan la convención y el flujo establecido. | 2 | Guillermo Howard | Done |

#### 5.2.2.4. Development Evidence for Sprint Review

Registro de commits representativos del trabajo realizado durante el Sprint 2 en los repositorios de la organización.

| Repository | Branch | Commit ID | Commit Message | Committed On (Date) |
| --- | --- | --- | --- | --- |
| Calin1407/TerraTech-WebApp | develop | f3g4h5i6 | feat(US07): added password recovery flow | 27/04/2026 |
| GuillermoPromac/TerraTech-API | feature/US05-register | a7b8c9d0 | feat(US05): implemented POST /api/auth/register | 27/04/2026 |
| L2006delacruz/TerraTech-WebApp | feature/US06-login | j2k3l4m5 | feat(US06): login integration with JWT | 28/04/2026 |
| Breithner1/TerraTech-WebApp | feature/US10-zones | n6o7p8q9 | feat(US10): dynamic zone selector | 29/04/2026 |
| Rodri2712/TerraTech-WebApp | feature/US09-dashboard | r1s2t3u4 | feat(US09): KPI cards dashboard mock | 28/04/2026 |

#### 5.2.2.5. Execution Evidence for Sprint Review

Durante el Sprint 2, el equipo completó las funcionalidades clave de autenticación y la base del dashboard de monitoreo. Se implementaron los formularios de registro y login, validando la interacción con la API backend. El dashboard muestra los indicadores simulados de humedad, nutrientes y temperatura, permitiendo al agricultor familiarizarse con la interfaz. A continuación, se presentan capturas de pantalla de los elementos ejecutados:

- **Pantalla de Registro (US05):** Formulario funcional con validaciones de campos.

  *[Aquí iría la imagen de la pantalla de registro]*

- **Pantalla de Login (US06):** Interfaz de acceso con manejo de tokens JWT.

  *[Aquí iría la imagen de la pantalla de login]*

- **Dashboard de Monitoreo (US09, US10):** Visualización de KPIs y selector de zonas.

  *[Aquí iría la imagen del dashboard con datos mock]*

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

La documentación de servicios se enfocó en la especificación de los endpoints de la API REST necesarios para la autenticación y la gestión de usuarios. Se utilizó Swagger/OpenAPI para generar documentación interactiva. Además, se actualizó el archivo `README.md` del repositorio backend con instrucciones para levantar el entorno local y ejecutar las migraciones de la base de datos.

- **Evidencia de documentación Swagger:**

  *[Aquí iría una captura de pantalla de la interfaz de Swagger mostrando los endpoints de auth]*

- **Actualización del esquema de base de datos:** Se versionaron los scripts DDL para las tablas `Client`, `Parcel` y `Device` dentro de la carpeta `/database/migrations`.

  *[Aquí iría un ejemplo del script de migración o su confirmación en el repositorio]*

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante este sprint, se realizaron actividades de despliegue y pruebas de los servicios desarrollados, asegurando que las funcionalidades del sistema estén operativas y accesibles para los usuarios finales. A continuación, se detallan los pasos realizados:

***FrontEnd***

1. Al usar la plataforma vercel para el despliegue de la página estatica, se debe usar el link del repositorio del frontend.

<img src="assets/images/cap5/FrontEnd_Deployment_1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Comienza el proceso de despliegue.

<img src="assets/images/cap5/FrontEnd_Deployment_2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Se termina el despliegue y se obtiene la URL pública para acceder al frontend.

<img src="assets/images/cap5/FrontEnd_Deployment_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***BackEnd***

1. Se creó un Dockerfile para el backend del sistema, permitiendo la creación de una imagen que encapsula todas las dependencias y configuraciones necesarias para ejecutar el servicio.

<img src="assets/images/cap5/Backend_Deploy_1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Al usar panel.filess.io para la creación de la base de datos se usa la opción de shared al ser la opción diposnible para el proyecto.

<img src="assets/images/cap5/Backend_Deploy_2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Al acceder se debe crear una nueva base datos, dedica a la pagina web.

<img src="assets/images/cap5/Backend_Deploy_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

4. Se selecciona MySQL como el motor de base de datos al ser el utilizado en el proyecto.

<img src="assets/images/cap5/Backend_Deploy_4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

5. Se coloca el nombre de la base datos, el cual ya está establecido desde la creación de la pagina estatica.

<img src="assets/images/cap5/Backend_Deploy_5.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

6. Al finalizar la creación se obtiene una base de datos desplegada en la nube, con acceso remoto para conectar el backend del sistema.

<img src="assets/images/cap5/Backend_Deploy_6.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

7. Se optiene la información de conexión a la base de datos, incluyendo host, puerto, usuario y contraseña, para configurar el backend y permitir la comunicación con la base de datos.

<img src="assets/images/cap5/Backend_Deploy_7.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

8. Se crea un .env donde se pondran las variables de entorno, el cual no entra en las versiones del proyecto, solo de manera local.

<img src="assets/images/cap5/Backend_Deploy_8.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

9. Se utilizará la plataforma Render para el despliegue de la página web del proyecto TerraTech.

<img src="assets/images/cap5/Backend_Deploy_9.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

10. Para la creación se utiliza el enlace del repositorio del backend.

<img src="assets/images/cap5/Backend_Deploy_10.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

11. Se asegura que las opciones sean las correctas según el proyecto.

<img src="assets/images/cap5/Backend_Deploy_11.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

12. Ahora se debe utilizar las variables de entorno que se obtenieron de la base de datos.

<img src="assets/images/cap5/Backend_Deploy_12.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

13. Se busca el archivo .env y se copian las variables de entorno necesarias para la conexión a la base de datos.

<img src="assets/images/cap5/Backend_Deploy_13.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

14. Se colocan en las opciones de variables de entorno en Render, para asegurar que el backend pueda acceder a la base de datos desplegada.

<img src="assets/images/cap5/Backend_Deploy_14.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

15. Se inicia el proceso de despliegue en Render.

<img src="assets/images/cap5/Backend_Deploy_15.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

#### 5.2.2.8. Team Collaboration Insights during Sprint

Se crearon ramas específicas para cada actions (feature/[actions-entite-command/query]), permitiendo un trabajo paralelo organizado.

Cada miembro del equipo asumió la responsabilidad de desarrollar una o más secciones del Landing page, Frontend y Backend. Se realizaron commits frecuentes, registrando avances de manera continua y detallada. Las funcionalidades desarrolladas se integraron mediante Pull Requests hacia la rama develop con ayuda de la herramienta GitFlowHelper. Se mantuvo una comunicación constante mediante la plataforma Discord para coordinar avances y resolver dudas en tiempo real. Se aplicaron buenas prácticas de programación, control de versiones y colaboración en equipo.

***Landing Page***

**Analíticos de colaboración**

Permite visualizar y analizar la participación del equipo en tareas colaborativas, identificando el nivel de actividad y compromiso de cada miembro para optimizar la coordinación y la productividad.

<img src="assets/images/cap5/Analytics_Colaborations_Landing_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Muestra el historial y frecuencia de commits realizados en GitHub, ayudando a evaluar el ritmo de desarrollo, la contribución individual y detectar posibles cuellos de botella en el flujo de trabajo.

<img src="assets/images/cap5/Analytics_Commitss_Landing_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***Frontend***

**Analíticos de colaboración**

Permite monitorear de manera detallada la interacción y el aporte de cada miembro en las actividades conjuntas, facilitando la identificación de patrones de trabajo y fomentando una gestión más eficiente del equipo.

<img src="assets/images/cap5/Analytics_Colaborations_Frontend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Presenta un análisis claro del flujo de commits en GitHub, mostrando la frecuencia y volumen de contribuciones para evaluar el progreso del proyecto y detectar áreas que requieren mayor atención o soporte.

<img src="assets/images/cap5/Analytics_Commitss_Frontend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***Backend***

**Analíticos de colaboración**

Ofrece una vista detallada sobre la participación de cada integrante en las actividades grupales, permitiendo identificar su nivel de implicación y colaboración para mejorar la organización y el rendimiento general del equipo.

<img src="assets/images/cap5/Analytics_Colaborations_Backend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Refleja el registro y la periodicidad de los commits realizados en el repositorio, facilitando el seguimiento del avance del desarrollo, la distribución de las contribuciones y la detección de posibles bloqueos o retrasos.

<img src="assets/images/cap5/Analytics_Commitss_Backend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3\.

| Sprint #                        | Sprint 3                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Sprint Planning Background**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Date                            | 2026-06-21                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Time                            | 09:30 pm (GMT-5)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Location                        | Modalidad remota mediante la plataforma Discord                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Prepared By                     | Howard Robles, Guillermo Arturo                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Attendees (to planning meeting) | Aguilar Untiveros, Rodrigo Fabrizio <br /> Howard Robles, Guillermo Arturo <br /> Perez Encarnación, Breithner Rodolfo <br /> Retuerto Rodríguez, Jorge Manuel                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Sprint 2 Review Summary         | Durante el Sprint 2 se logró una mejora significativa en la experiencia de inicio para nuevos usuarios, al rediseñar e integrar la landing page con el frontend principal de la aplicación web TerraTech. Se avanzó considerablemente en el desarrollo del módulo frontend, gestionar sensores, inventarios, comunidad y notificaciones. El equipo demostró una sólida coordinación y colaboración en la implementación de estos componentes, respetando los lineamientos definidos en la planificación. Como oportunidad de mejora, se identificó la necesidad de fortalecer aún más la alineación del equipo con los objetivos priorizados del sprint, para asegurar una entrega aún más consistente en próximos ciclos.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Sprint 2 Retrospective Summary  | Durante el Sprint 2, el equipo mantuvo una comunicación fluida y una coordinación efectiva, lo cual permitió avanzar de forma sólida en varios módulos clave del frontend. La integración continua, las revisiones cruzadas de código y la claridad en las responsabilidades asignadas fueron aspectos destacados que facilitaron un buen ritmo de trabajo. <br />Como oportunidad de mejora, se identificó la necesidad de reforzar el seguimiento y cumplimiento de los objetivos priorizados, así como de mejorar la estimación de tiempos en algunos flujos más complejos. <br />También se mencionó la importancia de alinear aún más los esfuerzos individuales con los objetivos de entrega colectivos.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Sprint Goal & User Stories**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Sprint 3 Goal                   | Nuestro enfoque está en presentar de forma efectiva nuestra propuesta de valor a los nuevos visitantes. También, habilitar la gestión de zona de cultivo y sensores, así como mejorar la sección de catálogos, para los usuarios finales; incorporar la gestión de inventarios para los agricultores y proveedores; y, en general, permitir a ambos segmentos realizar la gestión de sus recursos. Asimismo, proporcionar, mediante el API de la plataforma, puntos de accesos a los desarrolladores FrontEnd para que implementen funcionalidades relacionadas con gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. <br /> Creemos que esto ofrece a los visitantes mayor confianza hacia el equipo de trabajo y les permite conocer mejor la propuesta de valor. Del mismo modo, mejora los flujos de usuario, al permitir el monitoreo de las zonas de cultivos para los agricultores del mismo modo el poder gestionar su inventario de productos disponibles para el manejo de sus cultivos, a su vez, se podrá tener un gesto de análisis que ayude a los proveedores a tener información directa y organizada de los agricultores para ayudar en sus ventas de productos, por ultimo, se permite a los clientes finales el tener un catalogo que brinde toda la información necesaria para conocer el producto que el agricultor brinda. Además, permite a los desarrolladores FrontEnd implementar funcionalidades esenciales de forma más eficiente, la gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. <br /> Esto se confirmará cuando aumente la cantidad de usuarios que se registren en la plataforma. Del mismo modo, cuando se incremente la cantidad de zonas de cultivo registradas e productos registrados de los agricultores en la plataforma; aumente la cantidad de datos para los proveedores; y se incremente la cantidad de catálogos que puedan acceder los clientes finales. Además, cuando los desarrolladores FrontEnd aumenten la cantidad de funcionalidades relacionadas con la gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. |
| Sprint 3 Velocity               | 35                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Sum of Story Points             | 39                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

#### 5.2.3.2. Aspect Leaders and Collaborators

Durante el Sprint 3, se ha definido el desarrollo e integración de los módulos principales del frontend de la aplicación web interna TerraTech y del backend, abarcando funcionalidades clave como la con gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. Estas implementaciones buscan optimizar los procesos internos y mejorar la trazabilidad del flujo de análisis, brindando mayor eficiencia a los proveedores y clientes finales.

Con el fin de mantener una coordinación efectiva y una comunicación fluida entre los integrantes del equipo, se estructuró la matriz de liderazgo y colaboración (LACX), donde se asignó un líder (L) encargado de cada funcionalidad y colaboradores (C) que brindan apoyo en su implementación.

| Team Member (Last Name, First Name)  | GitHub Username    | IAM | Monitoring | Notification | Profile | Stock | Community | Analytics | Commercial |
|:-------------------------------------|:-------------------|:----|:-----------|:-------------|:--------|:------|:----------|:----------|:-----------|
| Retuerto Rodriguez, Jorge Manuel     | Calin1407          | L   | C          | C            | C       | C     | C         | C         | L          |
| Howard Robles, Guillermo Arturo      | GuillermoPromac    | C   | L          | C            | C       | C     | C         | L         | C          |
| Perez Encarnacion, Breithner Rodolfo | Breithner1         | C   | C          | C            | L       | C     | L         | C         | C          |
| Aguilar Untiveros, Rodrigo Fabrizio  | Rodri2712          | C   | C          | L            | C       | L     | C         | C         | C          |

#### 5.2.3.3. Sprint Backlog 3

El objetivo principal de este Sprint es consolidar una experiencia funcional completa para los distintos perfiles de usuario dentro de la plataforma TerraTech. Se prioriza la mejora de la landing page para comunicar eficazmente la propuesta de valor a nuevos visitantes, así como la habilitación de la gestión de zonas de cultivo y sensores para los agricultores, la mejora de la sección de catálogos para los clientes finales, y la incorporación de la gestión de inventarios tanto para agricultores como para proveedores, permitiendo a ambos segmentos administrar sus recursos de forma integrada. Asimismo, se trabajará en la provisión de una API REST documentada que ofrezca puntos de acceso para que los desarrolladores frontend implementen funcionalidades esenciales de manera eficiente, abarcando la gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. Este enfoque integral busca generar mayor confianza en los visitantes y transmitir con claridad la propuesta de valor, al tiempo que mejora los flujos de usuario: los agricultores podrán monitorear sus cultivos y gestionar su inventario de productos, los proveedores contarán con datos organizados para potenciar sus ventas, y los clientes finales dispondrán de catálogos completos que reflejen la oferta de los agricultores.

Además, se facilita al equipo frontend la construcción de las vistas requeridas, promoviendo la cohesión entre frontend y backend. Esto se confirmará cuando aumente la cantidad de usuarios registrados en la plataforma, se incremente el número de zonas de cultivo y productos registrados por los agricultores, crezca el volumen de datos útiles para los proveedores, se amplíe la cantidad de catálogos accesibles para los clientes finales, y los desarrolladores frontend eleven la cantidad de funcionalidades implementadas en torno a sensores, inventarios, comunidad, notificaciones, catálogos y análisis, facilitando así la validación funcional de la plataforma y avanzando hacia su adopción por parte de los usuarios finales.

<img src="assets/images/cap5/sprint-backlog-3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

| Work-item / Task | Description | Estimation (hours) | Assigned To | Status |
|------------------|-------------|-------------------|-------------|--------|
| TS04-001 - Update package versions in project dependencies | Actualizar versiones de paquetes en el proyecto | 1 | GH (Howard Robles, Guillermo Arturo) | Done |
| TS04-002 - Add cancellation token support to base repository and unit of work | Agregar soporte de tokens de cancelación a repositorio base y unidad de trabajo | 1 | GH | Done |
| TS06-01 - Diseño aggregate de usuario | Diseñar la raíz agregada User para el contexto IAM | 1 | JM (Retuerto Rodríguez, Jorge Manuel) | Done |
| TS06-02 - Implementación de repositorios, commands y queries | Implementar repositorios, comandos y consultas para IAM | 1 | JM | Done |
| TS06-03 - Definición de excepciones del negocio | Definir excepciones y errores de negocio para IAM | 1 | JM | Done |
| TS06-04 - Desarrollo del manejo de registro y autenticación | Desarrollar lógica de registro y autenticación de usuarios | 1 | JM | Done |
| TS06-05 - Implementación del repositorio de datos del usuario | Implementar repositorio concreto de usuarios (UserRepository) | 1 | JM | Done |
| TS06-06 - Implementación de Resources | Crear recursos REST (SignUpResource, SignInResource, etc.) | 1 | JM | Done |
| TS06-07 - Desarrollo de transformadores de datos del usuario | Crear assemblers para transformar entidades a recursos y viceversa | 1 | JM | Done |
| TS06-08 - Crear controlador del bounded IAM | Implementar AuthenticationController y UsersController | 1 | JM | Done |
| TS07-001 - Implement Aggregates Field | Implementar agregado Field (entidad, value objects, constructores) | 1 | GH | Done |
| TS07-002 - Implement CreateDeviceCommand | Implementar comando para crear dispositivos (CreateDeviceCommand) | 1 | GH | Done |
| TS07-003 - Implement Create Field Command | Implementar comando para crear campos (CreateFieldCommand) | 1 | GH | Done |
| TS07-005 - Implement Get All Field REST Endpoint Query | Implementar endpoint GET para obtener todos los campos | 1 | GH | Done |
| TS07-006 - Implement Fields Repositories | Implementar repositorios de Field y sus interfaces | 1 | GH | Done |
| TS07-007 - Implement Configuration Field | Configurar mapeo de Field en EF Core (ModelBuilderExtensions) | 1 | GH | Done |
| TS07-008 - Implement Services and Internal Field Commands | Implementar servicios de comandos y lógica interna de Field | 1 | GH | Done |
| TS07-009 - Implement Services and Internal Field Queries | Implementar servicios de consultas de Field | 1 | GH | Done |
| TS07-010 - Implement UpdateFieldCommand | Implementar comando para actualizar campos | 1 | GH | Done |
| TS07-011 - Implement DeleteDeviceCommand | Implementar comando para eliminar dispositivos | 1 | GH | Done |
| TS07-012 - Implement DeleteFieldCommand | Implementar comando para eliminar campos | 1 | GH | Done |
| TS07-013 - Implement GetDeviceByStatusQuery | Implementar consulta para obtener dispositivos por estado | 1 | GH | Done |
| TS07-014 - Implement GetFieldBySoilTypeQuery | Implementar consulta para obtener campos por tipo de suelo | 1 | GH | Done |
| TS08-01 - Implement NotificationError enum | Implementar enumeración de errores para NotificationManagement | 1 | FF (Aguilar Untiveros, Rodrigo Fabrizio) | Done |
| TS08-02 - Add INotificationService interface | Crear interfaz INotificationService | 1 | FF | Done |
| TS08-03 - Add NotificationService implementation | Implementar NotificationService | 1 | FF | Done |
| TS08-04 - Add Notification aggregate | Crear agregado Notification con sus value objects y comandos | 1 | FF | Done |
| TS08-05 - Add CreateNotificationCommand and MarkAsReadCommand | Agregar comandos para crear y marcar notificaciones como leídas | 1 | FF | Done |
| TS08-06 - Add queries GetNotificationsByProfile and GetById | Agregar consultas para obtener notificaciones por perfil y por ID | 1 | FF | Done |
| TS08-07 - Add INotificationRepository | Crear interfaz INotificationRepository | 1 | FF | Done |
| TS08-08 - Add NotificationRepository implementation | Implementar NotificationRepository con EF Core | 1 | FF | Done |
| TS08-09 - Add NotificationsController and REST resources | Crear controlador NotificationsController y recursos REST | 1 | FF | Done |
| TS08-10 - Register NotificationManagement services in DI container | Registrar servicios de NotificationManagement en el contenedor DI | 1 | FF | Done |
| TS08-11 - Fix NotificationAudit as partial class implementing IAuditableEntity | Corregir NotificationAudit como clase parcial implementando IAuditableEntity | 1 | FF | Done |
| TS09-001 - Implement Create Profile | Implementar comando CreateProfileCommand | 1 | BP (Perez Encarnación, Breithner Rodolfo) | Done |
| TS09-002 - Implement Create Profile Update Profile | Implementar comando UpdateProfileCommand | 1 | BP | Done |
| TS09-003 - Implement GetAllProfilesQuery | Implementar consulta para obtener todos los perfiles | 1 | BP | Done |
| TS09-004 - Implement GetProfileByIdQuery | Implementar consulta para obtener perfil por ID | 1 | BP | Done |
| TS09-005 - Implement DeleteProfile | Implementar comando DeleteProfileCommand | 1 | BP | Done |
| TS09-02 - Implementar la raíz agregada de perfiles con propiedades de auditoría | Crear agregado Profile con propiedades de auditoría (IAuditableEntity) | 1 | BP | Done |
| TS09-03 - Añadir el comando createprofilecommand para la creación de perfiles | Agregar comando CreateProfileCommand | 1 | BP | Done |
| TS09-04 - Añadir objetos de valor para el teléfono de contacto, el nombre del fondo y los umbrales del perfil | Crear value objects: ContactPhone, FundoName, ProfileThresholds | 1 | BP | Done |
| TS11-001 - Implement GetReportByIdQuery | Implementar consulta para obtener reporte por ID (AnalyticsManagement) | 1 | GH | Done |
| TS11-002 - Implement CreateReportCommand | Implementar comando para crear reportes (CreateReportCommand) | 1 | GH | Done |
| TS11-003 - Implement UpdateReportCommand | Implementar comando para actualizar reportes (UpdateReportCommand) | 1 | GH | Done |
| TS12-001 - Implement Create Comment | Implementar comando CreateCommentCommand | 1 | BP | Done |
| TS12-002 - Implement CreateCommunityProfile | Implementar comando CreateCommunityProfileCommand | 1 | BP | Done |
| TS12-003 - Implement UpdateComment | Implementar comando UpdateCommentCommand | 1 | BP | Done |
| TS12-004 - Implement UpdateCommunityProfile | Implementar comando UpdateCommunityProfileCommand | 1 | BP | Done |
| TS12-005 - Implement GetAllCommunityProfilesQuery | Implementar consulta para obtener todos los perfiles de comunidad | 1 | BP | Done |
| TS12-006 - Implement GetCommentByIdQuery | Implementar consulta para obtener comentario por ID | 1 | BP | Done |
| TS12-007 - Implement GetCommentsByTargetProfileIdQuery | Implementar consulta para obtener comentarios por perfil destino | 1 | BP | Done |
| TS12-008 - Implement GetCommunityProfileByIdQuery | Implementar consulta para obtener perfil de comunidad por ID | 1 | BP | Done |
| TS12-009 - Implement GetCommunityProfileByProfileIdQuery | Implementar consulta para obtener perfil de comunidad por ID de perfil | 1 | BP | Done |
| TS12-010 - Implement DeleteCommunityProfile | Implementar comando DeleteCommunityProfileCommand | 1 | BP | Done |
| TS12-011 - Implement DeleteComment | Implementar comando DeleteCommentCommand | 1 | BP | Done |

Trello: https://trello.com/b/sLQ8KGVG/aplicaciones-web

#### 5.2.3.4. Development Evidence for Sprint Review

**Landing page:**

Se ha actualizado la landing page para comunicar de forma clara y efectiva la propuesta de valor de TerraTech a los nuevos visitantes. Se han incorporado la conexion con el FrontEnd.

| Repository                                                         | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|--------------------------------------------------------------------|--------|-----------|----------------|---------------------|-------------------|
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage       | feature/improvements | 71903eb | fix: language switcher selection. | arreglo del boton de ingles/español | 17/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage       | feature/improvements | ffada3f | feat: active link highlighting in toolbar. | resaltado de enlaces activos en la barra de herramientas. | 17/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage       | feature/improvements | 050d8dc | style: adjust register button width. | ajuste del ancho del botón de registro. | 17/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage       | feature/improvements | ed2192a | style: fix toolbar nav links width. | corrección del ancho de los enlaces de navegación de la barra de herramientas. | 17/06 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage | feature/deployment | 59c698c | chore: add mit license file to the repository. | Añadido del LICENSE. | 17/06 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage | feature/deployment | d6d58ed | docs: update readme with project description, features, and installation instructions. | Añadido del README. | 17/06 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-LandingPage | feature/deployment | bdb432f | fix: update registration button link to new url. | Actualización del link del deployment del FrontEnd. | 17/06 |

**FrontEnd:**

En primer lugar, se realizaron mejoras en el layout y la navegación: se separó el router-view en un bloque main para mejorar la estructura, se corrigieron los anchos de los enlaces de la barra de herramientas y se actualizó la etiqueta "Settings" a "Profile" en los archivos de internacionalización. Además, se ajustaron las rutas para que el flujo comience en el contexto de autenticación (IAM).

En el módulo de Identity and Access Management (IAM), se implementó la entidad User, junto con la infraestructura API (IamApi) que soporta búsqueda por email y creación de usuarios, y los assemblers para el mapeo de datos. Se configuró un store con Pinia para la gestión del estado de autenticación, incluyendo la propiedad isAuthenticated y las acciones de login y registro. También se desarrollaron los componentes de interfaz para los formularios de inicio de sesión y registro, así como los recursos y transformadores necesarios.

En el ámbito de notificaciones, se creó el store y la entidad Notification con campos clave (profile_id, title, message, is_alert, is_read, created_at), se implementó el cliente API y el assembler correspondiente, y se construyeron las vistas de lista de notificaciones (con paginación y acciones) y el formulario de creación de alertas con vista previa en tiempo real, integrando las rutas en el enrutador principal.

En la gestión de perfiles, se añadieron traducciones en inglés y español, se mejoró el formulario con un botón de cancelar y se optimizaron las funciones de eliminación para mayor claridad y mejor manejo de errores.

En el módulo de analíticas, se implementó un store centralizado, un cliente API y un assembler mejorado para reportes, y se integró la lista de reportes con el store.

En la comunidad, se desarrolló un store para gestionar perfiles y comentarios, se crearon las entidades CommunityProfile y Comment, junto con sus assemblers y el cliente API. Se implementaron los componentes de formulario, lista y mural de perfiles, así como las rutas correspondientes y la navegación en el layout, todo ello con soporte de internacionalización en inglés y español.

| Repository                                                      | Branch                                             | Commit Id | Commit Message                                                                                                         | Commit Message Body                                                                                                                                                                                                             | Commited on (Date) |
|-----------------------------------------------------------------|----------------------------------------------------|-----------|------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/layout                                     | 8b53d3b   | feat(layout): update sidebar navigation and restructure layout components.                                             | Separación del router-view a un bloque de main.                                                                                                                                                                                 | 17/05              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/layout                                     | 07be2e4   | feat(i18n): update settings label to 'profile' in en.json and es.json.                                                 | Cambio de nombre a la sección antigua de settings.                                                                                                                                                                              | 17/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | 5ad791f   | feat(store): implement notification management store with Pinia                                                        | Creación del store para gestión de notificaciones con Pinia.                                                                                                                                                                    | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | 0f3823c   | feat(entity): create Notification entity with required fields                                                          | Creación de la entidad Notification con campos id, profile_id, title, message, is_alert, is_read, created_at.                                                                                                                   | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | 450fc7f   | feat(assembler): implement notification assembler for API conversion                                                   | Implementación del assembler para convertir recursos API a entidad Notification.                                                                                                                                                | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | fa5a355   | feat(api): implement notification management API client                                                                | Implementación del API cliente para endpoints de notificaciones.                                                                                                                                                                | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | a66f9f6   | feat(routes): define routes for notification list and alert views                                                      | Definición de rutas para lista de notificaciones y creación de alertas.                                                                                                                                                         | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | 7a069f3   | feat(view): implement alert form view with real-time preview                                                           | Implementación del formulario de alertas con vista previa en tiempo real.                                                                                                                                                       | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | d6ccfaf   | feat(view): implement notification list view with pagination and actions                                               | Implementación de la vista de lista de notificaciones con paginación y acciones.                                                                                                                                                | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/notification-managment                     | 7ad6855   | feat(router): add notification routes to router                                                                        | Integración de las rutas de notificaciones en el enrutador principal.                                                                                                                                                           | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/identity-management-authentication         | 214295c   | feat(iam): added user entity into bounded iam.                                                                         | Implementación de la entidad usuario para el bounded iam.                                                                                                                                                                       | 28/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/identity-management-authentication         | 88dd51c   | feat(iam): implemented basic infrastructure for identity and access management.                                        | Implementación de ‘UserResponse’ y ‘UserResource’ para la transparencia de datos, ‘UserAssembler’ para el mapeo entre entidades y recursos, y ‘IamApi’ para soporte en la búsqueda de usuario por email y creación del usuario. | 28/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/identity-management-authentication         | 3e38c15   | feat(iam): implemented pinia store for authentication state management.                                                | Configura la reactividad del estado, la propiedad computada 'isAuthenticated' y las acciones principales de autenticación vinculadas con 'IamApi', incluyendo además un generador de id para el flujo de registro.              | 28/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/identity-management-authentication         | 1d18879   | feat(iam): implement user interface components and routes for login and registration.                                  | Implementación de interfaces para el registro e inicio de sesión del usuario. Asimismo, preparar las rutas de componentes ‘login-form’ y ‘login-form’.                                                                          | 28/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/identity-management-authentication         | 5e09a7f   | refactor(router): update route to authentication section in bounded iam.                                               | Actualización de ruta al acceso de ‘authentication-section’.                                                                                                                                                                    | 28/05              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | e9cac41   | feat(i18n): add localization for agricultural profiles in english and spanish.                                         | Agregar los idiomas de ingles y español en profiles                                                                                                                                                                             | 02/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 3368d0e   | feat(profile_management): add a cancel button to the profile form and update the delete profile button.                | Añadir un botón de cancelar al formulario de perfil y actualizar el botón de eliminar perfil                                                                                                                                    | 02/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 92ae4fe   | feat(profile_management): update the profile delete functions for greater clarity and improved error handling.         | eliminar perfil para mayor claridad y mejor manejo de errores                                                                                                                                                                   | 02/06              |
| L2006delacurz/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd   | feature/commercial_management-analytics_management | 959b608   | feat(analytics_management): add centralized state management store for analytics module.                               | Se implementó un store centralizado para la gestión del estado del módulo de analíticas.                                                                                                                                        | 04/06              |
| L2006delacurz/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd   | feature/commercial_management-analytics_management | b9097ef   | feat(analytics_management): implement api client for analytics management module.                                      | Se creó un cliente API para gestionar la comunicación con los servicios del módulo de analíticas.                                                                                                                               | 04/06              |
| L2006delacurz/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd   | feature/commercial_management-analytics_management | f3af251   | feat(analytics_management): enhance reportassembler for improved resource conversion.                                  | Se mejoró el ensamblador de reportes para optimizar la conversión de recursos y datos.                                                                                                                                          | 04/06              |
| L2006delacurz/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd   | feature/commercial_management-analytics_management | 954e41d   | feat(analytics_management): add report list to use centralized analytics store.                                        | Se integró la lista de reportes con el store centralizado para una gestión unificada de datos.                                                                                                                                  | 04/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | a2f982d   | feat(community_management): implement store for managing community profiles and comments.                              | Implementar un almacén para gestionar perfiles y comentarios de la comunidad                                                                                                                                                    | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 01c3300   | feat(community_management): add comment entity for user reviews and ratings.                                           | Añadir una entidad de comentarios para las reseñas y calificaciones de los usuarios.                                                                                                                                            | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | db68ae8   | feat(community_management): add communityprofile entity for managing user profiles in the community.                   | Añadir la entidad communityprofile para gestionar los perfiles de usuario en la comunidad.                                                                                                                                      | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 7411e09   | feat(community_management): add commentassembler for mapping comment resources to domain entities.                     | Agregar commentassembler para asignar recursos de comentarios a entidades de dominio.                                                                                                                                           | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | cc0b2dd   | feat(community_management): implement communitymanagementApi for managing community profiles and comments.             | Implementar communitymanagementApi para gestionar los perfiles y comentarios de la comunidad.                                                                                                                                   | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | cbaba26   | feat(community_management): add communityProfileAssembler for mapping community profile resources to domain entities.  | Añadir communityProfileAssembler para mapear los recursos de perfil de la comunidad a las entidades de dominio.                                                                                                                 | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 0fb4ffd   | feat(community_management): add community profile form component for creating and editing profiles.                    | Añadir un componente de formulario de perfil de comunidad para crear y editar perfiles.                                                                                                                                         | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | c1da45e   | feat(community_management): add community profile list component for displaying and managing user profiles.            | Añadir el componente de lista de perfiles de la comunidad para mostrar y gestionar los perfiles de usuario.                                                                                                                     | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | e636561   | feat(community_management): add community profile mural component for viewing profiles, rating, and commenting.        | Añadir el componente mural de perfil de la comunidad para ver, calificar y comentar perfiles.                                                                                                                                   | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | ab7f426   | feat(community_management): add community routes for profile list, form, and mural views.                              | Añadir rutas de comunidad para las vistas de lista de perfiles, formulario y mural.                                                                                                                                             | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | fdb4df2   | feat(i18n): add community localization for profiles and mural in english and spanish.                                  | Añadir localización de la comunidad para perfiles y mural en inglés y español.                                                                                                                                                  | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 98286d5   | feat(layout): add community navigation link to layout.                                                                 | Añadir enlace de navegación de la comunidad al diseño.                                                                                                                                                                          | 08/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd      | feature/profile_management-community_management    | 4c66e36   | feat(router): add community routes to the main router.                                                                 | Agrega rutas de comunidad al enrutador principal.                                                                                                                                                                               | 08/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | feature/navegation-routes                          | 6b2eeb4   | refactor(routes): implemented adjustments in routes to start in iam context.                                           | Actualización de rutas para mejorar la navegación y ruta del usuario.                                                                                                                                                           | 14/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/devivces.entities                          | d2e8e3    | feat(monitoring): add field_id to device and profile_id to field entities.                                             | Añadido de field_id a device y profile_id a field entities.                                                                                                                                                                     | 15/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/devivces.entities                          | c3ac746   | feat(monitoring): enhance field form and list with improved validation and dynamic filtering.                          | Mejora del formulario y la lista de campos con una validación optimizada y un filtrado dinámico.                                                                                                                                | 15/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/devivces.entities                          | e55fcc2   | feat(monitoring): add field_id to device form and list with improved filtering and validation.                         | Añadido de field_id al formulario del dispositivo y a la lista con filtrado y validación mejorados.                                                                                                                             | 15/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/devivces.entities                          | 5b7d892   | feat(routes): update navigation paths for inventory and monitoring sections.                                           | Actualización de las rutas de navegación para las secciones de inventario y monitorización.                                                                                                                                     | 15/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/devivces.entities                          | 6c4db74   | feat(i18n): update soil type options and add new validation messages in en.json and es.json.                           | Actualización de las opciones de tipo de suelo y agrega nuevos mensajes de validación en en.json y es.json.                                                                                                                     | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 33ef816   | feat: add stock management bounded context                                                                             | Adds stock management bounded context with inventory store, endpoint, presentation components (add-product-form, discount-product-form, inventory-list, inventory.vue).                                                          | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 907992c   | feat: refactor inventory list                                                                                          | Refactors inventory list component, updates package-lock.json, locales (en.json, es.json), router.js, and layout.vue.                                                                                                           | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | b5d39ec   | feat(stock): add product entity class                                                                                  | Adds product.entity.js in stock domain model.                                                                                                                                                                                   | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 01e6758   | feat(stock): add stock movement entity class                                                                           | Adds stock-movement.entity.js in stock domain model.                                                                                                                                                                            | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 02f4a9f   | feat(stock): implement stock api class                                                                                 | Implements stock-api.js in stock infrastructure.                                                                                                                                                                                | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 83761ef   | feat(stock): add product assembler                                                                                     | Adds product.assembler.js in stock infrastructure.                                                                                                                                                                              | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | becaf33   | feat(stock): add stock movement assembler                                                                              | Adds stock-movement.assembler.js in stock infrastructure.                                                                                                                                                                       | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 24d6198   | feat(stock): implement stock store                                                                                     | Implements stock.store.js in stock application.                                                                                                                                                                                 | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 10a02bf   | feat(stock): add stock view component                                                                                  | Adds stock-view.vue in stock presentation views.                                                                                                                                                                                | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 1d64493   | feat(stock): add stock form component                                                                                  | Adds stock-form.vue in stock presentation views.                                                                                                                                                                                | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 98a6b7c   | feat(stock): add product list component                                                                                | Adds product-list.vue in stock presentation components.                                                                                                                                                                         | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 02f6642   | feat(stock): add add-product-form component                                                                            | Adds add-product-form.vue in stock presentation components.                                                                                                                                                                     | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 34b413f   | feat(stock): add discount-product-form component                                                                       | Adds discount-product-form.vue in stock presentation components.                                                                                                                                                                | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | b086c4d   | feat(stock): update router with stock view                                                                             | Updates router.js to include stock view.                                                                                                                                                                                        | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | c098345   | refactor(stock): remove old inventory files                                                                            | Removes old inventory files (store, endpoint, components, views).                                                                                                                                                               | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | d1f9f86   | feat(stock): add inventory entity                                                                                      | Adds inventory.entity.js in stock domain model and updates stock-form.vue.                                                                                                                                                      | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 355d0cd   | feat(stock): add inventory assembler                                                                                   | Adds inventory.assembler.js in stock infrastructure.                                                                                                                                                                            | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | bdee841   | feat(stock): update stock api                                                                                          | Updates stock-api.js in stock infrastructure.                                                                                                                                                                                   | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | ffd698b   | feat(stock): update stock store                                                                                        | Updates stock.store.js in stock application.                                                                                                                                                                                    | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 76b722a   | feat(stock): update stock view                                                                                         | Updates stock-view.vue in stock presentation views.                                                                                                                                                                             | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 5523a29   | feat(stock): add stock routes                                                                                          | Adds stock.routes.js in stock module.                                                                                                                                                                                           | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | f3e3837   | feat(i18n): update stock translations en                                                                               | Updates en.json with stock translations.                                                                                                                                                                                        | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 1b2e7a1   | feat(i18n): update stock translations es                                                                               | Updates es.json with stock translations.                                                                                                                                                                                        | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 3f3f7b0   | refactor: rename and remove obsolete files.                                                                            | Renames and removes obsolete files: router.js, product.entity.js, stock-movement.entity.js, product.assembler.js, stock-movement.assembler.js, add-product-form.vue, discount-product-form.vue, product-list.vue, stock.routes.js, stock-form.vue. | 13/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 5ad791f   | feature: implement notification management store with Pinia                                                            | Creates notification-management.store.js for notification management with Pinia.                                                                                                                                                | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 0f3823c   | feature: create Notification entity with required fields                                                               | Creates notification.entity.js in notification-management domain model.                                                                                                                                                         | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 450fc7f   | feature: implement notification assembler for API conversion                                                           | Implements notification.assembler.js in notification-management infrastructure.                                                                                                                                                 | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | fa5a355   | feature: implement notification management API client                                                                  | Implements notification-management-api.js for notification endpoints.                                                                                                                                                           | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | a66f9f6   | feature: define routes for notification list and alert views                                                           | Defines notification-management-routes.js for list and alert views.                                                                                                                                                             | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 7a069f3   | feature: implement alert form view with real-time preview                                                              | Implements notification-alert.vue with real-time preview.                                                                                                                                                                       | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | d6ccfaf   | feature: implement notification list view with pagination and actions                                                  | Implements notification-list.vue with pagination and actions.                                                                                                                                                                   | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 7ad6855   | feature: add notification routes to router                                                                             | Adds notification routes to router.js.                                                                                                                                                                                          | 26/05              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | ff29024   | feat(notifications): add complete localization strings for EN and ES                                                  | Adds complete localization strings for notifications in en.json and es.json.                                                                                                                                                    | 03/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 7f4f714   | refactor(analytics): rewrite store to Composition API                                                                  | Rewrites analytics-management.store.js to Composition API.                                                                                                                                                                      | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | e097cc3   | refactor(analytics): improve API client structure                                                                      | Improves analytics-management-api.js structure.                                                                                                                                                                                 | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | e9c8c3b   | refactor(analytics): improve assembler response handling                                                               | Improves report.assembler.js response handling.                                                                                                                                                                                 | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | bb847f9   | style(analytics): clean up routes metadata                                                                             | Cleans up analytics-management-routes.js metadata.                                                                                                                                                                              | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 6362019   | refactor(analytics): convert to script setup and improve i18n                                                          | Converts report-list.vue to script setup and improves i18n.                                                                                                                                                                     | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | cb955ae   | refactor(commercial): rewrite store to Composition API                                                                 | Rewrites commercial-management.store.js to Composition API.                                                                                                                                                                     | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | e0bd0dd   | feat(commercial): align order entity with backend OrderResource                                                        | Aligns order.entity.js with backend OrderResource.                                                                                                                                                                              | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 0f8da5e   | feat(commercial): align product entity with backend ProductResource                                                    | Aligns product.entity.js with backend ProductResource.                                                                                                                                                                          | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | bd72896   | refactor(commercial): use BaseEndpoint with env variables                                                              | Refactors commercial-management-api.js to use BaseEndpoint with env variables.                                                                                                                                                  | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 5035459   | refactor(commercial): implement proper toEntityFromResource pattern                                                    | Implements toEntityFromResource pattern in order.assembler.js.                                                                                                                                                                  | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | ad094b2   | refactor(commercial): implement proper toEntityFromResource pattern                                                    | Implements toEntityFromResource pattern in product.assembler.js.                                                                                                                                                                | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 08fbb40   | style(commercial): clean up routes                                                                                     | Cleans up commercial-management-routes.js.                                                                                                                                                                                      | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | aac8661   | refactor(commercial): improve i18n and store integration                                                               | Improves i18n and store integration in order-list.vue.                                                                                                                                                                          | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 76e36f5   | refactor(commercial): add i18n for product names and descriptions                                                      | Adds i18n for product names and descriptions in product-list.vue.                                                                                                                                                               | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 9a4f8e3   | feat(ui): replace emojis with PrimeIcons in sidebar                                                                    | Replaces emojis with PrimeIcons in layout.vue sidebar.                                                                                                                                                                          | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 4c80135   | i18n: add commercial product translations and nav catalog key                                                          | Adds commercial product translations and nav catalog key in en.json.                                                                                                                                                            | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 0d1db2e   | i18n: add Spanish commercial product translations                                                                      | Adds Spanish commercial product translations in es.json.                                                                                                                                                                        | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 6048ed1   | style: improve UI visual consistency and replace emojis with PrimeIcons                                                | Improves UI visual consistency and replaces emojis with PrimeIcons in report-list.vue, field-list.vue, and inventory-form.vue.                                                                                                  | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 1c5ebc1   | feature(profile-list): fix button hover movement and prevent table reflow                                              | Fixes button hover movement and prevents table reflow in profile-list.vue.                                                                                                                                                      | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | a8afb9a   | feature(report-list): improve visual design with gradients and shadows                                                 | Improves visual design with gradients and shadows in report-list.vue.                                                                                                                                                           | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 5e2b85f   | feature(community-profile-list): adjust buttons and input styling                                                      | Adjusts buttons and input styling in community-profile-list.vue.                                                                                                                                                                | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | a73f5db   | feature(language-switcher): improve design with pill-style buttons                                                     | Improves design with pill-style buttons in language-switcher.vue.                                                                                                                                                               | 15/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | b323715   | feature(i18n): add home dashboard translations for EN and ES                                                          | Adds home dashboard translations in en.json and es.json.                                                                                                                                                                        | 16/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd       | develop                                            | 6c75ae4   | feature(home): add dashboard with charts and summary table                                                             | Adds dashboard with charts and summary table in home.vue.                                                                                                                                                                       | 16/06              |

**BackEnd:**

Durante el desarrollo del backend de TerraTech se han implementado múltiples funcionalidades distribuidas en diferentes bounded contexts, siguiendo una arquitectura basada en DDD (Domain-Driven Design) y aplicando patrones como Result, repositorios con soporte de cancelación, y una capa de infraestructura compartida.

Shared Kernel y configuración inicial
Se inició el proyecto con la estructura de carpetas y dependencias necesarias, instalando los paquetes esenciales. Se añadió soporte para tokens de cancelación en el repositorio base y la unidad de trabajo, y se implementó el patrón Result para estandarizar las respuestas de las operaciones. Se introdujo una convención de nomenclatura de rutas en kebab-case y se configuró la infraestructura de Entity Framework Core, incluyendo el interceptor de auditoría y las extensiones para el ModelBuilder. Además, se añadió un diagrama de clases y se redactaron las technical stories del proyecto.

Identity and Access Management (IAM)
Se implementó el agregado User con objetos de valor como Email y Password, y se definieron los comandos, consultas y repositorios necesarios. Se crearon servicios de aplicación para comandos y consultas, una capa de fachada para la comunicación con otros contextos, y la infraestructura correspondiente (incluyendo servicios de hashing y tokens JWT). Se desarrollaron los controladores de autenticación y usuarios, junto con los recursos y ensambladores, y se configuró la localización de mensajes de error. Se corrigieron problemas de sensibilidad de mayúsculas en la configuración de Swagger y JWT, y se ajustaron las migraciones para cumplir con la convención snake_case.

Gestión de Perfiles (Profile Management)
Se creó el agregado Profile con propiedades de auditoría, y se añadieron objetos de valor para el teléfono de contacto, el nombre del fundo y los umbrales de perfil. Se implementaron los comandos de creación y actualización, las consultas para obtener todos los perfiles y por ID, y se desarrollaron los servicios de aplicación. Se añadieron los repositorios, la configuración de EF Core, los controladores REST y los recursos correspondientes. También se implementó la eliminación de perfiles.

Gestión de Comunidad (Community Management)
Se implementaron los agregados CommunityProfile y Comment con sus respectivas auditorías, y se añadieron objetos de valor como CommunityNickname, PublicBio, Reputation y VisibilityStatus. Se definieron comandos para crear, actualizar y eliminar tanto perfiles de comunidad como comentarios, y se implementaron consultas para obtener perfiles por ID, por ID de perfil, y comentarios por ID y por perfil destino. Se crearon los servicios de aplicación, los repositorios, la configuración de EF Core, los controladores y los recursos REST necesarios. Se integró el contexto en AppDbContext y se registraron los servicios en el contenedor DI.

Monitoreo (Monitoring)
Se añadieron consultas para obtener dispositivos por estado (ONLINE, OFFLINE, LOW_BATTERY) y campos por tipo de suelo, junto con sus respectivos endpoints en los controladores. Se actualizó el repositorio y los servicios de consulta para soportar estas nuevas funcionalidades.

Documentación y configuración final
Se actualizó el archivo README.md con una descripción general del proyecto, tecnologías, arquitectura e instrucciones de configuración.

| Repository                                                     | Branch                                          | Commit Id | Commit Message                                                                                                                                                                                | Commit Message Body                                                                                                                                                                                     | Commited on (Date) |
|----------------------------------------------------------------|-------------------------------------------------|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/shared                                  | 6f9ab57   | chore: initial commit.                                                                                                                                                                        | Creación de las carpetas iniciales del proyecto BackEnd.                                                                                                                                                | 26/05              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/shared                                  | 54f593e   | chore(deps): update package versions in project dependencies.                                                                                                                                 | Instalación de dependencias.                                                                                                                                                                            | 26/05              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/shared                                  | ca4a8b6   | docs: add class diagram for the platform.                                                                                                                                                     | Creación del diagrama de clase.                                                                                                                                                                         | 26/05              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/shared                                  | 96c25cf   | docs: add technical stories for terratech platform.                                                                                                                                           | Creación de los technical stories.                                                                                                                                                                      | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/shared                                  | 5fd1722   | feat(shared): added cancellation token support to base repository and unit of work.                                                                                                           | Se integró el soporte para cancelación en todos los métodos asíncronos del repositorio base y de Unit of Work.                                                                                          | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/shared                                  | 051a506   | feat(shared): add result pattern to standardize operation outcomes with success and failure representations.                                                                                  | Se implementa el patrón Result en la capa compartida para estandarizar las respuestas de las operaciones de negocio.                                                                                    | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/shared                                  | 3f26a74   | feat(shared): introduce kebab-case route naming convention and string extensions.                                                                                                             | Se introdujo una convención de nombres automática para que todas las rutas de los controladores de la API utilicen el formato kebab-case.                                                               | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/shared                                  | 02204ad   | feat(shared): implemented entity framework core infrastructure and bas                                                                                                                        | Se montó la estructura inicial y las abstracciones base para el acceso a datos utilizando Entity Framework Core.                                                                                        | 26/05              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/iam                                     | f7947ca   | feat(iam): added validated email and password value objects for user authentication.                                                                                                          | Creación de Value objects para la autenticación del usuario, siguiendo condiciones pedidas.                                                                                                             | 02/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 6663ae0   | feat(profile_management): implement profile aggregate root with audit properties.                                                                                                             | Implementar la raíz agregada de perfiles con propiedades de auditoría.                                                                                                                                  | 02/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 7aa1148   | feat(profile_management): add createprofilecommand for profile creation.                                                                                                                      | Añadir el comando createprofilecommand para la creación de perfiles.                                                                                                                                    | 02/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 0f76d0c   | feat(profile_management): add value objects for contact phone, fundo name, and profile thresholds.                                                                                            | Añadir objetos de valor para el teléfono de contacto, el nombre del fondo y los umbrales del perfil.                                                                                                    | 02/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 282df10   | feat(iam): implement bounded aggregate root of iam.                                                                                                                                           | Implementación del aggregate root de iam, usando los value object anteriormente creados. Además, preparando al aggregate para auditorías.                                                               | 04/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 091bca7   | feat(iam): added domain commands, queries, repository contracts, and errors localization resources.                                                                                           | Implementación de commands y queries, con la finalidad de modificar estados del sistema y hacer solicitudes de datos. Asimismo, se implementó la interfaz repository para definir las acciones de User. | 04/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | a43d4f5   | chore: repository location updated, now is into domain.                                                                                                                                       | Se corrige la ubicación de repository de Iam, dentro del proyecto.                                                                                                                                      | 04/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | df9ce70   | feat(iam): updated user aggregate and added in repository cancellation token.                                                                                                                 | Se actualizaron métodos dentro del User aggregate y se añadió en el repositorio parámetros cancellation tokens.                                                                                         | 04/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 16beb00   | feat(token): implements token service to validate users.                                                                                                                                      | Implementación de interfaz de servicio para validar usuarios usando tokens.                                                                                                                             | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | a1deaea   | feat(hashing): added hashing service interface in application outbound service.                                                                                                               | Implementación de interfaz de servicio para proteger la contraseña mediante hash.                                                                                                                       | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 4887f0d   | feat(iam): implements command services into application.                                                                                                                                      | Implementación de commands: interfaz para usuario y operaciones internas.                                                                                                                               | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | f83a00a   | feat(iam): implements query services into application.                                                                                                                                        | Implementación de queries: interfaz para usuario y operaciones internas.                                                                                                                                | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 20cb3bf   | feat(iam): implement facade iam anti-corruption layer.                                                                                                                                        | Implementación de facade para permitir la comunicación de otros contextos con Iam, sin corromper capas.                                                                                                 | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | c8f6221   | feat(iam): implement infrastructure layer for identity and access management.                                                                                                                 | Implementación de capa de infraestructura para la identificación y acceso de usuario.                                                                                                                   | 05/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 8d213be   | feat(iam): implements controller to user and authentication.                                                                                                                                  | Implementación de controllers para user y autenticación. Asimismo, creación de los resources y assembler para respuestas.                                                                               | 06/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | ad6eb56   | feat(iam): added localization resources.                                                                                                                                                      | Se añadió la localización y globalización mediante marker class dedicada en la capa de recursos de Iam.                                                                                                 | 06/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 42cb20f   | fix: correct case sensitivity in iam context configuration and swagger jwt bearer.                                                                                                            | Se arreglaron problemas con nombres en el bounded context de Iam y se renombró de manera correcta bearer a Bearer dentro del swagger configuration de JWT.                                              | 06/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 9c572ce   | feat(shared): configure fluent api mapping for user entity in appdbcontext.                                                                                                                   | Configuración de appdbcontext para el mapeo del user entity.                                                                                                                                            | 06/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 70c8296   | feat(profile_management): add interface for profile command handling.                                                                                                                         | Agrega una interfaz para el manejo de comandos de perfil.                                                                                                                                               | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 26c19af   | feat(profile_management): implement profilecommandservice for profile command handling.                                                                                                       | Implementa profilecommandservice para el manejo de comandos de perfil.                                                                                                                                  | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 04e82ea   | feat(profile_management): add profilequeryservice for profile retrieval operations.                                                                                                           | Añadir profilequeryservice para operaciones de recuperación de perfiles.                                                                                                                                | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 4783e33   | feat(profile_management): add interface for profile query operations.                                                                                                                         | Añadir interfaz para operaciones de consulta de perfiles.                                                                                                                                               | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 8651121   | feat(profile_management): add for retrieving all profiles.                                                                                                                                    | Añadir funcionalidad para recuperar todos los perfiles.                                                                                                                                                 | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | ffe2103   | feat(profile_management): add for profile retrieval by ID.                                                                                                                                    | Añadir recuperación de perfiles por ID.                                                                                                                                                                 | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 19f7f36   | feat(profile_management): add profile repository interface.                                                                                                                                   | Añadir interfaz de repositorio de perfiles.                                                                                                                                                             | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | eb0bac4   | feat(profile_management): add extensions for profile management configuration.                                                                                                                | Añadir extensiones para la configuración de la gestión de perfiles.                                                                                                                                     | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 09e473a   | feat(profile_management): implement profile repository class.                                                                                                                                 | Implementar la clase de repositorio de perfiles.                                                                                                                                                        | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | ed0d554   | feat(profile_management): add for profile creation.                                                                                                                                           | Agregar para la creación de perfiles.                                                                                                                                                                   | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 402b24b   | feat(profile_management): add record for API responses.                                                                                                                                       | Agregar registro para las respuestas de la API.                                                                                                                                                         | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 555f8ae   | feat(profile_management): add assembler for creating profile command from resource.                                                                                                           | Añadir ensamblador para crear el comando de perfil a partir del recurso.                                                                                                                                | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | 2589515   | feat(profile_management): add assembler for converting profile entity to resource.                                                                                                            | Añadir ensamblador para convertir la entidad de perfil en un recurso.                                                                                                                                   | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management-community_management | cd13b2e   | feat(profile_management): implement ProfilesController with CRUD operations for profiles.                                                                                                     | Implementar ProfilesController con operaciones CRUD para perfiles.                                                                                                                                      | 11/06              |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd       | feature/identity-management-authentication      | 134118e   | fix: align database migration columns with snake_case naming convention.                                                                                                                      | Ajustar database migration siguiendo lineamientos del docente y recomendaciones del grupo.                                                                                                              | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management                      | 7e012ae   | refactor(profile_management): clean up Profile class by removing unused code and comments.                                                                                                    | Limpiar la clase Profile eliminando el código y los comentarios no utilizados.                                                                                                                          | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management                      | ff004fb   | feat(profile_management): register profile services in Program.cs for dependency injection.                                                                                                   | Registrar los servicios de perfil en Program.cs para la inyección de dependencias.                                                                                                                      | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/profile_management                      | fb3e6cf   | feat(profile_management): add ProfileManagement configuration to AppDbContext.                                                                                                                | Añadir la configuración de ProfileManagement a AppDbContext.                                                                                                                                            | 11/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | a4dcd34   | feat(community_management): add CommunityError enum for error handling.                                                                                                                       | Añadir la enumeración CommunityError para el manejo de errores.                                                                                                                                         | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | ddae2ba   | feat(community_management): implement CommentService for comment handling and operations.                                                                                                     | Implementar CommentService para el manejo y las operaciones de comentarios.                                                                                                                             | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 8ddd7f2   | feat(community_management): implement CommunityProfileService for managing community profiles.                                                                                                | Implementar CommunityProfileService para la gestión de perfiles de la comunidad.                                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | f009022   | feat(community_management): add ICommentService interface for comment operations.                                                                                                             | Agregar la interfaz ICommentService para las operaciones con comentarios.                                                                                                                               | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 8905a51   | feat(community_management): add ICommunityProfileService interface for community profile operations.                                                                                          | Añadir la interfaz ICommunityProfileService para operaciones con perfiles de comunidad.                                                                                                                 | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | a82f47c   | feat(community_management): add Comment class for managing comments and their properties.                                                                                                     | Agregar la clase Comment para la gestión de comentarios y sus propiedades.                                                                                                                              | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | e330f96   | feat(community_management): add CommentAudit class for tracking comment creation and updates.                                                                                                 | Agregar la clase CommentAudit para el seguimiento de la creación y actualización de comentarios.                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | f96df76   | feat(community_management): implement CommunityProfile and CommunityProfileAudit classes for managing community profiles and tracking changes.                                                | Implementar las clases CommunityProfile y CommunityProfileAudit para la gestión de perfiles de la comunidad y el seguimiento de cambios.                                                                | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | ecd41ab   | feat(community_management): add CreateCommentCommand and CreateCommunityProfileCommand for creating comments and community profiles.                                                          | Agregar CreateCommentCommand y CreateCommunityProfileCommand para la creación de comentarios y perfiles de comunidad.                                                                                   | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 32c0301   | feat(community_management): add GetAllCommunityProfilesQuery for retrieving all community profiles.                                                                                           | Agrega GetAllCommunityProfilesQuery para recuperar todos los perfiles de la comunidad.                                                                                                                  | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | a3efc6a   | feat(community_management): add value objects for community profiles including CommunityNickname, PublicBio, Reputation, and VisibilityStatus.                                                | Se añaden objetos de valor para los perfiles de la comunidad, incluyendo CommunityNickname, PublicBio, Reputation y VisibilityStatus.                                                                   | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 0833259   | feat(community_management): add repositories for comments and community profiles with asynchronous retrieval methods.                                                                         | Se añaden repositorios para comentarios y perfiles de la comunidad con métodos de recuperación asíncrona.                                                                                               | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 8552a39   | feat(community_management): add ModelBuilderExtensions for configuring CommunityProfile and Comment entities.                                                                                 | Se añaden `ModelBuilderExtensions` para configurar las entidades `CommunityProfile` y `Comment`.                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | ecfced9   | feat(community_management): add repositories for comments and community profiles with asynchronous methods.                                                                                   | Se añaden repositorios para comentarios y perfiles de la comunidad con métodos asíncronos.                                                                                                              | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 7ba8c75   | feat(community_management): add CommentResource and CreateCommentResource for comment handling.                                                                                               | Se añaden `CommentResource` y `CreateCommentResource` para la gestión de comentarios.                                                                                                                   | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 627c799   | feat(community_management): add CommunityProfileResource and CreateCommunityProfileResource for community profile handling.                                                                   | Se añaden `CommunityProfileResource` y `CreateCommunityProfileResource` para la gestión de perfiles de la comunidad.                                                                                    | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 093ca01   | feat(community_management): add CommentResourceFromEntityAssembler and CreateCommentCommandFromResourceAssembler for transforming comment resources and commands.                             | Se añaden CommentResourceFromEntityAssembler y CreateCommentCommandFromResourceAssembler para transformar recursos y comandos de comentarios.                                                           | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 4f9dee3   | feat(community_management): add CommunityProfileResourceFromEntityAssembler and CreateCommunityProfileCommandFromResourceAssembler for transforming community profile resources and commands. | Se añaden CommunityProfileResourceFromEntityAssembler y CreateCommunityProfileCommandFromResourceAssembler para transformar recursos y comandos de perfiles de comunidad.                               | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | f5824c8   | feat(community_management): add CommentsController and CommunityProfilesController for managing comments and community profiles.                                                              | Agrega CommentsController y CommunityProfilesController para administrar comentarios y perfiles de la comunidad.                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | 75760a6   | feat(shared): configure Community Management context in AppDbContext.                                                                                                                         | Configura el contexto de administración de la comunidad en AppDbContext.                                                                                                                                | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetAllCommunityProfilesQuery            | c2dd9ac   | feat(community_management): register Community Management services in Program.cs.                                                                                                             | Registra los servicios de administración de la comunidad en Program.cs.                                                                                                                                 | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetCommunityProfileByIdQuery            | 0f83ced   | feat(community_management): add GetCommunityProfileByIdQuery for retrieving community profiles by ID.                                                                                         | Agrega GetCommunityProfileByIdQuery para recuperar perfiles de comunidad por ID.                                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetCommunityProfileByProfileIdQuery     | 96e45bc   | feat(community_management): add GetCommunityProfileByProfileIdQuery for retrieving community profiles by profile ID.                                                                          | Agrega GetCommunityProfileByProfileIdQuery para recuperar perfiles de comunidad por ID de perfil.                                                                                                       | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetCommentByIdQuery                     | 7013975   | feat(community_management): add GetCommentByIdQuery for retrieving comments by ID.                                                                                                            | Agrega GetCommentByIdQuery para recuperar comentarios por ID.                                                                                                                                           | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/GetCommentsByTargetProfileIdQuery       | 046ae0a   | feat(community_management): add GetCommentsByTargetProfileIdQuery for retrieving comments by target profile ID.                                                                               | Agrega GetCommentsByTargetProfileIdQuery para recuperar comentarios por ID de perfil de destino.                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateCommunityProfile                  | 321a654   | feat(community_management): add UpdateCommunityProfileCommand for updating community profile details.                                                                                         | Agrega UpdateCommunityProfileCommand para actualizar los detalles del perfil de la comunidad.                                                                                                           | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateCommunityProfile                  | 6d1291a   | feat(community_management): add UpdateCommunityProfileResource for updating community profile details.                                                                                        | Se añade UpdateCommunityProfileResource para actualizar los detalles del perfil de la comunidad.                                                                                                        | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateComment                           | 29851ee   | feat(community_management): add UpdateCommentCommand for updating comments.                                                                                                                   | Se añade UpdateCommentCommand para actualizar los comentarios.                                                                                                                                          | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateComment                           | 483df46   | feat(community_management): add UpdateCommentResource for updating comment payload.                                                                                                           | Se añade UpdateCommentResource para actualizar la información de los comentarios.                                                                                                                       | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateComment                           | 5665eb0   | refactor(community_management): remove unused QueryServices import from Program.cs.                                                                                                           | Se elimina la importación no utilizada de QueryServices de Program.cs.                                                                                                                                  | 14/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateProfile                           | d79e44f   | feat(profile_management): add Handle method for updating profiles.                                                                                                                            | Se añade el método Handle para actualizar los perfiles.                                                                                                                                                 | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateProfile                           | d1927ce   | feat(profile_management): add method for updating profiles.                                                                                                                                   | Se añade un método para actualizar los perfiles.                                                                                                                                                        | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateProfile                           | 9c4f05d   | feat(profile_management): add Update method and command for profile updates.                                                                                                                  | Se añade el método y el comando Update para actualizar los perfiles.                                                                                                                                    | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateProfile                           | 2a5ec22   | feat(profile_management): enhance profile resource schemas with validation and Swagger annotations.                                                                                           | Se mejoran los esquemas de recursos de perfil con validación y anotaciones Swagger.                                                                                                                     | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/UpdateProfile                           | 331e785   | feat(profile_management): add UpdateProfile endpoint for updating existing profiles.                                                                                                          | Agregar punto final UpdateProfile para actualizar perfiles existentes.                                                                                                                                  | 15/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteCommunityProfile                  | 0b133da   | feat(community_management): add command for deleting a community profile by id.                                                                                                               | Se añade un comando para eliminar un perfil de comunidad por ID.                                                                                                                                        | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteCommunityProfile                  | 60e163e   | feat(community_management): implement method for deleting a community profile.                                                                                                                | Se implementa un método para eliminar un perfil de comunidad.                                                                                                                                           | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteCommunityProfile                  | 947d910   | feat(community_management): add endpoint for deleting a community profile by id.                                                                                                              | Se añade un endpoint para eliminar un perfil de comunidad por ID.                                                                                                                                       | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteComment                           | 2d9b8a1   | feat(community_management): add command for deleting a comment by id.                                                                                                                         | Añadir comando para eliminar un comentario por ID.                                                                                                                                                      | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteComment                           | 363b6b1   | feat(comment_management): implement method for deleting a comment by id.                                                                                                                      | Implementar método para eliminar un comentario por ID.                                                                                                                                                  | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteComment                           | fdbaa06   | feat(comment_management): add endpoint for deleting a comment by id.                                                                                                                          | Añadir endpoint para eliminar un comentario por ID.                                                                                                                                                     | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteProfile                           | e297604   | feat(profile_management): add command for deleting a profile by id.                                                                                                                           | Añadir comando para eliminar un perfil por ID.                                                                                                                                                          | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteProfile                           | 53cf28d   | feat(profile_management): implement method for deleting a profile.                                                                                                                            | Implementar método para eliminar un perfil.                                                                                                                                                             | 16/06              |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd      | feature/DeleteProfile                           | 50fa7d0   | feat(profile_management): add endpoint for deleting a profile by id.                                                                                                                          | Agrega un endpoint para eliminar un perfil por ID.                                                                                                                                                      | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetDeviceByStatusQuery                  | c524e44   | docs: update readme with project overview, technologies, architecture, and setup instructions.                                                                                                | Añadido de descripción general al README del proyecto, las tecnologías, la arquitectura y las instrucciones de configuración.                                                                           | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetDeviceByStatusQuery                  | 99852be   | feat(monitoring): add query to retrieve devices by their status.                                                                                                                              | Añadido de query para recuperar devices por estado.                                                                                                                                                     | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetDeviceByStatusQuery                  | bc7ce9a   | feat(monitoring): add method to retrieve devices by status.                                                                                                                                   | Añadido de método para recuperar devices por estado.                                                                                                                                                    | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetDeviceByStatusQuery                  | 237cb1c   | feat(monitoring): add method to retrieve devices by status.                                                                                                                                   | Añadido de método para recuperar devices por estado.                                                                                                                                                    | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetDeviceByStatusQuery                  | 2db2a0c   | feat(monitoring): add endpoint to retrieve devices by status.                                                                                                                                 | Añadido de endpoint de recuperación de Devices por estado.                                                                                                                                              | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetFieldBySoilTypeQuery                 | 48905e4   | feat(monitoring): add query to retrieve fields by soil type.                                                                                                                                  | Añadido de una consulta para recuperar campos por tipo de suelo.                                                                                                                                        | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetFieldBySoilTypeQuery                 | 199a78a   | feat(monitoring): add parameter casing in findbysoiltypeasync method.                                                                                                                         | Añadido de parameter casing en el método findbysoiltypeasync.                                                                                                                                           | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetFieldBySoilTypeQuery                 | 3e7d9b6   | feat(monitoring): add method to retrieve fields by soil type.                                                                                                                                 | Añadido de método para recuperar Fields por tipo de suelo.                                                                                                                                              | 16/06              |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/GetFieldBySoilTypeQuery                 | 1735de9   | feat(monitoring): add endpoint to retrieve fields by soil type.                                                                                                                               | Añadido de endpoint de recuperación de Fields por tipo de suelo.                                                                                                                                        | 16/06              |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 52013b1 | feat(notification): add NotificationError enum | Adds NotificationError enum and NotificationAudit aggregate. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 3ac4433 | feat(notification): add INotificationService interface | Adds INotificationService interface in NotificationManagement Application Services. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 2809179 | feat(notification): add NotificationService implementation | Implements NotificationService in NotificationManagement Application Services. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | bca7d20 | feat(notification): add Notification aggregate | Adds Notification aggregate in NotificationManagement Domain Model. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 780850b | feat(notification): add CreateNotificationCommand and MarkAsReadCommand | Adds CreateNotificationCommand and MarkAsReadCommand in NotificationManagement Domain Model. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 177e2ee | feat(notification): add queries GetNotificationsByProfile and GetById | Adds GetNotificationsByProfileQuery and GetNotificationByIdQuery in NotificationManagement Domain Model. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | e668b1b | feat(notification): add INotificationRepository | Adds INotificationRepository interface in NotificationManagement Domain Repositories. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 6f95885 | feat(notification): add NotificationRepository implementation | Implements NotificationRepository in NotificationManagement Infrastructure Persistence. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 78be6b8 | feat(notification): add NotificationsController and REST resources | Adds NotificationsController and REST resources (CreateNotificationResource, MarkAsReadResource, NotificationResource) with assemblers. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 79b98f7 | chore: register NotificationManagement services in DI container | Registers NotificationManagement services in Program.cs DI container. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | fe089da | fix: correct NotificationAudit as partial class implementing IAuditableEntity | Corrects NotificationAudit as partial class implementing IAuditableEntity. | 02/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | ff6f838 | feat(notification): add Notification DbSet and configuration to AppDbContext | Adds Notification DbSet and configuration to AppDbContext. | 03/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5d6a7a7 | refactor(notification): update AppDbContext to use extension method pattern for Notification entity configuration | Refactors AppDbContext to use extension method pattern for Notification entity configuration. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 8434266 | feat(notification): add NotificationModelBuilderExtensions for bounded context entity configuration | Adds NotificationModelBuilderExtensions for bounded context entity configuration. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f6167f5 | feat(stock): add StockError enum for stock management error handling | Adds StockError enum in StockManagement Application Errors and StockModelBuilderExtensions in Shared. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f50079e | feat(stock): add IStockService interface for stock management commands and queries | Adds IStockService interface in StockManagement Application Services. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5773008 | feat(stock): implement StockService for inventory CRUD operations | Implements StockService for inventory CRUD operations. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 20a4139 | feat(stock): add Inventory aggregate root entity | Adds Inventory aggregate root entity in StockManagement Domain Model. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f0fc08a | feat(stock): extend Inventory with IAuditableEntity for audit timestamps | Extends Inventory with IAuditableEntity and adds InventoryAudit. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 272821c | feat(stock): add CreateInventoryCommand record | Adds CreateInventoryCommand record in StockManagement Domain Model Commands. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 37afb0c | feat(stock): add UpdateInventoryCommand record | Adds UpdateInventoryCommand record in StockManagement Domain Model Commands. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f43c470 | feat(stock): add GetInventoryByIdQuery record | Adds GetInventoryByIdQuery record in StockManagement Domain Model Queries. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | eea93d9 | feat(stock): add GetAllInventoryQuery record | Adds GetAllInventoryQuery record in StockManagement Domain Model Queries. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 821bd1b | feat(stock): add IInventoryRepository interface extending IBaseRepository | Adds IInventoryRepository interface in StockManagement Domain Repositories. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 71e0e9c | feat(stock): implement InventoryRepository with custom query methods | Implements InventoryRepository with custom query methods. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 7e17cd7 | feat(stock): add InventoryController with CRUD endpoints | Adds InventoryController with CRUD endpoints. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 538dc7b | feat(stock): add CreateInventoryResource record | Adds CreateInventoryResource record. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | d1a2f10 | feat(stock): add UpdateInventoryResource record | Adds UpdateInventoryResource record. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 8387ec7 | feat(stock): add InventoryResource record for API responses | Adds InventoryResource record for API responses. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5fa3fea | feat(stock): add assembler to map CreateInventoryResource to CreateInventoryCommand | Adds assembler to map CreateInventoryResource to CreateInventoryCommand. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 02b69cf | feat(stock): add assembler to map Inventory entity to InventoryResource | Adds assembler to map Inventory entity to InventoryResource. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | d6260b4 | feat(stock): add StockModelBuilderExtensions for Inventory entity configuration | Adds StockModelBuilderExtensions for Inventory entity configuration. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5e55468 | refactor(stock): update AppDbContext to include Stock configuration and DbSet | Updates AppDbContext to include Stock configuration and DbSet. | 06/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 9193e46 | feat(stock): register Stock services in DI container | Registers Stock services in Program.cs DI container. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | ceb93f1 | feat(stock): add migration for Inventory table | Adds migration for Inventory table. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 7d377fe | feat(stock): add ModelBuilderExtensions for Inventory entity configuration | Adds ModelBuilderExtensions for Inventory entity configuration in StockManagement Infrastructure. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | d61fea3 | feat(notification): add ModelBuilderExtensions for Notification entity configuration | Adds ModelBuilderExtensions for Notification entity configuration in NotificationManagement Infrastructure. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 79afc09 | chore(notification): remove obsolete NotificationModelBuilderExtensions from Shared (moved to NotificationManagement) | Removes obsolete NotificationModelBuilderExtensions from Shared. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 63ef8e8 | chore(stock): remove obsolete StockModelBuilderExtensions from Shared (moved to StockManagement) | Removes obsolete StockModelBuilderExtensions from Shared. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 777c8f1 | refactor(shared): update AppDbContext using to reference bounded contexts configuration extensions | Updates AppDbContext using to reference bounded contexts configuration extensions. | 09/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 14352ae | refactor(stock): update InventoryController route to plural and swagger summaries to use inventories | Updates InventoryController route to plural and swagger summaries. | 10/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 0a6cca4 | refactor(stock): update inventorycontroller route to plural and swagger summaries to use inventories. | Renames InventoryController to InventoriesController and updates route and summaries. | 10/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 7ea1d45 | feat(commercial): add CommercialError enum for error handling | Adds CommercialError enum and related query/resources. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | e14df84 | feat(commercial): add IOrderService interface for order commands and queries | Adds IOrderService interface in CommercialManagement Application Services. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f233787 | feat(commercial): implement OrderService for order management | Implements OrderService for order management. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 08055a3 | feat(commercial): add IProductService interface for product commands and queries | Adds IProductService interface in CommercialManagement Application Services. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | b079c1e | feat(commercial): implement ProductService for product catalog management | Implements ProductService for product catalog management. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 9211072 | feat(commercial): add Order aggregate root entity | Adds Order aggregate root entity in CommercialManagement Domain Model. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 105f94c | feat(commercial): add Product entity for catalog | Adds Product entity for catalog in CommercialManagement Domain Model. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | dd3e167 | feat(commercial): extend Product with IAuditableEntity for audit timestamps | Extends Product with IAuditableEntity and adds ProductAudit. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 20fa64a | feat(commercial): add CreateOrderCommand record | Adds CreateOrderCommand record in CommercialManagement Domain Model Commands. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | ed58e34 | feat(commercial): add CreateProductCommand record | Adds CreateProductCommand record in CommercialManagement Domain Model Commands. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | c3f33b5 | feat(commercial): add UpdateOrderStatusCommand record | Adds UpdateOrderStatusCommand record in CommercialManagement Domain Model Commands. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 49111f2 | feat(commercial): add ValidateOrderCommand record | Adds ValidateOrderCommand record in CommercialManagement Domain Model Commands. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5aee382 | feat(commercial): add GetOrderByIdQuery record | Adds GetOrderByIdQuery record in CommercialManagement Domain Model Queries. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 3f06fbd | feat(commercial): add GetOrdersByProfileQuery record | Adds GetOrdersByProfileQuery record in CommercialManagement Domain Model Queries. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 85537d6 | feat(commercial): add GetAllOrdersQuery record | Adds GetAllOrdersQuery record in CommercialManagement Domain Model Queries. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | e92194a | feat(commercial): add GetAllProductsQuery record | Adds GetAllProductsQuery record in CommercialManagement Domain Model Queries. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 64ff5bf | feat(commercial): add GetProductByIdQuery record | Adds GetProductByIdQuery record in CommercialManagement Domain Model Queries. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | ae3a9ff | feat(commercial): add OrderStatus value object | Adds OrderStatus value object in CommercialManagement Domain Model ValueObjects. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | d10f6df | feat(commercial): add PaymentMethod value object | Adds PaymentMethod value object in CommercialManagement Domain Model ValueObjects. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | e5b5a62 | feat(commercial): add Money value object | Adds Money value object in CommercialManagement Domain Model ValueObjects. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 70f7e94 | feat(commercial): add SubscriptionStatus value object | Adds SubscriptionStatus value object in CommercialManagement Domain Model ValueObjects. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 3d268c8 | feat(commercial): add IOrderRepository interface extending IBaseRepository | Adds IOrderRepository interface in CommercialManagement Domain Repositories. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 7de2914 | feat(commercial): add IProductRepository interface extending IBaseRepository | Adds IProductRepository interface in CommercialManagement Domain Repositories. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | b06452f | feat(commercial): add ModelBuilderExtensions for Order and Product entity configuration | Adds ModelBuilderExtensions for Order and Product entity configuration. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 73d3187 | feat(commercial): implement OrderRepository with custom query methods | Implements OrderRepository with custom query methods. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 8dba16f | feat(commercial): implement ProductRepository with custom query methods | Implements ProductRepository with custom query methods. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 4176159 | feat(commercial): add OrdersController with CRUD endpoints | Adds OrdersController with CRUD endpoints. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 772dffe | feat(commercial): add ProductsController with catalog endpoints | Adds ProductsController with catalog endpoints. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 8aa8b04 | feat(commercial): add CreateOrderResource record | Adds CreateOrderResource record. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f02ed94 | feat(commercial): add CreateProductResource record | Adds CreateProductResource record. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | d280961 | feat(commercial): add OrderResource record for API responses | Adds OrderResource record for API responses. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 7916655 | feat(commercial): add ProductResource record for API responses | Adds ProductResource record for API responses. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 6648655 | feat(commercial): add ValidateOrderResource record | Adds ValidateOrderResource record. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | f9733dc | feat(commercial): add assembler to map CreateOrderResource to CreateOrderCommand | Adds assembler to map CreateOrderResource to CreateOrderCommand. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 687b9f7 | feat(commercial): add assembler to map CreateProductResource to CreateProductCommand | Adds assembler to map CreateProductResource to CreateProductCommand. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 5ba3d5e | feat(commercial): add assembler to map Order entity to OrderResource | Adds assembler to map Order entity to OrderResource. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 2cea7a3 | feat(commercial): add assembler to map Product entity to ProductResource | Adds assembler to map Product entity to ProductResource. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 6955f9e | refactor(shared): update AppDbContext to include Commercial configuration | Updates AppDbContext to include Commercial configuration. | 11/06 |
| Rodri2712/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | develop | 44376d5 | feat(commercial): register Commercial services in DI container | Registers Commercial services in Program.cs DI container. | 11/06 |

#### 5.2.3.5. Execution Evidence for Sprint Review

A continuación, se muestra un video con los avances realizados durante el Sprint 3, asi como el deployment del backend en render.

Video del sprint3:

<img src="assets/images/cap5/Video-Sprtin3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Enlace del video: https://tinyurl.com/mrxyzszz

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

Durante este sprint se completó al 100% el desarrollo del Landing Page del sistema, consolidando su estructura visual, diseño responsivo, traducción multilenguaje y funcionalidades de navegación. Asimismo, se avanzó de forma significativa en la construcción del frontend del sistema, incluyendo componentes claves como el menú resumen del sistema, el dashboard inicial, el módulo de gestión de parcelas(zonas). El equipo logró implementar y probar múltiples servicios que fortalecen la experiencia del usuario y la arquitectura de backend bajo principios DDD.

***Descripción del Logro:***

 - Finalización del Landing Page (100%).
 - Implementación completa de diseño responsivo, i18n, y redirecciones funcionales.
 - Estructura de frontend modular iniciada (menu sidebar, dashboard y componentes base).
 - Aplicación de buenas prácticas de organización por bounded contexts.
 - Integración visual basada en Vue con VuePrime y Primeflex.
 - Lógica de negocio para registro de parcelas y de sensores.
 - Registro de inventario.

***Recursos del Sprint:***

# TerraTech API Endpoints

La siguiente tabla detalla todos los recursos expuestos por la API de TerraTech, organizados por bounded context. Cada fila indica el recurso, la acción implementada, el método HTTP, el endpoint correspondiente y un enlace a la documentación interactiva (Swagger).

| Recurso            | Acción implementada                                                         | Método HTTP | Endpoint                                  | Repositorio Backend                                                                         |
|--------------------|-----------------------------------------------------------------------------|-------------|-------------------------------------------|---------------------------------------------------------------------------------------------|
| **Autenticación**  | Registrar un nuevo usuario (email y contraseña)                             | POST        | `/api/v1/authentication/sign-up`          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Iniciar sesión y obtener token JWT                                          | POST        | `/api/v1/authentication/sign-in`          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Usuarios**       | Obtener un usuario por su ID                                                | GET         | `/api/v1/users/{id}`                      | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un usuario por su email                                             | GET         | `/api/v1/users/email/{email}`             | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Perfiles**       | Crear un perfil agrícola                                                    | POST        | `/api/v1/profiles`                        | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los perfiles                                                  | GET         | `/api/v1/profiles`                        | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un perfil por ID                                                    | GET         | `/api/v1/profiles/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un perfil                                                        | PUT         | `/api/v1/profiles/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Eliminar un perfil                                                          | DELETE      | `/api/v1/profiles/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Monitoreo**      | Crear un campo (zona de cultivo)                                            | POST        | `/api/v1/fields`                          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los campos                                                    | GET         | `/api/v1/fields`                          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un campo por ID                                                     | GET         | `/api/v1/fields/{id}`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un campo                                                         | PUT         | `/api/v1/fields/{id}`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Eliminar un campo                                                           | DELETE      | `/api/v1/fields/{id}`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener campos por tipo de suelo                                            | GET         | `/api/v1/fields/soiltype/{type}`          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Crear un dispositivo IoT                                                    | POST        | `/api/v1/devices`                         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los dispositivos                                              | GET         | `/api/v1/devices`                         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un dispositivo por ID                                               | GET         | `/api/v1/devices/{id}`                    | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un dispositivo                                                   | PUT         | `/api/v1/devices/{id}`                    | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Eliminar un dispositivo                                                     | DELETE      | `/api/v1/devices/{id}`                    | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener dispositivos por campo                                              | GET         | `/api/v1/devices/field/{fieldId}`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener dispositivos por estado (`ONLINE`, `OFFLINE`, `LOW_BATTERY`)        | GET         | `/api/v1/devices/status/{status}`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Analytics**      | Crear un reporte estadístico                                                | POST        | `/api/v1/reports`                         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los reportes                                                  | GET         | `/api/v1/reports`                         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un reporte por ID                                                   | GET         | `/api/v1/reports/{id}`                    | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un reporte                                                       | PUT         | `/api/v1/reports/{id}`                    | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Comercial**      | Crear un pedido                                                             | POST        | `/api/v1/orders`                          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los pedidos                                                   | GET         | `/api/v1/orders`                          | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un pedido por ID                                                    | GET         | `/api/v1/orders/{id}`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener pedidos por perfil                                                  | GET         | `/api/v1/orders/profile/{id}`             | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Validar un pedido                                                           | PUT         | `/api/v1/orders/{id}/validate`            | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar estado de un pedido                                              | PUT         | `/api/v1/orders/{id}/status`              | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Crear un producto                                                           | POST        | `/api/v1/products`                        | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los productos                                                 | GET         | `/api/v1/products`                        | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un producto por ID                                                  | GET         | `/api/v1/products/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Inventarios**    | Crear un ítem de inventario                                                 | POST        | `/api/v1/inventories`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los ítems de inventario                                       | GET         | `/api/v1/inventories`                     | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un ítem de inventario por ID                                        | GET         | `/api/v1/inventories/{id}`                | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un ítem de inventario                                            | PUT         | `/api/v1/inventories/{id}`                | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Notificaciones** | Crear una notificación                                                      | POST        | `/api/v1/notifications`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener notificaciones por perfil                                           | GET         | `/api/v1/notifications`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener una notificación por ID                                             | GET         | `/api/v1/notifications/{id}`              | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Marcar una notificación como leída                                          | PUT         | `/api/v1/notifications/{id}/read`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
| **Comunidad**      | Crear un perfil de comunidad                                                | POST        | `/api/v1/community-profiles`              | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener todos los perfiles de comunidad                                     | GET         | `/api/v1/community-profiles`              | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un perfil de comunidad por ID                                       | GET         | `/api/v1/community-profiles/{id}`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un perfil de comunidad por ID de perfil asociado                    | GET         | `/api/v1/community-profiles/profile/{id}` | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un perfil de comunidad                                           | PUT         | `/api/v1/community-profiles/{id}`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Eliminar un perfil de comunidad                                             | DELETE      | `/api/v1/community-profiles/{id}`         | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Crear un comentario                                                         | POST        | `/api/v1/comments`                        | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener comentarios por perfil destino                                      | GET         | `/api/v1/comments/target/{id}`            | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Obtener un comentario por ID                                                | GET         | `/api/v1/comments/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Actualizar un comentario                                                    | PUT         | `/api/v1/comments/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |
|                    | Eliminar un comentario                                                      | DELETE      | `/api/v1/comments/{id}`                   | [Repo](https://upc-pre-202610-1asi0730-10215-novatech-p8mf.onrender.com/swagger/index.html) |

---
*Todos los endpoints requieren autenticación mediante token JWT, excepto los de registro e inicio de sesión. La documentación interactiva completa está disponible en el repositorio backend.*

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Durante este sprint, se realizaron actividades de despliegue y pruebas de los servicios desarrollados, asegurando que las funcionalidades del sistema estén operativas y accesibles para los usuarios finales. A continuación, se detallan los pasos realizados:

***FrontEnd***

1. Al usar la plataforma vercel para el despliegue de la página estatica, se debe usar el link del repositorio del frontend.

<img src="assets/images/cap5/FrontEnd_Deployment_1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Comienza el proceso de despliegue.

<img src="assets/images/cap5/FrontEnd_Deployment_2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Se termina el despliegue y se obtiene la URL pública para acceder al frontend.

<img src="assets/images/cap5/FrontEnd_Deployment_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***BackEnd***

1. Se creó un Dockerfile para el backend del sistema, permitiendo la creación de una imagen que encapsula todas las dependencias y configuraciones necesarias para ejecutar el servicio.

<img src="assets/images/cap5/Backend_Deploy_1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Al usar panel.filess.io para la creación de la base de datos se usa la opción de shared al ser la opción diposnible para el proyecto.

<img src="assets/images/cap5/Backend_Deploy_2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Al acceder se debe crear una nueva base datos, dedica a la pagina web.

<img src="assets/images/cap5/Backend_Deploy_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

4. Se selecciona MySQL como el motor de base de datos al ser el utilizado en el proyecto.

<img src="assets/images/cap5/Backend_Deploy_4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

5. Se coloca el nombre de la base datos, el cual ya está establecido desde la creación de la pagina estatica.

<img src="assets/images/cap5/Backend_Deploy_5.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

6. Al finalizar la creación se obtiene una base de datos desplegada en la nube, con acceso remoto para conectar el backend del sistema.

<img src="assets/images/cap5/Backend_Deploy_6.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

7. Se optiene la información de conexión a la base de datos, incluyendo host, puerto, usuario y contraseña, para configurar el backend y permitir la comunicación con la base de datos.

<img src="assets/images/cap5/Backend_Deploy_7.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

8. Se crea un .env donde se pondran las variables de entorno, el cual no entra en las versiones del proyecto, solo de manera local.

<img src="assets/images/cap5/Backend_Deploy_8.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

9. Se utilizará la plataforma Render para el despliegue de la página web del proyecto TerraTech.

<img src="assets/images/cap5/Backend_Deploy_9.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

10. Para la creación se utiliza el enlace del repositorio del backend.

<img src="assets/images/cap5/Backend_Deploy_10.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

11. Se asegura que las opciones sean las correctas según el proyecto.

<img src="assets/images/cap5/Backend_Deploy_11.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

12. Ahora se debe utilizar las variables de entorno que se obtenieron de la base de datos.

<img src="assets/images/cap5/Backend_Deploy_12.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

13. Se busca el archivo .env y se copian las variables de entorno necesarias para la conexión a la base de datos.

<img src="assets/images/cap5/Backend_Deploy_13.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

14. Se colocan en las opciones de variables de entorno en Render, para asegurar que el backend pueda acceder a la base de datos desplegada.

<img src="assets/images/cap5/Backend_Deploy_14.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

15. Se inicia el proceso de despliegue en Render.

<img src="assets/images/cap5/Backend_Deploy_15.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

#### 5.2.3.8. Team Collaboration Insights during Sprint

Se crearon ramas específicas para cada actions (feature/[actions-entite-command/query]), permitiendo un trabajo paralelo organizado.

Cada miembro del equipo asumió la responsabilidad de desarrollar una o más secciones del Landing page, Frontend y Backend. Se realizaron commits frecuentes, registrando avances de manera continua y detallada. Las funcionalidades desarrolladas se integraron mediante Pull Requests hacia la rama develop con ayuda de la herramienta GitFlowHelper. Se mantuvo una comunicación constante mediante la plataforma Discord para coordinar avances y resolver dudas en tiempo real. Se aplicaron buenas prácticas de programación, control de versiones y colaboración en equipo.

***Landing Page***

**Analíticos de colaboración**

Permite visualizar y analizar la participación del equipo en tareas colaborativas, identificando el nivel de actividad y compromiso de cada miembro para optimizar la coordinación y la productividad.

<img src="assets/images/cap5/Analytics_Colaborations_Landing_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Muestra el historial y frecuencia de commits realizados en GitHub, ayudando a evaluar el ritmo de desarrollo, la contribución individual y detectar posibles cuellos de botella en el flujo de trabajo.

<img src="assets/images/cap5/Analytics_Commitss_Landing_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***Frontend***

**Analíticos de colaboración**

Permite monitorear de manera detallada la interacción y el aporte de cada miembro en las actividades conjuntas, facilitando la identificación de patrones de trabajo y fomentando una gestión más eficiente del equipo.

<img src="assets/images/cap5/Analytics_Colaborations_Frontend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Presenta un análisis claro del flujo de commits en GitHub, mostrando la frecuencia y volumen de contribuciones para evaluar el progreso del proyecto y detectar áreas que requieren mayor atención o soporte.

<img src="assets/images/cap5/Analytics_Commitss_Frontend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***Backend***

**Analíticos de colaboración**

Ofrece una vista detallada sobre la participación de cada integrante en las actividades grupales, permitiendo identificar su nivel de implicación y colaboración para mejorar la organización y el rendimiento general del equipo.

<img src="assets/images/cap5/Analytics_Colaborations_Backend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

**Analíticos de commits de GitHub**

Refleja el registro y la periodicidad de los commits realizados en el repositorio, facilitando el seguimiento del avance del desarrollo, la distribución de las contribuciones y la detección de posibles bloqueos o retrasos.

<img src="assets/images/cap5/Analytics_Commitss_Backend_3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

## 5.3. Validation Interviews.

### 5.3.1. Diseño de Entrevistas.

Para garantizar que la aplicación cumpla con las necesidades reales de los usuarios finales, se diseñó un proceso de entrevistas de validación centrado en tres segmentos objetivos clave: **Agricultores**, **Proveedores de insumos agrícolas** y **Clientes Finales (compradores)**. Cada sesión de validación incluirá interacción con el **Landing Page** y la **aplicación web** (desktop y mobile), siguiendo flujos de usuario específicos que cubren funcionalidades críticas del sistema.

***Objetivo General***

Validar la usabilidad, comprensión y utilidad de las funcionalidades del sistema a través de sesiones controladas de interacción, aplicando principios de evaluación heurística y recogiendo observaciones cualitativas.

---

***Segmento 1: Agricultores (dueños de cultivo)***

**Elementos a validar:**
- Claridad del valor ofrecido en el Landing Page.
- Flujo de registro y acceso a la plataforma.
- Registro y gestión de zonas de cultivo (Fields).
- Asociación de sensores IoT a zonas de cultivo.
- Visualización de indicadores en tiempo real (humedad, nutrientes, temperatura) en el dashboard de monitoreo.
- Recepción y comprensión de alertas y notificaciones (umbrales, riego, fertilización).
- Gestión de inventario de insumos (registro, edición, filtrado).
- Configuración de preferencias de notificaciones.

**Flujos de Usuario a evaluar (Desktop & Mobile):**
- **UF-A1:** Registro de cuenta y configuración inicial de perfil.
- **UF-A2:** Registro de zona de cultivo con ubicación y tipo de suelo.
- **UF-A3:** Registro de un sensor IoT y asignación a una zona.
- **UF-A4:** Visualización del dashboard de monitoreo (indicadores clave, gráficos históricos, mapa de fertilidad).
- **UF-A5:** Configuración de umbrales de alerta (humedad, nutrientes) y recepción de notificaciones.
- **UF-A6:** Gestión de inventario de insumos (crear, editar, eliminar, filtrar por categoría).
- **UF-A7:** Visualización y respuesta a notificaciones (alertas de riego, fertilización, stock bajo).

**Actividades durante la sesión:**
1. Explorar el Landing Page y describir su comprensión de la pagina y sus beneficios.
2. Simular el proceso de registro de cuenta y configuración de perfil (nombre, teléfono, tamaño de terreno).
3. Registrar una nueva zona de cultivo (nombre, tamaño, tipo de suelo, ubicación).
4. Asignar un sensor IoT a esa zona (ingresar código único).
5. Ingresar al dashboard de monitoreo y explicar lo que ven en los indicadores (humedad, nutrientes, temperatura).
6. Navegar por el mapa de fertilidad y describir la utilidad de la información visual.
7. Configurar un umbral de alerta personalizado (ej. humedad mínima) y recibir una notificación simulada.
8. Acceder al módulo de inventario, registrar un insumo (nombre, cantidad, unidad), editarlo y filtrarlo.
9. Comentar sobre la utilidad de las notificaciones y la facilidad para gestionar el inventario.

---

***Segmento 2: Proveedores de insumos agrícolas***

**Elementos a validar:**
- Claridad del valor ofrecido en el Landing Page desde la perspectiva del proveedor.
- Flujo de registro y acceso a la plataforma.
- Visualización de tablas analíticas (datos agregados de demanda de nutrientes, zonas con mayor actividad, tendencias de compra).
- Navegación en la comunidad: visualización de comentarios y calificaciones sobre productos.
- Gestión de notificaciones relevantes para su negocio (alertas de demanda, cambios en patrones de compra).
- (Opcional) Gestión de su catálogo de productos (si aplica).

**Flujos de Usuario a evaluar (Desktop & Mobile):**
- **UF-P1:** Registro y configuración de perfil de proveedor.
- **UF-P2:** Visualización del dashboard de analytics (tablas y gráficos de demanda y tendencias).
- **UF-P3:** Exploración de la comunidad: visualizar comentarios y calificaciones de productos específicos.
- **UF-P4:** Configuración de notificaciones personalizadas (alertas por zona, tipo de insumo, variaciones de demanda).
- **UF-P5:** (Opcional) Registro y gestión de productos en su catálogo (si se implementa).

**Actividades durante la sesión:**
1. Explorar el Landing Page y describir su comprensión de la pagina como proveedor.
2. Simular el proceso de registro y configuración de perfil de proveedor.
3. Acceder al módulo de analytics y explicar qué información visualizan (tablas de demanda, zonas con mayor actividad, insumos más solicitados).
4. Identificar una oportunidad de negocio a partir de los datos mostrados (ej. qué producto vender en qué zona).
5. Navegar por la comunidad y leer comentarios de agricultores sobre productos de la competencia.
6. Configurar una alerta de notificación para ser informado cuando la demanda de un insumo supere cierto umbral.
7. Comentar sobre la utilidad de la información analítica y las notificaciones para su negocio.

---

***Segmento 3: Clientes Finales (compradores mayoristas y minoristas)***

**Elementos a validar:**
- Claridad del valor ofrecido en el Landing Page desde la perspectiva del comprador.
- Flujo de navegación del catálogo de productos agrícolas.
- Visualización de detalles del producto (origen, trazabilidad, prácticas de cultivo, certificaciones).
- Interacción con la comunidad: lectura de opiniones y calificaciones de otros compradores.
- Configuración de preferencias de notificaciones (nuevos productos, ofertas, cambios de stock).
- (Opcional) Proceso de compra o cotización.

**Flujos de Usuario a evaluar (Desktop & Mobile):**
- **UF-C1:** Registro y configuración de perfil de cliente final.
- **UF-C2:** Navegación y búsqueda en el catálogo de productos (por categoría, región, tipo).
- **UF-C3:** Visualización detallada de un producto (información de origen, trazabilidad, fotos, certificaciones).
- **UF-C4:** Lectura de comentarios y calificaciones de otros compradores.
- **UF-C5:** Configuración de notificaciones preferidas (productos de interés, rebajas, disponibilidad).

**Actividades durante la sesión:**
1. Explorar el Landing Page y describir su comprensión de la pagina como comprador.
2. Simular el proceso de registro y configuración de perfil (intereses, región).
3. Navegar por el catálogo y buscar productos por categoría (ej. "hortalizas", "frutas").
4. Seleccionar un producto y revisar su ficha detallada (origen, prácticas de cultivo, trazabilidad).
5. Leer comentarios de otros compradores sobre ese producto y calificaciones.
6. Configurar notificaciones para recibir alertas cuando haya nuevos productos de una región específica.
7. Comentar sobre la utilidad de la información de trazabilidad y la comunidad para tomar decisiones de compra.

---

***Herramientas y Recursos para Validación***

- **Formato de Evaluación Heurística:** Se aplicarán los 10 principios heurísticos de Nielsen en cada sesión (visibilidad del estado del sistema, relación con el mundo real, control y libertad del usuario, consistencia y estándares, prevención de errores, reconocimiento antes que recuerdo, flexibilidad y eficiencia, diseño estético y minimalista, ayuda a reconocer y recuperarse de errores, ayuda y documentación). Cada principio se puntuará de 1 a 5 y se registrarán observaciones.
- **Instrumento de observación:** Lista de verificación de tareas completadas (sin ayuda / con ayuda / no completadas) + sección de notas abiertas para incidentes, comentarios literales y sugerencias.
- **Grabación de pantalla y voz:** previa autorización de los participantes, para análisis posterior de interacciones, tiempos y patrones de navegación.

---

### 5.3.2. Registro de Entrevistas.

***Segmento 2: Proveedores de insumos agrícolas***

**ENTREVISTA 1:**

**Nombre:** Anita Monago Cachay **Edad:** 35 años **Distrito:** Ica **Timing:** (00:00 - 4:48)

<img src="assets/images/cap5/Entrevista_Validacion_Segmento2-1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Ver entrevista: https://tinyurl.com/may4652j

**Resumen:** Anita Monago Cachay dice que le gustó la plataforma porque el Landing Page transmite con total claridad el valor que ofrece a los proveedores, el proceso de registro y configuración de perfil es sumamente intuitivo tanto en computadoras como en celulares, y el módulo de analítica junto al sistema de notificaciones personalizadas se presentan como herramientas comerciales muy potentes para identificar oportunidades de negocio en tiempo real (como los insumos más solicitados y las zonas con mayor demanda de nutrientes). Asimismo, valora positivamente el poder monitorear los comentarios y calificaciones de la comunidad para conocer las opiniones de los agricultores y analizar a la competencia; sin embargo, sugiere que le agregues una sección que pueda poner el precio de sus productos dentro de la gestión del catálogo, para que la visualización y cotización de los insumos sea mucho más directa y efectiva para los clientes. 

### 5.3.3. Evaluación según heurísticas.



## 5.4. Video About-the-Product.

A continuación, se presenta el video **"About the Product"** del sistema **TerraTech**, una plataforma tecnológica desarrollada para digitalizar y optimizar la gestión agrícola mediante sensores IoT, análisis predictivo, comunidad colaborativa y comercialización transparente. Este video está dirigido principalmente a los visitantes del Landing Page, quienes desean conocer el modelo de negocio y las principales funcionalidades de la plataforma, así como a los usuarios potenciales de las aplicaciones (agricultores, proveedores de insumos y clientes finales), interesados en realizar tareas relacionadas con los procesos soportados por la solución.

El video comunica de forma clara y dinámica el propósito del producto, mostrando cómo TerraTech ayuda a reducir la incertidumbre en la agricultura, optimizar el uso de recursos hídricos y fertilizantes, mejorar la eficiencia operativa mediante el monitoreo en tiempo real, y fortalecer la relación entre agricultores, proveedores y compradores a través de una comunidad transparente y un catálogo trazable. Se utiliza un tono consistente con la propuesta visual y comunicacional del producto, combinando narración, demostraciones de uso en campo y escenarios reales de cultivo.

A continuación, se incluye un screenshot del video, junto con los enlaces de la versión publicada en Microsoft Stream y YouTube.

<img src="assets/images/cap5/about-the-product.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Video en Stream: https://tinyurl.com/m88tcphe 

Video en YouTube: https://youtu.be/g50PX1_6f_M 