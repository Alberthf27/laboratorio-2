# Laboratorio 2
Uso de docker compose para el despliegue de 3 APIs y una base de datos Postgres
## STACK TECNICO:
API
- Copia de imagen de una API rest con Node.js 
    ```docker pull nmatsui/hello-world-api``` 
    
    Corremos la imagen en el puerto 3001 con el nombre api1 ```docker run -d --rm -p 3000:3000 nmatsui/hello-world-api```

- Otra instancia de la imagen esta vez con el nombre api2
    ```docker pull nmatsui/hello-world-api``` en el puerto 3000


BASE DE DATOS:
- Iniciamos directamente la isntancia con el comando: ```docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres○```

## COMANDOS

## CONFIGURACION ES