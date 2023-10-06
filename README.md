# AREP06 : TALLER DE TRABAJO INDIVIDUAL EN PATRONES ARQUITECTURALES

Proyecto para pulir conocimientos sobre AWS, Docker y bases de datos mongoDB.

### Preparacion

Clonamos el repositorio

```
    git clone https://github.com/sebasporras14/lab-06AREP.git 

```
esta carpeta contiene dos proyectos el cual contienen el Roundrobin y Logservice.

---
### Corriendo
Corremos los siguientes comando en cada uno de los proyectos tanto en Lab6 como en LAB601
	
	 mvn clean package install
	 mvn clean install

Una vez tengamos los dos proyectos bien compilados y listos para ejecutar, construimos sus imagenes respectivamente y la imagen de la base de datos mongo

```
    docker build --tag logservices .
    docker build --tag roundrobin-java .
    docker pull mongo
```
Una vez las imagenes esten listas usaremos,

```
    docker-compose up -d  
```
para generar los contenedores en docker.

![test](https://github.com/sebasporras14/lab-06AREP/blob/master/img/docker.png)

Nos dirigimos al http://localhost:8080/app.html y nos mostrara:

![test](https://github.com/sebasporras14/lab-06AREP/blob/master/img/localhost.png)


---

## Video prueba del despliegue 

https://youtu.be/Kn7rTojU56o

El video demuestra el despliegue en AWS.


## Construido con 
* [Maven](https://maven.apache.org/) - Dependency Management
* [java](https://rometools.github.io/rome/) - Used to generate RSS Feeds
* [Git](https://rometools.github.io/rome/):  It is a distributed version control system (VCS).
* [Docker](https://www.docker.com) Automates the deployment of applications within software containers.

## Autor

* **Sebastian Porras**

### Fecha

10/06/2023 

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
