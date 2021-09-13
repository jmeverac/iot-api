# iot-api
Prueba de Concepto de API ( Falcon - Swagger - TimescaleDB - Docker - Docker Compose )



## Instalacion


Instrucciones para instalar dockers:

 - Pull de todos los archivos hacia `~/`
 - Ejecutar el comando `docker-compose up -d`.   Todas las dependencias serán descargadas automaticamente de Docker Hub
 
 Con esto se tendrán corriendo 3 contenedores con las siguientes imagenes docker:
 
La API   `jmeverac/iot-api`, 
la base de datos TimescaleDB  `timescale/timescaledb`
y Swagger-UI `swaggerapi/swagger-ui`

## Ejecucion y Pruebas

La documentación OpenApi se mostrará en la ruta `http://localhost:8081`

 - Es importante subir el archivo CSV mediante el método POST en /file primero, ya que sirve para poblar la BD
 
 Se puede realizar esta acción con POSTMAN como se indica

[Postman-file.png](https://github.com/jmeverac/iot-api/blob/main/Postman-file.png)

 Posteriormente conectar a los demás Endpoints
 
 
 
 
 
 
 
 # iot-api
API Proof of Concept ( Falcon - Swagger - TimescaleDB - Docker - Docker Compose )



## Installation


Directions:

 - From this Github repo Pull into `~/`
 - Run the command `docker-compose up -d`.   Every dependency will be automatically pulled from Docker Hub
 
Afterwards three cointainers with the following images will be up:
 
API   `jmeverac/iot-api`, 
TimescaleDB  `timescale/timescaledb`
 Swagger-UI `swaggerapi/swagger-ui`

## Execution and Tests

OpenApi documentation will be available at `http://localhost:8081`

 - It is mandatory to first upload the CSV file with all the data using the POST method using the endpoint /file, since it will populate the DB
 
 Hint:   CURL or Postman can be used for that purpose.

[Postman-file.png](https://github.com/jmeverac/iot-api/blob/main/Postman-file.png)

Then the other endpoints will be able to provide data.
