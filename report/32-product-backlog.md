## 3.3. Product Backlog

<table border="1" cellpadding="6"cellspacing="0">
    <thead>
        <tr>
            <th><strong># Orden</strong></th>
            <th><strong>User Story Id</strong></th>
            <th><strong>Título</strong></th>
            <th><strong>Descripción</strong></th>
            <th><strong>Story Points (1/2/3/5/8)</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr><td>1</td><td>US01</td><td>Visualización de Hero Section</td><td>Como visitante, deseo ver un mensaje claro sobre el valor de AgroTech para comprender rápidamente qué ofrece la solución.</td><td>2</td></tr>
        <tr><td>2</td><td>US02</td><td>Visualización de Sección de Características</td><td>Como visitante, deseo conocer las características principales de AgroTech para evaluar si la solución satisface mis necesidades.</td><td>3</td></tr>
        <tr><td>3</td><td>US03</td><td>Envío de Formulario de Solicitud de Demo</td><td>Como visitante, deseo completar un formulario para solicitar una demostración para recibir información personalizada sobre AgroTech.</td><td>5</td></tr>
        <tr><td>4</td><td>US04</td><td>Enlace a Términos y Condiciones</td><td>Como visitante, deseo leer los términos y condiciones de servicio para conocer mis derechos y obligaciones al usar AgroTech.</td><td>1</td></tr>
        <tr><td>5</td><td>US05</td><td>Registro de Nuevo Usuario</td><td>Como agricultor, deseo crear una cuenta en AgroTech para acceder a la plataforma y configurar mis sembríos.</td><td>5</td></tr>
        <tr><td>6</td><td>US06</td><td>Inicio de Sesión</td><td>Como usuario registrado, deseo iniciar sesión con mi email y contraseña para acceder a mi dashboard y datos.</td><td>3</td></tr>
        <tr><td>7</td><td>US07</td><td>Recuperación de Contraseña</td><td>Como usuario registrado, deseo recuperar mi contraseña olvidada para volver a acceder a mi cuenta.</td><td>3</td></tr>
        <tr><td>8</td><td>US08</td><td>Visualización de Perfil de Usuario</td><td>Como agricultor, deseo ver y editar mi perfil para mantener actualizada mi información personal y de mi finca.</td><td>2</td></tr>
        <tr><td>9</td><td>US09</td><td>Visualización de Indicadores Clave</td><td>Como agricultor, deseo ver en tiempo real los valores de humedad, nutrientes y temperatura del suelo para tomar decisiones informadas sobre riego y fertilización.</td><td>5</td></tr>
        <tr><td>10</td><td>US10</td><td>Selección de Zona o Sensor Específico</td><td>Como agricultor, deseo seleccionar una zona específica de mi sembrío para ver los datos de sensores individuales.</td><td>3</td></tr>
        <tr><td>11</td><td>US11</td><td>Visualización de Histórico de Datos (Gráfico)</td><td>Como agricultor, deseo ver un gráfico con el histórico de humedad de los últimos 7 días para identificar tendencias y patrones.</td><td>5</td></tr>
        <tr><td>12</td><td>US12</td><td>Visualización de Mapa de Calor de Fertilidad</td><td>Como agricultor, deseo ver un mapa de calor de mi sembrío que indique las zonas más fértiles para planificar la rotación de cultivos y optimizar la siembra.</td><td>8</td></tr>
        <tr><td>13</td><td>US13</td><td>Zoom y Navegación en el Mapa</td><td>Como agricultor, deseo hacer zoom y desplazarme por el mapa para examinar zonas específicas con mayor detalle.</td><td>3</td></tr>
        <tr><td>14</td><td>US14</td><td>Recepción de Recomendación de Riego</td><td>Como agricultor, deseo recibir una recomendación automática sobre si debo regar o no para optimizar el uso del agua y evitar estrés hídrico.</td><td>5</td></tr>
        <tr><td>15</td><td>US15</td><td>Recepción de Recomendación de Fertilización</td><td>Como agricultor, deseo recibir una recomendación sobre qué nutriente aplicar y en qué cantidad para evitar sobrefertilización y reducir costos.</td><td>5</td></tr>
        <tr><td>16</td><td>US16</td><td>Registro de Nuevo Sensor</td><td>Como agricultor, deseo registrar un nuevo sensor en mi cuenta para empezar a monitorear una nueva zona o sembrío.</td><td>3</td></tr>
        <tr><td>17</td><td>US17</td><td>Configuración de Umbrales de Alerta</td><td>Como agricultor, deseo configurar umbrales personalizados para humedad y nutrientes para recibir alertas cuando los valores salgan del rango deseado.</td><td>3</td></tr>
        <tr><td>18</td><td>US18</td><td>Exportación de Reporte en PDF</td><td>Como administrador de cooperativa, deseo exportar un reporte mensual de rendimiento en formato PDF para compartirlo con los socios de la cooperativa.</td><td>5</td></tr>
        <tr><td>19</td><td>US19</td><td>Dashboard Agregado por Socio/Lote</td><td>Como administrador de cooperativa, deseo ver un dashboard consolidado de todos los socios o lotes para comparar el rendimiento y detectar oportunidades de mejora colectiva.</td><td>8</td></tr>
        <tr><td>20</td><td>US20</td><td>Documentación de Endpoints con Swagger</td><td>Como developer, deseo acceder a documentación interactiva de la API (Swagger/OpenAPI) para comprender cómo consumir los endpoints correctamente.</td><td>2</td></tr>
        <tr><td>21</td><td>US21</td><td>Endpoint de Obtención de Datos de Sensor</td><td>Como frontend developer, deseo consumir un endpoint GET /api/sensors/{id}/data para obtener los últimos valores de un sensor específico.</td><td>3</td></tr>
        <tr><td>22</td><td>US22</td><td>Endpoint de Envío de Recomendación (Webhook)</td><td>Como backend developer, deseo implementar un endpoint POST /api/recommendations/webhook para recibir datos del motor de recomendaciones y almacenarlos en la base de datos.</td><td>5</td></tr>
        <tr><td>23</td><td>US23</td><td>Integración con API de Clima</td><td>Como agricultor, deseo ver el pronóstico del clima junto a mis datos de suelo para coordinar el riego con las lluvias previstas.</td><td>5</td></tr>
        <tr><td>24</td><td>US24</td><td>Integración con Imágenes Satelitales</td><td>Como agricultor, deseo ver una imagen satelital reciente de mi sembrío para identificar visualmente áreas con problemas de crecimiento.</td><td>8</td></tr>
        <tr><td>25</td><td>TS01</td><td>Configuración de Repositorios con GitFlow</td><td>Como developer, deseo tener los repositorios configurados con GitFlow y Conventional Commits para mantener un historial limpio y facilitar el trabajo colaborativo.</td><td>2</td></tr>
        <tr><td>26</td><td>TS02</td><td>Despliegue Automático con Netlify / GitHub Actions</td><td>Como developer, deseo tener configurado despliegue automático (CI/CD) para que los cambios en la rama main se publiquen automáticamente en producción.</td><td>3</td></tr>
        <tr><td>27</td><td>TS03</td><td>Configuración de Base de Datos en la Nube</td><td>Como developer, deseo tener una base de datos PostgreSQL alojada en la nube (Azure/AWS) para persistir los datos de usuarios, sensores y recomendaciones.</td><td>3</td></tr>
        <tr><td>28</td><td>TS04</td><td>Configuración de Variables de Entorno</td><td>Como developer, deseo utilizar variables de entorno para configuraciones sensibles (API keys, connection strings) para evitar hardcodear credenciales en el repositorio.</td><td>2</td></tr>
    </tbody>
</table>