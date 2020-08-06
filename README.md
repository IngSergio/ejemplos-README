# __ms-glb-session__

Esta API se utiliza para la administración de sesiones de un usuario.

## Pre-requisitos

A continuación se muestran las herramientas necesarias, para poder ejecutar esta API localmente.

|HERRAMIENTA      |VERSIÓN       |DESCRIPCIÓN                  |LINK DE DESCARGA                               |
|---------------- |------------  |-----------------------------|-----------------------------------------------|
|Spring Tool Suite|4.7.0.RELEASE |IDE de desarrollo            |[SpringToolSuite](https://spring.io/tools/)    |
|Java             |1.8.0         |Lenguaje de programación     |[Java](https://www.java.com/es/download/)      |
|Git              |2.25.0        |Control de versiones         |[Git](https://git-scm.com/downloads)           |


## Inicio rapido 

* Clonar el proyecto

Abrir un terminal donde más convenga y pegar el siguiente código:

```
git clone https://sergiopmedel@bitbucket.org/naucalpandeveloper001/ms-glb-session.git
```  

* Importar proyecto en Spring Tool Suite

Una vez abierto el IDE, hacer lo siguiente:
```
-> File
   -> Import
      -> Existing Gradle Project 
         -> Buscar directorio de descarga y abrir proyecto
            -> Finish
```

* Ejecutando proyecto
```
-> Click derecho en el proyecto
   -> Run As 
      -> Spring Boot App 
```

## Despliegue

* Dirigirse a la siguiente dirección:
```
http://localhost:8010/swagger-ui.html
```
|HTTP      |END-POINT                    |DESCRIPCIÓN                           |
|----------|-----------------------------|--------------------------------------|
|POST      |/session                     |Crea una sesión de usuario            |
|PUT       |/session/{session-key}       |Actualiza una sesión de usuario       |
|DELETE    |/session/{session-key}       |Elimina una sesión de usuario         |
|GET       |/session/{session-key}       |Obtiene una sesión de usuario         |
|GET       |/session/{user-key}/validate |Valida si existe una sesión de usuario|

## Construido con 

* [SpringFramework](https://spring.io/) - El framework web usado
* [Gradle](https://gradle.org/) - Manejador de dependencias
* [Git](https://git-scm.com/) - Software de control de versiones

## Versionado

Para el versionado y alojamiento del código se utiliza [BitBucket](https://bitbucket.org/).

## Autores

* **Sergio Peña Medel** - [GitHub](https://github.com/IngSergio/)