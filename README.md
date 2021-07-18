## Clean Architecture - Zup Assessment

## How it works:
### **1. Docker. First, you need to install docker**
* Then open the terminal and check:
```bash
docker info
```
or check docker version
```bash
docker -v
```
and docker compose version
```bash
docker-compose -v
```
### **2. Spring boot app**
* Clone the repository:
```bash
git clone https://github.com/Juantorreal/zuporangetalents.git
```
* Build the maven project:
```bash
./mvnw clean package -DskipTests
```

## Run Spring Boot App & PostgreSQL
* Build and Running the containers:

This command will build the docker containers and start them.
```bash
docker-compose up --build
```

### **Guide for using endpoints the app:**

URL BASE =`http://localhost:8080`

[DOWNLOAD POSTMAN COLLECTION]()

* POST request to `/api/usuario/cadastrar` with a object as JSON creates a new "Usuario";
* POST request to `/api/usuario/{usuarioId}/cadastrar-comic/{comicId}` with a usuarioId and comidId creates a new Comic;
* GET request to `/api/usuario/consultar/{usuarioId}` returns the "Usuario";

### **4. Docker control commands**
* Check all the images you have:
```bash
docker images
```
### **5. End stop app**
*  Stop containers:
```bash
docker-compose down
```
* Remove old stopped containers of docker-compose
```bash
docker-compose rm -f
```



