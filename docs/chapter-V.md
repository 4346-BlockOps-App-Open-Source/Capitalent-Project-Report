# Capítulo V: Implementación, Validación y Despliegue del Producto

## 5.1. Software Configuration Management
En esta sección se abordarán los diferentes aspectos relacionados con la configuración de las herramientas necesarias para el desarrollo del proyecto, desde la creación de la Landing Page hasta el producto final que incluye el backend. También se explicarán las herramientas empleadas para el diseño UX/UI, convenciones de estilo, configuración de despliegue y más.

### 5.1.1. Software Development Environment Configuration
En esta parte se detallan las aplicaciones y productos de software que se utilizarán a lo largo del desarrollo del proyecto. Estas herramientas se organizan en las siguientes categorías:

#### Project Management

Requirements Management

Product UX/UI Design

Software Development

Software Testing

Software Documentation



#### Project Management
La gestión de proyectos tiene como objetivo la administración eficiente de los recursos y procesos para lograr los resultados esperados. Durante el desarrollo, se implementará un producto de software basado en el modelo SaaS accesible desde navegadores web; no se desarrollará una versión móvil del mismo.

Para mantener la organización y comunicación del equipo, se utilizó:

Discord: Plataforma social ideal para la creación de grupos y comunidades, usada aquí para realizar reuniones virtuales y llamadas grupales de coordinación.

#### Requirements Management
Este proceso asegura que las necesidades y expectativas de los clientes y partes interesadas sean documentadas, verificadas y satisfechas adecuadamente.

Pivotal Tracker: Herramienta de gestión de historias de usuario que facilita la organización de tareas en epopeyas y su priorización mediante un sistema de puntuaciones. Permite visualizar en tiempo real el avance del proyecto y realizar ajustes de manera colaborativa.

#### Product UX/UI Design
El diseño UX/UI es fundamental para crear productos que se adapten a las necesidades de los usuarios. En este proyecto, se busca construir un sitio web compatible con computadoras y dispositivos móviles. Para ello, se emplearon varias herramientas:

Figma: Aplicación en línea para la creación de wireframes y mockups, facilitando la transición de diseño a código.

UXPressia: Plataforma especializada en la creación de User Personas, Empathy Maps, Journey Maps, y otros artefactos de experiencia de usuario.

Miro: Pizarra digital colaborativa ideal para realizar lluvias de ideas, mapas mentales, wireframes, y actividades de ideación conjunta.

LucidChart: Herramienta online de diagramación en tiempo real que permite crear diagramas UML, modelos C4, mapas mentales, entre otros.

Overflow: Herramienta de diagramación de Userflows que facilita la colaboración en tiempo real, complementando el diseño de experiencias de usuario.

#### Software Development
En cuanto al desarrollo de la aplicación, se emplearon las siguientes herramientas:

Visual Studio Code: Editor de código fuente intuitivo, compatible con múltiples lenguajes de programación y extensible mediante plugins.

Rider: IDE de JetBrains especializado en el desarrollo de aplicaciones .NET y ASP.NET, donde C# será el lenguaje principal. Se utilizará para construir el Web Service del proyecto.

GitHub: Plataforma de hospedaje de repositorios Git, clave para la colaboración del equipo y el control de versiones del código y la documentación en formato Markdown.

#### Software Testing
Esta disciplina se centra en la validación y verificación del correcto funcionamiento del software desarrollado.

Lenguaje Gherkin: Lenguaje específico de dominio (DSL) utilizado para describir historias de usuario y escenarios de prueba, estructurando los casos de prueba bajo patrones como Característica, Escenario, Dado, Cuando, Entonces.

#### Software Documentation
La documentación de software incluye todos los textos e ilustraciones que explican el uso, funcionalidad y operación del producto. Esta documentación puede estar integrada en el código fuente o presentarse como manuales independientes.


### 5.1.2. Source Code Management

En esta sección se explica qué métodos se emplearon para registrar los cambios realizados, además de definir la semántica y las convenciones de nombres que se aplicarán a los commits y las versiones a lo largo del desarrollo del proyecto.

Primero, es importante señalar que utilizaremos GitHub como plataforma principal para el control de versiones del informe, la landing page, el servicio web y el frontend del proyecto. Para ello, se han creado los repositorios correspondientes.

-Url de la organización: 
-Repositorio Landing page: 

#### GitFlow
GitFlow es una metodología de trabajo que organiza el desarrollo a través de ramas principales y ramas auxiliares. Optamos por emplear este modelo porque facilita mantener el código limpio y estructurado, permitiéndonos trabajar en equipo de forma más eficiente. Su fortaleza radica en la variedad de tipos de ramas que ofrece, cada una con un propósito específico:

#### Ramas Principales:

- Main: Es la rama base del proyecto, de la cual se derivan todas las demás. Contiene el código estable y listo para ser puesto en producción. Cada actualización en esta rama representa una nueva versión del proyecto.

- Develop: Se deriva de la rama Main y sirve como la rama de integración donde se combinan las nuevas funcionalidades desarrolladas. El código que esté listo en esta rama se transferirá posteriormente a Main para generar una nueva versión (release) del proyecto.

#### Ramas de Apoyo:

## Feature: Son ramas que nacen a partir de Develop, creadas para trabajar en funciones específicas del proyecto. Se generan tantas ramas Feature como funcionalidades existan. Al completar su desarrollo, deben integrarse nuevamente en Develop y ser eliminadas. La nomenclatura que se utiliza para nombrarlas sigue un formato específico:



### 5.1.3. Source Code Style Guide & Conventions
Esta sección define los estándares y convenciones de codificación para asegurar consistencia y legibilidad en la base de código.

### 5.1.4. Software Deployment Configuration
Esta sección detalla la configuración y los procesos requeridos para desplegar el software en entornos de producción o pruebas.

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1
Esta sección ofrece una visión general del primer sprint, incluyendo planificación, ejecución y actividades de revisión.

#### 5.2.1.1. Sprint Planning 1
Esta subsección cubre la fase de planificación del Sprint 1, incluyendo objetivos, tareas y asignación de recursos.

#### 5.2.1.2. Aspect Leaders and Collaborators
Esta subsección identifica a los líderes clave y colaboradores responsables de los distintos aspectos del Sprint 1.

#### 5.2.1.3. Sprint Backlog 1
Esta subsección enumera las tareas y entregables planificados para el Sprint 1.

#### 5.2.1.4. Development Evidence for Sprint Review
Esta subsección muestra la evidencia del trabajo de desarrollo completado durante el Sprint 1 para fines de revisión.

#### 5.2.1.5. Execution Evidence for Sprint Review
Esta subsección resalta la evidencia de ejecución, incluyendo tareas completadas y hitos alcanzados durante el Sprint 1.

#### 5.2.1.6. Services Documentation Evidence for Sprint Review
Esta subsección proporciona evidencia documental relacionada con los servicios implementados durante el Sprint 1.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review
Esta subsección incluye evidencia del despliegue exitoso del software durante el Sprint 1.

#### 5.2.1.8. Team Collaboration Insights during Sprint
Esta subsección reflexiona sobre la colaboración del equipo, los desafíos y las lecciones aprendidas durante el Sprint 1.
