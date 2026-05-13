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
        <strong>Scenario 1: Carga correcta de la página</strong><br>
        <em>Given</em> el visitante accede a la URL del Landing Page<br>
        <em>When</em> la página termina de cargar<br>
        <em>Then</em> se visualiza el Hero Section con título, subtítulo y botón CTA "Solicitar Demo"<br>
        <em>And</em> el botón "Solicitar Demo" es clicable y visible sin necesidad de scroll<br><br>
        <strong>Scenario 2: Responsive en móvil</strong><br>
        <em>Given</em> el visitante accede desde un dispositivo móvil con ancho de 320px<br>
        <em>When</em> la página se renderiza<br>
        <em>Then</em> el Hero Section se adapta verticalmente sin desbordamiento horizontal<br>
        <em>And</em> el tamaño de la fuente del título es mínimo de 1.5rem
      </td>
      <td>EPIC1</td>
    </tr>
    <tr>
      <td><strong>US02</strong></td>
      <td>Visualización de Sección de Características</td>
      <td>Como <strong>visitante</strong>, deseo <strong>conocer las características principales de AgroTech</strong> para <strong>evaluar si la solución satisface mis necesidades</strong>.</td>
      <td>
        <strong>Scenario 1: Visualización de 3 características</strong><br>
        <em>Given</em> el visitante ha cargado el Landing Page<br>
        <em>When</em> hace scroll hasta la sección de características<br>
        <em>Then</em> se muestran exactamente tres características: "Sensor de Humedad", "Sensor de Nutrientes", "Alertas en Tiempo Real"<br><br>
        <strong>Scenario 2: Cada característica tiene ícono y descripción</strong><br>
        <em>Given</em> la sección de características está visible<br>
        <em>When</em> el visitante observa cada característica<br>
        <em>Then</em> cada una tiene un ícono representativo (formato SVG o FontAwesome), un título H3 y una descripción de máximo 150 caracteres
      </td>
      <td>EPIC1</td>
    </tr>
    <tr>
      <td><strong>US03</strong></td>
      <td>Envío de Formulario de Solicitud de Demo</td>
      <td>Como <strong>visitante</strong>, deseo <strong>completar un formulario para solicitar una demostración</strong> para <strong>recibir información personalizada sobre AgroTech</strong>.</td>
      <td>
        <strong>Scenario 1: Envío exitoso</strong><br>
        <em>Given</em> el visitante accede al formulario de demo en el Landing Page<br>
        <em>When</em> completa todos los campos (Nombre, Email, Teléfono, Tamaño de terreno en hectáreas) y presiona "Enviar"<br>
        <em>Then</em> se muestra un mensaje de éxito "Gracias, nos contactaremos pronto"<br>
        <em>And</em> el formulario se limpia automáticamente<br><br>
        <strong>Scenario 2: Validación de campos obligatorios</strong><br>
        <em>Given</em> el visitante está en el formulario<br>
        <em>When</em> intenta enviar sin completar el campo Email<br>
        <em>Then</em> se muestra un mensaje de error "El correo electrónico es requerido"<br>
        <em>And</em> el formulario no se envía al servidor<br><br>
        <strong>Scenario 3: Validación de formato de email</strong><br>
        <em>Given</em> el visitante ingresa "correo-invalido" en el campo Email<br>
        <em>When</em> presiona "Enviar"<br>
        <em>Then</em> se muestra un mensaje en rojo "Ingrese un correo electrónico válido (ej: usuario@dominio.com)"<br>
        <em>And</em> el campo Email tiene borde rojo
      </td>
      <td>EPIC1</td>
    </tr>
    <tr>
      <td><strong>US04</strong></td>
      <td>Enlace a Términos y Condiciones</td>
      <td>Como <strong>visitante</strong>, deseo <strong>leer los términos y condiciones de servicio</strong> para <strong>conocer mis derechos y obligaciones al usar AgroTech</strong>.</td>
      <td>
        <strong>Scenario 1: Acceso desde footer del Landing Page</strong><br>
        <em>Given</em> el visitante está en el Landing Page<br>
        <em>When</em> hace clic en el enlace "Términos y Condiciones" en el footer<br>
        <em>Then</em> se abre una nueva pestaña con el documento completo de términos<br>
        <em>And</em> el documento tiene fecha de última actualización visible<br><br>
        <strong>Scenario 2: Acceso desde Web Application (logueado)</strong><br>
        <em>Given</em> el usuario ha iniciado sesión en la Web App<br>
        <em>When</em> hace clic en "Términos y Condiciones" en el footer de la aplicación<br>
        <em>Then</em> se abre un modal con el mismo documento<br>
        <em>And</em> el modal tiene botón "Aceptar" y botón "Cerrar"
      </td>
      <td>EPIC1</td>
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
        <strong>Scenario 1: Registro exitoso</strong><br>
        <em>Given</em> el usuario accede a la página /register<br>
        <em>When</em> ingresa Nombre (mínimo 2 caracteres), Email válido, Contraseña (mínimo 6 caracteres) y confirma contraseña correctamente<br>
        <em>And</em> presiona "Registrarme"<br>
        <em>Then</em> se crea la cuenta con rol "Agricultor"<br>
        <em>And</em> se envía un correo de verificación con enlace válido por 24 horas<br>
        <em>And</em> se redirige automáticamente a /login<br><br>
        <strong>Scenario 2: Email ya registrado</strong><br>
        <em>Given</em> el usuario ingresa un email que ya existe en la base de datos<br>
        <em>When</em> presiona "Registrarme"<br>
        <em>Then</em> se muestra el mensaje "Este correo ya está registrado. Inicia sesión o recupera tu contraseña"<br>
        <em>And</em> se habilita un enlace a /forgot-password<br><br>
        <strong>Scenario 3: Contraseñas no coinciden</strong><br>
        <em>Given</em> el usuario ingresa "123456" en Contraseña y "12345" en Confirmar Contraseña<br>
        <em>When</em> presiona "Registrarme"<br>
        <em>Then</em> se muestra el mensaje "Las contraseñas no coinciden"<br>
        <em>And</em> el campo Confirmar Contraseña se marca con borde rojo
      </td>
      <td>EPIC2</td>
    </tr>
    <tr>
      <td><strong>US06</strong></td>
      <td>Inicio de Sesión</td>
      <td>Como <strong>usuario registrado</strong>, deseo <strong>iniciar sesión con mi email y contraseña</strong> para <strong>acceder a mi dashboard y datos</strong>.</td>
      <td>
        <strong>Scenario 1: Login exitoso</strong><br>
        <em>Given</em> el usuario está en la página /login<br>
        <em>When</em> ingresa email y contraseña válidos (registrados previamente y verificados)<br>
        <em>And</em> presiona "Iniciar Sesión"<br>
        <em>Then</em> se genera un token JWT válido por 8 horas<br>
        <em>And</em> se redirige al dashboard principal /dashboard<br>
        <em>And</em> el nombre del usuario aparece en el header de la aplicación<br><br>
        <strong>Scenario 2: Credenciales incorrectas</strong><br>
        <em>Given</em> el usuario ingresa email "campo@example.com" (existente) y contraseña "wrong123"<br>
        <em>When</em> presiona "Iniciar Sesión"<br>
        <em>Then</em> se muestra el mensaje "Credenciales inválidas. Intente nuevamente"<br>
        <em>And</em> no se genera token<br>
        <em>And</em> el usuario permanece en /login<br><br>
        <strong>Scenario 3: Email no verificado</strong><br>
        <em>Given</em> el usuario se registró pero no verificó su email<br>
        <em>When</em> intenta iniciar sesión con credenciales correctas<br>
        <em>Then</em> se muestra "Por favor, verifica tu correo electrónico antes de iniciar sesión"<br>
        <em>And</em> se ofrece opción de "Reenviar correo de verificación"
      </td>
      <td>EPIC2</td>
    </tr>
    <tr>
      <td><strong>US07</strong></td>
      <td>Recuperación de Contraseña</td>
      <td>Como <strong>usuario registrado</strong>, deseo <strong>recuperar mi contraseña olvidada</strong> para <strong>volver a acceder a mi cuenta</strong>.</td>
      <td>
        <strong>Scenario 1: Envío de enlace de recuperación</strong><br>
        <em>Given</em> el usuario está en la página /login y hace clic en "¿Olvidaste tu contraseña?"<br>
        <em>When</em> ingresa su email registrado "campo@example.com" y presiona "Enviar enlace"<br>
        <em>Then</em> se envía un correo con un enlace único (token) válido por 1 hora<br>
        <em>And</em> se muestra mensaje "Revisa tu correo para restablecer tu contraseña"<br><br>
        <strong>Scenario 2: Restablecimiento exitoso</strong><br>
        <em>Given</em> el usuario hace clic en el enlace del correo y accede a /reset-password?token=valid_token<br>
        <em>When</em> ingresa nueva contraseña "newPass123" y la confirma correctamente<br>
        <em>And</em> presiona "Restablecer Contraseña"<br>
        <em>Then</em> la contraseña se actualiza en la base de datos (hasheada con bcrypt)<br>
        <em>And</em> se redirige a /login con mensaje "Contraseña actualizada. Inicia sesión"<br><br>
        <strong>Scenario 3: Token expirado o inválido</strong><br>
        <em>Given</em> el usuario hace clic en un enlace de recuperación con token inválido o expirado<br>
        <em>When</em> intenta restablecer su contraseña<br>
        <em>Then</em> se muestra "El enlace ha expirado o es inválido. Solicita uno nuevo"<br>
        <em>And</em> se habilita un botón "Solicitar nuevo enlace"
       </td>
      <td>EPIC2</td>
    </tr>
    <tr>
      <td><strong>US08</strong></td>
      <td>Visualización de Perfil de Usuario</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver y editar mi perfil</strong> para <strong>mantener actualizada mi información personal y de mi finca</strong>.</td>
      <td>
        <strong>Scenario 1: Visualización de perfil</strong><br>
        <em>Given</em> el usuario ha iniciado sesión y navega a "Mi Perfil"<br>
        <em>When</em> la página carga<br>
        <em>Then</em> se muestran los campos precargados: Nombre, Email (no editable), Teléfono, Ubicación (ciudad/departamento), Tamaño de terreno (hectáreas)<br>
        <em>And</em> se muestra la fecha de registro de la cuenta<br><br>
        <strong>Scenario 2: Edición exitosa del perfil</strong><br>
        <em>Given</em> el usuario está en su perfil<br>
        <em>When</em> modifica el campo Teléfono de "999888777" a "999111222" y presiona "Guardar Cambios"<br>
        <em>Then</em> se muestra mensaje verde "Perfil actualizado correctamente"<br>
        <em>And</em> la base de datos refleja el nuevo número de teléfono<br><br>
        <strong>Scenario 3: Validación de campos</strong><br>
        <em>Given</em> el usuario ingresa un tamaño de terreno negativo "-5" en hectáreas<br>
        <em>When</em> presiona "Guardar Cambios"<br>
        <em>Then</em> se muestra error "El tamaño del terreno debe ser mayor a 0"<br>
        <em>And</em> no se actualiza el perfil
       </td>
      <td>EPIC2</td>
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
        <strong>Scenario 1: Carga inicial del dashboard</strong><br>
        <em>Given</em> el agricultor inicia sesión con rol "Agricultor" y tiene al menos un sensor asociado<br>
        <em>When</em> accede a /dashboard<br>
        <em>Then</em> se muestran tres tarjetas con valores actuales: Humedad (%, con barra de progreso), Nutrientes (N-P-K en ppm), Temperatura del suelo (°C)<br>
        <em>And</em> cada tarjeta muestra la última fecha y hora de actualización (formato DD/MM/YYYY HH:MM:SS)<br><br>
        <strong>Scenario 2: Actualización automática por WebSocket</strong><br>
        <em>Given</em> el dashboard está visible y hay conexión WebSocket activa<br>
        <em>When</em> el backend recibe un nuevo dato del sensor (cada 5 minutos)<br>
        <em>Then</em> los valores en las tarjetas se actualizan sin recargar la página<br>
        <em>And</em> se muestra una animación de "actualizado" durante 1 segundo en la tarjeta modificada<br><br>
        <strong>Scenario 3: Pérdida de conexión con el sensor</strong><br>
        <em>Given</em> un sensor no envía datos durante más de 30 minutos<br>
        <em>When</em> el dashboard intenta actualizar<br>
        <em>Then</em> se muestra un ícono de advertencia amarillo ⚠️ y el mensaje "Datos desactualizados - Sensor sin conexión"
       </td>
      <td>EPIC3</td>
    </tr>
    <tr>
      <td><strong>US10</strong></td>
      <td>Selección de Zona o Sensor Específico</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>seleccionar una zona específica de mi sembrío</strong> para <strong>ver los datos de sensores individuales</strong>.</td>
      <td>
        <strong>Scenario 1: Desplegable de zonas</strong><br>
        <em>Given</em> el agricultor tiene configuradas 3 zonas con nombres "Norte", "Centro", "Sur"<br>
        <em>When</em> hace clic en el selector de zona (combobox) en la parte superior del dashboard<br>
        <em>Then</em> se despliegan las 3 opciones disponibles<br>
        <em>And</em> se muestra la zona activa actualmente ("Norte" por defecto)<br><br>
        <strong>Scenario 2: Cambio de zona actualiza todos los indicadores</strong><br>
        <em>Given</em> el dashboard muestra datos de la zona Norte (humedad 45%)<br>
        <em>When</em> el agricultor selecciona "Sur" en el selector<br>
        <em>Then</em> los indicadores (humedad, nutrientes, temperatura) se actualizan con los datos de los sensores en la zona Sur<br>
        <em>And</em> el gráfico histórico también se actualiza para mostrar datos de la zona Sur<br>
        <em>And</em> se registra en un log interno el cambio de zona
       </td>
      <td>EPIC3</td>
    </tr>
    <tr>
      <td><strong>US11</strong></td>
      <td>Visualización de Histórico de Datos (Gráfico)</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver un gráfico con el histórico de humedad de los últimos 7 días</strong> para <strong>identificar tendencias y patrones</strong>.</td>
      <td>
        <strong>Scenario 1: Carga del gráfico por defecto (7 días)</strong><br>
        <em>Given</em> el agricultor está en el dashboard y hace clic en la pestaña "Histórico"<br>
        <em>When</em> la pestaña se activa<br>
        <em>Then</em> se muestra un gráfico de líneas o área con los valores de humedad de los últimos 7 días<br>
        <em>And</em> el eje X muestra fechas (formato "DD/MM") y el eje Y muestra porcentaje de humedad (0-100%)<br>
        <em>And</em> se dibuja una línea horizontal punteada en el umbral mínimo configurado (ej: 30%)<br><br>
        <strong>Scenario 2: Cambio de rango de fechas a 30 días</strong><br>
        <em>Given</em> el gráfico histórico está visible con rango "7 días"<br>
        <em>When</em> el agricultor selecciona "30 días" en el selector de rango de fechas<br>
        <em>Then</em> el gráfico se actualiza mostrando los últimos 30 días de datos<br>
        <em>And</em> la carga de datos toma menos de 2 segundos (con paginación o lazy loading)<br><br>
        <strong>Scenario 3: Tooltip al pasar el mouse</strong><br>
        <em>Given</em> el gráfico histórico está visible<br>
        <em>When</em> el agricultor pasa el mouse sobre un punto del gráfico<br>
        <em>Then</em> se muestra un tooltip con: fecha exacta, valor de humedad, y si ese día hubo alerta (ícono rojo si aplica)
       </td>
      <td>EPIC3</td>
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
        <strong>Scenario 1: Carga del mapa interactivo</strong><br>
        <em>Given</em> el agricultor accede a la sección "Mapa de Fertilidad" desde el menú principal<br>
        <em>When</em> la página carga y existe al menos una zona con datos de sensores<br>
        <em>Then</em> se muestra un mapa interactivo (basado en Leaflet o Google Maps) con superposición de colores:<br>
        - Verde (#2ecc71) para niveles óptimos (humedad >60% y nutrientes óptimos)<br>
        - Amarillo (#f1c40f) para niveles moderados (humedad 30-60% o nutrientes medios)<br>
        - Rojo (#e74c3c) para niveles críticos (humedad <30% o nutrientes bajos)<br>
        <em>And</em> cada zona del mapa es clicable<br><br>
        <strong>Scenario 2: Leyenda explicativa y acciones sugeridas</strong><br>
        <em>Given</em> el mapa de calor está visible<br>
        <em>When</em> el agricultor hace clic en el ícono de información (i) en la esquina superior derecha del mapa<br>
        <em>Then</em> se muestra un modal con leyenda de colores y para cada color una acción sugerida:<br>
        - "Verde: Mantener plan actual"<br>
        - "Amarillo: Monitorear cada 12 horas"<br>
        - "Rojo: Regar/fertilizar en las próximas 2 horas"<br>
        <em>And</em> el modal tiene botón "Entendido" para cerrar
       </td>
      <td>EPIC4</td>
    </tr>
    <tr>
      <td><strong>US13</strong></td>
      <td>Zoom y Navegación en el Mapa</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>hacer zoom y desplazarme por el mapa</strong> para <strong>examinar zonas específicas con mayor detalle</strong>.</td>
      <td>
        <strong>Scenario 1: Zoom con mouse y controles táctiles</strong><br>
        <em>Given</em> el mapa de fertilidad está visible en el navegador<br>
        <em>When</em> el agricultor usa la rueda del mouse hacia arriba (o pellizca hacia afuera en móvil)<br>
        <em>Then</em> el mapa hace zoom in, centrado en la posición del cursor/punto de contacto<br>
        <em>And</em> se muestran las calles o parcelas con mayor nivel de detalle (nombres de zonas visibles)<br><br>
        <strong>Scenario 2: Desplazamiento (pan) del mapa</strong><br>
        <em>Given</em> el mapa está con zoom nivel 15 (alta resolución)<br>
        <em>When</em> el agricultor arrastra el mapa con el mouse (click sostenido + mover) o con el dedo en móvil<br>
        <em>Then</em> la vista se desplaza suavemente para explorar otras áreas<br>
        <em>And</em> el nivel de zoom se mantiene constante durante el desplazamiento<br><br>
        <strong>Scenario 3: Botones de zoom incluidos</strong><br>
        <em>Given</em> el mapa está visible<br>
        <em>When</em> el agricultor hace clic en el botón "+" en la interfaz del mapa<br>
        <em>Then</em> el mapa hace zoom in sin necesidad de mouse<br>
        <em>And</em> el botón "-" hace zoom out
       </td>
      <td>EPIC4</td>
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
        <strong>Scenario 1: Recomendación de riego cuando humedad es críticamente baja</strong><br>
        <em>Given</em> el agricultor ha iniciado sesión y está en el Dashboard<br>
        <em>And</em> el sensor de la zona "Norte" reporta una humedad del 25%<br>
        <em>And</em> el umbral mínimo configurado para esa zona es del 30%<br>
        <em>When</em> el sistema procesa la última lectura (cada 5 minutos)<br>
        <em>Then</em> el Dashboard debe mostrar una tarjeta de alerta con fondo rojo<br>
        <em>And</em> la alerta debe decir: "【RIEGO URGENTE】Zona Norte: Humedad al 25%. Se recomienda regar por 25 minutos."<br>
        <em>And</em> debe enviarse una notificación push al móvil del agricultor (si está habilitado)<br><br>
        <strong>Scenario 2: Recomendación "No regar" cuando humedad adecuada</strong><br>
        <em>Given</em> el sensor de humedad de la zona "Sur" muestra un valor del 65%<br>
        <em>And</em> los umbrales configurados son min 30% y max 80%<br>
        <em>When</em> el sistema procesa la lectura<br>
        <em>Then</em> se muestra un mensaje informativo con fondo verde: "✅ Zona Sur: Suelo con humedad adecuada (65%). No es necesario regar."<br>
        <em>And</em> NO se envía notificación push (para no saturar)<br><br>
        <strong>Scenario 3: Alerta por humedad excesiva</strong><br>
        <em>Given</em> el sensor de humedad reporta 85% y umbral máximo es 80%<br>
        <em>When</em> el sistema evalúa la condición<br>
        <em>Then</em> se muestra alerta naranja: "⚠️ Zona Centro: Humedad excesiva (85%). Suspender riego. Riesgo de pudrición de raíces."
       </td>
      <td>EPIC5</td>
    </tr>
    <tr>
      <td><strong>US15</strong></td>
      <td>Recepción de Recomendación de Fertilización</td>
      <td>Como <strong>agricultor</strong>, deseo <strong>recibir una recomendación sobre qué nutriente aplicar y en qué cantidad</strong> para <strong>evitar sobrefertilización y reducir costos</strong>.</td>
      <td>
        <strong>Scenario 1: Recomendación específica de Nitrógeno</strong><br>
        <em>Given</em> el sensor de nutrientes de la zona "Este" reporta: N=15 ppm, P=25 ppm, K=40 ppm<br>
        <em>And</em> los rangos óptimos son: N (20-40 ppm), P (15-30 ppm), K (30-50 ppm)<br>
        <em>When</em> el sistema de recomendaciones evalúa los datos (cada 15 minutos)<br>
        <em>Then</em> se muestra una tarjeta violeta: "🌱 RECOMENDACIÓN FERTILIZACIÓN - Zona Este: Aplicar 8 kg/ha de Nitrógeno (Urea 46-0-0). Nivel bajo: 15 ppm (óptimo: 20-40)."<br>
        <em>And</em> se guarda la recomendación en la tabla `Recommendations` con tipo "fertilizer"<br><br>
        <strong>Scenario 2: Todos los nutrientes en niveles óptimos</strong><br>
        <em>Given</em> la zona "Oeste" reporta N=35 ppm, P=22 ppm, K=45 ppm<br>
        <em>When</em> el usuario consulta la sección "Recomendaciones"<br>
        <em>Then</em> se muestra mensaje informativo: "✅ Zona Oeste: Los niveles de nutrientes son adecuados. Mantener plan actual de fertilización."<br>
        <em>And</em> No se generan alertas ni tareas pendientes<br><br>
        <strong>Scenario 3: Múltiples deficiencias</strong><br>
        <em>Given</em> la zona "Norte" reporta N=10 ppm, P=8 ppm, K=20 ppm<br>
        <em>When</em> el sistema procesa los datos<br>
        <em>Then</em> se muestra una tarjeta roja prioritaria: "⚠️ DEFICIENCIAS MÚLTIPLES - Zona Norte: Aplicar 12 kg/ha de NPK 20-20-20. N(10), P(8), K(20) están por debajo de rangos óptimos."
       </td>
      <td>EPIC5</td>
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
        <strong>Scenario 1: Registro exitoso con código único</strong><br>
        <em>Given</em> el agricultor está en la sección "Mis Sensores" (/sensors)<br>
        <em>When</em> hace clic en "Agregar Sensor" y completa:<br>
        - Código único del dispositivo (formato AGRO-XXXXXX, ej: AGRO-3F7D22)<br>
        - Nombre de la zona (ej: "Parcela 5 - Tomates")<br>
        - Cultivo actual (selector: Tomate, Maíz, Papa, etc.)<br>
        <em>And</em> presiona "Registrar Sensor"<br>
        <em>Then</em> el sensor aparece en la lista con estado "Activo"<br>
        <em>And</em> comienza a recibir datos en los próximos 5 minutos<br>
        <em>And</em> se muestra mensaje verde: "Sensor AGRO-3F7D22 registrado exitosamente"<br><br>
        <strong>Scenario 2: Código de sensor inválido o inexistente</strong><br>
        <em>Given</em> el agricultor ingresa un código "XYZ123" que no existe en el inventario global de sensores<br>
        <em>When</em> presiona "Registrar Sensor"<br>
        <em>Then</em> se muestra error en rojo: "❌ Código de sensor inválido. Verifica que el código sea correcto o contacta a soporte."<br>
        <em>And</em> el sensor no se agrega a la lista<br><br>
        <strong>Scenario 3: Código ya registrado por otro usuario</strong><br>
        <em>Given</em> el código AGRO-3F7D22 ya está asociado a la cuenta de "campo@example.com"<br>
        <em>When</em> otro agricultor intenta registrar el mismo código<br>
        <em>Then</em> se muestra error: "Este sensor ya está registrado por otro usuario. Si es tuyo, contacta a soporte."
       </td>
      <td>EPIC6</td>
    </tr>
    <tr>
      <td><strong>US17</strong></td>
      <td>Configuración de Umbrales de Alerta</strong></td>
      <td>Como <strong>agricultor</strong>, deseo <strong>configurar umbrales personalizados para humedad y nutrientes</strong> para <strong>recibir alertas cuando los valores salgan del rango deseado</strong>.</td>
      <td>
        <strong>Scenario 1: Configuración de umbrales de humedad por zona</strong><br>
        <em>Given</em> el agricultor está en "Configuración de Alertas" y ha seleccionado la zona "Norte"<br>
        <em>When</em> establece:<br>
        - Humedad mínima: 25% (por defecto 30%)<br>
        - Humedad máxima: 75% (por defecto 80%)<br>
        <em>And</em> presiona "Guardar configuración"<br>
        <em>Then</em> se guarda la configuración en la base de datos para esa zona específica<br>
        <em>And</em> se muestra mensaje: "Umbrales actualizados para zona Norte"<br><br>
        <strong>Scenario 2: Alerta por superación de umbral personalizado</strong><br>
        <em>Given</em> el umbral máximo personalizado para zona "Centro" es 70% (más estricto que el default 80%)<br>
        <em>And</em> el sensor reporta 72% de humedad<br>
        <em>When</em> el sistema evalúa la condición<br>
        <em>Then</em> se genera una alerta: "💧 Zona Centro: Humedad excesiva (72% - supera umbral configurado del 70%). Suspender riego por 12 horas."<br>
        <em>And</em> la alerta se guarda en el historial<br><br>
        <strong>Scenario 3: Restablecer umbrales a valores por defecto</strong><br>
        <em>Given</em> el agricultor ha modificado los umbrales previamente<br>
        <em>When</em> hace clic en "Restablecer valores por defecto"<br>
        <em>Then</em> los umbrales vuelven a: Humedad min 30%, Humedad max 80%, N min 20 ppm, N max 40 ppm, etc.<br>
        <em>And</em> se muestra mensaje de confirmación
       </td>
      <td>EPIC6</td>
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
      <td>Exportación de Reporte en PDF</strong></td>
      <td>Como <strong>administrador de cooperativa</strong>, deseo <strong>exportar un reporte mensual de rendimiento en formato PDF</strong> para <strong>compartirlo con los socios de la cooperativa</strong>.</strong></td>
      <td>
        <strong>Scenario 1: Generación de PDF con parámetros específicos</strong><br>
        <em>Given</em> el administrador con rol "AdminCooperativa" está en la sección "Reportes" (/reports)<br>
        <em>When</em> selecciona el mes "Mayo 2026", el tipo de reporte "Rendimiento por zona" y hace clic en "Exportar PDF"<br>
        <em>Then</em> se descarga un archivo PDF con nombre "Reporte_AgroTech_Mayo2026.pdf"<br>
        <em>And</em> el PDF tiene menos de 5 MB y se genera en menos de 10 segundos<br><br>
        <strong>Scenario 2: Contenido completo del reporte PDF</strong><br>
        <em>Given</em> el PDF se genera correctamente<br>
        <em>When</em> el administrador lo abre con Acrobat Reader o navegador<br>
        <em>Then</em> contiene obligatoriamente:<br>
        - Encabezado con logo de AgroTech y fecha de generación<br>
        - Tabla resumen de riego (total de litros por zona)<br>
        - Gráfico de consumo de agua por semana<br>
        - Tendencias de nutrientes (evolución N-P-K a lo largo del mes)<br>
        - Lista de alertas generadas (mínimo fecha, zona, tipo)<br>
        - Recomendaciones para el próximo mes<br><br>
        <strong>Scenario 3: Filtros combinados</strong><br>
        <em>Given</em> el administrador selecciona un rango de fechas personalizado "01/04/2026 al 15/04/2026"<br>
        <em>When</em> genera el PDF<br>
        <em>Then</em> el reporte solo incluye datos dentro de ese rango<br>
        <em>And</em> en el PDF se indica "Período: 01/04/2026 - 15/04/2026"
       </td>
      <td>EPIC7</strong></td>
    </tr>
    <tr>
      <td><strong>US19</strong></td>
      <td>Dashboard Agregado por Socio/Lote</strong></td>
      <td>Como <strong>administrador de cooperativa</strong>, deseo <strong>ver un dashboard consolidado de todos los socios o lotes</strong> para <strong>comparar el rendimiento y detectar oportunidades de mejora colectiva</strong>.</strong></td>
      <td>
        <strong>Scenario 1: Vista de lista de socios con métricas clave</strong><br>
        <em>Given</em> el administrador inicia sesión con rol "AdminCooperativa" y hay al menos 5 socios registrados<br>
        <em>When</em> accede al dashboard principal de la cooperativa (/cooperative-dashboard)<br>
        <em>Then</em> se muestra una tabla con columnas:<br>
        - Nombre del socio / email<br>
        - Hectáreas totales<br>
        - Humedad promedio (últimos 7 días)<br>
        - Rendimiento estimado (toneladas/hectárea)<br>
        - Número de alertas activas<br>
        <em>And</em> la tabla se puede ordenar por cualquiera de las columnas<br><br>
        <strong>Scenario 2: Detalle individual por socio</strong><br>
        <em>Given</em> el administrador está en la tabla de socios<br>
        <em>When</em> hace clic en el nombre "Juan Pérez"<br>
        <em>Then</em> se abre una vista detallada con todos los indicadores de Juan Pérez:<br>
        - Lista de zonas/sensores que posee<br>
        - Gráficos individuales de humedad, nutrientes, temperatura<br>
        - Historial de recomendaciones personalizadas<br>
        - Botón para enviar mensaje directo al socio<br><br>
        <strong>Scenario 3: Comparativa rápida entre socios</strong><br>
        <em>Given</em> el administrador está en la vista consolidada<br>
        <em>When</em> selecciona checkboxes de "Juan Pérez" y "María López" y hace clic en "Comparar"<br>
        <em>Then</em> se muestra un gráfico de barras comparativo de rendimiento y consumo de agua<br>
        <em>And</em> se genera una tabla lado a lado
        </strong>
      </td>
      <td>EPIC7</strong></td>
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
      <td><strong>US20</strong></strong></td>
      <td>Documentación de Endpoints con Swagger</strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>acceder a documentación interactiva de la API (Swagger/OpenAPI)</strong> para <strong>comprender cómo consumir los endpoints correctamente</strong>.</strong></td>
      <td>
        <strong>Scenario 1: Acceso a Swagger UI en entorno de desarrollo</strong><br>
        <em>Given</em> la API (backend .NET Core) está desplegada en entorno de desarrollo<br>
        <em>When</em> el developer accede a `https://api-dev.agrotech.com/swagger/index.html`<br>
        <em>Then</em> se muestra la interfaz de Swagger UI con todos los endpoints agrupados por controlador<br>
        <em>And</em> cada endpoint muestra método HTTP, ruta, parámetros y ejemplos de request/response<br><br>
        <strong>Scenario 2: Prueba de endpoint desde Swagger</strong><br>
        <em>Given</em> Swagger UI está abierto y el developer tiene un token JWT válido<br>
        <em>When</em> selecciona `GET /api/sensors/{id}` ingresa `sens-001` como id y hace clic en "Try it out" y luego "Execute"<br>
        <em>Then</em> se ejecuta la petición real al servidor y se muestra la respuesta HTTP con código 200 y el JSON correspondiente<br>
        <em>And</em> se muestra el tiempo de respuesta en milisegundos<br><br>
        <strong>Scenario 3: Documentación actualizada</strong><br>
        <em>Given</em> se agrega un nuevo endpoint `POST /api/irrigation/schedule`<br>
        <em>When</em> se genera el build del proyecto<br>
        <em>Then</em> Swagger se actualiza automáticamente con el nuevo endpoint y sus modelos de datos<br>
        <em>And</em> no se requieren cambios manuales en archivos de documentación
        </strong>
      </td>
      <td>EPIC8</strong></strong></td>
    </tr>
    <tr>
      <tr><strong>US21</strong></strong></td>
      <td>Endpoint de Obtención de Datos de Sensor</strong></td>
      <td>Como <strong>frontend developer</strong>, deseo <strong>consumir un endpoint GET /api/sensors/{id}/data</strong> para <strong>obtener los últimos valores de un sensor específico</strong>.</strong></td>
      <td>
        <strong>Scenario 1: Respuesta exitosa con datos completos</strong><br>
        <em>Given</em> existe un sensor con ID `sens-001` asociado a una zona y con al menos una lectura en las últimas 24 horas<br>
        <em>When</em> se realiza una petición `GET /api/sensors/sens-001/data` con header `Authorization: Bearer <token>`<br>
        <em>Then</em> la respuesta debe tener:<br>
        - HTTP 200 OK<br>
        - Content-Type: application/json<br>
        - Body con estructura exacta:<br>
        ```json<br>
        {<br>
          "sensorId": "sens-001",<br>
          "zoneName": "Norte",<br>
          "humidity": 65.5,<br>
          "nutrients": { "n": 30, "p": 15, "k": 45 },<br>
          "temperature": 22.3,<br>
          "timestamp": "2026-05-08T10:00:00Z",<br>
          "batteryLevel": 92<br>
        }<br>
        ```<br><br>
        <strong>Scenario 2: Sensor no encontrado (404)</strong><br>
        <em>Given</em> no existe sensor con ID `sens-999` en la base de datos<br>
        <em>When</em> se realiza `GET /api/sensors/sens-999/data`<br>
        <em>Then</em> la respuesta es HTTP 404 Not Found con body:<br>
        ```json<br>
        { "error": "Sensor not found", "details": "The sensor with ID sens-999 does not exist" }<br>
        ```<br><br>
        <strong>Scenario 3: Sensor sin datos recientes</strong><br>
        <em>Given</em> el sensor `sens-002` existe pero su última lectura fue hace más de 48 horas<br>
        <em>When</em> se consulta `GET /api/sensors/sens-002/data`<br>
        <em>Then</em> la respuesta es HTTP 200 pero incluye un flag `"dataStale": true` y `"message": "Last reading was 52 hours ago"`
        </strong>
      </td>
      <td>EPIC8</strong></strong></td>
    </tr>
    <tr>
      <td><strong>US22</strong></strong></strong></td>
      <td>Endpoint de Envío de Recomendación (Webhook)</strong></strong></td>
      <td>Como <strong>backend developer</strong>, deseo <strong>implementar un endpoint POST /api/recommendations/webhook</strong> para <strong>recibir datos del motor de recomendaciones y almacenarlos en la base de datos</strong>. </strong></strong></td>
      <td>
        <strong>Scenario 1: Recepción válida de recomendación desde motor externo</strong><br>
        <em>Given</em> un motor de IA externo envía un payload válido a `https://api.agrotech.com/api/recommendations/webhook`<br>
        <em>And</em> el header contiene `X-API-Key: secret-key-12345`<br>
        <em>When</em> el payload es:<br>
        ```json<br>
        { "zoneId": "Z01", "action": "water", "durationMinutes": 20, "priority": "high", "reason": "Soil moisture below threshold" }<br>
        ```<br>
        <em>Then</em> el sistema almacena la recomendación en la tabla `Recommendations`<br>
        <em>And</em> responde HTTP 201 Created con Location header apuntando a `/api/recommendations/{id}`<br>
        <em>And</em> la recomendación aparece inmediatamente en el dashboard del agricultor<br><br>
        <strong>Scenario 2: Payload inválido - falta campo requerido</strong><br>
        <em>Given</em> el webhook recibe un payload sin el campo obligatorio `zoneId`<br>
        <em>When</em> el payload es `{ "action": "fertilize", "durationMinutes": 10 }`<br>
        <em>Then</em> la respuesta es HTTP 400 Bad Request con body:<br>
        ```json<br>
        { "error": "Validation failed", "details": "zoneId is required" }<br>
        ```<br>
        <em>And</em> no se almacena ninguna recomendación<br><br>
        <strong>Scenario 3: API Key inválida o faltante</strong><br>
        <em>Given</em> la petición no incluye el header `X-API-Key` o incluye una incorrecta<br>
        <em>When</em> se intenta consumir el webhook<br>
        <em>Then</em> la respuesta es HTTP 401 Unauthorized con mensaje "Invalid or missing API Key"<br>
        <em>And</em> no se procesa la recomendación
        </strong>
      </strong></td>
      <td>EPIC8</strong></strong></strong></td>
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
      <td><strong>US23</strong> </strong> </strong></td>
      <td>Integración con API de Clima</strong> </strong> </strong></td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver el pronóstico del clima junto a mis datos de suelo</strong> para <strong>coordinar el riego con las lluvias previstas</strong>.</strong> </strong> </strong></td>
      <td>
        <strong>Scenario 1: Visualización del pronóstico en el dashboard</strong><br>
        <em>Given</em> el agricultor ha iniciado sesión y su perfil tiene configurada una ubicación (latitud/longitud)<br>
        <em>When</em> accede al dashboard principal (/dashboard)<br>
        <em>Then</em> se muestra un widget climático en la esquina superior derecha con:<br>
        - Pronóstico de lluvia para las próximas 24 horas (probabilidad % y mm estimados)<br>
        - Temperatura actual y pronóstico min/max<br>
        - Humedad ambiental %<br>
        - Velocidad del viento<br>
        <em>And</em> los datos provienen de la API de OpenWeatherMap o similar<br><br>
        <strong>Scenario 2: Actualización automática del clima</strong><br>
        <em>Given</em> el widget climático está visible y la última actualización fue hace más de 3 horas<br>
        <em>When</em> pasa el tiempo configurado (background job o polling cada 3 horas)<br>
        <em>Then</em> los datos climáticos se actualizan automáticamente sin necesidad de recargar la página<br>
        <em>And</em> se muestra un tooltip "Actualizado hace X minutos"<br><br>
        <strong>Scenario 3: Recomendación combinada (clima + suelo)</strong><br>
        <em>Given</em> el pronóstico indica lluvia del 80% en las próximas 6 horas (10 mm)<br>
        <em>And</em> el sensor de humedad del suelo reporta 35% (moderadamente bajo)<br>
        <em>When</em> el motor de recomendaciones evalúa ambos factores<br>
        <em>Then</em> se muestra una alerta amarilla: "⛈️ Pronóstico de lluvia alta en 6 horas. Suspender riego planificado para hoy. Ahorrarás aproximadamente 500 litros."
        </strong>
       </strong> </strong> </strong></td>
      <td>EPIC9</strong> </strong> </strong></strong></td>
    </tr>
    <tr>
      <td><strong>US24</strong> </strong> </strong> </strong></td>
      <td>Integración con Imágenes Satelitales</strong> </strong> </strong> </strong></td>
      <td>Como <strong>agricultor</strong>, deseo <strong>ver una imagen satelital reciente de mi sembrío</strong> para <strong>identificar visualmente áreas con problemas de crecimiento</strong>.</strong> </strong> </strong> </strong></td>
      <td>
        <strong>Scenario 1: Carga de imagen satelital más reciente</strong><br>
        <em>Given</em> el agricultor accede a la sección "Mapa Satelital" desde el menú<br>
        <em>When</em> la página carga y el backend obtiene la imagen de Sentinel Hub o Google Earth Engine<br>
        <em>Then</em> se muestra una imagen satelital con fecha de captura visible (ej: "10/05/2026 - Sentinel-2 L2A")<br>
        <em>And</em> el mapa permite cambiar entre vista satelital y vista de mapa base<br>
        <em>And</em> se puede hacer zoom hasta nivel 18 (máximo detalle)<br><br>
        <strong>Scenario 2: Selección de fecha histórica</strong><br>
        <em>Given</em> el mapa satelital está visible con la imagen más reciente<br>
        <em>When</em> el agricultor selecciona una fecha diferente en el calendario (ej: "01/04/2026")<br>
        <em>Then</em> la imagen se actualiza con la imagen satelital disponible más cercana a esa fecha<br>
        <em>And</em> se muestra mensaje: "Mostrando imagen del 01/04/2026 (nubosidad: 12%)"<br>
        <em>If</em> no hay imagen disponible para esa fecha, se muestra error: "No hay imágenes disponibles para la fecha seleccionada"<br><br>
        <strong>Scenario 3: Comparación antes/después</strong><br>
        <em>Given</em> el agricultor está viendo una imagen satelital del mes actual<br>
        <em>When</em> activa el modo "Comparación" y selecciona fecha anterior "01/03/2026"<br>
        <em>Then</em> se muestra un control deslizante que permite comparar ambas imágenes lado a lado<br>
        <em>And</em> se resaltan automáticamente las áreas con diferencia de vegetación (NDVI)
        </strong>
       </strong> </strong> </strong> </strong></td>
      <td>EPIC9</strong> </strong> </strong> </strong> </strong></td>
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
      <td><strong>TS01</strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Configuración de Repositorios con GitFlow</strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>tener los repositorios configurados con GitFlow y Conventional Commits</strong> para <strong>mantener un historial limpio y facilitar el trabajo colaborativo</strong>.</strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>
        <strong>Scenario 1: Estructura de branches según GitFlow</strong><br>
        <em>Given</em> se accede al repositorio en GitHub/GitLab<br>
        <em>When</em> se listan las branches en el repositorio `agrotech-app`<br>
        <em>Then</em> deben existir las ramas permanentes: `main` (producción) y `develop` (integración)<br>
        <em>And</em> debe existir al menos una rama `feature/autenticacion` activa para desarrollo nuevo<br>
        <em>And</em> no debe permitirse push directo a `main` (protegida, solo vía Pull Request con al menos 1 aprobación)<br><br>
        <strong>Scenario 2: Mensajes de commit con Conventional Commits</strong><br>
        <em>Given</em> se revisa el historial de commits del repositorio<br>
        <em>When</em> se observan los últimos 10 mensajes de commit<br>
        <em>Then</em> el 100% sigue el formato `<type>(<scope>): <subject>`<br>
        <em>And</em> los tipos permitidos incluyen: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`<br>
        <em>And</em> ejemplos válidos: `feat(sensors): add endpoint for humidity data`, `fix(auth): resolve token expiration bug`<br><br>
        <strong>Scenario 3: Pull Request template configurado</strong><br>
        <em>Given</em> un developer crea una Pull Request de `feature/nueva-funcion` hacia `develop`<br>
        <em>When</em> se abre la PR<br>
        <em>Then</em> se carga automáticamente un template con checklists de:<br>
        - Descripción de cambios<br>
        - Tipo de cambio (feature, fix, breaking change)<br>
        - Tests ejecutados<br>
        - Screenshots (si aplica UI)
        </strong>
       </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>EPIC10</strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
    </tr>
    <tr>
      <td><strong>TS02</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Despliegue Automático con Netlify / GitHub Actions</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>tener configurado despliegue automático (CI/CD)</strong> para <strong>que los cambios en la rama main se publiquen automáticamente en producción</strong>.</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>
        <strong>Scenario 1: Despliegue automático del frontend (Landing Page + Web App)</strong><br>
        <em>Given</em> se hace push a la rama `main` del repositorio `agrotech-frontend`<br>
        <em>When</em> Netlify detecta el cambio (webhook configurado)<br>
        <em>Then</em> ejecuta el build (`npm run build`) y despliega en `https://agrotech.netlify.app`<br>
        <em>And</em> el despliegue completo toma menos de 2 minutos<br>
        <em>And</em> se envía notificación al canal #deployments de Slack/Discord<br><br>
        <strong>Scenario 2: CI/CD para backend API con GitHub Actions</strong><br>
        <em>Given</em> se hace push a `main` del repositorio `agrotech-api`<br>
        <em>When</em> GitHub Actions ejecuta el workflow definido en `.github/workflows/deploy.yml`<br>
        <em>Then</em> primero corre los tests unitarios (`dotnet test`)<br>
        <em>And</em> si los tests pasan, compila la API (`dotnet publish`)<br>
        <em>And</em> luego despliega a Azure App Service o Railway<br>
        <em>And</em> si algún test falla, el despliegue se cancela y se envía alerta<br><br>
        <strong>Scenario 3: Variables de entorno en Netlify</strong><br>
        <em>Given</em> la aplicación requiere variables como `VITE_API_URL`<br>
        <em>When</em> se configura en Netlify UI (o netlify.toml)<br>
        <em>Then</em> el build las inyecta automáticamente<br>
        <em>And</em> no están hardcodeadas en el repositorio
        </strong>
       </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>EPIC10</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
    </tr>
    <tr>
      <td><strong>TS03</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Configuración de Base de Datos en la Nube</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>tener una base de datos PostgreSQL alojada en la nube</strong> para <strong>persistir los datos de usuarios, sensores y recomendaciones</strong>.</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>
        <strong>Scenario 1: Conexión exitosa desde la API</strong><br>
        <em>Given</em> la API está configurada con la cadena de conexión de Supabase (o Neon.tech o Azure PostgreSQL)<br>
        <em>When</em> se ejecuta `dotnet run` en entorno local apuntando a la nube<br>
        <em>Then</em> la API se conecta a la base de datos remota sin errores de timeout o SSL<br>
        <em>And</em> los logs muestran "Database connection established successfully"<br><br>
        <strong>Scenario 2: Aplicación de migraciones automáticas al inicio</strong><br>
        <em>Given</em> existen migraciones pendientes en el proyecto EF Core<br>
        <em>When</em> la API se inicia en entorno de staging/producción<br>
        <em>Then</em> se ejecuta `context.Database.Migrate()` automáticamente<br>
        <em>And</em> las tablas `Users`, `Sensors`, `Recommendations`, `Zones` se crean o actualizan sin errores<br>
        <em>And</em> se registra en logs qué migraciones se aplicaron<br><br>
        <strong>Scenario 3: Backup automático diario</strong><br>
        <em>Given</em> la base de datos está en producción<br>
        <em>When</em> el servicio de nube configurado<br>
        <em>Then</em> debe realizar backups automáticos diarios con retención mínima de 7 días<br>
        <em>And</em> debe ser posible restaurar desde la UI del proveedor
        </strong>
       </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>EPIC10</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
    </tr>
    <tr>
      <td><strong>TS04</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Configuración de Variables de Entorno</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>Como <strong>developer</strong>, deseo <strong>utilizar variables de entorno para configuraciones sensibles</strong> para <strong>evitar hardcodear credenciales en el repositorio</strong>.</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></strong></td>
      <td>
        <strong>Scenario 1: Frontend con Vite - uso de .env</strong><br>
        <em>Given</em> el frontend requiere una API key de Google Maps y la URL del backend<br>
        <em>When</em> se revisa el repositorio en GitHub<br>
        <em>Then</em> no debe haber ninguna API key hardcodeada en archivos `.js`, `.ts` o `.jsx`<br>
        <em>And</em> debe existir un archivo `.env.example` con variables como `VITE_MAP_API_KEY=`, `VITE_API_URL=`<br>
        <em>And</em> `.env` está incluido en `.gitignore`<br><br>
        <strong>Scenario 2: Backend .NET con User Secrets (desarrollo) y variables de entorno (producción)</strong><br>
        <em>Given</em> el backend requiere connection string, API key de clima y JWT Secret<br>
        <em>When</em> se revisa `appsettings.json` en el repositorio<br>
        <em>Then</em> contiene placeholders: `"ConnectionString": "${DB_CONNECTION}"`, `"JwtSecret": "${JWT_SECRET}"`<br>
        <em>And</em> en entorno de desarrollo se usa `dotnet user-secrets set "DB_CONNECTION" "valor_local"`<br>
        <em>And</em> en producción se inyecta mediante variables de entorno del sistema o servicio de nube (Azure App Settings, Railway env vars)<br><br>
        <strong>Scenario 3: Validación al arrancar</strong><br>
        <em>Given</em> la API intenta iniciar sin la variable `JWT_SECRET` configurada<br>
        <em>When</em> se ejecuta `dotnet run`<br>
        <em>Then</em> la API falla intencionalmente con mensaje: "FATAL: Missing required environment variable: JWT_SECRET"<br>
        <em>And</em> no expone información sensible
        </strong>
       </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
      <td>EPIC10</strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong> </strong></td>
    </tr>
  </tbody>
</table>