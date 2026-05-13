## 4.8. Database Design

### 4.8.1. Database Diagram

```plantuml
@startuml
' ==================== LIGHT THEME CONFIGURATION ====================
skinparam backgroundColor #FFFFFF
skinparam defaultFontColor #333333
skinparam classFontColor #1A1A1A
skinparam classAttributeFontColor #555555
skinparam class {
    BackgroundColor #F8F9FA
    BorderColor #DEE2E6
    HeaderBackgroundColor #E9ECEF
    HeaderFontColor #0066CC
    FontColor #1A1A1A
}

skinparam stereotype {
    BackgroundColor #FFFFFF
    BorderColor #ADB5BD
    FontColor #0066CC
}

skinparam arrow {
    Color #6C757D
    FontColor #495057
    Thickness 1
}

skinparam note {
    BackgroundColor #FFF3CD
    BorderColor #FFEEBA
    FontColor #856404
}

title <color:#0066CC><size:18>AgroTech IoT - Database Diagram</size></color>


entity User {
    * user_id : String
    --
    * email : String
    * password_hash : String
}

entity Profile {
    * profile_id : String
    --
    * user_id : String <<FK>>
    * fundo_name : String
    * contact_phone : String
    * moisture_threshold : Number
    * temp_threshold : Number
}

entity Community_profile {
    * community_profile_id : String
    --
    * profile_id : String <<FK>>
    * nickname : String
    * reputation_score : Number
    * public_bio : String
    * visibility_status : Boolean
}

entity Comment {
    * comment_id : String
    --
    * author_profile_id : String <<FK>>
    * target_profile_id : String <<FK>>
    * content : String
    * created_at : Date
}

entity Subscription {
    * subscription_id : String
    --
    * profile_id : String <<FK>>
    * product_id : String <<FK>>
    * order_id : String <<FK>>
    * start_date : Date
    * end_date : Date
    * status : String
    * auto_renew : Boolean
}

entity Order {
    * order_id : String
    --
    * profile_id : String <<FK>>
    * product_id : String <<FK>>
    * status : String
    * total_amount : Number
    * created_at : Date
}

entity Product {
    * product_id : String
    --
    * name : String
    * description : String
    * price : Number
    * type : String
}

entity Field {
    * field_id : String
    --
    * profile_id : String <<FK>>
    * name : String
    * size_m2 : Number
    * soil_type : String
    * location_lat_long : String
}

entity Device {
    * device_id : String
    --
    * field_id : String <<FK>>
    * mac_address : String
    * status : String
    * last_sync : Date
}

entity Report {
    * report_id : String
    --
    * device_id : String <<FK>>
    * generated_at : Date
    * mean_value : Number
    * variance : Number
    * standard_deviation : Number
    * technical_interpretation : String
}

entity Inventory {
    * inventory_id : String
    --
    * product_id : String <<FK>>
    * stock_quantity : Number
    * warehouse_location : String
}

entity Notification {
    * notification_id : String
    --
    * profile_id : String <<FK>>
    * title : String
    * message : String
    * is_alert : Boolean
    * is_read : Boolean
}

' Relationships
User ||--|| Profile

' Operational Hub (Profile)
Profile ||--|| Community_profile
Profile ||--o{ Order
Profile ||--o{ Subscription
Profile ||--o{ Notification
Profile ||--o{ Field

' Social Interaction
Community_profile ||--o{ Comment
Community_profile ||--o{ Comment

' Logic Connections
Order }o--|| Product
Subscription }o--|| Product
Subscription ||--|| Order

Field ||--o{ Device
Device ||--o{ Report
Product ||--|| Inventory

@enduml
```

### 4.8.2. Class Dictionary
<table border="1">
<thead>
<tr>
<th>Entity</th>
<th>Definition</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>user</code></td>
<td>Almacena las credenciales principales de acceso al sistema, incluyendo correo electrónico y contraseña cifrada de cada usuario registrado.</td>
</tr>

<tr>
<td><code>profile</code></td>
<td>Contiene la información del perfil agrícola asociado a cada usuario, como nombre del fundo, teléfono de contacto y los umbrales configurados de humedad y temperatura.</td>
</tr>

<tr>
<td><code>community_profile</code></td>
<td>Representa el perfil público del agricultor dentro de la comunidad, incluyendo apodo, biografía, puntuación de reputación y configuración de visibilidad.</td>
</tr>

<tr>
<td><code>comment</code></td>
<td>Registra los comentarios realizados entre perfiles de la comunidad, almacenando autor, destinatario, contenido y fecha de creación.</td>
</tr>

<tr>
<td><code>product</code></td>
<td>Define los productos y servicios ofrecidos por la plataforma, incluyendo nombre, descripción, precio y tipo de producto.</td>
</tr>

<tr>
<td><code>order</code></td>
<td>Registra las órdenes de compra realizadas por los perfiles, incluyendo producto adquirido, estado del pedido, monto total y fecha de creación.</td>
</tr>

<tr>
<td><code>subscription</code></td>
<td>Gestiona las suscripciones de los perfiles a productos o servicios, incluyendo fechas de inicio y fin, estado y configuración de renovación automática.</td>
</tr>

<tr>
<td><code>field</code></td>
<td>Almacena los terrenos o parcelas agrícolas administradas por cada perfil, incluyendo nombre, tamaño en metros cuadrados, tipo de suelo y ubicación geográfica.</td>
</tr>

<tr>
<td><code>device</code></td>
<td>Registra los dispositivos IoT instalados en cada parcela, con dirección MAC, estado operativo y fecha de última sincronización.</td>
</tr>

<tr>
<td><code>report</code></td>
<td>Almacena los reportes estadísticos generados a partir de los datos de los dispositivos IoT, incluyendo promedio, varianza, desviación estándar e interpretación técnica.</td>
</tr>

<tr>
<td><code>inventory</code></td>
<td>Gestiona el inventario disponible de cada producto, incluyendo cantidad en stock y ubicación del almacén.</td>
</tr>

<tr>
<td><code>notification</code></td>
<td>Registra las notificaciones y alertas enviadas a los perfiles, incluyendo título, mensaje, indicador de alerta y estado de lectura.</td>
</tr>
</tbody>
</table>