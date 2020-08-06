# __ms-glb-session__

Esta API se utiliza para la administración de sesiones de un usuario.

## Pre-requisitos

A continuación se muestran las herramientas necesarias, para poder ejecutar esta API localmente.

|HERRAMIENTA      |VERSIÓN       |DESCRIPCIÓN                  |LINK DE DESCARGA                               |
|---------------- |--------------|-----------------------------|-----------------------------------------------|
|Spring Tool Suite|4.7.0.RELEASE |IDE de desarrollo            |[SpringToolSuite](https://spring.io/tools/)    |
|Java             |1.8.0         |Lenguaje de programación     |[Java](https://www.java.com/es/download/)      |
|Git              |2.25.0        |Control de versiones         |[Git](https://git-scm.com/downloads)           |

***
## Inicio rapido 

* Clonar el proyecto

  Abrir un terminal donde más convenga y pegar el siguiente código:

```
git clone https://asteci@bitbucket.org/naucalpandeveloper001/ms-glb-session.git
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
***
## Despliegue

* Consideraciones para el despliegue

El API depende de los siguientes componentes, para que se ejecute de manera correcta:

* [encrypt-tool](https://fers-22@bitbucket.org/naucalpandeveloper002/encrypt-tool.git) - Componente que se encarga de encriptar datos
* [glb-config-service](https://ArielAlexisNava@bitbucket.org/naucalpandeveloper/glb-config-service.git) - Patron de arquitectura que permite leer propiedades desde un repositorio
* [glb-registry-service](https://MarioIvan1901@bitbucket.org/naucalpandeveloper001/glb-registry-service.git) - Componente que registra y expone instancias de esta API

_Nota: Todos los componentes deberan de clonarse y seguir los pasos del apartado de_ __Inicio rapido__

Una vez considerado lo anterior, abrimos la siguiente dirección:
```
http://localhost:8010/swagger-ui.html
```
_Nota: El puerto puede cambiarse en el archivo de propiedades, esto si de alguna manera esta ocupado en su PC_
|HTTP      |END-POINT                    |DESCRIPCIÓN                           |
|----------|-----------------------------|--------------------------------------|
|POST      |/session                     |Crea una sesión de usuario            |
|PUT       |/session/{session-key}       |Actualiza una sesión de usuario       |
|DELETE    |/session/{session-key}       |Elimina una sesión de usuario         |
|GET       |/session/{session-key}       |Obtiene una sesión de usuario         |
|GET       |/session/{user-key}/validate |Valida si existe una sesión de usuario|

***
## Construido con 

* [SpringFramework](https://spring.io/) - Framework usado para el desarrollo del API
* [Gradle](https://gradle.org/) - Manejador de dependencias
* [Git](https://git-scm.com/) - Software de control de versiones

***
## Versionado

Para el versionado y alojamiento del código se utiliza [BitBucket](https://bitbucket.org/)
***
## Autores

* **Sergio Peña Medel** - [GitHub](https://github.com/IngSergio/)