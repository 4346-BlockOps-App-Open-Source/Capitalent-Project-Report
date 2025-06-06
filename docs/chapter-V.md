# Capítulo V: Implementación, Validación y Despliegue del Producto

## 5.1. Software Configuration Management
En esta sección se abordarán los diferentes aspectos relacionados con la configuración de las herramientas necesarias para el desarrollo del proyecto, desde la creación de la Landing Page hasta el producto final que incluye el backend. También se explicarán las herramientas empleadas para el diseño UX/UI, convenciones de estilo, configuración de despliegue y más.

### 5.1.1. Software Development Environment Configuration
En esta parte se detallan las aplicaciones y productos de software que se utilizarán a lo largo del desarrollo del proyecto. Estas herramientas se organizan en las siguientes categorías:

#### Project Management

- Requirements Management

- Product UX/UI Design

- Software Development

- Software Testing

- Software Documentation



#### Project Management
La gestión de proyectos tiene como objetivo la administración eficiente de los recursos y procesos para lograr los resultados esperados. Durante el desarrollo, se implementará un producto de software basado en el modelo SaaS accesible desde navegadores web; no se desarrollará una versión móvil del mismo.

Para mantener la organización y comunicación del equipo, se utilizó:

- Discord: Plataforma social ideal para la creación de grupos y comunidades, usada aquí para realizar reuniones virtuales y llamadas grupales de coordinación.

#### Requirements Management
Este proceso asegura que las necesidades y expectativas de los clientes y partes interesadas sean documentadas, verificadas y satisfechas adecuadamente.

- Pivotal Tracker: Herramienta de gestión de historias de usuario que facilita la organización de tareas en epopeyas y su priorización mediante un sistema de puntuaciones. Permite visualizar en tiempo real el avance del proyecto y realizar ajustes de manera colaborativa.

#### Product UX/UI Design
El diseño UX/UI es fundamental para crear productos que se adapten a las necesidades de los usuarios. En este proyecto, se busca construir un sitio web compatible con computadoras y dispositivos móviles. Para ello, se emplearon varias herramientas:

- Figma: Aplicación en línea para la creación de wireframes y mockups, facilitando la transición de diseño a código.

- UXPressia: Plataforma especializada en la creación de User Personas, Empathy Maps, Journey Maps, y otros artefactos de experiencia de usuario.

- Miro: Pizarra digital colaborativa ideal para realizar lluvias de ideas, mapas mentales, wireframes, y actividades de ideación conjunta.

- LucidChart: Herramienta online de diagramación en tiempo real que permite crear diagramas UML, modelos C4, mapas mentales, entre otros.

- Overflow: Herramienta de diagramación de Userflows que facilita la colaboración en tiempo real, complementando el diseño de experiencias de usuario.

#### Software Development
En cuanto al desarrollo de la aplicación, se emplearon las siguientes herramientas:

- Visual Studio Code: Editor de código fuente intuitivo, compatible con múltiples lenguajes de programación y extensible mediante plugins.

- Rider: IDE de JetBrains especializado en el desarrollo de aplicaciones .NET y ASP.NET, donde C# será el lenguaje principal. Se utilizará para construir el Web Service del proyecto.

- GitHub: Plataforma de hospedaje de repositorios Git, clave para la colaboración del equipo y el control de versiones del código y la documentación en formato Markdown.

#### Software Testing
Esta disciplina se centra en la validación y verificación del correcto funcionamiento del software desarrollado.

- Lenguaje Gherkin: Lenguaje específico de dominio (DSL) utilizado para describir historias de usuario y escenarios de prueba, estructurando los casos de prueba bajo patrones como Característica, Escenario, Dado, Cuando, Entonces.

#### Software Documentation
La documentación de software incluye todos los textos e ilustraciones que explican el uso, funcionalidad y operación del producto. Esta documentación puede estar integrada en el código fuente o presentarse como manuales independientes.


### 5.1.2. Source Code Management

En esta sección se explica qué métodos se emplearon para registrar los cambios realizados, además de definir la semántica y las convenciones de nombres que se aplicarán a los commits y las versiones a lo largo del desarrollo del proyecto.

Primero, es importante señalar que utilizaremos GitHub como plataforma principal para el control de versiones del informe, la landing page, el servicio web y el frontend del proyecto. Para ello, se han creado los repositorios correspondientes.

- Url del repositorio: https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report.git
- Repositorio Landing page: https://github.com/4346-BlockOps-App-Open-Source/Landing-Page-Capitalent.git

#### GitFlow
GitFlow es una metodología de trabajo que organiza el desarrollo a través de ramas principales y ramas auxiliares. Optamos por emplear este modelo porque facilita mantener el código limpio y estructurado, permitiéndonos trabajar en equipo de forma más eficiente. Su fortaleza radica en la variedad de tipos de ramas que ofrece, cada una con un propósito específico:

#### Ramas Principales:

- Main: Es la rama base del proyecto, de la cual se derivan todas las demás. Contiene el código estable y listo para ser puesto en producción. Cada actualización en esta rama representa una nueva versión del proyecto.

- Develop: Se deriva de la rama Main y sirve como la rama de integración donde se combinan las nuevas funcionalidades desarrolladas. El código que esté listo en esta rama se transferirá posteriormente a Main para generar una nueva versión (release) del proyecto.

#### Ramas de Apoyo:

- Feature: Son ramas que nacen a partir de Develop, creadas para trabajar en funciones específicas del proyecto. Se generan tantas ramas Feature como funcionalidades existan. Al completar su desarrollo, deben integrarse nuevamente en Develop y ser eliminadas. La nomenclatura que se utiliza para nombrarlas sigue un formato específico:

```
feature/benefits
feature/profile
feature/memberships
```
- Release: Son ramas que se crean a partir de Develop y se utilizan para preparar una nueva versión del proyecto lista para ser publicada. Es importante mencionar que, si es necesario añadir nuevas funcionalidades, deberá crearse una nueva rama Release, siguiendo las reglas de Semantic Versioning 2.0.0, que se detallarán más adelante.

- Hotfix: Estas ramas se originan desde Main y se emplean para solucionar de manera rápida errores detectados en el código que ya está en producción (Main). Una vez corregido el problema, la rama Hotfix debe integrarse tanto en Main como en Develop.

#### Semantic Versioning

Es un conjunto de reglas que nos ayudan a administrar adecuadamente la numeración de versiones de nuestro proyecto. Lo aplicaremos en las ramas **Release**, utilizando el formato **X.Y.Z** (Mayor, Menor, Parche):

- **Versión de Parche (Z):** Se incrementa cuando se corrigen errores que no afectan la compatibilidad con versiones anteriores.
- **Versión Menor (Y):** Se incrementa al agregar nuevas funcionalidades que mantienen la compatibilidad con versiones previas.
- **Versión Mayor (X):** Se incrementa si se introducen cambios que rompen la compatibilidad con versiones anteriores. Cuando esto sucede, los valores de Y y Z se reinician a 0.

**Ejemplos de ramas Release:**
```
release-1.0.5
release-2.1.3
release-2.2.1
```

#### Conventional Commits

Se trata de un conjunto de normas para estructurar nuestros mensajes de commit, facilitando un historial de cambios claro y fácil de entender para todo el equipo. La estructura básica es:

```
<type> [scope opcional]: <descripción>
[cuerpo opcional]
[footer opcional]
```

- **type:** Define el tipo de cambio realizado:
  - `feat:` para nuevas funcionalidades.
  - `docs:` para cambios en la documentación.
  - `fix:` para correcciones de errores.
  - `chore:` para tareas menores que no afectan el código fuente.
  - `refactor:` para reestructuración interna sin alterar el comportamiento del proyecto.
  - `build:` para cambios en el sistema de construcción o en dependencias externas.
  - `perf:` para mejoras en el rendimiento.

- **scope (opcional):** Especifica el área o módulo afectado por el cambio.
- **description (obligatorio):** Breve explicación en minúsculas y en modo imperativo sobre lo que se modificó.
- **body (opcional):** Detalla información adicional sobre el cambio.
- **footer (opcional):** Se utiliza para indicar información relevante sobre cambios importantes o advertencias.


### 5.1.3. Source Code Style Guide & Conventions


#### Nomenclatura General

En nuestro proyecto, los nombres de variables, objetos, elementos y funciones estarán en **minúsculas**. Esto sigue la recomendación de W3Schools, que señala que mezclar mayúsculas y minúsculas puede dificultar la legibilidad.

**Ejemplos:**
```css
.gallery {}
.video {}
.login {}
```


#### Sangría

En archivos HTML, CSS y JavaScript utilizaremos **2 espacios** para la sangría en bloques de código. El uso de la tecla "Tabulación" está desaconsejado.

**Ejemplos:**

HTML:
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Título</title>
  </head>
  <body>
    <h1>Encabezado</h1>
    <p>Párrafo.</p>
  </body>
</html>
```

CSS:
```css
html {
  background: #fff; /* Fondo blanco */
  color: #404;       /* Color gris */
}
```

JavaScript:
```javascript
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```


#### HTML: 

- **Declaración del Doctype:** Siempre inicia el documento con `<!DOCTYPE html>`.
- **Líneas en blanco:** Agrega líneas en blanco entre secciones grandes para mejorar la legibilidad.

**Ejemplo:**
```html
<body>

<h1>Famous Cities</h1>

<h2>Tokyo</h2>
<p>Tokyo is the capital of Japan...</p>

<h2>London</h2>
<p>London is the capital city of England...</p>

</body>
```

- **Atributos entre comillas dobles:** Aunque no es obligatorio, mejora la legibilidad.
```html
<table class="striped">
```

- **No omitir `<title>`:** Siempre agrega un `<title>` en la cabecera del documento para mejorar el SEO y la accesibilidad.
```html
<title>HTML Style Guide and Coding Conventions</title>
```

- **Saltos de línea en HTML:** Evita líneas de código excesivamente largas, indenta con 4 espacios en subelementos.
```html
<button mat-icon-button color="primary" class="menu-button"
(click)="openMenu()">
  <mat-icon>menu</mat-icon>
</button>
```


#### CSS: 

- **Uso de Shorthand:** Escribe propiedades combinadas en una sola línea para mayor eficiencia.
```css
padding: 0 1em 2em;
border-top: 0;
font: 100%/1.6 palatino, georgia, serif;
```

- **Formato de declaración:** Deja un espacio entre el selector y la llave, y entre la propiedad y su valor.
```css
html {
  background: #fff;
  color: #404;
}
```

- **Uso de comillas:** Utilizar **comillas simples** en CSS.
```css
html {
  font-family: 'open sans', arial, sans-serif;
}
```



#### JavaScript: 

- **Espacios alrededor de operadores y comas:**
```javascript
let x = y + z;
const myArray = ['Volvo', 'Saab', 'Fiat'];
```

- **Finalizar con punto y coma las declaraciones:**
```javascript
const cars = ['Volvo', 'Saab', 'Fiat'];
```

- **Llaves en funciones:** La apertura de llaves va al final de la línea de definición de la función.
```javascript
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```

- **Objetos:** Abrir y cerrar con llaves correctamente y usar comillas dobles en strings.
```javascript
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```


#### Gherkin: Buenas prácticas

Gherkin es el lenguaje que usaremos para definir nuestros escenarios de prueba de forma clara y estructurada.

- **Bloques Given-When-Then indentados:** Indenta correctamente los pasos del escenario. Usa indentación adicional para `And`.
```gherkin
Scenario: Administrador accede al catálogo de menús diarios
  Given que el administrador está autenticado
  When el administrador navega a "Catálogo de Menús"
    Then el sistema muestra una lista de menús diarios
      And permite filtrar y buscar menús
```

- **Uso de tablas:** Para datos estructurados dentro de un escenario.
```gherkin
Then se mostrará el mensaje:
  | Mensaje |
  | Se completaron los requisitos adecuadamente |
```

- **Reducir ruido:** Usar valores estándar entre comillas simples para simplificar escenarios.
```gherkin
When escribo claramente los requisitos 'dominio en C'
```

- **Separadores entre escenarios:** Agrega un salto de línea y un comentario.
```gherkin
Scenario: Administrador recibe notificación
Given que el administrador está autenticado
When el pedido cambia de estado
  Then el sistema envía una notificación
    And muestra detalles relevantes

# --------------------------

Scenario: Otro escenario
Given otro contexto
When otra acción ocurre
  Then otro resultado se muestra
```

### 5.1.4. Software Deployment Configuration
Esta sección detalla la configuración y los procesos requeridos para desplegar el software en entornos de producción o pruebas.

*Landing Page*
Para el despliegue de la landing page se utilizara github 

Paso 1: Para desplegar el LandingPage hay que dirigirse al repositorio del landingPage y luego entrar a la opción de settings

![Image](https://github.com/user-attachments/assets/47d11712-73e1-4715-b153-f589bf3dc052)

Paso 2: Ahora entraremos a la opción de Pages donde seleccionaremos la rama del proyecto que queremos desplegar

![Image](https://github.com/user-attachments/assets/6fa7f37d-c148-4215-86e4-a5d46f2f9d78)

Paso 3: Luego se podra visualizar el enlace de la landing page desplegada

![Image](https://github.com/user-attachments/assets/ecf92104-9d78-4680-939d-0c88425cea40)

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1
Esta sección ofrece una visión general del primer sprint, incluyendo planificación, ejecución y actividades de revisión.

#### 5.2.1.1. Sprint Planning 1

<table>
  <tbody>
    <tr>
      <td><strong>Sprint #</strong></td>
      <td>Sprint 1</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Planning Background</strong></td>
    </tr>
    <tr>
      <td><strong>Date</strong></td>
      <td>2025-04-12</td>
    </tr>
    <tr>
      <td><strong>Time</strong></td>
      <td>7:50 PM</td>
    </tr>
    <tr>
      <td><strong>Location</strong></td>
      <td>Remote via the GitHub platform</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Prepared by</strong></td>
    </tr>
    <tr>
      <td><strong>Attendees (for the planning meeting)</strong></td>
      <td>All members of the Capitalent team</td>
    </tr>
    <tr>
      <td><strong>Sprint 0 Review Summary</strong></td>
      <td>As this is the first development sprint, no sprint review has been completed yet.</td>
    </tr>
    <tr>
      <td><strong>Sprint 0 Retrospective Summary</strong></td>
      <td>As this is the first development sprint, no sprint retrospective has been completed yet.</td>
    </tr>
    <tr>
      <td colspan="2"><strong>Sprint Goal & User Stories</strong></td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Goal</strong></td>
      <td>Our main focus for this sprint is to build the landing page for Capitalent. This page is crucial for engaging potential users, showcasing the platform's value, and increasing sign-ups. We aim to track user interaction with the page to measure the success of this initiative.</td>
    </tr>
    <tr>
      <td><strong>Sprint 1 Velocity</strong></td>
      <td>12</td>
    </tr>
    <tr>
      <td><strong>Sum of Story Points</strong></td>
      <td>26</td>
    </tr>
  </tbody>
</table>


#### 5.2.1.2. Aspect Leaders and Collaborators
<table>
  <tbody>
    <tr>
      <td><strong>Team Member (Last Name, First Name)</strong></td>
      <td><strong>GitHub Username</strong></td>
      <td><strong>Landing Page</strong></td>
    </tr>
    <tr>
      <td>Elescano Leon, Piero Hugo</td>
      <td>PieroHugo</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Gutarra Velapatiño, Sebastian</td>
      <td>SebastianGutarra</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Llerena Delgado, Renzo Miguel</td>
      <td>Renxoll</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Mechan Chumpitaz, Rodrigo Nicolás</td>
      <td>Rodrigo270304</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Villafuerte Tapia, Renzo Alonso</td>
      <td>RenzoVi21</td>
      <td>C</td>
    </tr>
  </tbody>
</table>


#### 5.2.1.3. Sprint Backlog 1

<table>
  <tbody>
    <tr>
      <td><strong>Sprint #</strong></td>
      <td>Sprint 1</td>
    </tr>
    <tr>
      <td><strong>User Story</strong></td>
      <td><strong>Work-item / Task</strong></td>
    </tr>
    <tr>
      <td><strong>Id</strong></td>
      <td>Title</td>
      <td><strong>Id</strong></td>
      <td><strong>Title</strong></td>
      <td><strong>Description</strong></td>
      <td><strong>Estimation (Hours)</strong></td>
      <td><strong>Assigned To</strong></td>
      <td><strong>Status</strong></td>
    </tr>
    <!-- Main Section -->
    <tr>
      <td>US-01</td>
      <td>Visualización clara del valor de la plataforma</td>
      <td>US-01</td>
      <td>Mostrar los beneficios clave de Capitalent en la página de inicio</td>
      <td>Como usuario nuevo, quiero ver los beneficios clave de Capitalent en la página de inicio para motivarme a registrarme.</td>
      <td>3</td>
      <td>Renzo Llerena</td>
      <td>Done</td>
    </tr>
    <!-- Call-to-Action Section -->
    <tr>
      <td>US-02</td>
      <td>Llamado a la acción visible</td>
      <td>US-02</td>
      <td>Resaltar un botón de registro destacado</td>
      <td>Como usuario, quiero ver un botón de registro destacado en la página principal para empezar rápidamente.</td>
      <td>2</td>
      <td>Renzo Llerena</td>
      <td>Done</td>
    </tr>
    <!-- Responsive Design -->
    <tr>
      <td>US-21</td>
      <td>Visualización en dispositivos móviles</td>
      <td>US-21</td>
      <td>Diseño responsivo para usuarios móviles</td>
      <td>Como usuario móvil, quiero que la interfaz esté adaptada a teléfonos para consultar señales fácilmente.</td>
      <td>2</td>
      <td>Rodrigo Mechan</td>
      <td>Done</td>
    </tr>
    <!-- About Section -->
    <tr>
      <td>US-46</td>
      <td>Diseño atractivo y moderno</td>
      <td>US-46</td>
      <td>Crear un diseño visualmente atractivo y moderno</td>
      <td>Como usuario, quiero que la landing page tenga un diseño atractivo y moderno para dar una buena impresión y facilitar la navegación.</td>
      <td>5</td>
      <td>Piero Elescano</td>
      <td>Done</td>
    </tr>
    <!-- Contact Section -->
    <tr>
      <td>US-47</td>
      <td>Información clara sobre características y beneficios</td>
      <td>US-47</td>
      <td>Mostrar las características y beneficios principales de Capitalent</td>
      <td>Como usuario, quiero ver de forma clara y concisa las principales características y beneficios de Capitalent en la página de inicio para poder tomar una decisión informada.</td>
      <td>4</td>
      <td>Renzo Villafuerte</td>
      <td>Done</td>
    </tr>
    <!-- Footer Section -->   
    <tr>
      <td>US-48</td>
      <td>Optimización para dispositivos móviles</td>
      <td>US-49</td>
      <td>Hacer la landing page completamente responsive para dispositivos móviles</td>
      <td>Como usuario de móvil, quiero que la landing page se vea bien y sea fácil de navegar desde mi teléfono para poder acceder a la información desde cualquier lugar.</td>
      <td>3</td>
      <td>Piero Elescano</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-49</td>
      <td>Información sobre precios y suscripción</td>
      <td>US-50</td>
      <td>Mostrar claramente la estructura de precios de la plataforma</td>
      <td>Como usuario, quiero ver claramente la estructura de precios de la plataforma en la landing page para entender las opciones de suscripción disponibles.</td>
      <td>4</td>
      <td>Sebastian Gutarra</td>
      <td>Done</td>
    </tr>
    <tr>
      <td>US-50</td>
      <td>Sección de contacto con soporte</td>
      <td>US-51</td>
      <td>Incluir una sección de contacto para soporte</td>
      <td>Como usuario, quiero tener acceso fácil a una sección de contacto para poder obtener ayuda si tengo preguntas o problemas al visitar la landing page.</td>
      <td>3</td>
      <td>Rodrigo Mechan</td>
      <td>Done</td>
    </tr>
  </tbody>
</table>

#### 5.2.1.4. Development Evidence for Sprint Review
Esta subsección muestra la evidencia del trabajo de desarrollo completado durante el Sprint 1 para fines de revisión.
| Repository                  | Branch               | Commit Id | Commit Message                      | Committed on | Team Member                |
|------------------------------|----------------------|-----------|-------------------------------------|--------------|-----------------------------|
| Capitalent/landing-page      | main                 | d0fc541   | first commit                     | 25/04/2025   | Piero Elescano              |
| Capitalent/landing-page      | feature/home         | 1a794a4   | implementación de sección Home    | 26/04/2025      | Piero Elescano              |
| Capitalent/landing-page      | feature/about        | a55c8a5 | implementación de sección About   | 26/04/2025     | Renzo Llerena               |
| Capitalent/landing-page      | feature/how-it-works | ee99afa | implementación de sección How It Works | 27/04/2025  | Renzo Villafuerte           |
| Capitalent/landing-page      | feature/pricing      | 4ebddc0 | implementación de sección Pricing | 27/04/2025      | Sebastián Gutarra           |
| Capitalent/landing-page      | feature/contact      | ac6e7eb | implementación de sección Contact | 27/04/2025      | Rodrigo Mechan              |


#### 5.2.1.5. Execution Evidence for Sprint Review
Esta subsección resalta la evidencia de ejecución, incluyendo tareas completadas y hitos alcanzados durante el Sprint 1.
El equipo de desarrollo ha finalizado con éxito el sprint 1, que consistió en la implementación y el despliegue de la landing page de Capitalent. A continuación, se presentarán las evidencias correspondientes.

![Landing page](/assest/img/chapter-V/landing-home.png)

![Landing page](/assest/img/chapter-V/landing-about.png)

![Landing page](/assest/img/chapter-V/landing-how.png)

![Landing page](/assest/img/chapter-V/landing-price.png)

![Landing page](/assest/img/chapter-V/landing-contact.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review
No se dispone de pruebas de documentación, ya que el enfoque principal del primer sprint estuvo centrado en la creación de la landing page.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review
Esta subsección incluye evidencia del despliegue exitoso del software durante el Sprint 1.
Para el despliegue de la Landing Page, el equipo utilizó GitHub Pages. Se trabajaron en un repositorio de GitHub y organizaron el trabajo en diversas ramas. En la sección de configuración y Pages, para luego poder hacer el despliegue de la web.

![Image](https://github.com/user-attachments/assets/6fa7f37d-c148-4215-86e4-a5d46f2f9d78)


Link de la landing page: https://4346-blockops-app-open-source.github.io/Landing-Page-Capitalent/ 


![Landing page](/assest/img/chapter-V/landing-home.png)

#### 5.2.1.8. Team Collaboration Insights during Sprint
En esta sección se muestra cómo el equipo ha trabajado de manera colaborativa para completar la entrega del sprint. Se incluyen las métricas relacionadas con la creación de la landing page, utilizando HTML, CSS y JavaScript, así como los commits correspondientes.

![Image](https://github.com/user-attachments/assets/8ce3d44d-34ae-429c-b0a0-07e94be2fd6e)


