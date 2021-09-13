# iot-api
Repositorio para Api / Prueba de Concepto de API ( Falcon - Swagger - TimescaleDB - Docker - Docker Compose )



## Instalacion


Instrucciones para instalar dockers:

 - Descargar Carpeta `/dist` y colocarla en la ruta del usuario `~/`, debe quedar así:   `~/dist`
 - Descargar el archivo `docker-compose.yaml` en `~/`
 - Ejecutar el comando `docker-compose up -d`.   Todas las dependencias serán descargadas.
 
 Con esto se tendrán corriendo 3 dockers:
 
La API   `jmeverac/iot-api`
La base de datos TimescaleDB  `timescale/timescaledb`
Swagger-UI `swaggerapi/swagger-ui`

## Ejecucion y Pruebas

La documentación OpenApi se mostrará en la ruta `http://localhost:8081`

 - Es importante subir el archivo CSV mediante el método POST en /file primero, ya que sirve para poblar la BD
 
 Se puede realizar esta acción con POSTMAN como se indica

[enter link description here](http://localhost/imagen.jpg)

 Posteriormente conectar a los demás Endpoints
