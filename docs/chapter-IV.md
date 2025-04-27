# Capítulo IV: Product Design

## 4.1. Style Guidelines
Esta sección presenta los estándares que definen el formato y el diseño de la solución, asegurando calidad, coherencia visual y una experiencia de usuario profesional.
### 4.1.1. General Style Guidelines
**Diseño visual:**  
El diseño de Capitalent transmite profesionalismo, tecnología y confianza. Se emplea una interfaz limpia y moderna que permite a los usuarios navegar fácilmente y acceder a información clave.

**Colores:**  
Se eligió una paleta de colores basada en tonos oscuros, combinada con acentos vibrantes que destacan acciones importantes como botones y señales del sistema. Esta gama armoniza con el logotipo y representa tecnología, análisis y precisión.
![Image](https://github.com/user-attachments/assets/ebf64483-2d40-4051-a61a-5327ffa6996a)
![Image](https://github.com/user-attachments/assets/5b22965b-1e64-43a9-b0bc-45fa82471121)

**Tipografía:**  
La fuente utilizada garantiza buena legibilidad en todo tipo de pantallas. Se optó por una tipografía sans-serif moderna Montserrat e Inter, que aporta una apariencia fresca y profesional.

![Image](https://github.com/user-attachments/assets/ce0e0ef3-0d75-41de-8f4f-0730c766a254)

![Image](https://github.com/user-attachments/assets/253e6d1d-4cf9-4771-802e-8b8250336163)

**Branding:**  
El nombre del producto es **Capitalent**, acompañado de un logotipo minimalista con formas geométricas y líneas limpias, evocando análisis técnico y precisión financiera. El diseño busca transmitir seriedad e innovación.

![Image](https://github.com/user-attachments/assets/a9b94ac1-c8b5-41a4-aea0-919070eb067b)

### 4.1.2. Web Style Guidelines
La landing page fue diseñada con enfoque *responsive* para adaptarse a todo tipo de dispositivos (smartphones, tablets, laptops y escritorios). Se implementó el patrón **Z** para guiar intuitivamente la mirada del usuario desde la cabecera hacia las secciones de valor: *About, How it works, Pricing, Contact*.

Cada sección ocupa un bloque visual claro, con tipografía consistente y elementos interactivos bien distribuidos.
## 4.2. Information Architecture
En esta sección se presenta la estructura del software y la organización de la información, adaptada a los segmentos objetivo como inversionistas individuales y profesionales del trading.
### 4.2.1. Organization Systems
**Visual Hierarchy:**  
El diseño visual enfatiza bloques como: análisis del mercado, señal inteligente, tipos de planes y formulario de contacto. La jerarquía se apoya en tamaños de fuente, uso del color y espaciado.

**Sequential:**  
Se plantea un flujo paso a paso para guiar al usuario en el uso de la aplicacion
### 4.2.2. Labeling Systems
Las etiquetas son claras y comprensibles para el usuario objetivo. Los botones y enlaces están nombrados según su función:

- **Main:** Dirige a la sección principal.  
- **About:** Redirige a la explicación de Capitalent.  
- **How it works:** Explica el funcionamiento (*Track → Analyze → Signal*).  
- **Pricing:** Muestra los tipos de planes y precios.  
- **Contact:** Lleva al formulario para contacto directo.

Los textos de cada sección resumen en pocas palabras su propósito, permitiendo escaneo rápido por parte del usuario.
### 4.2.3. SEO Tags and Meta Tags
Se utilizan etiquetas HTML en el `<head>` para facilitar el posicionamiento en buscadores (SEO) y mejorar la descripción de la página al compartirla:

```html
<title>Capitalent</title>
<meta name="description" content="A financial intelligence platform that analyzes the markets in real time and gives you clear buy or sell signals.
No noise. No confusion.">
```
### 4.2.4. Searching Systems
**¿Qué se busca?**  
Los usuarios puedan consultar:
- Señales recientes.  
- Mercados disponibles.  
- Historial de activos.  
- Tipos de planes y beneficios.  

**¿Qué resultados se mostrarán?**  
Resultados filtrados por relevancia: tipo de señal (compra/venta), activo, tiempo de actualización, etc.

**Interfaz de búsqueda:**  
Diseñada para facilitar búsquedas rápidas, con filtros desplegables y etiquetas visibles. Se prioriza una experiencia fluida tanto en dispositivos móviles como en escritorio.

### 4.2.5. Navigation Systems
La navegación es fluida, intuitiva y completamente responsive, permitiendo al usuario desplazarse por toda la pagina sin perder el contexto.

- **Hierarchical Navigation:**  
  Navegación estructurada desde el inicio hacia secciones específicas.

- **Global Navigation System:**  
  Una barra fija facilita el desplazamiento entre secciones clave.

- **Local Navigation System:**  
  Permite la navegación entre funcionalidades dentro de la página.

## 4.3. Landing Page UI Design
En esta seccion se presenta el diseño de la landing page de la aplicaion web Capitalent, esta landing tiene como objetivo captar la atencion de los usuarios y captar su atencion hacia nuestra aplicaion
Link de la landing page en Figma: 
https://www.figma.com/design/MJbmJuMkMYV0asoRbzektf/LandingPage?node-id=0-1&t=hYuGXzRJbU8K49Xy-1
### 4.3.1. Landing Page Wireframe
El landing page esta divido en siete secciones que se presentaran acontinuacion los wireframes:

-**Main**

![Wireframe](/assest/img/chapter-IV/main-wireframe.png)

-**About**

![Wireframe](/assest/img/chapter-IV/about-wireframe.png)

-**How it works**

![Wireframe](/assest/img/chapter-IV/how-works-wireframe.png)

-**Pricing**

![Wireframe](/assest/img/chapter-IV/pricing-wireframe.png)

-**Contact**

![Wireframe](/assest/img/chapter-IV/contact-wireframe.png)

### 4.3.2. Landing Page Mock-up
El landing page esta divido en siete secciones que se presentaran acontinuacion los mockups:

-**Main**

![Mockup](/assest/img/chapter-IV/main-mockup.png)

-**About**

![Mockup](/assest/img/chapter-IV/about-mockup.png)

-**How it works**

![Mockup](/assest/img/chapter-IV/how-it-works-mockup.png)

-**Pricing**

![Mockup](/assest/img/chapter-IV/pricing-mockup.png)

-**Contact**

![Mockup](/assest/img/chapter-IV/contact-mockup.png)

## 4.4. Web Applications UX/UI Design
En esta seccion presentamos los wireframes y mockups de la aplicación web, proporcionando una visión clara de la estructura y disposición de las diferentes páginas y funcionalidades. 
Link a los Wireframes y Mockups de la Web Application en Figma:
https://www.figma.com/design/OvUOH7TZTKmGwNUNRgIzsW/Web-Aplication?node-id=522-824&t=MLWRXEjdwY7cx3xO-1
### 4.4.1. Web Applications Wireframes
Presentamos los web application wireframes dividido en secciones:

-**Log in**

![Web Wireframe](/assest/img/chapter-IV/log-in-wireframe.png)

-**Sign in**

![Web Wireframe](/assest/img/chapter-IV/sign-in-wireframe.png)

-**Select plan**

![Web Wireframe](/assest/img/chapter-IV/select-plan-wireframe.png)

-**Home**

![Web Wireframe](/assest/img/chapter-IV/home-wireframe.png)

-**Signals**

![Web Wireframe](/assest/img/chapter-IV/signal-wireframe.png)

-**Assets**

![Web Wireframe](/assest/img/chapter-IV/assets-wireframe.png)

-**Settings**

![Web Wireframe](/assest/img/chapter-IV/settings-wireframe.png)

### 4.4.2. Web Applications Wireflow Diagrams

![Wireflows](/assest/img/chapter-IV/user-flow-wireframe-log-in.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-wireframe.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-wireframe1.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-wireframe2.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-wireframe3.PNG)

### 4.4.3. Web Applications Mock-ups
Presentamos los web application wireframes dividido en secciones:

-**Log in**

![Web Mockup](/assest/img/chapter-IV/log-in-screen.png)

-**Sign in**

![Web Mockup](/assest/img/chapter-IV/sign-in-mockup.png)

-**Select plan**

![Web Mockup](/assest/img/chapter-IV/select-plan-mockup.png)

-**Home**

![Web Mockup](/assest/img/chapter-IV/home-mockup.png)

-**Signals**

![Web Mockup](/assest/img/chapter-IV/signal-mockup.png)

-**Assets**

![Web Mockup](/assest/img/chapter-IV/asstes-mockup.png)

-**Settings**

![Web Mockup](/assest/img/chapter-IV/settings-mockup.png)

### 4.4.4. Web Applications User Flow Diagrams

![Wireflows](/assest/img/chapter-IV/user-flow-mockup-log-in.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-mockup.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-mockup1.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-mockup2.PNG)

![Wireflows](/assest/img/chapter-IV/user-flow-mockup3.PNG)

## 4.5. Web Applications Prototyping
Los prototipos de la plataforma Capitalent son esenciales para validar y perfeccionar el diseño de interacción, garantizando una experiencia óptima para los inversores. Nuestro enfoque se basa en cuatro pilares clave: usabilidad (facilidad de uso), accesibilidad (inclusividad), consistencia (unificación de criterios) y eficiencia (rendimiento ágil). Estos prototipos permiten evaluar la interacción de los usuarios con las herramientas financieras, asegurando que cada funcionalidad sea intuitiva y responda a las necesidades reales del mercado.

link: https://www.figma.com/design/OvUOH7TZTKmGwNUNRgIzsW/Web-Aplication?node-id=6-2&t=GX68CVW0OYCd5F4V-1

![Prototype](/assest/img/chapter-IV/prototipos-web-app.png)

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Software Architecture Context Diagram
Diagrama de contexto de la arquitectura de Capitalent.
![DiagramaContexto](https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/structurizr-101598-Contexto.png)

### 4.6.2. Software Architecture Container Diagrams
Diagramas de contenedores de la arquitectura de Capitalent.
![DiagramaContenedor](https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/structurizr-101598-Contenedor.png)

### 4.6.3. Software Architecture Components Diagrams
Diagramas de componentes de la arquitectura de Capitalent.
![DiagramaComponente](https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/structurizr-101598-Aircrafts%20BC%20Component%20Diagram.png)

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

![DiagramaDeClases]( https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/Diagrama%20en%20blanco%20(1).png )

### 4.7.2. Class Dictionary

| Clase | Atributos | Descripción |
|:------|:----------|:------------|
| Usuario  | id, nombres, apellidos, edad, fecha de registro, teléfono | Representa el usuario de Capitalent. |
| Portafolio | id, id del usuario, valor total actual, rendimiento histórico | Entidad que registra todos los activos adquiridos por el usuario y calcula el valor actual |
| Historial de señales | id, id del usuario | Registra el historial de las señales |
| Activo  | id, nombre, tipo, cantidad, valor actual, valor de compra | Una determinada adquisición, que el usuario puede poseer, comprar o vender, puede ser criptomonedas, acciones o bonos. |
| Señal | id, nombre, estrategia, timeframe, RSI, notificación | Representa una señal y su estrategia |
| Criptomoneda | id, nombre, volatilidad, cambio de precio en 24 hrs | Activo digital cuyo valor varía en el mercado. |

## 4.8. Database Design

### 4.8.1. Database Diagram
Diagrama de la base de datos que cuenta con las relaciones entre las tablas, sus llaves primarias y llaves foráneas que referencian otras tablas.

![Databasediagram]( https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/Diagrama%20en%20blanco.png )
