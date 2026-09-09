# Laboratorio 2
Uso de docker compose para el despliegue de 3 APIs y una base de datos Postgres
## STACK TECNICO:
API
- Copia de imagen de una API rest con Node.js 
    ```docker pull nmatsui/hello-world-api``` 

    ![alt text](Laboratorio-2/image-1.png)

    Corremos la imagen en el puerto 3001 con el nombre api1 ```docker run -d --rm -p 3000:3000 nmatsui/hello-world-api```

- Otra instancia de la imagen esta vez con el nombre api2
    ```docker pull nmatsui/hello-world-api``` en el puerto 3000


BASE DE DATOS:
- Iniciamos directamente la isntancia con el comando: ```docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres○```

## COMANDOS
- Realizamos la creacion de el archivo docker-compose.yaml y verificamos 

![alt text](Laboratorio-2/image-2.png)


Luego de eliminar las instancias creadas, pasamos a crear de manera declarativa haciendo uso del yaml con el comando: 
```docker compose up```

![alt text](Laboratorio-2/{CB2E4A5D-CBAD-4F5C-A720-641EFCF56952}.png)

ahora verificamos si estan creadas las isntaancias con el comando ```docker ps``` y visualizamos la salida:

![alt text](Laboratorio-2/{DAF01B39-BF91-40D0-A94D-E4CB58EA33FA}.png)

## CONFIGURACION ES
