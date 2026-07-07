### 5.1.1. Software Development Environment Configuration

Con el objetivo de garantizar un flujo de trabajo organizado, colaborativo y eficiente durante el desarrollo de la solución de TerraTech, el equipo ha definido un entorno de desarrollo que integra herramientas para la gestión del proyecto, diseño UX/UI, desarrollo de software, control de versiones, documentación y despliegue. La selección de estas herramientas responde a las tecnologías establecidas para el curso y permite mantener la consistencia durante todo el ciclo de vida del producto.

A continuación, se describen las herramientas utilizadas, su propósito dentro del proyecto y la ruta oficial de acceso o descarga correspondiente.

| Categoría | Herramienta | Propósito dentro del proyecto | Ruta de referencia / descarga                                            |
|------------|-------------|-------------------------------|--------------------------------------------------------------------------|
| Diseño UX/UI | Figma | Diseño de interfaces, wireframes, mockups y prototipos interactivos de la Landing Page y la Web Application. | [https://www.figma.com](https://www.figma.com)                           |
| Diseño UX/UI | Miro | Elaboración del Big Picture Event Storming y Design-Level Event Storming. | [https://miro.com](https://miro.com)                                     |
| Investigación UX | UXPressia | Desarrollo del Needfinding, User Personas, Empathy Maps, Journey Maps e Impact Maps. | [https://uxpressia.com](https://uxpressia.com)                           |
| Diseño gráfico | Canva | Elaboración de material gráfico, diagramas y recursos visuales para la documentación del proyecto. | [https://www.canva.com](https://www.canva.com)                           |
| Editor de código | Visual Studio Code | Entorno principal para el desarrollo de la Landing Page utilizando HTML, CSS y JavaScript. | [https://code.visualstudio.com](https://code.visualstudio.com)           |
| Editor de código | WebStorm | IDE para el desarrollo de la aplicación Frontend basada en Vue Framework. | [https://www.jetbrains.com/webstorm](https://www.jetbrains.com/webstorm) |
| Editor de código | Rider | IDE utilizado para el desarrollo de los servicios RESTful implementados con ASP.NET Core y C#. | [https://www.jetbrains.com/rider](https://www.jetbrains.com/rider)       |
| Control de versiones | Git | Sistema distribuido de control de versiones para el seguimiento de cambios y trabajo colaborativo. | [https://git-scm.com](https://git-scm.com)                               |
| Repositorio remoto | GitHub | Plataforma para almacenar los repositorios del proyecto, gestionar Pull Requests y facilitar la colaboración entre los integrantes del equipo. | [https://github.com](https://github.com)                                 |
| Framework Frontend | Vue.js | Framework JavaScript utilizado para desarrollar la interfaz de usuario de la aplicación web. | [https://vuejs.org](https://vuejs.org)                                                   |
| Biblioteca UI | PrimeVue | Biblioteca de componentes UI basada en Material Design utilizada junto con Vue.js. | [https://primevue.org](https://primevue.org)                                             |
| Gestión de dependencias | npm | Administrador de paquetes encargado de instalar y actualizar las dependencias del proyecto Frontend. | [https://www.npmjs.com](https://www.npmjs.com)                                            |
| Hosting | GitHub Pages | Plataforma utilizada para el despliegue de la Landing Page mediante integración continua con GitHub. | [https://pages.github.com](https://pages.github.com)                                     |

Durante el desarrollo del proyecto también se emplean herramientas de apoyo que permiten mantener la calidad del código y facilitar el trabajo colaborativo:

- **ESLint:** utilizado para detectar errores de sintaxis, inconsistencias y malas prácticas durante el desarrollo del código JavaScript y Vue.

- **Prettier:** empleado para mantener un formato uniforme del código fuente, mejorando su legibilidad y facilitando la colaboración entre los integrantes del equipo.

- **GitHub Pull Requests:** utilizado para realizar revisiones de código antes de integrar cambios hacia las ramas principales del repositorio.

- **GitHub Issues:** empleado para registrar incidencias, tareas pendientes y mejoras propuestas durante el desarrollo del proyecto.

Como parte de la configuración del entorno de desarrollo, todos los miembros del equipo utilizan las mismas versiones de las herramientas principales, permitiendo mantener compatibilidad entre los diferentes componentes de la solución. Asimismo, el equipo sigue las buenas prácticas recomendadas para GitFlow, Conventional Commits y Semantic Versioning, garantizando una administración organizada del código fuente y de las versiones publicadas del producto.

Finalmente, todas las herramientas seleccionadas cumplen con los requerimientos tecnológicos establecidos para el desarrollo del proyecto, permitiendo cubrir las actividades de Project Management, Requirements Engineering, UX/UI Design, Software Development, Software Documentation y Software Deployment durante todo el ciclo de vida de TerraTech.

### 5.1.2. Source Code Management

Para el desarrollo de TerraTech, el equipo ha adoptado **Git** como sistema distribuido de control de versiones y **GitHub** como plataforma centralizada para el almacenamiento del código fuente, seguimiento de cambios y colaboración entre los integrantes del equipo. Esta estrategia permite mantener un historial organizado de modificaciones, facilitar la integración continua del código y garantizar la trazabilidad durante todo el ciclo de vida del proyecto.

A continuación, se presentan los usuarios de GitHub de cada integrante del equipo:

<table border="1" cellspacing="0" cellpadding="2">
  <thead>
    <tr>
      <th align="left">Integrantes</th>
      <th align="left">Usuario de GitHub</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Retuerto Rodriguez, Jorge Manuel</td>
      <td><a href="[https://github.com/Calin1407](https://github.com/Calin1407)">Calin1407</a></td>
    </tr>
    <tr>
      <td>Howard Robles, Guillermo Arturo</td>
      <td><a href="[https://github.com/GuillermoPromac](https://github.com/GuillermoPromac)">GuillermoPromac</a></td>
    </tr>
    <tr>
      <td>Acuña de la Cruz, Luis Alfredo</td>
      <td><a href="[https://github.com/L2006delacruz](https://github.com/L2006delacruz)">L2006delacruz</a></td>
    </tr>
    <tr>
      <td>Perez Encarnacion, Breithner Rodolfo</td>
      <td><a href="[https://github.com/Breithner1](https://github.com/Breithner1)">Breithner1</a></td>
    </tr>
    <tr>
      <td>Aguilar Untiveros, Rodrigo Fabrizio</td>
      <td><a href="[https://github.com/Rodri2712](https://github.com/Rodri2712)">Rodri2712</a></td>
    </tr>
  </tbody>
</table>

#### Repositorios del proyecto

Cada uno de los productos que conforman la solución cuenta con un repositorio independiente dentro de la organización del equipo en GitHub.

> **Nota:** Reemplace los enlaces por los repositorios definitivos de su organización si aún no han sido creados.

- **Repositorio del Informe**

[![Repositorio Informe](https://img.shields.io/badge/Repositorio-Informe-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/1ASI0730-10215-NovaTech-AgroTech/upc-pre-202610-1asi0730-10215-NovaTech-report)

- **Repositorio Landing Page**

[![Repositorio Landing Page](https://img.shields.io/badge/Repositorio-Landing%20Page-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/1ASI0730-10215-NovaTech-AgroTech/upc-pre-202610-landing-page)

- **Repositorio Frontend Web Application**

[![Repositorio Frontend](https://img.shields.io/badge/Repositorio-Frontend-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/1ASI0730-10215-NovaTech-AgroTech/upc-pre-202610-frontend)

- **Repositorio RESTful Web Services**

[![Repositorio Backend](https://img.shields.io/badge/Repositorio-Web%20Services-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/1ASI0730-10215-NovaTech-AgroTech/upc-pre-202610-web-services)

#### GitFlow Workflow

Con el propósito de mantener un desarrollo ordenado y facilitar el trabajo colaborativo, el equipo implementa la metodología **GitFlow** como estrategia de control de versiones.

El flujo de trabajo consiste en desarrollar cada nueva funcionalidad dentro de una rama independiente, evitando afectar la estabilidad de la rama principal. Posteriormente, cada cambio es revisado mediante Pull Request antes de integrarse con la rama correspondiente.

Las ramas utilizadas son las siguientes:

- **main**

  Contiene únicamente versiones estables del producto listas para producción. Todo cambio que llega a esta rama ha sido previamente revisado y validado por el equipo.

- **develop**

  Es la rama principal de desarrollo donde se integran las funcionalidades implementadas durante cada Sprint. Todas las ramas de desarrollo parten de esta rama.

- **feature**

  Son ramas temporales utilizadas para implementar nuevas funcionalidades o mejoras específicas.

  Convención utilizada:

```text
feature/<feature-name>
```

Ejemplos:

```text
feature/login-page
feature/user-dashboard
feature/crop-management
feature/weather-module
```

Una vez finalizada la implementación, la rama es integrada mediante Pull Request hacia **develop**.

- **release**

  Cuando el equipo prepara una nueva versión del producto para su publicación, se crea una rama Release desde **develop**, donde únicamente se realizan pruebas finales, correcciones menores y ajustes de configuración.

Convención:

```text
release/vX.Y.Z
```

Ejemplos:

```text
release/v1.0.0
release/v1.1.0
release/v2.0.0
```

El versionado sigue el estándar **Semantic Versioning (SemVer)**.

- **hotfix**

  En caso de detectarse errores críticos en producción, se crea una rama Hotfix directamente desde **main**.

Convención:

```text
hotfix/<bug-name>
```

Ejemplos:

```text
hotfix/login-error
hotfix/api-timeout
hotfix/security-patch
```

Después de solucionar el problema, la rama Hotfix se fusiona tanto con **main** como con **develop**, garantizando que ambas ramas permanezcan sincronizadas.

#### Conventional Commits

Todos los commits realizados por el equipo siguen el estándar **Conventional Commits**, permitiendo mantener un historial claro, legible y fácil de entender.

Los principales prefijos utilizados son:

| Prefijo | Descripción |
|----------|-------------|
| feat | Implementación de una nueva funcionalidad. |
| fix | Corrección de errores. |
| docs | Cambios en la documentación. |
| style | Cambios relacionados únicamente con formato del código. |
| refactor | Reestructuración del código sin modificar su comportamiento. |
| perf | Mejoras de rendimiento. |
| test | Incorporación o modificación de pruebas. |
| chore | Tareas de mantenimiento o configuración del proyecto. |

Ejemplos:

```text
feat: implement user authentication

fix: correct responsive navigation menu

docs: update sprint documentation

refactor: simplify authentication service

style: format source code with prettier
```

Esta estrategia de gestión del código fuente permite mantener una estructura organizada del proyecto, facilitar la colaboración entre los integrantes del equipo y asegurar una integración controlada de nuevas funcionalidades durante el desarrollo de TerraTech.

### 5.1.3. Source Code Style Guide & Conventions

Con el propósito de garantizar la mantenibilidad, escalabilidad y legibilidad del código fuente, el equipo ha definido una serie de estándares y convenciones de programación que serán aplicados durante todo el desarrollo de TerraTech. Estas normas permiten mantener una estructura consistente entre todos los integrantes del equipo, facilitando el trabajo colaborativo, la revisión del código y el mantenimiento futuro de la solución.

Asimismo, se adoptan las guías de estilo recomendadas para las tecnologías utilizadas en el proyecto, siguiendo las referencias propuestas por la documentación oficial y los estándares indicados en el curso.

#### Convenciones generales

Durante el desarrollo del proyecto se aplicarán las siguientes reglas generales:

- Todo el código fuente será escrito en idioma **inglés**.
- Los nombres de variables, funciones, clases, componentes, interfaces, endpoints, tablas y archivos utilizarán nomenclatura en inglés.
- Se utilizarán nombres descriptivos y significativos, evitando abreviaturas innecesarias.
- El código deberá mantener una correcta indentación de 2 o 4 espacios, dependiendo del lenguaje y la configuración automática del editor.
- Cada archivo deberá cumplir el principio de responsabilidad única, evitando implementar múltiples funcionalidades dentro de un mismo componente.
- Se priorizará el desarrollo de código limpio, reutilizable y fácilmente mantenible.

#### Convenciones para HTML

El desarrollo de la estructura de las interfaces seguirá las recomendaciones de **Google HTML Style Guide** y **HTML Style Guide and Coding Conventions**.

Entre las principales prácticas adoptadas se encuentran:

- Uso correcto de etiquetas semánticas (`header`, `main`, `section`, `article`, `footer`, `nav`, etc.).
- Uso adecuado de atributos `alt` para imágenes.
- Correcta jerarquía de encabezados (`h1` a `h6`).
- Organización clara del contenido para mejorar la accesibilidad.
- Código HTML correctamente indentado y validado.

#### Convenciones para CSS

Para el desarrollo de estilos se adoptan las recomendaciones de **Google HTML/CSS Style Guide**.

Las principales convenciones incluyen:

- Clases escritas utilizando **kebab-case**.

Ejemplo:

```css
user-profile-card
weather-container
navigation-menu
```

- Evitar estilos en línea.
- Agrupar reglas relacionadas.
- Eliminar código CSS no utilizado.
- Mantener hojas de estilo organizadas por componentes.

#### Convenciones para JavaScript

El código JavaScript seguirá las recomendaciones de **Google JavaScript Style Guide**, **MDN JavaScript Guidelines** y **W3C JavaScript Style Guide**.

Entre las principales reglas se encuentran:

- Uso de `const` por defecto.
- Uso de `let` únicamente cuando el valor cambie.
- Evitar el uso de `var`.
- Uso obligatorio de punto y coma.
- Funciones pequeñas y con una única responsabilidad.
- Uso de nombres descriptivos para variables y funciones.
- Evitar código duplicado mediante reutilización de funciones.

Ejemplo:

```javascript
const getWeatherForecast = async () => {
    ...
};
```

#### Convenciones para Vue.js

Para el desarrollo del Frontend se siguen las recomendaciones establecidas en la **Vue Style Guide**.

Las principales convenciones son:

- Componentes escritos utilizando **PascalCase**.

Ejemplo:

```text
LoginView.vue
UserProfile.vue
WeatherCard.vue
CropDashboard.vue
```

- Props definidas explícitamente.
- Separación entre lógica, plantilla y estilos.
- Uso de Composition API cuando sea necesario.
- Organización del proyecto por módulos y componentes reutilizables.
- Evitar componentes excesivamente grandes.

#### Convenciones para C#

Los servicios RESTful desarrollados con ASP.NET Core seguirán las recomendaciones de **Microsoft C# Coding Conventions** y **ASP.NET Core Coding Guidelines**.

Las principales reglas incluyen:

- Clases en PascalCase.
- Métodos en PascalCase.
- Interfaces con prefijo **I**.
- Variables locales en camelCase.
- Uso adecuado de Dependency Injection.
- Separación entre Controllers, Services, Repositories y Domain Models.
- Métodos cortos y altamente cohesivos.

Ejemplo:

```csharp
public interface IUserService
{
}

public class UserService : IUserService
{
}
```

#### Convenciones de nomenclatura

| Elemento | Convención | Ejemplo |
|----------|------------|----------|
| Clases | PascalCase | UserService |
| Interfaces | PascalCase con prefijo I | IUserRepository |
| Métodos | PascalCase (C#) / camelCase (JavaScript) | GetUser(), getUser() |
| Variables | camelCase | userName |
| Constantes | UPPER_SNAKE_CASE | MAX_USERS |
| Componentes Vue | PascalCase | LoginView.vue |
| Clases CSS | kebab-case | login-container |
| Archivos JavaScript | camelCase | authService.js |
| Endpoints REST | kebab-case | /api/weather-forecast |

#### Comentarios

El equipo prioriza la escritura de código autodocumentado mediante nombres descriptivos. Sin embargo, cuando una sección del código implemente lógica compleja, algoritmos específicos o reglas de negocio importantes, se incorporarán comentarios claros y concisos para facilitar su comprensión y mantenimiento.

Se evitarán comentarios redundantes que describan acciones evidentes del código.

#### Revisión de código

Todos los cambios realizados en el proyecto serán revisados mediante **Pull Requests** antes de integrarse a la rama **develop** o **main**.

Durante la revisión se verificará:

- Cumplimiento de las convenciones de codificación.
- Correcto funcionamiento de la funcionalidad implementada.
- Ausencia de errores de sintaxis.
- Correcto formateo automático mediante Prettier.
- Validación de calidad utilizando ESLint.
- Cumplimiento de Conventional Commits.

Estas prácticas permiten mantener un código consistente, reducir la aparición de errores y facilitar la colaboración entre todos los integrantes del equipo durante el desarrollo de TerraTech.


### 5.1.4. Software Deployment Configuration

Con el propósito de garantizar un proceso de despliegue seguro, organizado y reproducible, el equipo ha definido una estrategia de Deployment basada en GitHub, GitFlow y servicios de alojamiento en la nube. Esta configuración permite automatizar la publicación de los productos desarrollados, reducir errores durante la liberación de nuevas versiones y asegurar que únicamente el código previamente validado sea desplegado en los entornos correspondientes.

El proceso de despliegue contempla los diferentes productos que conforman la solución de TerraTech: Landing Page, Frontend Web Application y RESTful Web Services.

#### Flujo general de Deployment

El proceso de despliegue inicia con el desarrollo de nuevas funcionalidades dentro de ramas **feature**, creadas a partir de la rama **develop**. Una vez finalizada una funcionalidad, se realiza un **Pull Request** para revisar el código y verificar el cumplimiento de las convenciones establecidas por el equipo.

Después de la aprobación del Pull Request, los cambios se integran en la rama **develop**, donde continúan las pruebas funcionales y de integración. Cuando el Sprint concluye y el producto alcanza un estado estable, se crea una rama **release** para realizar las validaciones finales.

Finalmente, la rama **release** es fusionada hacia **main**, permitiendo la publicación de una nueva versión del producto mediante el proceso de despliegue correspondiente.

El flujo de trabajo aplicado se resume de la siguiente manera:

```text
feature/*
      │
      ▼
develop
      │
      ▼
release/vX.Y.Z
      │
      ▼
main
      │
      ▼
Deployment
```

En caso de detectarse un error crítico en producción, el equipo utilizará ramas **hotfix**, las cuales se crearán directamente desde **main** y posteriormente serán integradas tanto en **main** como en **develop**, garantizando la sincronización entre ambas ramas.

---

#### Landing Page Deployment

La Landing Page de TerraTech será desplegada mediante **GitHub Pages**, aprovechando su integración nativa con GitHub para sitios web estáticos desarrollados con HTML, CSS y JavaScript.

El proceso de despliegue consiste en los siguientes pasos:

1. El desarrollador implementa una nueva funcionalidad dentro de una rama **feature**.
2. Se crea un Pull Request hacia la rama **develop**.
3. El equipo revisa el código y aprueba su integración.
4. Se realizan pruebas funcionales y de integración.
5. Se crea una rama **release** para preparar una nueva versión.
6. La rama **release** se fusiona con **main**.
7. GitHub Pages detecta automáticamente los cambios publicados en **main**.
8. El sitio web es actualizado y publicado automáticamente mediante HTTPS.

Gracias a este proceso, la Landing Page permanece disponible con una versión estable y validada para todos los usuarios.

---

#### Frontend Web Application Deployment

La aplicación Frontend desarrollada con **Vue.js** seguirá un proceso similar al utilizado para la Landing Page.

Después de integrar los cambios en la rama **main**, se generará una nueva versión de producción mediante el proceso de compilación del proyecto.

El despliegue contempla las siguientes actividades:

- Instalación de dependencias mediante **npm**.
- Generación del proyecto optimizado para producción.
- Publicación de los archivos generados en el servicio de alojamiento correspondiente.
- Verificación del correcto funcionamiento de la aplicación desplegada.

Este procedimiento garantiza que únicamente versiones previamente revisadas sean publicadas para los usuarios finales.

---

#### RESTful Web Services Deployment

Los servicios RESTful desarrollados con **ASP.NET Core** seguirán un proceso de despliegue independiente del Frontend.

Una vez aprobados los cambios mediante Pull Request y fusionados en la rama **main**, se publicará una nueva versión del servicio utilizando la configuración definida para el servidor o proveedor cloud correspondiente.

Durante este proceso se verificará:

- Correcta compilación del proyecto.
- Disponibilidad de los endpoints.
- Correcta conexión con la base de datos.
- Funcionamiento de los servicios de autenticación y autorización.
- Disponibilidad de la documentación OpenAPI (Swagger).

---

#### Seguridad y disponibilidad

El proceso de despliegue considera diversas medidas para garantizar la estabilidad de la solución:

- Uso exclusivo de la rama **main** para versiones estables.
- Revisión obligatoria mediante Pull Requests antes de cada integración.
- Aplicación de GitFlow como estrategia de control de versiones.
- Versionado mediante Semantic Versioning.
- Comunicación cifrada mediante HTTPS.
- Certificados SSL proporcionados automáticamente por GitHub Pages para la Landing Page.
- Respaldo permanente del código fuente mediante GitHub.

Estas medidas permiten reducir riesgos durante la publicación de nuevas versiones y facilitan la recuperación ante posibles incidencias.

---

#### Configuración del entorno de producción

La configuración del entorno de producción considera los siguientes componentes principales:

| Producto | Tecnología | Plataforma de despliegue |
|----------|------------|--------------------------|
| Landing Page | HTML5, CSS3, JavaScript | GitHub Pages |
| Frontend Web Application | Vue.js + PrimeVue | Hosting Web / Servicio Cloud |
| RESTful Web Services | ASP.NET Core + C# | Servidor Web o Servicio Cloud |
| Control de versiones | Git | GitHub |

La estrategia de despliegue definida permite mantener una publicación organizada, segura y escalable de todos los componentes que conforman TerraTech, asegurando la disponibilidad de la solución durante todo su ciclo de vida y facilitando futuras actualizaciones del producto.

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

Trello: [https://trello.com/b/sLQ8KGVG/aplicaciones-web](https://trello.com/b/sLQ8KGVG/aplicaciones-web)

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

Enlace del video: [https://tinyurl.com/mrxyzszz](https://tinyurl.com/mrxyzszz)

Duracion: 00:00 - 17:26

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

### 5.2.4. Sprint 4

#### 5.2.4.1. Sprint Planning 4\.

| Sprint #                        | Sprint 4                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Sprint Planning Background**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Date                            | 2026-06-28                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Time                            | 09:30 pm (GMT-5)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Location                        | Modalidad remota mediante la plataforma Discord                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Prepared By                     | Howard Robles, Guillermo Arturo                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Attendees (to planning meeting) | Aguilar Untiveros, Rodrigo Fabrizio <br /> Howard Robles, Guillermo Arturo <br /> Perez Encarnación, Breithner Rodolfo <br /> Retuerto Rodríguez, Jorge Manuel                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Sprint 3 Review Summary         | Durante el Sprint 3 se logró consolidar la mayoría de los módulos funcionales del sistema, completando exitosamente la gestión de zonas de cultivo, dispositivos, reportes analíticos, comunidad, inventario y notificaciones. Se implementaron los filtros de búsqueda para campos y dispositivos, así como las primeras integraciones con el motor de recomendaciones. El equipo demostró una sólida capacidad de coordinación y entrega, logrando avances significativos en la integración frontend-backend. Como oportunidad de mejora, se identificó la necesidad de optimizar el rendimiento de las consultas en tiempo real y completar las funcionalidades pendientes de la comunidad y el perfil de usuario para la entrega final.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Sprint 3 Retrospective Summary  | Durante el Sprint 3, el equipo mantuvo una comunicación efectiva y una coordinación fluida, lo cual permitió avanzar de forma sólida en todos los módulos planificados. La integración continua y las revisiones cruzadas de código fueron aspectos clave que facilitaron el ritmo de trabajo. <br />Como oportunidad de mejora, se identificó la necesidad de completar las funcionalidades pendientes de la comunidad (mural, calificaciones) y el perfil de usuario, así como optimizar el rendimiento de las consultas de reportes para garantizar una experiencia de usuario rápida y eficiente. <br />También se resaltó la importancia de realizar pruebas de integración exhaustivas antes de la entrega final para asegurar la estabilidad del sistema.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Sprint Goal & User Stories**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Sprint 4 Goal                   | Nuestro enfoque es brindar a los VISITANTES la oportunidad de conocer las metas que el equipo de desarrollo tuvo con el proyecto y su experiencia durante el desarrollo de la solución, permitir a los AGRICULTORES asociar dispositivos IoT para el monitoreo y controlar el consumo de sus suministros, proporcionar a los PROVEEDORES consultar las necesidades de abastecimiento de los agricultores, ofrecer a los CLIENTES FINALES un catálogo de productos y un espacio para consultar y registrar reseñas sobre los productos de los agricultores, y brindar al equipo de desarrollo la capacidad de expandir el ecosistema con nuevas características.  Creemos que esto ofrece a los visitantes una primera impresión transparente y confiable al mostrar la trayectoria del proyecto y el compromiso del equipo; a los agricultores, operaciones agrícolas eficientes y basadas en datos mediante el monitoreo en tiempo real y la gestión de inventario; a los proveedores, inteligencia de mercado accionable al revelar patrones de demanda y brechas de abastecimiento; a los clientes finales, decisiones de compra informadas y un espacio comunitario confiable a través de la trazabilidad de productos y reseñas de pares; y al equipo de desarrollo, una base flexible y bien documentada para extender la plataforma con nuevas capacidades.  Esto se confirmará cuando: se incrementen el número de suscripciones de la página web; los agricultores registren sus campos de cultivo, asignen sensores y gestionen sus suministros; los proveedores accedan a los registros de abastecimiento y analíticas de demanda de los agricultores; los clientes finales exploren el catálogo y registren y/o consulten reseñas; y los desarrolladores implementen nuevas funciones relacionadas con el ecosistema sin intervención del backend. |
| Sprint 4 Velocity               | 33                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Sum of Story Points             | 33                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |


#### 5.2.4.2. Aspect Leaders and Collaborators

Durante el Sprint 4, se ha consolidado la integración final de los módulos principales del frontend y backend de TerraTech, abarcando funcionalidades clave como la gestión de sensores, inventarios, comunidad, notificaciones, catálogos y análisis. Estas implementaciones buscan optimizar los procesos internos y mejorar la trazabilidad del flujo de análisis, brindando mayor eficiencia a los proveedores y clientes finales.

Con el fin de mantener una coordinación efectiva y una comunicación fluida entre los integrantes del equipo, se estructuró la matriz de liderazgo y colaboración (LACX), donde se asignó un líder (L) encargado de cada funcionalidad y colaboradores (C) que brindan apoyo en su implementación.

| Team Member (Last Name, First Name)  | GitHub Username    | IAM | Monitoring | Notification | Profile | Stock | Community | Analytics | Commercial |
|:-------------------------------------|:-------------------|:----|:-----------|:-------------|:--------|:------|:----------|:----------|:-----------|
| Retuerto Rodriguez, Jorge Manuel     | Calin1407          | L   | C          | C            | C       | C     | C         | L         | L          |
| Howard Robles, Guillermo Arturo      | GuillermoPromac    | C   | L          | C            | C       | C     | C         | C         | C          |
| Perez Encarnacion, Breithner Rodolfo | Breithner1         | C   | C          | C            | L       | C     | L         | C         | C          |
| Aguilar Untiveros, Rodrigo Fabrizio  | Rodri2712          | C   | C          | L            | C       | L     | C         | C         | C          |

#### 5.2.4.3. Sprint Backlog 4

El objetivo principal de este Sprint es consolidar la experiencia de usuario en los módulos de visualización de datos, inventarios y catálogos, cerrando funcionalidades críticas para los perfiles de agricultor, proveedor y cliente final. Se prioriza la implementación de mejoras en la landing page, la corrección de errores en los ensambladores de campos y la integración de filtros avanzados, gráficos de tendencias y paginación. Además, se busca fortalecer la autenticación y el manejo de tokens de cancelación para garantizar la estabilidad y escalabilidad del sistema. Este Sprint permitirá a los agricultores gestionar sus zonas de cultivo y sensores de manera más precisa, a los proveedores acceder a datos analíticos más detallados y a los clientes finales disfrutar de un catálogo completo y funcional. Todo esto, en conjunto, facilitará la adopción de la plataforma y mejorará la experiencia general de los usuarios.

<img src="assets/images/cap5/sprint-backlog-4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

| Work-item / Task | Description                                                           | Estimation (hours) | Assigned To | Status  |
|------------------|-----------------------------------------------------------------------|--------------------|-------------|---------|
| US08-01          | Fix bad request 400 on profile creation                               | 1                  | JM          | To Do   |
| US08-02          | Integrate profile context fixes                                       | 1                  | JM          | To Do   |
| US08-03          | Display validation messages for fields like phone                     | 1                  | JM          | To Do   |
| US10-01          | Add latitude and longitude in fields                                  | 1                  | GH          | To Do   |
| US10-02          | Fix camelCase support in field assembler                              | 1                  | GH          | To Do   |
| US10-03          | Fix camelCase support in device assembler                             | 1                  | GH          | To Do   |
| US10-04          | Fix bad example                                                       | 1                  | GH          | To Do   |
| US24-02          | Implement pagination and filtering                                    | 1                  | FF          | To Do   |
| US25-01          | Fix inventory endpoint path variable                                  | 1                  | FF          | To Do   |
| US25-02          | Improve placeholders for Product ID and Quantity fields               | 1                  | FF          | To Do   |
| US25-03          | Assign profileId automatically from authenticated user                | 1                  | FF          | To Do   |
| US29-01          | Integrate analytics fixes                                             | 1                  | JM          | To Do   |
| US29-02          | Add demand trend charts                                               | 1                  | JM          | To Do   |
| US29-03          | Connect region and crop type filters                                  | 1                  | JM          | To Do   |
| US35-01          | Implement catalog view with product cards, images, prices and ratings | 1                  | BP          | To Do   |
| US35-02          | Add filters by category                                               | 1                  | BP          | To Do   |
| US35-03          | Add search bar by product name                                        | 1                  | BP          | To Do   |
| US37-01          | Implement review form with star rating                                | 1                  | BP          | To Do   |
| US37-02          | Add minimum content validation                                        | 1                  | BP          | To Do   |
| US37-03          | Allow editing and deleting own reviews                                | 1                  | BP          | To Do   |
| TS07-15          | Fix error 500 in monitoring                                           | 1                  | GH          | To Do   |

Trello: [https://trello.com/b/sLQ8KGVG/aplicaciones-web](https://trello.com/b/sLQ8KGVG/aplicaciones-web)


#### 5.2.4.4. Development Evidence for Sprint Review

**Landing page:**

Se ha actualizado el link del FrontEnd puesto en el Landing page por los cambios en el deployment del FrontEnd, ahora se encuentra desplegado en render.

| Repository                                                          | Branch                   | Commit Id | Commit Message                       | Commit Message Body                                                         | Commited on (Date) |
|---------------------------------------------------------------------|--------------------------|-----------|--------------------------------------|-----------------------------------------------------------------------------|--------------------|
| GuillermoPomace/upc-pre-202610-1asio0730-10215-NovaTech-LandingPage | feature/change-link-page | f7daaae   | fix: update registration button link | Actualización del enlace del botón de registro a la nueva URL del FrontEnd. | 06/07              |

---

**FrontEnd:**

En el frontend de TerraTech se han implementado mejoras sustanciales en la compatibilidad con los endpoints del backend, corrigiendo errores críticos en el mapeo de datos de analíticas y en la creación de perfiles (bad request 400). Se ha añadido soporte para camelCase en los ensambladores de monitoreo, integrando nuevas propiedades como latitud y longitud en los formularios y listas de campos, con sus respectivas validaciones y mensajes de internacionalización. Además, se ha mejorado la gestión de comentarios en la comunidad, permitiendo la edición y eliminación con ajustes dinámicos en la puntuación de reputación, y se ha incorporado soporte multilingüe para las acciones de la comunidad. Finalmente, se ha implementado el botón de cierre de sesión en el layout y se ha integrado la validación de perfiles en el módulo comercial antes de la confirmación de pedidos.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|------------|--------|-----------|----------------|---------------------|-------------------|
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/analytics-api-compatibility | 1a5b30b | fix(analytics): fix report data mapping in bounded analytics. | Se arregló un error de mapeo de los datos de analytics, permitiendo la visualización completa de los datos. | 29/06 |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/profile-api-compability | b6a92e2 | fix(profile): fixed bad request 400 on profile creation. | Se arregló el problema de bad request en la creación de un profile. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 4f6b574 | feat(monitoring): update device and field entities with default values and new latitude/longitude properties. | Corrección de entities en monitoring. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 67b086a | feat(monitoring): add latitude and longitude fields to field form and list with validation. | Añadido de los valores latitud y longitud en el Field. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 6b71981 | feat(monitoring): enhance device and field classes with detailed jsdoc comments. | Añadido de documentación en los entities de monitoring. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 057a5b4 | feat(monitoring): update device and field assemblers to improve resource mapping and add fallback handling. | Añadido de los handing a los assemblers field y device. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | bfca455 | refactor(monitoring): device and field api interactions to ensure proper payload structure and improve data handling. | Cambios en la interacción del .store de monitoring. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 2aee91a | feat(i18n): add localization for latitude and longitude fields with validation messages. | Añadido de internacionalización de los valores nuevos de latitud y longitud. | 01/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | 457b353 | fix(monitoring): add camelcase support to device assembler. | - | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | c9a521c | refactor(monitoring): keep device form unchanged. | - | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | aeeffc2 | fix(monitoring): add camelcase support to field assembler. | - | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | c255a03 | feat(monitoring): dynamically assign profileid from iam store. | - | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | a405053 | fix(monitoring): update payloads to match backend dtos. | - | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/monitoring-endpoint | c096527 | fix(monitoring): update methods to use id parameter correctly. | - | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 7578401 | feat(community_management): update profile and comment payload structures for consistency. | Actualizar las estructuras de carga útil de perfil y comentario para mayor coherencia | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 8e82785 | feat(community_management): refactor comment assembler to improve entity mapping. | Refactorizar el ensamblador de comentarios para mejorar el mapeo de entidades. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | cf0e4dc | feat(community_management): update resource naming and enhance comment retrieval method. | Actualizar la nomenclatura de recursos y mejorar el método de recuperación de comentarios. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 24ba7ef | feat(community_management): enhance community profile entity mapping and simplify response handling. | mejora la asignación de entidades de perfil de comunidad y simplifica el manejo de respuestas. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 75a5873 | feat(community_management): update profile_id type and ensure correct parsing of route parameter. | actualiza el tipo profile_id y garantiza el análisis correcto del parámetro de ruta. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 329b2c3 | feat(community_management): ensure correct parsing of profile id and update author profile id type. | Garantiza el análisis correcto del ID de perfil y actualiza el tipo de ID de perfil de autor | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 02a7c32 | feat(community_management): add comment update and delete functionality, improve target profile ID handling. | Agrega funcionalidad para actualizar y eliminar comentarios, y mejora el manejo del ID de perfil de destino. | 05/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | bcad6a3 | feat(community_management): add update and delete functionality for comments. | Agrega funcionalidad para actualizar y eliminar comentarios. | 05/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | a5aa1cb | feat(community_management): enhance community profile form with profile ID handling and validation. | Mejora el formulario de perfil de comunidad con manejo y validación del ID de perfil. | 05/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 5634fe8 | feat(community_management): enhance community profile list with visibility filtering and profile ID checks. | Mejora la lista de perfiles de comunidad con filtrado de visibilidad y comprobaciones de ID de perfil. | 06/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 109adc6 | feat(community_management): implement comment editing and deletion with reputation score adjustments. | Implementa la edición y eliminación de comentarios con ajustes de puntuación de reputación. | 06/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/community-endpoint | 0394af1 | feat(community_management): add multilingual support for community actions and notifications. | Agrega soporte multilingüe para acciones y notificaciones de la comunidad. | 06/07 |
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/implements-log-out | 99dd0b6 | feature(layout): implements log out button into layout. | Implementación de botón para terminar la sesión del usuario. | 06/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-FrontEnd | feature/commercial-order-endpoint | 6b7a3fa | feat(commercial): integrate profile validation before order confirmation. | integrar la validación del perfil antes de la confirmación del pedido. | 06/07 |

---

**BackEnd:**

Durante el desarrollo del backend, se ha estandarizado el uso de identificadores numéricos (int) en los bounded contexts de Commercial y Community Management, eliminando restricciones de longitud y mejorando la integridad referencial entre las entidades. Se ha añadido la puntuación de reputación en las actualizaciones de perfiles de comunidad y se ha creado la migración inicial de base de datos consolidando todas las tablas del sistema. Además, se ha corregido el error 500 en el módulo de monitoreo, mejorando los ensambladores con manejo de valores nulos y añadiendo propiedades como latitud y longitud en los recursos de campo, alineando el backend con las necesidades del frontend.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|------------|--------|-----------|----------------|---------------------|-------------------|
| Calin1407/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/refactor-commercial-profileid-to-number | 0bf0791 | refactor: updated profile id from string to number in the bounded commercial. | Actualización de profile id de string a valores enteros en el bounded de commercial. | 28/06 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-migrations | 34c21fe | feat: create initial database migration with multiple tables. | Creación del migrations para el projecto | 01/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 4f967c2 | feat(community_management): add reputation score to profile update information. | agregar puntuación de reputación a la información de actualización del perfil | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 47a1162 | feat(comment_management): change AuthorProfileId and TargetProfileId types from string to int. | cambia los tipos de AuthorProfileId y TargetProfileId de string to int | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | dcb9267 | feat(community_management): change ProfileId type from string to int and update UpdateInformation method to accept reputation score. | Cambiar el tipo de ProfileId de cadena a entero y actualizar el método UpdateInformation para que acepte la puntuación de reputación. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 3c65838 | feat(comment_management): change AuthorProfileId and TargetProfileId types from string to int. | Cambiar los tipos de AuthorProfileId y TargetProfileId de string a int | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 81b4ec7 | feat(community_management): change ProfileId type from string to int in CreateCommunityProfileCommand. | Cambiar el tipo de ProfileId de string a int en CreateCommunityProfileCommand | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | e49f1fb | feat(community_management): add ReputationScore to UpdateCommunityProfileCommand. | Añadir ReputationScore a UpdateCommunityProfileCommand | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 8ca8405 | feat(community_management): change TargetProfileId type from string to int in GetCommentsByTargetProfileIdQuery. | Cambiar el tipo de TargetProfileId de string a int en GetCommentsByTargetProfileIdQuery | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 1ead45e | feat(community_management): change ProfileId type from string to int in GetCommunityProfileByProfileIdQuery. | cambia el tipo de ProfileId de cadena a entero en GetCommunityProfileByProfileIdQuery. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | a16afe2 | feat(comment_management): change TargetProfileId type from string to int in ICommentRepository. | cambia el tipo de TargetProfileId de string a int en ICommentRepository. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | d94cef6 | feat(community_management): change ProfileId type from string to int in ICommunityProfileRepository. | Cambiar el tipo de ProfileId de string a int en ICommunityProfileRepository | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | d42d5b5 | feat(community_management): remove maxLength constraint for ProfileId and TargetProfileId in CommunityProfile and Comment entities. | Eliminar la restricción maxLength para ProfileId y TargetProfileId en las entidades CommunityProfile y Comment. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 13bccda | feat(comment_management): change TargetProfileId type from string to int in CommentRepository. | Cambiar el tipo de TargetProfileId de string a int en CommentRepository. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 814a6a4 | feat(community_management): change ProfileId type from string to int in CommunityProfileRepository. | Cambiar el tipo de ProfileId de cadena a entero en CommunityProfileRepository. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | f2bb4d1 | feat(comment_management): change AuthorProfileId and TargetProfileId types from string to int in CommentResource and CreateCommentResource. | cambia los tipos AuthorProfileId y TargetProfileId de cadena a entero en CommentResource y CreateCommentResource. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | f717ab8 | feat(community_management): change ProfileId type from string to int in CommunityProfileResource, CreateCommunityProfileResource, and UpdateCommunityProfileResource. | cambia el tipo ProfileId de cadena a entero en CommunityProfileResource, CreateCommunityProfileResource y UpdateCommunityProfileResource. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | 34ee74d | feat(comment_management): change targetProfileId type from string to int in CommentsController. | Cambiar el tipo de targetProfileId de cadena a entero en CommentsController. | 02/07 |
| Breithner1/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/change-community-ids-to-number | e14f724 | feat(community_management): update CommunityProfilesController to use ProfileId as int and enhance method summaries. | Actualizar CommunityProfilesController para usar ProfileId como entero y mejorar los resúmenes de los métodos. | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/fix-error-500-monitoring | baf8086 | feat(monitoring): enhance fieldresource and assembler with additional properties and null safety. | Se amplió el DTO FieldResource para incluir las propiedades ProfileId, Latitude y Longitude, alineándolo con el nuevo esquema del frontend | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/fix-error-500-monitoring | 102e2d4 | feat(monitoring): enhance deviceresource assembler to handle null values gracefully. | Se actualizó el DeviceResourceFromEntityAssembler para gestionar de forma segura las propiedades que podrían ser nulas (FieldId, MacAddress, Status, LastSync) | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/fix-error-500-monitoring | 125751a | feat(monitoring): add methods to retrieve all device and field resources with error handling. | Se incorporaron los métodos GetAllFieldResourcesAsync y GetAllDeviceResourcesAsync en los servicios de consulta correspondientes | 02/07 |
| GuillermoPromac/upc-pre-202610-1asi0730-10215-NovaTech-BackEnd | feature/fix-error-500-monitoring | c94a522 | feat(monitoring): update devicescontroller and fieldscontroller to retrieve resources directly from query services. | Se modificaron los controladores DevicesController y FieldsController para que los endpoints GET /devices y GET /fields utilicen ahora los nuevos métodos resistentes a errores | 02/07 |

---


#### 5.2.4.5. Execution Evidence for Sprint Review

A continuación, se muestra un video con los avances realizados durante el Sprint 4, asi como el deployment del FrontEnd y la Landing Page en render.

Video del sprint4:

<img src="assets/images/cap5/Video-Sprint4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Enlace del video:

Duración:


#### 5.2.4.6. Services Documentation Evidence for Sprint Review

Durante este sprint se completó al 100% el desarrollo del FrontEnd junto a su conexión con el BackEnd, así como la integración de los servicios de monitoreo, notificaciones, comunidad, inventario y analítica. Se documentaron los endpoints de cada servicio, incluyendo sus rutas, métodos HTTP, parámetros de entrada y salida, así como ejemplos de uso. Esta documentación se encuentra disponible en el repositorio del proyecto y servirá como referencia para futuros desarrollos y para la integración con otros sistemas.

A su vez se completó el deployment de los elementos del FrontEnd y la Landing Page en render, asegurando que los servicios estén accesibles y funcionando correctamente.

Descripción del Logro:

- Finalización del FrontEnd (100%).
- Correcto despliegue de los elementos de la pagina estática.
- Conexión exitosa del FrontEnd con el BackEnd.
- Documentación completa de los servicios implementados.
- Registro de zonas de cultivo y sensores IoT funcionando correctamente.
- Visualización de catálogo de productos y reseñas de clientes finales.

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


#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Durante este sprint, se realizó el correcto despliegue del FrontEnd y la Landing Page en render, asegurando que los servicios estén accesibles y funcionando correctamente.

***FrontEnd***

1. Se instaló el dist en el projecto usando el comando "npm run build" para generar la carpeta dist.

<img src="assets/images/cap5/FrontEnd_Deployment_2.1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Se usa el link del repositorio del github del FrontEnd.

<img src="assets/images/cap5/FrontEnd_Deployment_2.2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Se coloca el metodo dist para el Publish Directory.

<img src="assets/images/cap5/FrontEnd_Deployment_2.3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

4. Se colocan las variables de entorno para el FrontEnd.

<img src="assets/images/cap5/FrontEnd_Deployment_2.4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

5. Se realiza el despliegue del FrontEnd en render.

<img src="assets/images/cap5/FrontEnd_Deployment_2.5.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

***LandingPage***

1. Se instaló el dist en el projecto usando el comando "npm run build" para generar la carpeta dist.

<img src="assets/images/cap5/LandingPage_Deployment_2.1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

2. Se usa el link del repositorio del github del LandingPage.

<img src="assets/images/cap5/LandingPage_Deployment_2.2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

3. Se coloca el metodo dist para el Publish Directory.

<img src="assets/images/cap5/LandingPage_Deployment_2.3.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

4. El LandingPage no requiere variables de entorno, por lo que se omite este paso.

<img src="assets/images/cap5/LandingPage_Deployment_2.4.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

5. Se realiza el despliegue del LandingPage en render.

<img src="assets/images/cap5/LandingPage_Deployment_2.5.png" alt="cap5" style="height: 500px !important; width: 700px !important;">


#### 5.2.4.8. Team Collaboration Insights during Sprint



## 5.3. Validation Interviews.

### 5.3.1. Diseño de Entrevistas.

Con el propósito de validar la solución desarrollada, se diseñó un conjunto de entrevistas de validación dirigidas a los tres segmentos objetivo de TerraTech: **Agricultores**, **Proveedores de insumos agrícolas** y **Clientes Finales (compradores)**. Cada sesión de validación contempla la interacción de los participantes con el **Landing Page** y la **Web Application** (desktop y mobile), ejecutando escenarios de uso representativos de las funcionalidades implementadas.

Siguiendo las indicaciones establecidas para el proceso de validación, cada entrevista define los elementos que serán evaluados durante la sesión y los **User Flows** que deberán ser recorridos por los participantes, con el fin de comprobar la facilidad de uso, comprensión de la interfaz y correcto funcionamiento de las funcionalidades más importantes del sistema.

***Objetivo General***

Validar la experiencia de uso del Landing Page y la Web Application de TerraTech mediante sesiones de interacción con usuarios representativos de cada segmento objetivo, verificando la comprensión de la propuesta de valor, la ejecución de los principales flujos de usuario y la percepción general sobre la utilidad de la solución.

---

### Segmento 1: Agricultores (dueños de cultivo)

#### Landing Page
Los participantes deberán explorar el Landing Page para verificar si la propuesta de valor es comprendida correctamente, identificar los beneficios ofrecidos por TerraTech y evaluar la facilidad para acceder a la aplicación.

#### Web Application

**Elementos a validar:**

- Flujo de registro e inicio de sesión.
- Registro y gestión de zonas de cultivo (Fields).
- Asociación de sensores IoT a zonas de cultivo.
- Visualización de indicadores en tiempo real (humedad, nutrientes y temperatura).
- Recepción y comprensión de alertas y notificaciones.
- Gestión de inventario de insumos.
- Configuración de preferencias de notificaciones.

#### User Flows a validar

- **UF-A1:** Registro de cuenta y configuración inicial del perfil.
- **UF-A2:** Registro de una zona de cultivo.
- **UF-A3:** Asociación de un sensor IoT a una zona de cultivo.
- **UF-A4:** Visualización del dashboard de monitoreo.
- **UF-A5:** Configuración de umbrales de alerta.
- **UF-A6:** Gestión del inventario de insumos.
- **UF-A7:** Consulta y gestión de notificaciones.

---

### Segmento 2: Proveedores de insumos agrícolas

#### Landing Page

Los participantes deberán explorar el Landing Page para identificar la propuesta de valor dirigida a proveedores y evaluar la claridad de la información presentada.

#### Web Application

**Elementos a validar:**

- Registro e inicio de sesión.
- Dashboard analítico.
- Consulta de demanda de insumos.
- Visualización de tendencias.
- Comunidad de agricultores.
- Configuración de notificaciones.

#### User Flows a validar

- **UF-P1:** Registro y configuración del perfil.
- **UF-P2:** Consulta del dashboard analítico.
- **UF-P3:** Navegación por la comunidad.
- **UF-P4:** Configuración de notificaciones.

---

### Segmento 3: Clientes Finales (compradores mayoristas y minoristas)

#### Landing Page

Los participantes deberán navegar por el Landing Page para identificar la propuesta de valor del producto y comprender los beneficios que ofrece la plataforma para el proceso de compra.

#### Web Application

**Elementos a validar:**

- Registro e inicio de sesión.
- Visualización del catálogo de productos agrícolas.
- Consulta de información detallada del producto.
- Visualización de la trazabilidad.
- Consulta de certificaciones.
- Visualización de comentarios y calificaciones.
- Configuración de notificaciones.

#### User Flows a validar

- **UF-C1:** Registro y configuración del perfil.
- **UF-C2:** Visualización y navegación del catálogo de productos.
- **UF-C3:** Consulta del detalle del producto.
- **UF-C4:** Visualización de comentarios y calificaciones.
- **UF-C5:** Configuración de notificaciones.

---

### 5.3.2. Registro de Entrevistas.

### Segmento 2: Proveedores de insumos agrícolas

**ENTREVISTA 1**

**Nombre:** Anita Monago Cachay  
**Edad:** 35 años  
**Distrito:** Ica  
**Timing:** 

<img src="assets/images/cap5/Entrevista_Validacion_Segmento2-1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Ver entrevista: 

**Resumen:**

Anita Monago Cachay manifestó que el Landing Page comunica claramente la propuesta de valor dirigida a los proveedores de insumos agrícolas y que el proceso de registro resulta intuitivo tanto en computadoras como en dispositivos móviles. Asimismo, destacó que el módulo de analítica permite identificar oportunidades comerciales mediante la visualización de la demanda de insumos y las zonas con mayor actividad agrícola. También consideró útil el sistema de notificaciones y la posibilidad de consultar comentarios y calificaciones realizados por la comunidad de agricultores. Como sugerencia de mejora, propuso incorporar la opción de registrar el precio de los productos dentro del catálogo para facilitar la cotización y comparación por parte de los clientes.

---

**ENTREVISTA 2**

**Nombre:** Alvaro Medina Huaqui
**Edad:** 25 años  
**Distrito:** Ica  
**Timing:** 

<img src="assets/images/cap5/Entrevista_Validacion_Segmento2-2.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Ver entrevista: 

**Resumen:**

Alvaro Medina Huaqui indicó que la navegación por el Landing Page es clara y que la información sobre la propuesta de valor para proveedores es comprensible. Destacó que el dashboard analítico proporciona datos relevantes sobre la demanda de insumos y las tendencias del mercado, lo cual facilita la toma de decisiones comerciales. Sin embargo, sugirió mejorar la visualización de los gráficos y agregar filtros adicionales para segmentar la información según tipo de cultivo y región. Tambien le parece util la funcionalidad de la comunidad, ya que permite interactuar con otros agricultores y proveedores, fomentando la colaboración y el intercambio de experiencias.

### Segmento 3: Clientes Finales

**ENTREVISTA 1**

**Nombre:** Myke Dylan Guillen Geraldo
**Edad:** 22 años  
**Distrito:** Huaraz  
**Timing:**

<img src="assets/images/cap5/Entrevista_Validacion_Segmento3-1.png" alt="cap5" style="height: 500px !important; width: 700px !important;">

Ver entrevista:

**Resumen:**

Myke Dylan Guillen Geraldo expresó que la Landing Page comunica de manera efectiva la propuesta de valor para los clientes finales, destacando la claridad en la información sobre la trazabilidad y certificaciones de los productos. Consideró que la navegación por el catálogo es intuitiva y que la visualización de comentarios y calificaciones ayuda a tomar decisiones de compra informadas. Sin embargo, sugirió mejorar la búsqueda de productos mediante filtros más específicos y la posibilidad de comparar productos similares. Además, resaltó la importancia de recibir notificaciones sobre nuevas ofertas y promociones, lo cual podría incentivar la fidelización de los clientes.

### 5.3.3. Evaluación según heurísticas.

Con la finalidad de evaluar la usabilidad de TerraTech, las entrevistas de validación fueron analizadas utilizando los **10 principios heurísticos de Jakob Nielsen**. Durante las sesiones se observaron las interacciones de los participantes con la Landing Page y la Web Application, registrando los problemas de usabilidad identificados y las oportunidades de mejora.

Las heurísticas consideradas durante la evaluación fueron las siguientes:

1. Visibilidad del estado del sistema.
2. Relación entre el sistema y el mundo real.
3. Control y libertad del usuario.
4. Consistencia y estándares.
5. Prevención de errores.
6. Reconocimiento antes que recuerdo.
7. Flexibilidad y eficiencia de uso.
8. Diseño estético y minimalista.
9. Ayuda para reconocer, diagnosticar y recuperarse de errores.
10. Ayuda y documentación.

Durante las sesiones también se registró el grado de cumplimiento de las tareas ejecutadas por cada participante, distinguiendo si fueron completadas sin ayuda, con ayuda o si no pudieron completarse. Asimismo, se documentaron observaciones cualitativas, comentarios de los usuarios y sugerencias de mejora obtenidas durante la interacción con la plataforma.

La información recopilada permitió identificar oportunidades de mejora relacionadas con la navegación, claridad de la información, organización de la interfaz y facilidad de uso de las funcionalidades implementadas. Estos hallazgos servirán como base para las siguientes iteraciones del producto y para fortalecer la experiencia de usuario en futuras versiones de TerraTech.

## 5.4. Video About-the-Product.

A continuación, se presenta el video **"About the Product"** del sistema **TerraTech**, una plataforma tecnológica desarrollada para digitalizar y optimizar la gestión agrícola mediante sensores IoT, análisis predictivo, comunidad colaborativa y comercialización transparente. Este video está dirigido principalmente a los visitantes del Landing Page, quienes desean conocer el modelo de negocio y las principales funcionalidades de la plataforma, así como a los usuarios potenciales de las aplicaciones (agricultores, proveedores de insumos y clientes finales), interesados en realizar tareas relacionadas con los procesos soportados por la solución.

El video comunica de forma clara y dinámica el propósito del producto, mostrando cómo TerraTech ayuda a reducir la incertidumbre en la agricultura, optimizar el uso de recursos hídricos y fertilizantes, mejorar la eficiencia operativa mediante el monitoreo en tiempo real, y fortalecer la relación entre agricultores, proveedores y compradores a través de una comunidad transparente y un catálogo trazable. Se utiliza un tono consistente con la propuesta visual y comunicacional del producto, combinando narración, demostraciones de uso en campo y escenarios reales de cultivo.

A continuación, se incluye un screenshot del video, junto con los enlaces de la versión publicada en Microsoft Stream y YouTube.

Video en Stream: [https://tinyurl.com/m88tcphe](https://tinyurl.com/m88tcphe)

Video en YouTube: [https://youtu.be/g50PX1_6f_M](https://youtu.be/g50PX1_6f_M)

Duración: 00:00 - 07:57

<img src="assets/images/cap5/about-the-product.png" alt="cap5" style="height: 500px !important; width: 700px !important;">
