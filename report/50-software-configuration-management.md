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

- Acceso Público: Se ha generado una URL pública (file:///C:/Users/acer/Desktop/LADING%20PAGE%20APP%20WEB/landing%20page/index.html) siguiendo el estándar de la plataforma, facilitando el acceso a potenciales clientes (agricultores y proveedores) y permitiendo la vinculación futura a un dominio personalizado

<img src="./report/assets/portada-landingpage.jpg" style="width: 90%; max-width: 1200px; height: 600px;">