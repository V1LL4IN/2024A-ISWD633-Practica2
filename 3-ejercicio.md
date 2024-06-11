### Crear contenedor de Postgres sin que exponga los puertos. Usar la imagen: postgres:11.21-alpine3.17

<img width="1373" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/70b858ff-68b2-4c8b-bf66-26dddc2ce77e">


### Crear un cliente de postgres. Usar la imagen: dpage/pgadmin4

<img width="1217" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/1cdb3100-c1ad-44f3-8a96-10f1e4ec3c23">


La figura presenta el esquema creado en donde los puertos son:
- a: 8080
- b: 80
- c: 5432

![Imagen](imagenes/esquema-ejercicio3.PNG)

## Desde el cliente
### Acceder desde el cliente al servidor postgres creado.

<img width="1544" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/a793b12d-2a77-4605-9018-b32994a6cab2">

<img width="1705" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/466a109d-8963-4049-abd7-9e793b866e3c">

### Crear la base de datos info, y dentro de esa base la tabla personas, con id (serial) y nombre (varchar), agregar un par de registros en la tabla, obligatorio incluir su nombre.

<img width="1190" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/f6ca2d31-e054-440e-8f5d-c59cf634c4ae">

<img width="1228" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/757c7bad-91cb-4df6-af52-481088fc8ab4">


## Desde el servidor postgresl
### Acceder al servidor
### Conectarse a la base de datos info
### Realizar un select *from personas
<img width="741" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/c4dcfec8-4ffd-45fb-8e59-cd674754d8d2">
