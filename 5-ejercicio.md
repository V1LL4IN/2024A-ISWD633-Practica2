## Esquema para el ejercicio
![Imagen](imagenes/esquema-ejercicio5.PNG)

### Crear la red

<img width="508" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/03ca1799-c02d-4476-85e5-17526c96e7cb">

### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias

<img width="1558" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/1e421ba7-8d78-474d-9631-dd3ffc096772">


### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias

<img width="1691" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/07b48594-4fb8-461f-8d34-dff56b5d781c">

De acuerdo con el trabajo realizado, en la el esquema de ejercicio el puerto a es 9300

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.

![image](https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/2d9031bf-a3c5-45ce-b7b8-103edfdd65ff)


Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
# COLOCAR UNA CAPTURA DEL SITO EN DONDE SEA VISIBLE LA PUBLICACIÓN.

![image](https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/566d79b5-22f7-4b6a-9259-dd112ba04b22)


### Eliminar el contenedor wordpress
<img width="557" alt="image" src="https://github.com/V1LL4IN/2024A-ISWD633-Practica2/assets/135792941/c363ea2d-a37c-4346-afe4-ae5baeb66cff">

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress

### ¿Qué ha sucedido, qué puede observar?
Todas las configuraciones, incluyendo el tema y las publicaciones, se mantienen intactas. Esto se debe a que la base de datos, que contiene toda la información del sitio, reside en el contenedor de MySQL, que no se ha eliminado. 





