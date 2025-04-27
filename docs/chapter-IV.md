# Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines
Descripción de las pautas generales de estilo para el diseño del producto.

### 4.1.2. Web Style Guidelines
Especificaciones de estilo aplicables al diseño web.

## 4.2. Information Architecture

### 4.2.1. Organization Systems
Definición y estructura de los sistemas de organización.

### 4.2.2. Labeling Systems
Lineamientos para los sistemas de etiquetado.

### 4.2.3. SEO Tags and Meta Tags
Uso de etiquetas SEO y metaetiquetas para optimización.

### 4.2.4. Searching Systems
Diseño y funcionalidad de los sistemas de búsqueda.

### 4.2.5. Navigation Systems
Estructura y diseño de los sistemas de navegación.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe
Esquema inicial de la página de aterrizaje.

### 4.3.2. Landing Page Mock-up
Prototipo visual de la página de aterrizaje.

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes
Esquemas iniciales para aplicaciones web.

### 4.4.2. Web Applications Wireflow Diagrams
Diagramas de flujo de interacción para aplicaciones web.

### 4.4.3. Web Applications Mock-ups
Prototipos visuales para aplicaciones web.

### 4.4.4. Web Applications User Flow Diagrams
Diagramas de flujo de usuario para aplicaciones web.

## 4.5. Web Applications Prototyping
Proceso de creación de prototipos para aplicaciones web.

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

![DiagramaDeClases](https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/Diagrama%20en%20blanco.png)

### 4.7.2. Class Dictionary

| Clase | Atributos | Descripción |
|:------|:----------|:------------|
| Usuario  | id, nombres, apellidos, edad, fecha de registro, teléfono | Representa el usuario de Capitalent. |
| Portafolio | id, id del usuario, valor total actual, rendimiento histórico | Entidad que registra todos los activos adquiridos por el usuario y calcula el valor actual |
| Billetera | id, id del usuario, saldo, tipo de moneda, transacciones | Guarda un determinado monto de cierta moneda |
| Activo  | id, nombre, tipo, cantidad, valor actual, valor de compra | Una determinada adquisición, que el usuario puede poseer, comprar o vender, puede ser criptomonedas, acciones o bonos. |
| Transacción | id, billetera de origen, de destino, tipo de moneda, monto, fecha | Movimiento de un monto entre dos billeteras virtuales |
| Criptomoneda | id, nombre, volatilidad, cambio de precio en 24 hrs | Activo digital cuyo valor varía en el mercado. |

## 4.8. Database Design

### 4.8.1. Database Diagram
Diagrama de la base de datos que cuenta con las relaciones entre las tablas, sus llaves primarias y llaves foráneas que referencian otras tablas.

![Databasediagram](https://github.com/4346-BlockOps-App-Open-Source/Capitalent-Project-Report/blob/feature/chap4/assest/img/chapter-IV/DATABASE%20DIAGRAM.png)
