## 4.8. Database Design

### 4.8.1. Database Diagram

```plantuml
@startuml
!theme plain

' ==================== DARK THEME CONFIGURATION ====================
skinparam backgroundColor #1A1B26
skinparam defaultFontColor #A9B1D6
skinparam classFontColor #C0CAF5
skinparam classAttributeFontColor #9AA5CE
skinparam class {
    BackgroundColor #24283B
    BorderColor #414868
    HeaderBackgroundColor #1F2335
    HeaderFontColor #7DCFFF
    FontColor #C0CAF5
}

skinparam stereotype {
    BackgroundColor #1A1B26
    BorderColor #565F89
    FontColor #7DCFFF
}

skinparam arrow {
    Color #565F89
    FontColor #787C99
    Thickness 1
}

skinparam note {
    BackgroundColor #24283B
    BorderColor #414868
    FontColor #A9B1D6
}


title <color:#7DCFFF><size:16>AgroTech - Database Diagram</size></color>

'||-- Business layer --||
entity client {
+id_client: VARCHAR(36) <<PK>>
---
name: VARCHAR(255)
email: VARCHAR(255)
password: VARCHAR(255)
role: VARCHAR(50)
created_at: TIMESTAMP
}

entity subscription_plan {
+id_plan: VARCHAR(36) <<PK>>
---
name: VARCHAR(100)
price: DECIMAL(10,2)
iot_limit: INT
features: TEXT
}

entity user_subscription {
+id_user_subscription: VARCHAR(36) <<PK>>
---
start_date: TIMESTAMP
end_date: TIMESTAMP
payment_status: VARCHAR(50)
id_plan: VARCHAR(36) <<FK>>
id_user: VARCHAR(36) <<FK>>
}

'||-- Physical layer --||
entity parcel {
+id_parcel: VARCHAR(36) <<PK>>
---
name: VARCHAR(255)
latitude: DECIMAL(10,8)
longitude: DECIMAL(11,8)
altitude: DECIMAL(10,2)
category: VARCHAR(100)
id_client: VARCHAR(36) <<FK>>
}

entity device {
+id_device: VARCHAR(36) <<PK>>
---
status: VARCHAR(50)
battery: DECIMAL(5,2)
version: VARCHAR(50)
last_connection: TIMESTAMP
id_parcel: VARCHAR(36) <<FK>>
}

'||-- Raw data --||
entity sensor_data_raw {
+id_sensor_data_raw: VARCHAR(36) <<PK>>
---
raw_humidity: DECIMAL(10,2)
raw_temperature: DECIMAL(10,2)
raw_ph_level: DECIMAL(10,2)
raw_nitrogen: DECIMAL(10,2)
raw_phosphorus: DECIMAL(10,2)
raw_potassium: DECIMAL(10,2)
received_at: TIMESTAMP
id_device: VARCHAR(36) <<FK>>
}

'||-- Analytics data --||
entity sensor_record {
+id_sensor_record: VARCHAR(36) <<PK>>
---
humidity: DECIMAL(10,2)
temperature: DECIMAL(10,2)
ph_level: DECIMAL(10,2)
nitrogen: DECIMAL(10,2)
phosphorus: DECIMAL(10,2)
potassium: DECIMAL(10,2)
recorded_at: TIMESTAMP
id_device: VARCHAR(36) <<FK>>
}

entity plot_snapshot {
+id_snapshot: VARCHAR(36) <<PK>>
---
avg_humidity: DECIMAL(10,2)
avg_temperature: DECIMAL(10,2)
avg_ph: DECIMAL(10,2)
recorded_at: TIMESTAMP
id_parcel: VARCHAR(36) <<FK>>
}

'||-- Outcomes --||
entity harvest {
+id_harvest: VARCHAR(36) <<PK>>
---
quantity: DECIMAL(10,2)
harvest_date: DATE
sustainability_score: DECIMAL(5,2)
id_parcel: VARCHAR(36) <<FK>>
}

'||-- Alerts & rules --||
entity alert_rule {
+id_alert_rule: VARCHAR(36) <<PK>>
---
name: VARCHAR(255)
condition: TEXT
threshold_min: DECIMAL(10,2)
threshold_max: DECIMAL(10,2)
severity: VARCHAR(50)
is_active: BOOLEAN
}

entity alert {
+id_alert: VARCHAR(36) <<PK>>
---
type: VARCHAR(100)
severity: VARCHAR(50)
message: TEXT
is_resolved: BOOLEAN
created_at: TIMESTAMP
id_parcel: VARCHAR(36) <<FK>>
id_alert_rule: VARCHAR(36) <<FK>>
}

entity notification {
+id_notification: VARCHAR(36) <<PK>>
---
channel: VARCHAR(50)
sent_at: TIMESTAMP
read_at: TIMESTAMP
status: VARCHAR(50)
id_alert: VARCHAR(36) <<FK>>
id_client: VARCHAR(36) <<FK>>
}

'||-- Recommendations --||
entity recommendation {
+id_recommendation: VARCHAR(36) <<PK>>
---
title: VARCHAR(255)
description: TEXT
recommended_action: TEXT
created_at: TIMESTAMP
expires_at: TIMESTAMP
is_applied: BOOLEAN
id_parcel: VARCHAR(36) <<FK>>
}

'||-- Subscription payments log --||
entity subscription_payments {
+id_payment: VARCHAR(36) <<PK>>
---
amount: DECIMAL(10,2)
payment_date: TIMESTAMP
payment_method: VARCHAR(50)
transaction_id: VARCHAR(255)
status: VARCHAR(50)
id_user_subscription: VARCHAR(36) <<FK>>
}

'||-- Notifications log --||
entity notifications_log {
+id_log: VARCHAR(36) <<PK>>
---
sent_at: TIMESTAMP
delivery_status: VARCHAR(50)
retry_count: INT
error_message: TEXT
id_notification: VARCHAR(36) <<FK>>
}

'||-- Relations --||
client ||--o{ parcel
client ||--|| user_subscription
client ||--o{ notification

subscription_plan ||--o{ user_subscription

parcel ||--o{ device
parcel ||--o{ plot_snapshot
parcel ||--o{ harvest
parcel ||--o{ alert
parcel ||--o{ recommendation

device ||--o{ sensor_data_raw
sensor_data_raw ||--|| sensor_record

alert_rule ||--o{ alert
alert ||--o{ notification

user_subscription ||--o{ subscription_payments
notification ||--o{ notifications_log

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
<td><code>client</code></td>
<td>Almacena la información de los clientes del sistema, incluyendo nombre, email, contraseña cifrada, rol y fecha de registro.</td>
</tr>
<tr>
<td><code>subscription_plan</code></td>
<td>Define los planes de suscripción disponibles, con nombre, precio, límite de dispositivos IoT y características incluidas.</td>
</tr>
<tr>
<td><code>user_subscription</code></td>
<td>Registra la suscripción activa o histórica de cada cliente a un plan, incluyendo fechas de inicio/fin y estado de pago.</td>
</tr>
<tr>
<td><code>subscription_payments</code></td>
<td>Registra el historial de pagos realizados por cada suscripción, incluyendo monto, método de pago, ID de transacción y estado.</td>
</tr>
<tr>
<td><code>parcel</code></td>
<td>Almacena las parcelas agrícolas de los clientes, con datos de ubicación geográfica (latitud, longitud, altitud), nombre y categoría.</td>
</tr>
<tr>
<td><code>device</code></td>
<td>Registra los dispositivos IoT instalados en parcelas, con estado operativo, nivel de batería, versión de firmware y última conexión.</td>
</tr>
<tr>
<td><code>sensor_data_raw</code></td>
<td>Almacena los datos crudos recibidos directamente de los sensores IoT antes de cualquier limpieza o procesamiento.</td>
</tr>
<tr>
<td><code>sensor_record</code></td>
<td>Almacena las lecturas de sensores ya procesadas y validadas, incluyendo humedad, temperatura, pH, nitrógeno, fósforo y potasio.</td>
</tr>
<tr>
<td><code>plot_snapshot</code></td>
<td>Guarda resúmenes analíticos periódicos de cada parcela, con valores promedio de humedad, temperatura y pH en un momento dado.</td>
</tr>
<tr>
<td><code>harvest</code></td>
<td>Registra las cosechas obtenidas de cada parcela, con cantidad producida, fecha y puntuación de sostenibilidad calculada.</td>
</tr>
<tr>
<td><code>alert_rule</code></td>
<td>Define las reglas de negocio para generar alertas, incluyendo condiciones, umbrales mínimo/máximo, severidad y estado activo.</td>
</tr>
<tr>
<td><code>alert</code></td>
<td>Registra las alertas generadas cuando se detectan condiciones anormales en una parcela, con tipo, severidad, mensaje y estado de resolución.</td>
</tr>
<tr>
<td><code>notification</code></td>
<td>Gestiona el envío de notificaciones a clientes basadas en alertas, incluyendo canal, fechas de envío/lectura y estado de entrega.</td>
</tr>
<tr>
<td><code>notifications_log</code></td>
<td>Registra el historial detallado de envío de notificaciones, incluyendo estado de entrega, reintentos y mensajes de error.</td>
</tr>
<tr>
<td><code>recommendation</code></td>
<td>Almacena las recomendaciones generadas automáticamente para parcelas, incluyendo título, descripción, acción sugerida y estado de aplicación.</td>
</tr>
</tbody>
</table>