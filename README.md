# API Task Microservice

## Overview

Esta api permite la consulta, creacion, actualizacion y eliminacion de **tareas**, las peticiones se deben autenticar con JTW.

## Pre-requirements

- JAVA 17
- Maven

## Implemented Libraries

- Spring Boot
- Spring Security
- JWT
- Lombok
- Mapstruct

## Content

* [Dependencias](#dependencies)
* [Unit Test](#test)
* [Solution Diagram Data Base](#diagramDB)
* [Solution Diagram Architecture](#diagramA)
* [API Documentation](#swagger)
* [How to run component locally](#run)
* [Additional notes](#notes)


## <a name="dependencies"></a>Dependencies POM

    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-validation</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-data-jpa</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-security</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-test</artifactId>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <optional>true</optional>
        </dependency>
        <dependency>
            <groupId>com.h2database</groupId>
            <artifactId>h2</artifactId>
            <scope>runtime</scope>
        </dependency>
        <dependency>
            <groupId>io.jsonwebtoken</groupId>
            <artifactId>jjwt-api</artifactId>
            <version>${jsonwebtoken.version}</version>
        </dependency>
        <dependency>
            <groupId>io.jsonwebtoken</groupId>
            <artifactId>jjwt-impl</artifactId>
            <version>${jsonwebtoken.version}</version>
            <scope>runtime</scope>
        </dependency>
        <dependency>
            <groupId>io.jsonwebtoken</groupId>
            <artifactId>jjwt-jackson</artifactId>
            <version>${jsonwebtoken.version}</version>
            <scope>runtime</scope>
        </dependency>
        <dependency>
            <groupId>io.springfox</groupId>
            <artifactId>springfox-boot-starter</artifactId>
            <version>${springfox.version}</version>
        </dependency>
        <dependency>
            <groupId>io.springfox</groupId>
            <artifactId>springfox-swagger-ui</artifactId>
            <version>${springfox.version}</version>
        </dependency>
    </dependencies>

## <a name="test"></a>Unit Tests

- Junit
- MockMvc

**Test:**

![test](./docs/img/test2.PNG)

**Coverage:**

![coverage](./docs/img/test1.PNG)

## <a name="diagramDB"></a>Solution Diagram Data Base

![DiagramaBD](./docs/img/diagramaBD.PNG)


## <a name="diagramA"></a>Solution Diagram Architecture

![Diagrama](./docs/img/diagrama.jpg)

## <a name="swagger"></a>swaggwer-ui

![swagger](./docs/img/swagger-ui.PNG)

## <a name="run"></a>How to run component locally

**Microservice settings:**

- Setup Spring application using [YML file](src/main/resources), i.e. server port.

**Run:**
- `co.com.task.api.MicroserviceApplication` main method.

**Login:**

![Login](./docs/img/login.PNG)

**Config Token:**

![Token](./docs/img/token.PNG)

**GetAll Task:**

![getAllTask](./docs/img/getAllTask.PNG)

**getById Task:**

![getById Task](./docs/img/getByIdUser.PNG)

**save Task:**

![save Task](./docs/img/saveTask.PNG)

**update Task:**

![update Task](./docs/img/updateTask.PNG)

**delete Task:**

![delete Task](./docs/img/deleteTask.PNG)

**GetAll User:**

![getAllUser](./docs/img/getAllUser.PNG)

**getById User:**

![getById User](./docs/img/getByIdUser.PNG)

**save Task:**

![save User](./docs/img/saveUser.PNG)

**update Task:**

![update User](./docs/img/updateUser.PNG)

**delete Task:**

![delete User](./docs/img/deleteUser.PNG)



## <a name="note"></a>Additional notes

Desarrollado por Edwin Gonzalez  edwinhalo2y3@hotmail.com
