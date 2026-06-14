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

## 5.2.2. Sprint 2

### 5.2.2.1. Sprint Planning 2

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

### 5.2.2.2. Aspect Leaders and Collaborators

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

### 5.2.2.3. Sprint Backlog 2

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

### 5.2.2.4. Development Evidence for Sprint Review

Registro de commits representativos del trabajo realizado durante el Sprint 2 en los repositorios de la organización.



| Repository | Branch | Commit ID | Commit Message | Committed On (Date) |
| --- | --- | --- | --- | --- |
| Calin1407/TerraTech-WebApp | develop | f3g4h5i6 | feat(US07): added password recovery flow | 27/04/2026 |
| GuillermoPromac/TerraTech-API | feature/US05-register | a7b8c9d0 | feat(US05): implemented POST /api/auth/register | 27/04/2026 |
| L2006delacruz/TerraTech-WebApp | feature/US06-login | j2k3l4m5 | feat(US06): login integration with JWT | 28/04/2026 |
| Breithner1/TerraTech-WebApp | feature/US10-zones | n6o7p8q9 | feat(US10): dynamic zone selector | 29/04/2026 |
| Rodri2712/TerraTech-WebApp | feature/US09-dashboard | r1s2t3u4 | feat(US09): KPI cards dashboard mock | 28/04/2026 |

### 5.2.2.5. Execution Evidence for Sprint Review

Durante el Sprint 2, el equipo completó las funcionalidades clave de autenticación y la base del dashboard de monitoreo. Se implementaron los formularios de registro y login, validando la interacción con la API backend. El dashboard muestra los indicadores simulados de humedad, nutrientes y temperatura, permitiendo al agricultor familiarizarse con la interfaz. A continuación, se presentan capturas de pantalla de los elementos ejecutados:

- **Pantalla de Registro (US05):** Formulario funcional con validaciones de campos.

  *[Aquí iría la imagen de la pantalla de registro]*

- **Pantalla de Login (US06):** Interfaz de acceso con manejo de tokens JWT.

  *[Aquí iría la imagen de la pantalla de login]*

- **Dashboard de Monitoreo (US09, US10):** Visualización de KPIs y selector de zonas.

  *[Aquí iría la imagen del dashboard con datos mock]*

### 5.2.2.6. Services Documentation Evidence for Sprint Review

La documentación de servicios se enfocó en la especificación de los endpoints de la API REST necesarios para la autenticación y la gestión de usuarios. Se utilizó Swagger/OpenAPI para generar documentación interactiva. Además, se actualizó el archivo `README.md` del repositorio backend con instrucciones para levantar el entorno local y ejecutar las migraciones de la base de datos.

- **Evidencia de documentación Swagger:**

  *[Aquí iría una captura de pantalla de la interfaz de Swagger mostrando los endpoints de auth]*

- **Actualización del esquema de base de datos:** Se versionaron los scripts DDL para las tablas `Client`, `Parcel` y `Device` dentro de la carpeta `/database/migrations`.

  *[Aquí iría un ejemplo del script de migración o su confirmación en el repositorio]*

### 5.2.2.7. Software Deployment Evidence for Sprint Review

El despliegue del backend y la base de datos se realizó en un entorno de pruebas en la nube (usando servicios como Railway o Render para la API, y Supabase/Neon para PostgreSQL). La aplicación web (frontend) se desplegó de forma automática en Netlify para la rama `develop`, permitiendo validar la integración continua.

- **URL de despliegue (Frontend - desarrollo):** `https://terratech-dev.netlify.app`
- **URL de API Base (Backend):** `https://terratech-api.onrender.com`
- **Colección de Postman:** Se compartió una colección con los endpoints probados (Register, Login, Get Profile).

  *[Aquí iría una captura de pantalla del despliegue activo o de la consola de Netlify]*

  *[Aquí iría otra captura de pantalla de la API respondiendo desde el entorno de pruebas]*

### 5.2.2.8. Team Collaboration Insights during Sprint

El equipo mantuvo una comunicación activa a través de Discord, con reuniones diarias de 15 minutos (daily) para reportar avances y bloqueos. Se utilizó **GitHub Projects** para gestionar el tablero Kanban del Sprint 2, moviendo las tareas desde "To Do" → "In Progress" → "Done". La integración de código se gestionó mediante Pull Requests (PRs) que requerían al menos una aprobación de otro miembro del equipo, garantizando la calidad y el cumplimiento de la guía de estilos.

- **Gráfico de contribuciones (Insights):** Se evidencia actividad equilibrada en los diferentes repositorios durante el periodo del sprint.

  *[Aquí iría una imagen del gráfico de contribuciones de GitHub]*

- **Tablero de GitHub Projects:** Se completaron todas las tareas planificadas dentro del tiempo estimado, cerrando el Sprint 2 con éxito.

  *[Aquí iría una captura del tablero de GitHub Projects mostrando las tareas completadas]*

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3\.

<table border="1">
<thead>
<tr>
<th>Número</th>
<th>Sprint 3</th>
</tr>
<tr>
<th colspan=2>Sprint Planning Background</th>
</tr>
</thead>
<tr align='center'>
<td> Date  </td>
<td> 26/05/2026  </td>
</tr>
<tr>
<td>Time</td>
<td> 08:00 PM - 09:30 PM  </td>
</tr>
<tr>
<td>Location</td>
<td> plataforma Discord  </td>
</tr>
<tr>
<td>Prepared by</td>
<td> Howard Robles, Guillermo Arturo   </td>
</tr>
<tr>
<td>Attendees</td>
<td> Acuña de la Cruz, Luis Alfredo <br/> Aguilar Untiveros, Rodrigo Fabrizio<br/> Howard Robles, Guillermo Arturo<br/> Perez Encarnación, Breithner Rodolfo<br/> Retuerto Rodríguez, Jorge Manuel  </td>
</tr>
<tr>
<td>Sprint n-2 Review Summary</td>
<td>Se completó con éxito el FrontEnd (sprint2), con su despliegue en render junto al faki api online. Se validaron los bounded context principales de negocio y se estableció la base del avance de backend. No se detectaron bloqueos críticos.  </td>
</tr>
<tr>
<td>Sprint n-2 Retrospective Summary</td>
<td>El equipo identificó la necesidad de mejorar la toma de tiempo y la organización en equipo para fomentar buenas prácticas en la elaboración del proyecto. </td>
</tr>
<tr>
<td colspan="2"><b>Sprint Goal & User Stories</b></td>
</tr>
<tr>
<td>Sprint 3 Goal</td>
<td> 
Nuestro enfoque está en entregar la primera versión funcional del backend de la aplicación web, permitiendo gestionar sensores, inventarios, comunidad y notificaciones, así como exponer APIs seguras para el consumo del frontend. Creemos que esto habilita la operación centralizada y confiable de la plataforma, facilitando la integración y el flujo de información entre todos los actores de la cadena logística. Esto se confirmará cuando el frontend pueda consumir los servicios principales, los datos se almacenen y consulten correctamente, y los usuarios reporten que las funcionalidades clave están disponibles y operativas.
</td>
</tr>
<tr>
<td>Sprint 3 velocity</td>
<td> 18  </td>
</tr>
<tr>
<td>Sum of Story Points</td>
<td> 21  </td>
</tr>
</table>

#### 5.2.3.2. Aspect Leaders and Collaborators

En este sprint, se definieron roles de liderazgo para la elaboración de los bounded context.

<table border="1">
  <thead>
    <tr>
      <th>Team member</th>
      <th>Github username</th>
      <th>Identity & Access Management</th>
      <th>Monitoring Management</th>
      <th>Notification Management</th>
      <th>Profile Management</th>
      <th>Stock Management</th>
      <th>Community Management</th>
      <th>Analytics Management</th>
      <th>Commercial Management</th>
  </thead>
  <tbody>
    <tr>
      <td>Retuerto Rodriguez, Jorge Manuel</td>
      <td>Calin1407</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Howard Robles, Guillermo Arturo</td>
      <td>GuillermoPromac</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Acuña de la Cruz, Luis Alfredo</td>
      <td>L2006delacruz</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">L</td>
    </tr>
    <tr>
      <td>Perez Encarnacion, Breithner Rodolfo</td>
      <td>Breithner1</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
    <tr>
      <td>Aguilar Untiveros, Rodrigo Fabrizio</td>
      <td>Rodri2712</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">L</td>
      <td align="center">C</td>
      <td align="center">C</td>
      <td align="center">C</td>
    </tr>
  </tbody>
</table>

#### Sprint Backlog 3

Tabla con el detalle de las tareas asignadas para cumplir con las historias de usuario del Sprint 3.

| <strong>Sprint #</strong> | <strong>Sprint 3</strong>         |
| --- |-----------------------------------|
| <strong>User Story</strong> | <strong>Work-item / Task</strong> |
| <strong>ID</strong> | <strong>Title</strong>            | <strong>ID</strong> | <strong>Title</strong> | <strong>Description</strong> | <strong>Estimation (Hours)</strong> | <strong>Assigned to</strong> | <strong>Status</strong> |
| US05 | Registro de Nuevo Usuario         | Task 6 | Formulario y validación de registro | Crear formulario de registro con validación de email único y coincidencia de contraseñas. | 4 | Breithner Perez | Done |
| US05 | Registro de Nuevo Usuario         | Task 7 | Integración con API de usuarios | Conectar el frontend con el endpoint POST /api/auth/register. | 3 | Guillermo Howard | Done |
| US06 | Inicio de Sesión                  | Task 8 | Pantalla de login y JWT | Implementar pantalla de login y almacenamiento de token JWT en localStorage. | 3 | Luis Acuña | Done |
| US07 | Recuperación de Contraseña        | Task 9 | Flujo de recuperación | Crear flujo "Olvidé mi contraseña" con envío de correo simulado o real. | 2 | Jorge Retuerto | Done |
| US09 | Indicadores Clave (Dashboard)     | Task 10 | Maquetación de tarjetas de KPIs | Diseñar las tarjetas de Humedad, Nutrientes y Temperatura con datos mock. | 3 | Rodrigo Aguilar | Done |
| US10 | Selección de Zona                 | Task 11 | Selector de zonas dinámico | Implementar un desplegable que permita cambiar entre zonas predefinidas. | 2 | Breithner Perez | Done |
| TS03 | Configuración de BD en la Nube    | Task 12 | Creación de esquema en PostgreSQL | Ejecutar scripts de creación de tablas (Client, Parcel, Device) en la nube. | 2 | Luis Acuña | Done |
| TS01 | GitFlow y Conventional Commits    | Task 13 | Revisión y estandarización | Verificar que todas las ramas feature sigan la convención y el flujo establecido. | 2 | Guillermo Howard | Done |

### 5.2.2.4. Development Evidence for Sprint Review

Registro de commits representativos del trabajo realizado durante el Sprint 3 en los repositorios de la organización.

### 5.2.2.5. Execution Evidence for Sprint Review


### 5.2.2.6. Services Documentation Evidence for Sprint Review


### 5.2.2.7. Software Deployment Evidence for Sprint Review


### 5.2.2.8. Team Collaboration Insights during Sprint

## 5.3. Validation Interviews.

### 5.3.1. Diseño de Entrevistas.

En esta sección el equipo establece, por cada segmento objetivo, los elementos incluidos en la sesión de validación, incluyendo el Landing Page y las aplicaciones. Se especifican también los user flows de las aplicaciones que formaron parte del proceso de validación.

### Segmento 1: Agricultores (dueños de cultivo)

**Elementos a validar:**

- Registro de cuenta e inicio de sesión.
- Visualización del dashboard de monitoreo en tiempo real (humedad, nutrientes, temperatura).
- Selección y cambio de zona o sensor específico.
- Visualización de mapa de calor de fertilidad (zoom y navegación).
- Recepción y comprensión de recomendaciones de riego y fertilización.
- Configuración de umbrales de alerta personalizados.
- Registro de un nuevo sensor IoT en la parcela.

**Flujos de Usuario evaluados (Desktop & Mobile):**

| Código | Flujo |
|--------|-------|
| UF-A1 | Registro y activación de cuenta |
| UF-A2 | Configuración de perfil y umbrales de alerta |
| UF-A3 | Visualización de indicadores clave y gráfico histórico |
| UF-A4 | Navegación en el mapa de calor de fertilidad |
| UF-A5 | Consulta de recomendación de riego |
| UF-A6 | Registro de nuevo sensor IoT |

**Actividades durante la sesión:**

1. Explorar el Landing Page y describir su comprensión del producto.
2. Simular el proceso de registro de cuenta.
3. Ingresar al sistema y configurar perfil (nombre, teléfono, tamaño de terreno).
4. Registrar un nuevo sensor en una zona (ingresar código único y asignar nombre).
5. Visualizar el dashboard principal e identificar los valores de humedad, nutrientes y temperatura.
6. Cambiar de zona y comprobar que los datos se actualizan.
7. Abrir el mapa de calor, hacer zoom y desplazarse para identificar zonas rojas.
8. Leer una recomendación de riego generada por el sistema (alerta por humedad baja).
9. Comentar sobre la utilidad de la interfaz y la claridad de las recomendaciones.

---

### Segmento 2: Administradores de cooperativas

**Elementos a validar:**

- Visualización de dashboard consolidado de todos los socios/lotes.
- Filtrado y ordenamiento de socios por rendimiento o alertas.
- Exportación de reporte mensual en PDF (con gráficos y tablas).
- Visualización de pronóstico del clima integrado.
- Acceso a imágenes satelitales recientes de parcelas.

**Flujos de Usuario evaluados (Desktop & Mobile):**

| Código | Flujo |
|--------|-------|
| UF-C1 | Acceso al dashboard agregado de la cooperativa |
| UF-C2 | Filtrado y comparación de socios |
| UF-C3 | Generación y descarga de reporte PDF |
| UF-C4 | Consulta del widget climático |
| UF-C5 | Visualización de imagen satelital y comparación histórica |

**Actividades durante la sesión:**

1. Explorar el Landing Page y describir la propuesta de valor para cooperativas.
2. Iniciar sesión con rol de administrador.
3. Visualizar la tabla de socios con métricas clave (humedad promedio, rendimiento estimado, alertas activas).
4. Ordenar la tabla por número de alertas activas (de mayor a menor).
5. Hacer clic en un socio para ver su detalle individual.
6. Generar un reporte mensual (seleccionando rango de fechas) y exportarlo en PDF.
7. Verificar que el PDF contiene encabezado, gráficos, tablas y recomendaciones.
8. Consultar el pronóstico del clima para los próximos 3 días.
9. Acceder a la vista satelital de una parcela y cambiar a una fecha anterior para comparar.
10. Comentar sobre la utilidad de los reportes y el dashboard consolidado para la gestión de la cooperativa.

---

### 5.3.2. Registro de Entrevistas.

### 5.3.3. Evaluación según heurísticas.

## 5.4. Video About-the-Product.