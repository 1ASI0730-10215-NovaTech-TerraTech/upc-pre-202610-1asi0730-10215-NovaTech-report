## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

```plantuml
@startuml
!theme plain
scale 2/3

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

title <color:#7DCFFF><size:16>AgroTech - Class Diagram</size></color>

' ==================== BUSINESS LAYER ====================
class Client {
    - idClient: String <<PK>>
    - name: String
    - email: String
    - password: String
    - role: String
    - createAt: LocalDateTime
    --
    + login()
    + updateProfile()
}

class SubscriptionPlan {
    - idPlan: String <<PK>>
    - name: String
    - price: Double
    - iotLimit: Int
    - features: String
    --
    + getPrice()
}

class UserSubscription {
    - idUserSubscription: String <<PK>>
    - startDate: LocalDateTime
    - endDate: LocalDateTime
    - paymentStatus: String
    - idPlan: String <<FK>>
    - idUser: String <<FK>>
    --
    + isActive()
    + renew()
}

' ==================== PHYSICAL LAYER ====================
class Parcel {
    - idParcel: String <<PK>>
    - name: String
    - latitude: Double
    - longitude: Double
    - altitude: Double
    - category: String
    - idClient: String <<FK>>
    --
    + getLocation()
}

class Device {
    - idDevide: String <<PK>>
    - status: String
    - battery: Double
    - version: String
    - lastConnection: LocalDateTime
    - idParcel: String <<FK>>
    --
    + sendData()
    + checkBattery()
}

' ==================== ANALYTICS LAYER ====================
class SensorRecord {
    - idSensorRecord: String <<PK>>
    - humidity: Double
    - temperature: Double
    - phLevel: Double
    - nitrogen: Double
    - phosphorus: Double
    - potassium: Double
    - recordedAt: LocalDateTime
    - idDevice: String <<FK>>
    --
    + getNutrients()
}

class PlotSnapshot {
    - idSnapshot: String <<PK>>
    - avgHumidity: Double
    - avgTemperature: Double
    - avgPH: Double
    - recordedAt: LocalDateTime
    - idParcel: String <<FK>>
    --
    + calculateAverages()
}

' ==================== OUTCOMES ====================
class Harvest {
    - idHarvest: String <<PK>>
    - quantity: Double
    - harvestDate: LocalDateTime
    - sustainabilityScore: Double
    - idParcel: String <<FK>>
    --
    + calculateScore()
}

' ==================== ALERTS ====================
class Alert {
    - idAlert: String <<PK>>
    - type: String
    - severity: String
    - message: String
    - isResolved: Boolean
    - createdAt: LocalDateTime
    - idParcel: String <<FK>>
    --
    + resolve()
}

class Notification {
    - idNotification: String <<PK>>
    - channel: String
    - sentAt: LocalDateTime
    - readAt: LocalDateTime
    - status: String
    - idAlert: String <<FK>>
    - idClient: String <<FK>>
    --
    + send()
    + markAsRead()
}

' ==================== RELATIONSHIPS ====================
Client ||--o{ Parcel : owns
Client ||--|| UserSubscription : has
Client ||--o{ Notification : receives

SubscriptionPlan ||--o{ UserSubscription : includes

Parcel ||--o{ Device : contains
Parcel ||--o{ PlotSnapshot : generates
Parcel ||--o{ Harvest : produces
Parcel ||--o{ Alert : triggers

Device ||--o{ SensorRecord : collects

Alert ||--o{ Notification : generates

@enduml
```

### 4.7.2. Class Dictionary

<table border="1">
<thead>
<tr>
<th>Class</th>
<th>Definition</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>Client</code></td>
<td>Entidad que representa un cliente del sistema, con información como nombre, email, contraseña, rol y fecha de creación. Permite inicio de sesión y actualización de perfil.</td>
</tr>
<tr>
<td><code>SubscriptionPlan</code></td>
<td>Entidad que define un plan de suscripción, incluyendo nombre, precio, límite de dispositivos IoT y características incluidas.</td>
</tr>
<tr>
<td><code>UserSubscription</code></td>
<td>Entidad que vincula un cliente con un plan de suscripción, gestionando fechas de inicio y fin, estado de pago, y permitiendo verificar si está activa o renovarla.</td>
</tr>
<tr>
<td><code>Parcel</code></td>
<td>Entidad que representa una parcela agrícola, con datos de ubicación (latitud, longitud, altitud), nombre, categoría y relación con el cliente propietario.</td>
</tr>
<tr>
<td><code>Device</code></td>
<td>Entidad que representa un dispositivo IoT instalado en una parcela, con estado, nivel de batería, versión de software y última conexión. Puede enviar datos y verificar batería.</td>
</tr>
<tr>
<td><code>SensorRecord</code></td>
<td>Entidad que almacena las lecturas de sensores de un dispositivo, incluyendo humedad, temperatura, nivel de pH, nitrógeno, fósforo y potasio.</td>
</tr>
<tr>
<td><code>PlotSnapshot</code></td>
<td>Entidad que representa un resumen analítico de una parcela en un momento dado, con valores promedio de humedad, temperatura y pH.</td>
</tr>
<tr>
<td><code>Harvest</code></td>
<td>Entidad que registra una cosecha, con cantidad producida, fecha y puntuación de sostenibilidad calculada en base a parámetros definidos.</td>
</tr>
<tr>
<td><code>Alert</code></td>
<td>Entidad que representa una alerta generada por condiciones anormales en una parcela, con tipo, severidad, mensaje y estado de resolución.</td>
</tr>
<tr>
<td><code>Notification</code></td>
<td>Entidad que gestiona el envío de notificaciones a clientes basadas en alertas, con canal de envío, estado de lectura y seguimiento de entrega.</td>
</tr>
</tbody>
</table>