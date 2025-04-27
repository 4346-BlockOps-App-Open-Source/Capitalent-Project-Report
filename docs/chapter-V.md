# Capítulo V: Implementación, Validación y Despliegue del Producto

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration
Esta sección describe la configuración del entorno de desarrollo de software, incluyendo herramientas, dependencias y flujos de trabajo.

### 5.1.2. Source Code Management
Esta sección detalla las prácticas y herramientas utilizadas para gestionar el código fuente, incluyendo sistemas de control de versiones y estrategias de ramificación.

### 5.1.3. Source Code Style Guide & Conventions
Esta sección define los estándares y convenciones de codificación para asegurar consistencia y legibilidad en la base de código.

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
