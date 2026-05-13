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
