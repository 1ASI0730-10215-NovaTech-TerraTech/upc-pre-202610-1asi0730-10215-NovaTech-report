### 4.6.2. Software Architecture Context Diagram

```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml

title AgroTech - System Context Diagram

Person(farmer, "Farmer", "Monitors crops and soil conditions")
Person(supplier, "Supplier", "Provides agricultural inputs and uses soil data")
Person(admin, "Cooperative Admin", "Manages reports and analytics")
Person(customer, "End Customer", "Consumes traceability information")

System(agrotech, "AgroTech Platform", "Smart agriculture platform using IoT and predictive analytics")

System_Ext(weather, "Weather API", "Provides weather forecasts")
System_Ext(satellite, "Satellite Imagery Service", "Provides crop and land imagery")
System_Ext(iot, "IoT Sensor Network", "Collects real-time soil data")

Rel(farmer, agrotech, "Uses", "HTTPS")
Rel(supplier, agrotech, "Accesses soil data", "HTTPS")
Rel(admin, agrotech, "Generates reports", "HTTPS")
Rel(customer, agrotech, "Checks traceability", "HTTPS")

Rel(agrotech, weather, "Fetches weather data", "REST API")
Rel(agrotech, satellite, "Retrieves satellite images", "REST API")
Rel(agrotech, iot, "Receives sensor data", "MQTT/HTTP")

@enduml
```

### 4.6.3. Software Architecture Container Diagrams

```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml

title AgroTech - Container Diagram

Person(user, "User", "Farmer / Supplier / Admin / Customer")

System_Boundary(agrotech, "AgroTech Platform") {

    Container(webapp, "Web Application", "React / Angular", "Provides UI for dashboards, maps, and authentication")

    Container(api, "Backend API", "Java / Spring Boot", "Handles business logic, IoT data, and analytics")

    ContainerDb(db, "PostgreSQL Database", "PostgreSQL", "Stores clients, parcels, devices, sensor records, alerts, harvests")

    Container(analytics, "Analytics Engine", "Python / Spark", "Calculates averages and sustainability scores")
}

System_Ext(iot_device, "IoT Device", "Hardware sensor", "Collects humidity, temperature, pH, nutrients")

Rel(user, webapp, "Uses", "HTTPS")
Rel(webapp, api, "Sends requests", "REST/JSON")
Rel(api, db, "Reads and writes", "JDBC")
Rel(analytics, db, "Reads data", "JDBC")
Rel(analytics, api, "Sends results", "REST")
Rel(iot_device, api, "Sends telemetry", "MQTT/HTTP")

@enduml
```

### 4.6.4. Software Architecture Components Diagrams

```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Component.puml

title AgroTech - Component Diagram

skinparam rectangle {
  FontColor white
}
skinparam arrow {
  Color white
  FontColor white
}

Container(api, "Backend API", "Java / Spring Boot", "Handles business logic, IoT data, and analytics") {
    
    Component(clientService, "Client Service", "Spring Service", "Manages client accounts, authentication, and profiles")
    Component(subscriptionService, "Subscription Service", "Spring Service", "Handles subscription plans and user subscriptions")
    Component(parcelService, "Parcel Service", "Spring Service", "Manages parcels and their geolocation data")
    Component(deviceService, "Device Service", "Spring Service", "Handles IoT devices, connectivity, and battery status")
    Component(sensorService, "Sensor Service", "Spring Service", "Processes sensor records and forwards to analytics")
    Component(snapshotService, "Snapshot Service", "Spring Service", "Generates plot snapshots with averages")
    Component(harvestService, "Harvest Service", "Spring Service", "Calculates sustainability scores and harvest outcomes")
    Component(alertService, "Alert Service", "Spring Service", "Generates alerts based on sensor data")
    Component(notificationService, "Notification Service", "Spring Service", "Sends notifications to clients")
}

ContainerDb(db, "PostgreSQL Database", "PostgreSQL", "Stores clients, parcels, devices, sensor records, alerts, harvests")

Container(analytics, "Analytics Engine", "Python / Spark", "Calculates averages and sustainability scores")

Container(webapp, "Web Application", "React / Angular", "Provides UI for dashboards, maps, and authentication")

System_Ext(iot_device, "IoT Device", "Hardware sensor", "Collects humidity, temperature, pH, nutrients")

Rel(webapp, clientService, "Uses", "REST/JSON")
Rel(webapp, subscriptionService, "Manages subscriptions", "REST/JSON")
Rel(webapp, parcelService, "Manages parcels", "REST/JSON")
Rel(webapp, alertService, "Checks alerts", "REST/JSON")
Rel(webapp, notificationService, "Receives notifications", "REST/JSON")

Rel(iot_device, deviceService, "Sends telemetry", "MQTT/HTTP")
Rel(deviceService, sensorService, "Stores sensor data", "REST/JSON")

Rel(sensorService, analytics, "Sends raw data", "REST")
Rel(analytics, snapshotService, "Returns averages", "REST")
Rel(analytics, harvestService, "Returns sustainability scores", "REST")

Rel(clientService, db, "Reads/Writes", "JDBC")
Rel(subscriptionService, db, "Reads/Writes", "JDBC")
Rel(parcelService, db, "Reads/Writes", "JDBC")
Rel(deviceService, db, "Reads/Writes", "JDBC")
Rel(sensorService, db, "Reads/Writes", "JDBC")
Rel(snapshotService, db, "Reads/Writes", "JDBC")
Rel(harvestService, db, "Reads/Writes", "JDBC")
Rel(alertService, db, "Reads/Writes", "JDBC")
Rel(notificationService, db, "Reads/Writes", "JDBC")

@enduml
```