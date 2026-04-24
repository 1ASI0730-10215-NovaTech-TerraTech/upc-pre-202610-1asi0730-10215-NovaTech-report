# Chapter III: Requirements Specification

<div style="page-break-before: always;"></div>

## 3.1. User Stories

<!-- ==================== EPIC01 ==================== -->
<h3>EPIC01: Landing Page & Marketing</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>USER ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US01</strong></td>
      <td>Visualización de Hero Section</td>
      <td>Como <strong>visitante</strong>, deseo <strong>ver un mensaje claro sobre el valor de AgroTech</strong> para <strong>comprender rápidamente qué ofrece la solución</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Carga correcta de la página<br>
        <em>Given</em> el visitante accede a la URL del Landing Page<br>
        <em>When</em> la página termina de cargar<br>
        <em>Then</em> se visualiza el Hero Section con título, subtítulo y botón CTA "Solicitar Demo"<br><br>
        <strong>Scenario 2:</strong> Responsive en móvil<br>
        <em>Given</em> el visitante accede desde un dispositivo móvil (320px width)<br>
        <em>When</em> la página se renderiza<br>
        <em>Then</em> el Hero Section se adapta verticalmente sin desbordamiento
      </td>
      <td>
        EPIC1
      </td>
    </tr>
    <tr>
      <td><strong>US02</strong></td>
      <td>Visualización de Sección de Características</td>
      <td>Como <strong>visitante</strong>, deseo <strong>conocer las características principales de AgroTech</strong> para <strong>evaluar si la solución satisface mis necesidades</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Visualización de 3 características<br>
        <em>Given</em> el visitante hace scroll hacia la sección de características<br>
        <em>When</em> la sección es visible<br>
        <em>Then</em> se muestran tres características: Sensor de Humedad, Sensor de Nutrientes, Alertas en Tiempo Real<br><br>
        <strong>Scenario 2:</strong> Cada característica tiene ícono y descripción<br>
        <em>Given</em> la sección de características está visible<br>
        <em>When</em> el visitante observa cada característica<br>
        <em>Then</em> cada una tiene un ícono representativo, un título y una breve descripción
      </td>
      <td>
        EPIC1
      </td>
    </tr>
    <tr>
      <td><strong>US03</strong></td>
      <td>Envío de Formulario de Solicitud de Demo</td>
      <td>Como <strong>visitante</strong>, deseo <strong>completar un formulario para solicitar una demostración</strong> para <strong>recibir información personalizada sobre AgroTech</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Envío exitoso<br>
        <em>Given</em> el visitante accede al formulario de demo<br>
        <em>When</em> completa los campos (Nombre, Email, Teléfono, Tamaño de terreno) y presiona "Enviar"<br>
        <em>Then</em> se muestra un mensaje de éxito "Gracias, nos contactaremos pronto" y se limpia el formulario<br><br>
        <strong>Scenario 2:</strong> Validación de campos obligatorios<br>
        <em>Given</em> el visitante está en el formulario<br>
        <em>When</em> intenta enviar sin completar el campo Email<br>
        <em>Then</em> se muestra un mensaje de error "El correo electrónico es requerido" y no se envía el formulario<br><br>
        <strong>Scenario 3:</strong> Validación de formato de email<br>
        <em>Given</em> el visitante ingresa "correo-invalido" en el campo Email<br>
        <em>When</em> presiona "Enviar"<br>
        <em>Then</em> se muestra un mensaje "Ingrese un correo electrónico válido"
      </td>
      <td>
        EPIC1
      </td>
    </tr>
    <tr>
      <td><strong>US04</strong></td>
      <td>Enlace a Términos y Condiciones</td>
      <td>Como <strong>visitante</strong>, deseo <strong>leer los términos y condiciones de servicio</strong> para <strong>conocer mis derechos y obligaciones al usar AgroTech</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Acceso desde footer<br>
        <em>Given</em> el visitante está en el Landing Page<br>
        <em>When</em> hace clic en el enlace "Términos y Condiciones" en el footer<br>
        <em>Then</em> se abre una nueva página o modal con el documento completo de términos<br><br>
        <strong>Scenario 2:</strong> Acceso desde Web Application<br>
        <em>Given</em> el usuario ha iniciado sesión en la Web App<br>
        <em>When</em> hace clic en "Términos" en el footer de la aplicación<br>
        <em>Then</em> se muestra el mismo documento
      </td>
      <td>
        EPIC1
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC02 ==================== -->
<h3>EPIC02: Autenticación y Gestión de Usuarios</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US05</strong></td>
      <td>Registro de Nuevo Usuario</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>crear una cuenta en AgroTech</strong> para <strong>acceder a la plataforma y configurar mis sembríos</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Registro exitoso<br>
        <em>Given</em> el usuario accede a la página de registro<br>
        <em>When</em> ingresa Nombre, Email, Contraseña y confirma contraseña, luego presiona "Registrarme"<br>
        <em>Then</em> se crea la cuenta, se envía un correo de verificación y se redirige al login<br><br>
        <strong>Scenario 2:</strong> Email ya registrado<br>
        <em>Given</em> el usuario ingresa un email que ya existe en la base de datos<br>
        <em>When</em> presiona "Registrarme"<br>
        <em>Then</em> se muestra el mensaje "Este correo ya está registrado. Inicia sesión o recupera tu contraseña"
      </td>
      <td>
        EPIC2
      </td>
    </tr>
    <tr>
      <td><strong>US06</strong></td>
      <td>Inicio de Sesión</td>
      <td>Como <strong>usuario registrado</strong>, deseo <strong>iniciar sesión con mi email y contraseña</strong> para <strong>acceder a mi dashboard y datos</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Login exitoso<br>
        <em>Given</em> el usuario está en la página de login<br>
        <em>When</em> ingresa email y contraseña válidos, luego presiona "Iniciar Sesión"<br>
        <em>Then</em> se redirige al dashboard principal de AgroTech<br><br>
        <strong>Scenario 2:</strong> Credenciales incorrectas<br>
        <em>Given</em> el usuario ingresa email o contraseña incorrectos<br>
        <em>When</em> presiona "Iniciar Sesión"<br>
        <em>Then</em> se muestra el mensaje "Credenciales inválidas. Intente nuevamente"
      </td>
      <td>
        EPIC2
      </td>
    </tr>
    <tr>
      <td><strong>US07</strong></td>
      <td>Recuperación de Contraseña</td>
      <td>Como <strong>usuario registrado</strong>, deseo <strong>recuperar mi contraseña olvidada</strong> para <strong>volver a acceder a mi cuenta</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Envío de enlace de recuperación<br>
        <em>Given</em> el usuario está en la página de login y hace clic en "Olvidé mi contraseña"<br>
        <em>When</em> ingresa su email registrado y presiona "Enviar enlace"<br>
        <em>Then</em> se envía un correo con un enlace único para restablecer la contraseña<br><br>
        <strong>Scenario 2:</strong> Restablecimiento exitoso<br>
        <em>Given</em> el usuario hace clic en el enlace del correo<br>
        <em>When</em> ingresa una nueva contraseña y la confirma<br>
        <em>Then</em> la contraseña se actualiza y se redirige al login
      </td>
      <td>
        EPIC2
      </td>
    </tr>
    <tr>
      <td><strong>US08</strong></td>
      <td>Visualización de Perfil de Usuario</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver y editar mi perfil</strong> para <strong>mantener actualizada mi información personal y de mi finca</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Visualización de perfil<br>
        <em>Given</em> el usuario ha iniciado sesión y navega a "Mi Perfil"<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestran los campos: Nombre, Email, Teléfono, Ubicación, Tamaño de terreno (hectáreas)<br><br>
        <strong>Scenario 2:</strong> Edición de perfil<br>
        <em>Given</em> el usuario está en su perfil<br>
        <em>When</em> modifica el campo Teléfono y presiona "Guardar Cambios"<br>
        <em>Then</em> se actualiza la información y se muestra mensaje de éxito
      </td>
      <td>
        EPIC2
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC03 ==================== -->
<h3>EPIC03: Dashboard de Monitoreo en Tiempo Real</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US09</strong></td>
      <td>Visualización de Indicadores Clave</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver en tiempo real los valores de humedad, nutrientes y temperatura del suelo</strong> para <strong>tomar decisiones informadas sobre riego y fertilización</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Carga del dashboard<br>
        <em>Given</em> el agricultor inicia sesión y accede al dashboard principal<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestran tres tarjetas con valores actuales: Humedad (%), Nutrientes (N-P-K ppm), Temperatura del suelo (°C)<br><br>
        <strong>Scenario 2:</strong> Actualización automática<br>
        <em>Given</em> el dashboard está visible<br>
        <em>When</em> pasan 5 minutos (o se recibe nuevo dato del sensor)<br>
        <em>Then</em> los valores se actualizan sin necesidad de recargar la página (WebSocket o polling)
      </td>
      <td>
        EPIC3
      </td>
    </tr>
    <tr>
      <td><strong>US10</strong></td>
      <td>Selección de Zona o Sensor Específico</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>seleccionar una zona específica de mi sembrío</strong> para <strong>ver los datos de sensores individuales</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Desplegable de zonas<br>
        <em>Given</em> el agricultor tiene configuradas 3 zonas (Norte, Centro, Sur)<br>
        <em>When</em> hace clic en el selector de zona<br>
        <em>Then</em> se muestran las 3 opciones disponibles<br><br>
        <strong>Scenario 2:</strong> Cambio de zona<br>
        <em>Given</em> el dashboard muestra datos de la zona Norte<br>
        <em>When</em> el agricultor selecciona "Sur" en el selector<br>
        <em>Then</em> los indicadores se actualizan con los datos de los sensores en la zona Sur
      </td>
      <td>
        EPIC3
      </td>
    </tr>
    <tr>
      <td><strong>US11</strong></td>
      <td>Visualización de Histórico de Datos (Gráfico)</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver un gráfico con el histórico de humedad de los últimos 7 días</strong> para <strong>identificar tendencias y patrones</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Carga de gráfico<br>
        <em>Given</em> el agricultor está en el dashboard<br>
        <em>When</em> hace clic en "Ver histórico" o desplaza hacia abajo<br>
        <em>Then</em> se muestra un gráfico de líneas con los valores de humedad de los últimos 7 días<br><br>
        <strong>Scenario 2:</strong> Cambio de rango de fechas<br>
        <em>Given</em> el gráfico histórico está visible<br>
        <em>When</em> el agricultor selecciona "30 días" en el selector de rango<br>
        <em>Then</em> el gráfico se actualiza mostrando los últimos 30 días
      </td>
      <td>
        EPIC3
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC04 ==================== -->
<h3>EPIC04: Mapa de Fertilidad</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US12</strong></td>
      <td>Visualización de Mapa de Calor de Fertilidad</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver un mapa de calor de mi sembrío que indique las zonas más fértiles</strong> para <strong>planificar la rotación de cultivos y optimizar la siembra</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Carga del mapa<br>
        <em>Given</em> el agricultor accede a la sección "Mapa de Fertilidad"<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestra un mapa interactivo con superposición de colores: verde (óptimo), amarillo (moderado), rojo (crítico)<br><br>
        <strong>Scenario 2:</strong> Leyenda explicativa<br>
        <em>Given</em> el mapa está visible<br>
        <em>When</em> el agricultor hace clic en el ícono de información<br>
        <em>Then</em> se muestra una leyenda que explica qué significa cada color y qué acciones recomienda
      </td>
      <td>
        EPIC4
      </td>
    </tr>
    <tr>
      <td><strong>US13</strong></td>
      <td>Zoom y Navegación en el Mapa</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>hacer zoom y desplazarme por el mapa</strong> para <strong>examinar zonas específicas con mayor detalle</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Zoom con mouse/touch<br>
        <em>Given</em> el mapa de fertilidad está visible<br>
        <em>When</em> el agricultor usa la rueda del mouse (o pellizco en móvil)<br>
        <em>Then</em> el mapa hace zoom in/out centrado en la posición del cursor<br><br>
        <strong>Scenario 2:</strong> Desplazamiento (pan)<br>
        <em>Given</em> el mapa está en zoom alto<br>
        <em>When</em> el agricultor arrastra el mapa con el mouse o dedo<br>
        <em>Then</em> la vista se desplaza para explorar otras áreas
      </td>
      <td>
        EPIC4
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC05 ==================== -->
<h3>EPIC05: Motor de Recomendaciones</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US14</strong></td>
      <td>Recepción de Recomendación de Riego</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>recibir una recomendación automática sobre si debo regar o no</strong> para <strong>optimizar el uso del agua y evitar estrés hídrico</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Recomendación "Regar"<br>
        <em>Given</em> el sensor de humedad muestra un valor &lt; 30%<br>
        <em>When</em> el agricultor accede al dashboard<br>
        <em>Then</em> se muestra una alerta con el mensaje "Recomendación: Regar zona [X] por 20 minutos"<br><br>
        <strong>Scenario 2:</strong> Recomendación "No regar"<br>
        <em>Given</em> el sensor de humedad muestra un valor &gt; 70%<br>
        <em>When</em> el agricultor accede al dashboard<br>
        <em>Then</em> se muestra el mensaje "Suelo con humedad adecuada. No es necesario regar"
      </td>
      <td>
        EPIC5
      </td>
    </tr>
    <tr>
      <td><strong>US15</strong></td>
      <td>Recepción de Recomendación de Fertilización</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>recibir una recomendación sobre qué nutriente aplicar y en qué cantidad</strong> para <strong>evitar sobrefertilización y reducir costos</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Recomendación de nitrógeno<br>
        <em>Given</em> el sensor de nutrientes muestra nivel bajo de Nitrógeno (&lt; 20 ppm)<br>
        <em>When</em> el agricultor accede al dashboard<br>
        <em>Then</em> se muestra "Recomendación: Aplicar 10 kg/ha de Nitrógeno en zona [X]"<br><br>
        <strong>Scenario 2:</strong> Todo en niveles adecuados<br>
        <em>Given</em> N, P, K están en rangos óptimos<br>
        <em>When</em> el agricultor consulta recomendaciones<br>
        <em>Then</em> se muestra "Los niveles de nutrientes son adecuados. Mantener plan actual."
      </td>
      <td>
        EPIC5
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC06 ==================== -->
<h3>EPIC06: Gestión de Sensores</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US16</strong></td>
      <td>Registro de Nuevo Sensor</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>registrar un nuevo sensor en mi cuenta</strong> para <strong>empezar a monitorear una nueva zona o sembrío</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Registro con código único<br>
        <em>Given</em> el agricultor está en la sección "Mis Sensores"<br>
        <em>When</em> hace clic en "Agregar Sensor" e ingresa el código único del dispositivo y una ubicación<br>
        <em>Then</em> el sensor aparece en la lista y comienza a enviar datos<br><br>
        <strong>Scenario 2:</strong> Validación de código inválido<br>
        <em>Given</em> el agricultor ingresa un código que no existe en el sistema<br>
        <em>When</em> presiona "Registrar"<br>
        <em>Then</em> se muestra error "Código de sensor inválido"
      </td>
      <td>
        EPIC6
      </td>
    </tr>
    <tr>
      <td><strong>US17</strong></td>
      <td>Configuración de Umbrales de Alerta</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>configurar umbrales personalizados para humedad y nutrientes</strong> para <strong>recibir alertas cuando los valores salgan del rango deseado</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Configuración de humedad<br>
        <em>Given</em> el agricultor está en "Configuración de Alertas"<br>
        <em>When</em> establece umbral mínimo de humedad en 25% y máximo en 80%<br>
        <em>Then</em> se guarda la configuración y se aplica a las alertas futuras<br><br>
        <strong>Scenario 2:</strong> Alerta por superación de umbral<br>
        <em>Given</em> el umbral máximo de humedad es 80%<br>
        <em>When</em> el sensor reporta 85%<br>
        <em>Then</em> el sistema genera una alerta "Humedad excesiva en zona [X]"
      </td>
      <td>
        EPIC6
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC07 ==================== -->
<h3>EPIC07: Reportes y Analytics</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US18</strong></td>
      <td>Exportación de Reporte en PDF</td>
      <td>Como <strong>administrador de cooperativa</strong>, deseo <strong>exportar un reporte mensual de rendimiento en formato PDF</strong> para <strong>compartirlo con los socios de la cooperativa</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Generación de PDF<br>
        <em>Given</em> el administrador está en la sección "Reportes"<br>
        <em>When</em> selecciona el mes "Mayo 2026" y hace clic en "Exportar PDF"<br>
        <em>Then</em> se descarga un archivo PDF con tablas y gráficos de rendimiento por zona<br><br>
        <strong>Scenario 2:</strong> Contenido del reporte<br>
        <em>Given</em> el PDF se genera correctamente<br>
        <em>When</em> el administrador lo abre<br>
        <em>Then</em> contiene: resumen de riego, consumo de agua, tendencias de nutrientes y recomendaciones
      </td>
      <td>
        EPIC7
      </td>
    </tr>
    <tr>
      <td><strong>US19</strong></td>
      <td>Dashboard Agregado por Socio/Lote</td>
      <td>Como <strong>administrador de cooperativa</strong>, deseo <strong>ver un dashboard consolidado de todos los socios o lotes</strong> para <strong>comparar el rendimiento y detectar oportunidades de mejora colectiva</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Vista de lista de socios<br>
        <em>Given</em> el administrador inicia sesión con rol "Admin Cooperativa"<br>
        <em>When</em> accede al dashboard principal<br>
        <em>Then</em> se muestra una tabla con todos los socios, hectáreas totales y promedio de rendimiento<br><br>
        <strong>Scenario 2:</strong> Detalle por socio<br>
        <em>Given</em> el administrador hace clic en el nombre de un socio<br>
        <em>When</em> se abre la vista detallada<br>
        <em>Then</em> se muestran los indicadores de ese socio específico (humedad, nutrientes, alertas)
      </td>
      <td>
        EPIC7
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC08 ==================== -->
<h3>EPIC08: API RESTful</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US20</strong></td>
      <td>Documentación de Endpoints con Swagger</td>
      <td>Como <strong>developer</strong>, deseo <strong>acceder a documentación interactiva de la API (Swagger/OpenAPI)</strong> para <strong>comprender cómo consumir los endpoints correctamente</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Acceso a Swagger UI<br>
        <em>Given</em> la API está desplegada en entorno de desarrollo<br>
        <em>When</em> el developer accede a `/swagger/index.html`<br>
        <em>Then</em> se muestra la interfaz de Swagger con todos los endpoints documentados<br><br>
        <strong>Scenario 2:</strong> Prueba de endpoint desde Swagger<br>
        <em>Given</em> Swagger UI está abierto<br>
        <em>When</em> el developer selecciona `GET /api/sensors/{id}` y hace clic en "Try it out"<br>
        <em>Then</em> se ejecuta la petición y se muestra la respuesta JSON
      </td>
      <td>
        EPIC8
      </td>
    </tr>
    <tr>
      <td><strong>US21</strong></td>
      <td>Endpoint de Obtención de Datos de Sensor</td>
      <td>Como <strong>frontend developer</strong>, deseo <strong>consumir un endpoint GET /api/sensors/{id}/data</strong> para <strong>obtener los últimos valores de un sensor específico</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Respuesta exitosa<br>
        <em>Given</em> existe un sensor con ID `sens-001`<br>
        <em>When</em> se realiza una petición `GET /api/sensors/sens-001/data`<br>
        <em>Then</em> la respuesta es HTTP 200 con JSON: `{ "sensorId": "sens-001", "humidity": 65.5, "nutrients": { "n": 30, "p": 15, "k": 45 }, "temperature": 22.3, "timestamp": "2026-04-06T10:00:00Z" }`<br><br>
        <strong>Scenario 2:</strong> Sensor no encontrado<br>
        <em>Given</em> no existe sensor con ID `sens-999`<br>
        <em>When</em> se realiza `GET /api/sensors/sens-999/data`<br>
        <em>Then</em> la respuesta es HTTP 404 con mensaje `{ "error": "Sensor not found" }`
      </td>
      <td>
        EPIC8
      </td>
    </tr>
    <tr>
      <td><strong>US22</strong></td>
      <td>Endpoint de Envío de Recomendación (Webhook)</td>
      <td>Como <strong>backend developer</strong>, deseo <strong>implementar un endpoint POST /api/recommendations/webhook</strong> para <strong>recibir datos del motor de recomendaciones y almacenarlos en la base de datos</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Recepción de recomendación válida<br>
        <em>Given</em> el motor externo envía un payload con `{ "zoneId": "Z01", "action": "water", "duration": 20, "priority": "high" }`<br>
        <em>When</em> se realiza `POST /api/recommendations/webhook`<br>
        <em>Then</em> se almacena la recomendación y se responde HTTP 201 Created<br><br>
        <strong>Scenario 2:</strong> Payload inválido<br>
        <em>Given</em> el payload no incluye `zoneId`<br>
        <em>When</em> se envía la petición<br>
        <em>Then</em> la respuesta es HTTP 400 Bad Request con detalle de error
      </td>
      <td>
        EPIC8
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC09 ==================== -->
<h3>EPIC09: Integración con Servicios Externos</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>US23</strong></td>
      <td>Integración con API de Clima</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver el pronóstico del clima junto a mis datos de suelo</strong> para <strong>coordinar el riego con las lluvias previstas</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Visualización de pronóstico<br>
        <em>Given</em> el agricultor está en el dashboard<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestra un widget con pronóstico de lluvia, temperatura y humedad ambiental para las próximas 24 horas<br><br>
        <strong>Scenario 2:</strong> Actualización automática<br>
        <em>Given</em> el widget climático está visible<br>
        <em>When</em> pasan 3 horas<br>
        <em>Then</em> los datos se actualizan automáticamente desde la API externa
      </td>
      <td>
        EPIC9
      </td>
    </tr>
    <tr>
      <td><strong>US24</strong></td>
      <td>Integración con Imágenes Satelitales</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver una imagen satelital reciente de mi sembrío</strong> para <strong>identificar visualmente áreas con problemas de crecimiento</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Carga de imagen satelital<br>
        <em>Given</em> el agricultor accede a la sección "Mapa Satelital"<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestra una imagen satelital de la última fecha disponible<br><br>
        <strong>Scenario 2:</strong> Selección de fecha<br>
        <em>Given</em> el mapa satelital está visible<br>
        <em>When</em> el agricultor selecciona una fecha diferente en el calendario<br>
        <em>Then</em> la imagen se actualiza con la imagen satelital de esa fecha
      </td>
      <td>
        EPIC9
      </td>
    </tr>
  </tbody>
</table>

<div style="page-break-before: always;"></div>

<!-- ==================== EPIC10 ==================== -->
<h3>EPIC10: Configuración y Despliegue (Technical Stories)</h3>
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>EPIC ID</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>TS01</strong></td>
      <td>Configuración de Repositorios con GitFlow</td>
      <td>Como <strong>developer</strong>, deseo <strong>tener los repositorios configurados con GitFlow y Conventional Commits</strong> para <strong>mantener un historial limpio y facilitar el trabajo colaborativo</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Estructura de branches<br>
        <em>Given</em> se accede al repositorio en GitHub<br>
        <em>When</em> se listan las branches<br>
        <em>Then</em> existen `main`, `develop`, y al menos una `feature/*` activa<br><br>
        <strong>Scenario 2:</strong> Conventional Commits<br>
        <em>Given</em> se revisa el historial de commits<br>
        <em>When</em> se observan los mensajes<br>
        <em>Then</em> siguen el formato `&lt;type&gt;(&lt;scope&gt;): &lt;subject&gt;`
      </td>
      <td>
        EPIC10
      </td>
    </tr>
    <tr>
      <td><strong>TS02</strong></td>
      <td>Despliegue Automático con Netlify / GitHub Actions</td>
      <td>Como <strong>developer</strong>, deseo <strong>tener configurado despliegue automático (CI/CD)</strong> para <strong>que los cambios en la rama main se publiquen automáticamente en producción</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Landing Page<br>
        <em>Given</em> se hace push a la rama `main` del repositorio<br>
        <em>When</em> Netlify detecta el cambio<br>
        <em>Then</em> ejecuta el despliegue y la URL pública se actualiza en &lt; 2 minutos<br><br>
        <strong>Scenario 2:</strong> Web Services<br>
        <em>Given</em> se hace push a `main` del repositorio `agrotech-api`<br>
        <em>When</em> GitHub Actions ejecuta el workflow<br>
        <em>Then</em> la API se despliega y los tests unitarios pasan
      </td>
      <td>
        EPIC10
      </td>
    </tr>
    <tr>
      <td><strong>TS03</strong></td>
      <td>Configuración de Base de Datos en la Nube</td>
      <td>Como <strong>developer</strong>, deseo <strong>tener una base de datos PostgreSQL alojada en la nube</strong> para <strong>persistir los datos de usuarios, sensores y recomendaciones</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Conexión exitosa<br>
        <em>Given</em> la aplicación está configurada con la cadena de conexión de la nube<br>
        <em>When</em> se ejecuta `dotnet run`<br>
        <em>Then</em> la API se conecta a la base de datos sin errores<br><br>
        <strong>Scenario 2:</strong> Migraciones aplicadas<br>
        <em>Given</em> existen migraciones pendientes<br>
        <em>When</em> se ejecuta `Update-Database`<br>
        <em>Then</em> las tablas se crean/actualizan correctamente
      </td>
      <td>
        EPIC10
      </td>
    </tr>
    <tr>
      <td><strong>TS04</strong></td>
      <td>Configuración de Variables de Entorno</strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>utilizar variables de entorno para configuraciones sensibles</strong> para <strong>evitar hardcodear credenciales en el repositorio</strong>.</td>
      <td>
        <strong>Scenario 1:</strong> Uso de `.env` para frontend<br>
        <em>Given</em> el frontend requiere una API key de mapas<br>
        <em>When</em> se revisa el repositorio<br>
        <em>Then</em> la API key no está hardcodeada, sino que se lee de `process.env.VITE_MAP_API_KEY`<br><br>
        <strong>Scenario 2:</strong> Uso de User Secrets / Azure Key Vault para backend<br>
        <em>Given</em> el backend requiere connection string<br>
        <em>When</em> se revisa `appsettings.json`<br>
        <em>Then</em> contiene `"ConnectionString": "${DB_CONNECTION}"` y el valor real está en variables de entorno
      </td>
      <td>
        EPIC10
      </td>
    </tr>
  </tbody>
</table>