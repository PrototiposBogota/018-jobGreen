# JobGreen

A continuación se describe los pasos para poder instalar el ambiente de desarrollo de sistema JobGreen


## Requisitos previos

 1. Tener instalado JRE java 1.8 o superior [Descargar](https://www.java.com/es/download/)
 2. Descargar el ide STS para el despliegue de la app [Descargar](https://spring.io/tools/sts/legacy.How+to+Download+and+Connect+with+STShow)
 3. Motor de base de datos para desarrollo MYSQL [enter link description here](https://www.mysql.com/downloads/)


## Configuración de base de datos

 1. Se debe de crear una base de datos con el nombre jobGreen
 2. tener un usuario con privilegios de crear, actualizar, eliminar y consultar
 
## Configuración de espacio de trabajo
 3. Importar el proyecto java en el sts
![enter image description here](https://lh3.googleusercontent.com/L2Eu0Cs3u7_YqdR6i3A50qaKVIN4PpHdvEiGUfDNb3qJJokOi6aE-z49namTf-FvN09NkgnK1NxW "importar")
 
 4. seleccionamos un proyecto de maven existente 
 ![enter image description here](https://lh3.googleusercontent.com/jICUAp6RqydJ-ddMhTIBSxGKwGCM7IEcldGdPBmfKJJtqraJjsYXUVDT9VZyV7gETORkfJg8aj9y)
 5. seleccionamos todos los proyectos y damos click en finalizar
 ![enter image description here](https://lh3.googleusercontent.com/mBhNMBv4wLo0DNEFhXQYJS8MKgPajruiUAspPrhKXcHiKFelfJT8g0Vb7gksRwI3-9Q4RKS4pATt)

## Configuración de archivos de arranque

 1. Se debe de abrir el archivo application-dev.properties el cual se encuentra en:
 ![enter image description here](https://lh3.googleusercontent.com/VhsjHFW1iYowoQeZSCKYOMoOrv_9MD_CQhAe5P2yAnP7B_hN-UdLdAGWAMMCcg4f8wZBt45oyvfH)
 2. modificar las credenciales de las base de datos en las lineas 
 spring.datasource.url = jdbc:mysql://localhost:3306/jobGreen
spring.datasource.username = usuario
spring.datasource.password = password
 4. Descomentar la siguiente linea con el fin que cuando arranque cree las tablas en la base de datos
 spring.jpa.hibernate.ddl-auto=create

