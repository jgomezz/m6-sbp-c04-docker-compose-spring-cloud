# Generar Docker Compose

## Parte 1

### user-service : generar jar
```
cd user-service
mvn clean package -DskipTests
cd ..
```
### product-service : generar jar
```
cd product-service
mvn clean package -DskipTests
cd ..
```

### Generar docker compose
```
docker compose build
```

### Inicializar servicios docker compose
```
docker compose up -d
```

### Detener un servicio en  docker compose
```
docker compose stop user-service-dev 
```

### Levantar un servicio en  docker compose
```
docker compose start user-service-dev
docker compose up -d user-service-dev
```