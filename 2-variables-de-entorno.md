# Variables de Entorno
### ¿Qué son las variables de entorno
# COMPLETAR

### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.


```
docker run -d --name mi_contenedor_nginx -e username=matias -e role=admin nginx:alpine
```

# COMPLETAR

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR

<img width="567" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/1aa0b200-9f32-49f4-99bd-593cdecac43f">

### Crear un contenedor con mysql:8 , mapear todos los puertos
# COMPLETAR

docker run -d --name my_mysql_container -p 3306:3306 mysql:8


### ¿El contenedor se está ejecutando?
No se está ejecutando
<img width="953" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/246808ea-0614-4cff-ab69-b2898ab5686b">

### Identificar el problema
Se deben especificar las variables de entorno para que pueda funcionar

<img width="801" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/c8ee4f47-d865-4d16-95ba-7d27adab4230">


### Eliminar el contenedor creado con mysql:8
```
docker rm my_mysql_container
```

### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

Previo a esto es necesario crear el archivo y colocar las variables en un archivo, **.env** se ha convertido en una convención estándar, pero también es posible usar cualquier extensión como **.txt**.
```
docker run -d --name <nombre contenedor> --env-file=<nombreArchivo>.<extensión> <nombre imagen>
```

**Considerar**
Es necesario especificar la ruta absoluta del archivo si este se encuentra en una ubicación diferente a la que estás ejecutando el comando docker run.

### Crear un contenedor con mysql:8 , mapear todos los puertos y configurar las variables de entorno mediante un archivo
```
docker run -d --name my_mysql_container --env-file=/Users/matiasvillarrealcruz/Documents/mysql.env -p 3306:3306 mysql:8
```


# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 

<img width="1217" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/707f52d9-835f-470d-a104-7d23c3a8a745">


### ¿Qué bases de datos existen en el contenedor creado?

<img width="314" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/3a44950d-22c8-41ea-b7b2-c9d11a06c26f">
