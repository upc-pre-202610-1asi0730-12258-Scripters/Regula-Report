# Capítulo V: Product Implementation, Validation & Deployment

# 5.1.1. Software Dev
elopment En
vironment Configuration.

| Tool / Software | Purpose in the Project | Access / Download |
|---|---|---|
| GitHub | Source code hosting and version control | https://github.com |
| Trello | Sprint task management | https://trello.com |
| Figma | Wireframes and mock-ups design | https://www.figma.com |
| Visual Studio Code | Landing page development | https://code.visualstudio.com |
| Google Chrome | Testing and responsive preview | https://www.google.com/chrome/ |
| Miro | Organization and event storming | https://miro.com/app/dashboard/ |
| LucidChart | Web Applications User Flow Diagrams | https://www.lucidchart.com/pages/es |

## Project Management

### Trello

<img src="././/assets/diagrams/trello.png">

**¿Por qué lo utilizamos?**  
Lo utilizamos para organizar tareas del sprint, asignarlas a los integrantes, dar seguimiento al avance y visualizar qué estaba pendiente, en proceso o terminado.

## Requirements Management

### Miro

![Tablero de Miro](././/assets/diagrams/miro.png)

**¿Por qué lo utilizamos?**  
Lo utilizamos para crear diagramas y representar visualmente procesos o estructuras del proyecto, como flujos, mapas o diagramas de análisis.

### UXPressia

![Artefactos en UXPressia](././/assets/diagrams/uxpressia.png)

**¿Por qué lo utilizamos?**  
Usamos UXPressia porque nos permitió crear y organizar de forma visual artefactos de análisis de usuarios, como User Personas, Journey Maps e Impact Maps, facilitando que el equipo entendiera mejor a los segmentos objetivo y mantuviera una visión compartida del usuario durante el diseño del producto.

## Product UX/UI Design

### Figma

![Diseños en Figma](././/assets/diagrams/figma.png)

**¿Por qué lo utilizamos?**  
Lo utilizamos para crear y compartir los wireframes, mockups y propuestas visuales del producto antes de implementarlo. También ayudó a que el equipo tuviera una referencia común del diseño.

### LucidChart

![Diagramas en LucidChart](././/assets/diagrams/lucidChart.png)

**¿Por qué lo utilizamos?**  
Usamos LucidChart porque nos permitió elaborar de manera clara y colaborativa los diagramas y flujos del proyecto, ayudando al equipo a representar visualmente procesos, relaciones y estructuras necesarias para el análisis, diseño y organización de la solución.

## Software Development

### Visual Studio Code

**¿Por qué lo utilizamos?**  
Lo utilizamos como editor de código para desarrollar el Landing Page, porque permite escribir, editar y organizar archivos HTML, CSS y JavaScript de manera práctica y rápida. Además, lo utilizamos para hacer los commits.

### Google Chrome

**¿Por qué lo utilizamos?**  
Lo utilizamos para probar el funcionamiento del Landing Page, revisar la navegación y verificar cómo se veía en diferentes tamaños de pantalla usando las herramientas del navegador.

## Software Documentation

### GitHub

![Repositorio en GitHub](././/assets/diagrams/github.png)
![Gitflow_muestra.png](assets/images/cap-05/Gitflow_muestra.png)
**¿Por qué lo utilizamos?**  
Lo utilizamos para guardar, organizar y controlar las versiones del código fuente del proyecto. También permitió que varios integrantes trabajaran sobre el mismo proyecto sin perder cambios, además de dejar evidencia de participación mediante commits, ramas y repositorios.

## 5.1.2. Source Code Management.

GitFlow Implementation

Para aplicar el flujo de trabajo GitFlow en nuestro control de versiones con Git, tomamos como referencia el artículo “A successful Git branching model” de Vincent Driessen. Esta fuente nos ayudó a definir las convenciones que seguiremos en la organización de ramas dentro del proyecto.

![Gitflow_muestra.png](assets/images/cap-05/Gitflow_muestra.png)

# Git Workflow Strategy

## Main branch

La rama principal del proyecto es **`main`**. En ella se mantiene la versión estable del código, es decir, la que representa el estado más confiable y listo para producción del proyecto.

**Notación:**

```text
main
```

---

## Develop branch

La rama **`develop`** contiene los cambios y avances más recientes que todavía no forman parte de la versión final en producción. Esta rama se usa para integrar, revisar y probar las nuevas modificaciones antes de incorporarlas a la rama principal.

**Notación:**

```text
develop
```

---

## Release branch

La rama **`release`** se utiliza para preparar una nueva versión del producto antes de su publicación. En esta rama se pueden realizar ajustes finales y correcciones necesarias, mientras la rama **`develop`** puede seguir recibiendo nuevos avances del proyecto.

Esta rama se crea a partir de **`develop`** y, una vez finalizada, debe fusionarse tanto con **`develop`** como con **`main`**.

**Notación:**

```text
release
```

---

## Feature branch

Las ramas **`feature`** se utilizan para desarrollar nuevas funciones o mejoras específicas del producto que se incorporarán en versiones posteriores. Cada una de estas ramas permite trabajar una característica de forma separada, sin afectar directamente la rama principal de desarrollo.

Estas ramas deben crearse a partir de **`develop`** y, cuando la funcionalidad esté terminada, deben fusionarse nuevamente en **`develop`**.

**Notación:**

```text
feature
```

---

# Convenciones de nombres

| Tipo de rama     | Convención                         |
| ---------------- | ---------------------------------- |
| Main branch      | `main`                             |
| Develop branch   | `develop`                          |
| Feature branches | `feature/<feature-name>`           |
| Release branches | `release/v<major>.<minor>.<patch>` |
| Hotfix branches  | `hotfix/<fix-name>`                |

---

# Conventional Commits

**Conventional Commits** es una convención que se usa para escribir los mensajes de commit de manera ordenada, clara y consistente. Su objetivo es que cada cambio en el código pueda entenderse rápidamente y que el historial del repositorio sea más fácil de leer y seguir.

Este enfoque también ayuda a identificar el tipo de cambio realizado, mejora la comunicación dentro del equipo y facilita el seguimiento del avance del proyecto a lo largo del tiempo.

| Tipo       | Descripción                                                   |
| ---------- | ------------------------------------------------------------- |
| `feat`     | Used to add a new feature                                     |
| `fix`      | Used to correct a bug or error                                |
| `docs`     | Used to update documentation                                  |
| `style`    | Used for formatting or style changes without affecting logic  |
| `refactor` | Used to improve code structure without changing functionality |
| `test`     | Used to add or modify tests                                   |
| `chore`    | Used for maintenance tasks or minor project changes           |
| `perf`     | Used to improve performance                                   |

---

## Repositorios del proyecto (GitHub)

El código fuente de cada producto se gestiona en repositorios independientes dentro de la organización pública del equipo en GitHub (**upc-pre-202610-1asi0730-12258-Scripters**).

| **Producto**                   | **Repositorio (URL)**                                                          |
| ------------------------------ | ------------------------------------------------------------------------------ |
| **Landing Page**               | https://github.com/upc-pre-202610-1asi0730-12258-Scripters/Regula-Web-Site.git |
| **Frontend Web Application**   | https://github.com/upc-pre-202610-1asi0730-12258-Scripters/Regula-Frontend.git |
| **Web Services (RESTful API)** | https://github.com/upc-pre-202610-1asi0730-12258-Scripters/regula-platform.git |


# 5.1.3. Source Code Style Guide & Conventions

Como regla general, todo el código fuente desarrollado durante el proyecto estará redactado en **inglés**. Esto incluye nombres de archivos, variables, funciones, clases, identificadores y comentarios cuando sean necesarios.

El propósito de esta convención es mantener un código uniforme, entendible y fácil de mantener para todos los integrantes del equipo. Además, seguir estándares comunes facilita el trabajo colaborativo y permite comprender más rápidamente la estructura del proyecto.

---

# HTML

Para el desarrollo en HTML, el equipo seguirá convenciones orientadas a mejorar la claridad, la estructura y la accesibilidad del código.

## Usar nombres de elementos en minúsculas

Las etiquetas HTML deben escribirse en minúsculas para conservar la consistencia y ajustarse a las prácticas estándar de desarrollo web.

```html
<body>
    <p>This is a paragraph</p>
</body>
```

---

## Cerrar correctamente todos los elementos HTML

Los elementos deben cerrarse de forma adecuada para mantener una estructura válida y fácil de leer.

```html
<body>
    <p>This is a paragraph</p>
    <p>This is another paragraph</p>
</body>
```

---

## Usar nombres de atributos en minúsculas

Los atributos también deben escribirse en minúsculas para mantener uniformidad en el código.

```html
<a href="https://www.w3schools.com/html/">
    Visit our HTML tutorial
</a>
```

---

## Incluir siempre el atributo `alt` y, cuando corresponda, `width` y `height`

Las imágenes deben contener un texto alternativo descriptivo mediante `alt`, mejorando la accesibilidad y proporcionando contexto cuando la imagen no pueda visualizarse.

```html
<img src="html5.gif"
     alt="HTML5 logo"
     style="width:128px;height:128px">
```

---

## Escribir los atributos de forma ordenada y consistente

Se debe evitar desorden o espaciado innecesario dentro de las etiquetas para conservar un código limpio y legible.

```html
<link rel="stylesheet" href="styles.css">
```

---

# CSS

Para CSS, el equipo priorizará nombres descriptivos y reglas organizadas para facilitar el mantenimiento de la interfaz.

## Usar nombres significativos para clases e identificadores

```css
#gallery {}

#login {}

.video {}
```

---

## Utilizar nombres cortos pero descriptivos

```css
#nav {}

.author {}
```

---

## Usar propiedades abreviadas cuando sea posible

```css
border-top: 0;
font: 100%/1.6 palatino, georgia, serif;
padding: 0 1em 2em;
```

---

## Evitar unidades innecesarias en valores cero

```css
margin: 0;
padding: 0;
```

---

## Mantener un orden consistente en las declaraciones

```css
background: fuchsia;
border: 1px solid;
border-radius: 4px;
color: black;
text-align: center;
text-indent: 2em;
```

---

# JavaScript

En JavaScript, el equipo adoptará convenciones que ayuden a que la lógica del programa sea clara, ordenada y fácil de mantener.

## Usar una sintaxis expandida y legible

```javascript
function myFunc() {
    console.log('Hello!');
}
```

---

## Usar `lowerCamelCase` para nombres de variables

```javascript
let playerScore = 0;
let speed = distance / time;
```

---

## Preferir `let` y `const` en lugar de `var`

```javascript
const myName = 'Chris';

console.log(myName);

let myAge = 40;

myAge++;

console.log('Happy birthday!');
```

---

## Usar `lowerCamelCase` para nombres de funciones

```javascript
function sayHello() {
    alert('Hello!');
}
```

---

# C#

Aunque el enfoque principal está puesto en el Landing Page, el equipo define desde esta etapa las convenciones que aplicará posteriormente en el desarrollo de servicios con ASP.NET Core y C# para mantener consistencia en todo el proyecto.

## Usar `PascalCase` para clases y métodos

```csharp
public class MyClass
{
    public void ExampleMethod()
    {
        // Method code
    }
}
```

---

## Usar `camelCase` para variables y parámetros

```csharp
public class MyClass
{
    public void ExampleMethod(int exampleNumber)
    {
        string exampleName = "Example";
    }
}
```

---

## Mantener una longitud razonable de línea

```csharp
public class MyClass
{
    public void ExampleMethod()
    {
        string message =
            "This is an example message that spans multiple lines " +
            "to demonstrate how to maintain a reasonable length.";

        Console.WriteLine(message);
    }
}
```

---

## Escribir comentarios claros y útiles

```csharp
public class MyClass
{
    // This method performs an addition operation and returns the result.
    public int Add(int a, int b)
    {
        return a + b;
    }
}
```

---

## Aplicar el principio de responsabilidad única

```csharp
public class MathematicalOperations
{
    public int Add(int a, int b)
    {
        return a + b;
    }

    public int Subtract(int a, int b)
    {
        return a - b;
    }
}
```

---

# Lenguaje Gherkin

Para los criterios de aceptación y la descripción de comportamientos esperados, el equipo seguirá convenciones que permitan redactar escenarios claros y fáciles de entender desde la perspectiva del negocio.

## Usar títulos descriptivos y concisos para los escenarios

```gherkin
Feature: Login

Scenario: Successful login
    Given a user is on the login page
    When they enter valid credentials
    Then they should be logged in successfully
```

---

## Mantener la estructura `Given - When - Then`

```gherkin
Scenario: Adding items to the shopping cart

Given the user is on the shopping page
When they add an item to the cart
Then the item should appear in the cart
```

---

## Usar un lenguaje entendible para el negocio

```gherkin
Scenario: Changing user settings

Given the user is logged in
When they navigate to the settings page
Then they should be able to update their profile
```

---

## Usar `Scenario Outline` cuando existan varios casos similares

```gherkin
Scenario Outline: Searching for products

Given the user is on the search page
When they search for "<product>"
Then they should see search results for "<product>"

Examples:
| product    |
| Laptop     |
| Smartphone |
```

---

## Agregar comentarios cuando se necesite contexto adicional

```gherkin
# This scenario checks the functionality of the logout feature

Scenario: User logout

Given the user is logged in
When they click on the logout button
Then they should be redirected to the login page
```
# 5.1.4. Software Deployment Configuration

Esta sección describe la configuración y los pasos necesarios para desplegar satisfactoriamente los productos digitales de la solución a partir de sus repositorios de código fuente.

Para la entrega actual, el alcance del despliegue corresponde únicamente al **Landing Page**. La configuración de despliegue de las **Frontend Web Applications** y de los **RESTful Web Services** será documentada en los Sprints en los que inicie su desarrollo.

---

# Despliegue del Landing Page (GitHub Pages + GitHub Actions)

El **Landing Page** se despliega mediante **GitHub Pages**, utilizando **GitHub Actions** para automatizar el proceso de integración y publicación continua.

## Pasos de configuración

1. **Crear el repositorio**

   Crear el repositorio del Landing Page dentro de la organización del equipo en GitHub y agregar a todos los integrantes como colaboradores.

2. **Subir el código fuente**

   Publicar el código fuente del proyecto (**HTML5**, **CSS3** y **JavaScript**) siguiendo la estrategia de ramas definida mediante **GitFlow**.

3. **Configurar GitHub Pages**

   Acceder a:

   ```text
   Settings → Pages
   ```

   y configurar:

  * **Source:** `Deploy from a branch`
  * **Branch:** `main`
  * **Folder:** `/ (root)`

4. **Configurar GitHub Actions**

   Crear un workflow de **GitHub Actions** que publique automáticamente el sitio cada vez que se integren cambios en la rama principal.

5. **Verificar el despliegue**

   Acceder a la URL pública generada por GitHub Pages y comprobar que todas las secciones del Landing Page se carguen correctamente.

---

## Publicación continua

Una vez completada la configuración anterior, cada cambio integrado en la rama **`main`** será publicado automáticamente en la URL pública del Landing Page, eliminando la necesidad de realizar procesos manuales de despliegue.

---

# Despliegue de Frontend Web Applications y Web Services

La configuración de despliegue de la **Frontend Web Application (Vue)** y de los **RESTful Web Services (ASP.NET Core)** será definida e implementada en los Sprints correspondientes a su desarrollo.

En dichas etapas se documentarán:

* El proveedor de nube utilizado.
* Los entornos de despliegue (desarrollo, pruebas y producción).
* La estrategia de integración y entrega continua (CI/CD).
* Los pasos necesarios para la publicación de cada producto.
* La configuración específica de infraestructura y servicios asociados.

Esta documentación será incorporada conforme avance el desarrollo del proyecto.








# 5.2.1. Sprint 1

El **Sprint 1** marca el inicio del trabajo de construcción dentro del enfoque ágil del proyecto. En esta primera iteración, el equipo se centra en desarrollar las funcionalidades más importantes definidas en la planificación inicial, llevando los requerimientos a una primera versión funcional del producto.

De esta manera, se empieza a construir una base sólida de forma progresiva e incremental.

---

# 5.2.1.1. Sprint Planning 1

## Información General

| Campo             | Información                |
| ----------------- | -------------------------- |
| **Sprint #**      | Sprint 1                   |
| **Fecha**         | 2026-04-18                 |
| **Hora**          | 11:00 PM                   |
| **Ubicación**     | Microsoft Teams (Virtual)  |
| **Preparado por** | Ramos Cerdan, Elias Daniel |

### Asistentes

* Tello Palacios, Fabrizio Rafael
* Espinoza Lopez, Paul Alexandro Angel
* Ramos Cerdan, Elias Daniel
* Lopez Torres, Leonardo Gabriel
* Lopez Montalvo, Kevin Edu

---

## Sprint Review Summary

Se lograron varios de los objetivos planteados para el producto, como el desarrollo de todos los capítulos del informe, el despliegue completo del **Landing Page** y la incorporación de la mayor parte de la información requerida en el reporte.

No obstante, una de las metas más importantes que también debía cumplirse fue la entrega del informe en formatos **PDF** y **Word**.

---

## Sprint Retrospective Summary

El Sprint 1 permitió completar satisfactoriamente el trabajo planificado; sin embargo, varias mejoras y correcciones tuvieron que realizarse en los momentos finales de la entrega.

Durante la retrospectiva, el **Team Leader** identificó las siguientes oportunidades de mejora:

* Mayor compromiso por parte de todos los integrantes.
* Realizar reuniones diarias para mantener el seguimiento del avance.
* Incrementar la comunicación entre los miembros del equipo.

---

## Sprint Goal

> **Nuestro enfoque está en lograr la primera versión funcional y desplegada del Landing Page, junto con la primera versión completa del informe correspondiente a la entrega AV1.**
>
> Creemos que esto aporta una primera presentación clara, accesible y funcional de la propuesta de valor del proyecto para los visitantes y stakeholders.
>
> El objetivo se considerará cumplido cuando el Landing Page esté publicado y accesible sin inconvenientes, sus principales secciones funcionen correctamente y el informe haya sido finalizado en el formato requerido.

---

## Sprint Velocity

| Métrica                 | Valor           |
| ----------------------- | --------------- |
| **Sum of Story Points** | *(Por definir)* |

---

# 5.2.1.2. Aspect Leaders and Collaborators

| Team Member                              | GitHub        | Navigation Bar / Hero | Beneficios / ¿Cómo funciona? | Planes | FAQ / Footer | Internacionalización |
| ---------------------------------------- | ------------- | :-------------------: | :--------------------------: | :----: | :----------: | :------------------: |
| **Tello Palacios, Fabrizio Rafael**      | `F4bris`      |           C           |               L              |    L   |       C      |           C          |
| **Espinoza Lopez, Paul Alexandro Angel** | `R3memo`      |           C           |               C              |    C   |       C      |           C          |
| **Ramos Cerdan, Elias Daniel**           | `eliocerdan`  |           L           |               C              |    C   |       C      |           C          |
| **Lopez Torres, Leonardo Gabriel**       | `Deiko-138`   |           C           |               C              |    C   |       C      |           C          |
| **Lopez Montalvo, Kevin Edu**            | `Lopescamos`  |           C           |               C              |    C   |       C      |           C          |
| **David Ignacio Vivar Cesar**            | `DarkBeider2` |           C           |               C              |    C   |       L      |           L          |

> **L = Leader**
> **C = Collaborator**

---

# 5.2.1.3. Sprint Backlog 1

| User Story                            | Task                                              | Descripción                                                                     | Horas | Responsable               | Estado |
| ------------------------------------- | ------------------------------------------------- | ------------------------------------------------------------------------------- | :---: | ------------------------- |:------:|
| **US-47 Hero Visualization**          | **T01** Implementar barra de navegación           | Crear la barra superior con logo, navegación principal y botón de crear cuenta. |   1   | Fabrizio Rafael Tello     |  Done  |
|                                       | **T02** Implementar sección Hero                  | Maquetar título principal, texto descriptivo, botón CTA e imagen principal.     |   2   | Paul Alexandro Espinoza   |  Done  |
|                                       | **T03** Configurar navegación del botón principal | Redirigir correctamente el botón "Empezar Ahora".                               |   1   | Fabrizio Rafael Tello     |  Done  |
| **US-48 Features Review**             | **T04** Redactar beneficios principales           | Adaptar los textos de beneficios a la propuesta de valor.                       |   1   | Paul Alexandro Espinoza   |  Done  |
| **US-49 Revisión de características** | **T05** Implementar sección de características    | Crear tarjetas de funcionalidades de la plataforma.                             |   2   | Kevin Edu Lopez           |  Done  |
|                                       | **T06** Ajustar contenido de características      | Revisar la claridad de cada característica.                                     |   1   | Kevin Edu Lopez           |  Done  |
| **US-50 Benefits Inquiry**            | **T07** Implementar sección de planes             | Crear las tarjetas de planes.                                                   |   3   | Elias Daniel Ramos        |  Done  |
|                                       | **T08** Agregar precios y beneficios              | Incorporar precios y características por plan.                                  |   2   | Elias Daniel Ramos        |  Done  |
|                                       | **T09** Implementar selector mensual/anual        | Agregar alternancia entre modalidad mensual y anual.                            |   2   | Elias Daniel Ramos        |  Done  |
|                                       | **T10** Agregar CTA de asesoría                   | Implementar el bloque "¿No sabes qué plan elegir?".                             |   1   | Elias Daniel Ramos        |  Done  |
| **US-49 Login and Sign Up**           | **T14** Implementar sección de contacto           | Crear el bloque "Contáctanos".                                                  |   3   | David Ignacio Vivar Cesar |  Done  |
|                                       | **T15** Crear formulario de solicitud             | Agregar campos del formulario de contacto.                                      |   2   | David Ignacio Vivar Cesar |  Done  |
|                                       | **T16** Validaciones básicas                      | Verificar campos obligatorios y política de privacidad.                         |   2   | David Ignacio Vivar Cesar |  Done  |
|                                       | **T17** Implementar Footer                        | Crear el pie de página con enlaces legales.                                     |   1   | David Ignacio Vivar Cesar |  Done  |
| **US-40 Internacionalización**        | **T18** Preparar textos para internacionalización | Separar textos para futuras traducciones.                                       |   2   | David Ignacio Vivar Cesar |  Done  |
|                                       | **T19** Crear recursos español e inglés           | Definir claves de traducción para toda la landing.                              |   3   | David Ignacio Vivar Cesar |  Done  |
|                                       | **T20** Validar cambio de idioma                  | Comprobar coherencia visual al cambiar de idioma.                               |   2   | David Ignacio Vivar Cesar |  Done  |

---

## Resumen del Sprint Backlog

* **Total de User Stories:** 5
* **Total de tareas:** 16
* **Estado general:** Todas las tareas completadas.
* **Resultado:** Se alcanzó la primera versión funcional del Landing Page con soporte de internacionalización, navegación, planes, formulario de contacto y secciones principales completamente implementadas.

# 5.2.1.4. Development Evidence for Sprint Review

A continuación, se presenta el reporte de control de cambios del repositorio **Regula-website**, gestionado por el equipo **Scripters**. Este historial refleja la evolución del desarrollo del Landing Page, incluyendo la implementación inicial, la incorporación del soporte multilenguaje y las configuraciones relacionadas con la integración y despliegue continuo (CI/CD).

| **Repository**                                           | **Branch**      | **Commit ID**                              | **Commit Message**                                               | **Date** |
| -------------------------------------------------------- | --------------- | ------------------------------------------ | ---------------------------------------------------------------- | :------: |
| `upc-pre-202610-1asi0730-12258-Scripters-Regula-website` | `feature/index` | `de24ed6071c7c331fda41232b4b26eac19b03fa0` | `Add multilingual support with Spanish and English translations` |   23/04  |
| `upc-pre-202610-1asi0730-12258-Scripters-Regula-website` | `feature/index` | `d2da75d07fe0ff34723fd7f94590cbf786d1306e` | `initial commit`                                                 |   23/04  |
| `upc-pre-202610-1asi0730-12258-Scripters-Regula-website` | `develop`       | `c4d2f2b7c326eb6d035a9c2e6102ebd664b20ca3` | `ci: cambios en integración/despliegue continuo`                 |   05/05  |
| `upc-pre-202610-1asi0730-12258-Scripters-Regula-website` | `develop`       | `a79dfe35868af29907e475a3e2074747941c0315` | `Merge branch 'hotfix/workflow-deploy'`                          |   05/05  |
| `upc-pre-202610-1asi0730-12258-Scripters-Regula-website` | `develop`       | `f5e2ddd2adf6113d2ad459b94d3a0b93350cdabf` | `Merge tag 'workflow-deploy' into develop`                       |   05/05  |

---

# 5.2.1.5. Execution Evidence for Sprint Review

## Evidencia 1 – Página principal (Hero Section)
![1.png](assets/images/cap-05/1.png)


> *(Insertar captura de pantalla correspondiente.)*

La siguiente captura muestra la pantalla principal del **Landing Page de REGULA**, un sistema inteligente para el monitoreo de cilindros de gas.

El diseño incorpora un fondo con temática industrial donde se observa un operario junto a un camión de carga. Sobre este fondo destaca un título principal acompañado de dos botones de acción, uno de ellos resaltado en color naranja para solicitar una demostración del sistema.

En la parte superior se encuentra la barra de navegación con las opciones principales, mientras que en la parte inferior se presentan tres beneficios destacados junto al eslogan de la plataforma.

---

## Evidencia 2 – Sección About Us y Benefits

![2.png](assets/images/cap-05/2.png)

> *(Insertar captura de pantalla correspondiente.)*

Esta evidencia muestra la sección **About Us** y el inicio de la sección **Benefits**.

Sobre un fondo azul oscuro se presenta una descripción general de REGULA y, debajo, cuatro tarjetas informativas con iconografía que describen:

* Ayuda ofrecida por la plataforma.
* Propuesta de valor.
* Misión.
* Visión.

En la parte inferior comienza la sección **"Everything you need to optimize your operations"**, donde se introducen las funcionalidades principales del sistema.

---

## Evidencia 3 – Sección Benefits


![3.png](assets/images/cap-05/3.png)
> *(Insertar captura de pantalla correspondiente.)*

La sección **Benefits** organiza las funcionalidades del sistema en una cuadrícula compuesta por seis tarjetas informativas.

Entre las principales características se encuentran:

* Monitoreo en tiempo real.
* Prevención de fugas de gas.
* Control de inventario.
* Gestión de distribución.
* Reportes inteligentes.
* Acceso desde cualquier lugar.

Finalmente, una barra inferior destaca el compromiso de la plataforma con la seguridad y confiabilidad del servicio.

---

## Evidencia 4 – Sección Plans

![4.png](assets/images/cap-05/4.png)

> *(Insertar captura de pantalla correspondiente.)*

La sección **Plans** presenta los distintos planes de suscripción disponibles para los clientes.

El usuario puede alternar entre modalidad **Monthly** y **Annual**, visualizando tres opciones:

| Plan                          | Precio     |
| ----------------------------- | ---------- |
| **Basic**                     | **S/ 99**  |
| **Standard** *(Most Popular)* | **S/ 199** |
| **Premium**                   | **S/ 349** |

Cada plan incluye una lista de beneficios específicos y un botón para seleccionar la suscripción correspondiente.

---

## Evidencia 5 – FAQ y Footer

![5.png](assets/images/cap-05/5.png)


La última evidencia muestra la sección **Frequently Asked Questions (FAQ)** y el **Footer** del Landing Page.

La sección FAQ está implementada mediante componentes tipo acordeón que responden preguntas frecuentes relacionadas con el funcionamiento del sistema.

El pie de página incluye:

* Logo de REGULA.
* Descripción breve de la plataforma.
* Enlaces a redes sociales.
* Navegación hacia las principales secciones del sitio.
* Enlaces legales y de contacto.

---

## Video Demostrativo

| Elemento       |![muestra_video.png](assets/images/cap-05/muestra_video.png)                                                                                                                                                                                                                                                                                                           |
| -------------- |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Demo Video** | https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a649_upc_edu_pe/IQAN0X585uvtQLbH5jFztyF9AQn7ygXYVZpqNAE-Og3lHe4?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=Y6vHjB  |
| **Duración**   | **00:28**                                                                                                                                                                                                                                                                                                                |

> El video demuestra el funcionamiento general del Landing Page, recorriendo las principales secciones implementadas durante el Sprint 1 y verificando su correcto comportamiento e integración.


# 5.2.1.6. Services Documentation Evidence for Sprint Review

El alcance de implementación definido para el **Sprint 1** comprendió exclusivamente el desarrollo y despliegue del **Landing Page de Regula**, por lo que no se contempló la construcción de **Web Services** durante esta iteración.

En consecuencia, **no se diseñó ni implementó ningún endpoint RESTful API**, motivo por el cual no existe documentación de servicios basada en **OpenAPI/Swagger** para presentar en esta sección.

La construcción del **RESTful API**, junto con su documentación técnica correspondiente, está prevista para los Sprints en los que se desarrolle la capa de servicios, de acuerdo con la priorización establecida en el **Product Backlog**.

En futuras iteraciones, esta sección incluirá:

* Tabla de endpoints implementados.
* Método HTTP correspondiente.
* Parámetros de entrada.
* Códigos de respuesta.
* Ejemplos de requests y responses.
* Documentación generada mediante OpenAPI/Swagger.
* Capturas de evidencia y enlaces al servicio publicado.

---

## Estado de la documentación de servicios

| Componente              | Estado                     |
| ----------------------- | -------------------------- |
| RESTful API             | ⏳ No implementado          |
| OpenAPI / Swagger       | ⏳ No disponible            |
| Endpoints documentados  | 0                          |
| Evidencias de servicios | No aplica para el Sprint 1 |

---

# 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante el **Sprint 1**, las actividades de despliegue estuvieron enfocadas en publicar la primera versión funcional del **Landing Page de Regula**, en concordancia con el **Sprint Goal** y el alcance definido para esta iteración.

![deloyment 1.png](assets/images/cap-05/deloyment%201.png)

El proceso de despliegue comprendió la configuración de la organización del equipo en GitHub, la habilitación del servicio de hosting mediante **GitHub Pages** y la automatización del proceso de publicación utilizando **GitHub Actions**.

---

## Creación de la organización y repositorio

El equipo configuró la organización pública:

```text
upc-pre-202610-1asi0730-12258-Scripters
```

Dentro de esta organización se creó el repositorio correspondiente al Landing Page y se agregaron todos los integrantes del equipo como colaboradores, permitiendo registrar de forma transparente la participación de cada miembro durante el desarrollo.

![deloyment 2.png](assets/images/cap-05/deloyment%202.png)


---

## Configuración del hosting mediante GitHub Pages

Se habilitó **GitHub Pages** como plataforma de hosting estático para el Landing Page.

La configuración utilizada fue la siguiente:

| Configuración | Valor                |
| ------------- | -------------------- |
| **Source**    | Deploy from a branch |
| **Branch**    | `main`               |
| **Folder**    | `/ (root)`           |

![deloyment 3.png](assets/images/cap-05/deloyment%203.png)

Gracias a esta configuración, el sitio queda publicado automáticamente en una URL pública accesible desde cualquier navegador web.

---

## Automatización del despliegue (CI/CD)

Con el objetivo de eliminar procesos manuales de publicación, el equipo configuró un **workflow de GitHub Actions** encargado de desplegar automáticamente el Landing Page cada vez que se integran cambios en la rama principal.

La evidencia de esta automatización puede observarse en los commits registrados durante el Sprint, incluyendo:

```text
ci: cambios en integración/despliegue continuo
```
![deloyment 4.png](assets/images/cap-05/deloyment%204.png)


Esta estrategia garantiza una integración continua (CI) y una entrega continua (CD), reduciendo errores durante el proceso de publicación.

---

## Verificación del despliegue

Como resultado del Sprint 1, el Landing Page quedó correctamente desplegado y disponible de forma pública.

### URL del proyecto

```text
https://upc-pre-202610-1asi0730-scripters.github.io/upc-pre-202610-1asi0730-12258-Scripters-Regula-website/
```

La validación del despliegue consistió en acceder al sitio desde distintos navegadores y verificar el correcto funcionamiento de todas las secciones implementadas.


![Deyploment 5.png](assets/images/cap-05/Deyploment%205.png)

Se comprobó el correcto funcionamiento de:
*  Hero Section
*  About Us
*  Benefits
*  Plans
*  FAQ
*  Footer
*  Cambio de idioma (Español / Inglés)

---

## Estado del despliegue por producto

| Producto                     | Estado                                      |
| ---------------------------- | ------------------------------------------- |
| **Landing Page**             | Desplegado y verificado mediante GitHub Pages |
| **Frontend Web Application** | Fuera del alcance del Sprint 1              |
| **RESTful Web Services**     | Fuera del alcance del Sprint 1              |

---


# 5.2.1.8. Team Collaboration Insights during Sprint

Durante el **Sprint 1**, las actividades de implementación se desarrollaron de forma colaborativa sobre el repositorio del **Landing Page (Regula-website)**, siguiendo la estrategia de trabajo basada en **GitFlow** definida por el equipo.

Cada integrante desarrolló sus tareas en ramas de tipo **`feature`**, correspondientes a las secciones del Landing Page asignadas en la matriz de líderes y colaboradores (Sección **5.2.1.2**). Posteriormente, los cambios fueron integrados a la rama **`develop`** mediante **Pull Requests**, utilizando la convención **Conventional Commits** para mantener un historial de cambios claro y organizado.

Gracias a este flujo de trabajo, el equipo logró mantener la trazabilidad del desarrollo mediante ramas, commits y revisiones de código, evidenciando la participación individual de cada integrante.

---

![team_collaboration.png](assets/images/cap-05/team_collaboration.png)
![team_collaboration.png.png](assets/images/cap-05/team_collaboration.png.png)
![team_collaboration.png.png.png](assets/images/cap-05/team_collaboration.png.png.png)

## Herramientas de colaboración

Durante el Sprint se utilizaron las siguientes herramientas para coordinar el trabajo del equipo:

| Herramienta         | Propósito                                                                                 |
| ------------------- | ----------------------------------------------------------------------------------------- |
| **GitHub**          | Control de versiones, gestión de ramas, Pull Requests y evidencia técnica del desarrollo. |
| **Trello**          | Planificación, asignación y seguimiento de tareas del Sprint.                             |
| **Microsoft Teams** | Reuniones de coordinación y seguimiento del avance del proyecto.                          |

---

## Flujo de trabajo aplicado

```text
feature/* 
      │
      ▼
Pull Request
      │
      ▼
develop
      │
      ▼
main
```

Cada funcionalidad fue desarrollada de manera independiente antes de ser integrada a la rama principal de desarrollo, reduciendo conflictos y facilitando la revisión del código.

---

## Evidencia de colaboración

A continuación, se presentan las capturas correspondientes a los analíticos de colaboración y al historial de commits del repositorio, las cuales evidencian el aporte realizado por cada integrante durante el Sprint.

### Analytics del repositorio

> *(Insertar captura de GitHub Insights - Contributors)*

---

### Historial de commits

> *(Insertar captura del historial de commits del repositorio)*

---

### Pull Requests y ramas

> *(Insertar captura de Pull Requests o Branches del repositorio)*

---

# Resumen de participación por integrante

| Integrante                               | Usuario de GitHub | Producto implementado | Aporte principal                                                      |
| ---------------------------------------- | ----------------- | --------------------- | --------------------------------------------------------------------- |
| **Tello Palacios, Fabrizio Rafael**      | `F4bris`          | Landing Page          | Barra de navegación, Hero y sección de planes.                        |
| **Espinoza Lopez, Paul Alexandro Angel** | `R3memo`          | Landing Page          | Implementación de la sección Hero y beneficios principales.           |
| **Ramos Cerdan, Elias Daniel**           | `eliocerdan`      | Landing Page          | Barra de navegación, Hero y sección de planes.                        |
| **Lopez Torres, Leonardo Gabriel**       | `Deiko-138`       | Landing Page          | Desarrollo de secciones de contenido y revisión general.              |
| **Lopez Montalvo, Kevin Edu**            | `Lopescamos`      | Landing Page          | Implementación de la sección de características y revisión funcional. |
| **David Ignacio Vivar Cesar**            | `DarkBeider2`     | Landing Page          | Desarrollo del FAQ, Footer e internacionalización del sitio.          |

---

## Participación por producto

| Producto                     | Estado de colaboración                               |
| ---------------------------- | ---------------------------------------------------- |
| **Landing Page**             | ✅ Implementado colaborativamente por todo el equipo. |
| **Frontend Web Application** | ⏳ Fuera del alcance del Sprint 1.                    |
| **RESTful Web Services**     | ⏳ Fuera del alcance del Sprint 1.                    |

---
# 5.2.2. Sprint 2

El **Sprint 2** representa la segunda iteración del proyecto y tiene como objetivo principal continuar con el desarrollo incremental de la solución, incorporando la primera versión funcional de la **Frontend Web Application de Regula** y mejorando el Landing Page desarrollado durante el Sprint anterior.

Durante esta iteración, el equipo se enfoca en implementar las funcionalidades esenciales que permitirán a los usuarios autenticarse en la plataforma y registrar digitalmente las operaciones de entrada y salida de balones de gas, sentando las bases para la digitalización de los procesos operativos de los distribuidores.

---

# 5.2.2.1. Sprint Planning 2

El **Sprint Planning 2** marca el inicio de la segunda iteración del proyecto. En esta reunión, el equipo revisó los resultados obtenidos en el Sprint anterior, analizó la retrospectiva realizada y definió el objetivo principal de la nueva iteración junto con los **User Stories** seleccionados para su implementación.

El foco del Sprint está orientado a entregar la **primera versión funcional y desplegada de la Frontend Web Application de Regula**, además de incorporar mejoras al Landing Page existente.

## Información General

| Campo           | Valor                            |
| --------------- | -------------------------------- |
| **Sprint #**    | Sprint 2                         |
| **Date**        | 2026-05-09                       |
| **Time**        | 11:00 PM                         |
| **Location**    | Google Meet                      |
| **Prepared By** | Kevin Lopez                      |
| **Attendees**   | Todos los integrantes del equipo |

---

## Sprint 1 Review Summary

Se alcanzó satisfactoriamente el objetivo principal del Sprint 1, logrando implementar y desplegar la primera versión funcional del **Landing Page** mediante GitHub Pages.

Las secciones **Hero, About Us, Benefits, Plans, FAQ y Footer** quedaron completamente operativas, incluyendo soporte de internacionalización.

Asimismo, se completó la primera versión del informe correspondiente a la entrega académica.

Como punto de mejora, parte del trabajo requirió correcciones durante la etapa final del Sprint.

---

## Sprint 1 Retrospective Summary

El equipo considera que el Sprint 1 fue productivo y permitió alcanzar los objetivos planteados.

Sin embargo, durante la retrospectiva se identificaron oportunidades de mejora:

* Incrementar el compromiso de todos los integrantes.
* Realizar reuniones de seguimiento con mayor frecuencia.
* Mantener una comunicación más constante entre los miembros del equipo.
* Reducir la carga de trabajo concentrada en los últimos días del Sprint.

---

## Sprint 2 Goal

> Nuestro enfoque está en ofrecer a las empresas y distribuidores de gas la **primera versión funcional y desplegada de la Frontend Web Application de Regula**, permitiéndoles acceder a la plataforma y registrar digitalmente las operaciones de entrada y salida de balones.
>
> Creemos que esta funcionalidad proporciona un reemplazo confiable para los registros manuales en papel y mejora significativamente el control operativo del inventario.
>
> El objetivo se considerará alcanzado cuando los usuarios puedan autenticarse en la aplicación web y registrar correctamente las operaciones de entrada y salida, visualizando el inventario actualizado en tiempo real.

---

## Sprint Velocity

| Métrica                 |  Valor |
| ----------------------- | :----: |
| **Sprint Velocity**     | **50** |
| **Sum of Story Points** | **70** |

---

# 5.2.2.2. Aspect Leaders and Collaborators

Durante el Sprint 2, la organización del trabajo se realizó tomando como referencia los **Bounded Contexts** definidos durante el diseño de la arquitectura de la solución.

Cada integrante asumió el rol de **Leader (L)** de uno o más bounded contexts específicos y colaboró como **Collaborator (C)** en otros módulos mediante revisiones de código y apoyo en el desarrollo.

Esta distribución favorece una mejor organización del trabajo y mantiene una relación directa con la asignación de tareas presentada en el Sprint Backlog.

## Leadership and Collaboration Matrix (LACX)

| Team Member                              | GitHub        | Distribution | Commercial Management | Report Analytics | Report Graphics | Inventory & Cylinder Tracking | Operational Analytics | Security & Alert Management |
| ---------------------------------------- | ------------- | :----------: | :-------------------: | :--------------: | :-------------: | :---------------------------: | :-------------------: | :-------------------------: |
| **Lopez Torres, Leonardo Gabriel**       | `Deiko-138`   |     **L**    |         **C**         |         -        |        -        |             **C**             |           -           |              -              |
| **Ramos Cerdan, Elias Daniel**           | `eliocerdan`  |     **C**    |         **L**         |         -        |        -        |               -               |           -           |              -              |
| **Tello Palacios, Fabrizio Rafael**      | `F4bris`      |       -      |           -           |       **L**      |      **C**      |               -               |         **C**         |              -              |
| **Lopez Montalvo, Kevin Edu**            | `Lopescamos`  |       -      |           -           |       **C**      |      **L**      |             **L**             |           -           |              -              |
| **Espinoza Lopez, Paul Alexandro Angel** | `R3memo`      |       -      |           -           |         -        |        -        |             **C**             |         **L**         |              -              |
| **David Ignacio Vivar Cesar**            | `DarkBeider2` |     **C**    |         **C**         |         -        |        -        |               -               |           -           |              -              |

> **L = Leader**
> **C = Collaborator**

---

La organización presentada en esta matriz guarda relación directa con la selección de tareas del **Sprint Backlog 2**, donde cada integrante lidera la implementación del bounded context bajo su responsabilidad y brinda apoyo en los módulos asignados como colaborador.

---

# 5.2.2.3. Sprint Backlog 2

El objetivo principal del **Sprint 2** es entregar la primera versión funcional y desplegada de la **Frontend Web Application de Regula**, permitiendo a los usuarios autenticarse y registrar digitalmente las operaciones de entrada y salida de balones de gas, junto con una versión mejorada del Landing Page.

Para lograr este objetivo, el equipo descompuso los **User Stories** priorizados en un conjunto de **Work Items / Tasks**, asignando cada uno según el bounded context liderado por cada integrante.

---

## Tablero de Sprint (Trello)

### Captura del tablero

![Spring_2.png](../../Pictures/Screenshots/Spring_2.png)

---

### URL pública del tablero

```text
https://trello.com/invite/b/68463601cda325ff0368125a/ATTIc7b4c3f9952980aa5b47d7f492e7ebab4EF89533/sprint-2
```

---


5.2.2.4.Development Evidence for Sprint Review.

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/security-and-alert-management|121dbe56440d98269bdfeb86ef9459dc6681b2dc|feat(security): refactor alert and warehouse entity constructors for improved readability and consistency|03/06/2026|
|Regula-Frontend|feature/security-and-alert-management|40bb661ad3367482e90d8e1bf6cfdda0850a2b4f|feat: add warehouse and company alert history|29/05/2026|
|Regula-Frontend|feature/security-and-alert-management|1fcd6ca7348155ab5051cb7a48c429c31fffd1c8|feat(security): add company alerts and warehouse status management views|28/05/2026|
|Regula-Frontend|feature/security-and-alert-management|a8e0924eda9ef72a95621ba9534db7ee1fa24220|feat(security): implement i18n for active alerts and history views|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|2c7bd6f7fd20bae74c15ec07e6bf492ce7a9a29e|feat(i18n): config translation support|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|ccce051d019f4253881550070b8523f121777fb7|feat(i18n): add translation support for navbar labels|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|75ad61e674ff95816c5f74bda127a653705a8053|feat(routing): add security hub container with nested child routes|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|9e4b33dba08a4a4e1f838c71080b703624ca23ce|feat(presentation): add operational security management views|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|94eba50508b10eeb34191d272254cc2a3393b4a2|feat(presentation): add security routes for operational security|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|288754dd874dd91665ec8477f79466b6a93c1d16|feat(infrastructure): add security API and assemblers|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|df807758e72edc22b61beeb55bb553b7c475eeb6|feat(domain): add operational-security domain entities|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|7f32e16b78e75e7d076ee5783ac1e30cb5f60ccb|feat(store): add Pinia security store for operations|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|20480336b0020b1d6cb1628bf18c5ac852da2f2f|chore(config): update json server|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|3efb97d4e674c1e9a3ce7d48bec9d832fc9c8f79|fix: json-server; update lockfile & remove BOM|<p>11/05/2026</p><p><br></p>|
|Regula-Frontend|develop|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/inventory-management|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/inventory-management|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/inventory-management|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/inventory-management|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/inventory-management|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/inventory-management|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/inventory-management|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/inventory-management|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/inventory-management|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/inventory-management|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/inventory-management|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/inventory-management|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/inventory-management|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/inventory-management|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/inventory-management|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/inventory-management|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/inventory-management|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/inventory-management|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/inventory-management|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/inventory-management|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/inventory-management|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/inventory-management|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/inventory-management|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/inventory-management|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/inventory-management|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/inventory-management|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/inventory-management|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/inventory-management|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/inventory-management|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/inventory-management|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/inventory-management|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-management|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/inventory-management|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-management|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-management|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/inventory-management|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/inventory-management|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/inventory-management|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/inventory-management|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/security-and-alert-management|121dbe56440d98269bdfeb86ef9459dc6681b2dc|feat(security): refactor alert and warehouse entity constructors for improved readability and consistency|03/06/2026|
|Regula-Frontend|feature/security-and-alert-management|40bb661|feat: add warehouse and company alert history|29/05/2026|
|Regula-Frontend|feature/security-and-alert-management|1fcd6ca|feat(security): add company alerts and warehouse status management views|28/05/2026|
|Regula-Frontend|feature/security-and-alert-management|a8e0924|feat(security): implement i18n for active alerts and history views|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|2c7bd6f|feat(i18n): config translation support|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|ccce051|feat(i18n): add translation support for navbar labels|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|75ad61e|feat(routing): add security hub container with nested child routes|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|9e4b33d|feat(presentation): add operational security management views|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|94eba50|feat(presentation): add security routes for operational security|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|288754d|feat(infrastructure): add security API and assemblers|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|dfb0775|feat(domain): add operational-security domain entities|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|7f32e16|feat(store): add Pinia security store for operations|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|2048033|chore(config): update json server|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|3efb97d|fix: json-server; update lockfile & remove BOM|11/05/2026|
|Regula-Frontend|feature/security-and-alert-management|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/security-and-alert-management|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/security-and-alert-management|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/commercial-management-distributor|fb2f06866ec3d9e1aa6c090af0d088bcbffcbb34|chore(commercial): remove unused gitkeep files|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|9f63eec68110eaa21fd55381a163565c15c2d5db|feat(assets): add commercial cylinder icon|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|87a1cc8f74b1b323c63dd78b20e3853cba1df122|chore(dependencies): sync package lock|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|afc26fabdc069a5fac63cb018b681638e46089b6|chore(data): update sales and debts data|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|0b41f0d64c6ea34bcf63f68adf70394c68c2d2be|feat(commercial): add distributor sales view|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|efbdcc653ddce6362a1c63d8758ac2463eaa09d4|feat(commercial): add distributor debts view|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|76c3805262b077c06cb0330df39ba237513729d0|feat(commercial): add sales table|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|21e3313f0b1f2a8e7c5da7c8e6b5821d160a0daf|feat(commercial): add sales summary panel|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|19f9325e3c0c446d64c190915dffc720e6a38e1e|feat(commercial): update register sale dialog|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|633672322ce40bf4198d4a5f87d2f0f31bb47c00|feat(commercial): update register payment panel|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|91b8e18159097bfbdb7bce0fc3e52f4845beaf8e|feat(commercial): update register debt panel|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|4640f16f5cb255d20a6a2e1eb24f387484edca8f|feat(commercial): update pending debts panel|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|fcbbedc76294c30bbcba6d9293b9fc6ff924bb68|feat(commercial): add commercial history panel|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|ea56810050ce7a102decb3ce1a50d8cf9b83f238|feat(commercial): update commercial store for sale and debts|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|d0e1d72f471a19016f28f0af125b0205823f7a94|feat(commercial): update commercial api|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|b508f724e9441d4fcab25dd683dfca64b3206241|feat(commercial): add cylinder type assembler|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|dfcf51e5b33643e7b630f91ea4b83e334c7a6992|feat(commercial): add debt movement assembler|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|d300b1fe753b1d74be2ef14ce1e8f69379a193da|feat(commercial): add client assembler|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|f87d7935fe320c8e0e0e1f5ee1352575c1f3eb89|feat(commercial): add sale assembler|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|b5ad2d818bd2c9d6fd75832402ea84a2f056817e|feat(commercial): add sale entity|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|da5f341a04dfdb39a744b50b979b98226ac165d6|feat(commercial): add debt movement entity|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|c30ecfbd2e96373efc6282ea7a5f83b1b7b401b3|feat(commercial): add cylinder type entity|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|8078b691ea601bd6c8384beaf18fc9f5c0ee1ab6|feat(commercial): add client entity|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|43ea797c474ec919fb6d20ba32aa1118b6dacdc7|feat(navigation): update debt management navigation|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|f2b2e52498d940f0a5ec72e9aa356499dd89248c|feat: update debt management routes|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|cfda3dffa3682928c5f245171c628abb5edcac85|feat: add distributor commercial sales module|03/06/2026|
|Regula-Frontend|feature/commercial-management-distributor|856e709a09f99a2053f60cd40acca852d7c3604a|refactor(main): simplify import paths for i18n, pinia, and router modules|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|2c8704b24794f7ce241a4c7a52883d8fa2ae013b|feat(styles): add Regula brand tokens and typography styles to enhance UI consistency|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|f848e45a9ebb71b4ed62145531108d64947fc377|feat(navbar): simplify app-navbar and enhance navigation for enterprise and distributor roles|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|0717c639adf3f2133b0e925c6d1f20515005e38b|refactor(i18n): update import paths for localization files|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|314a7061e38822e67c188e2368733d8732bfaa8b|refactor(pinia): move pinia.js to root directory for improved structure|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|f416863010055ea06418868cab9e6585f5078787|feat(router): add main router configuration with inventory routes and role selection|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|7eb357f04a3b98a9876b701a03df606d69c05905|feat(routes): add inventory route definitions for enterprise and distributor views|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|151a801f04ea81d8a16a206f41a035e021a6a2b6|feat(inventory): refactor inventory store usage and enhance data fetching in panels|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|e24f9e54af16ca3d248c59cb49648553ba8cc082|feat(distributor): refactor inventory store usage in distributor panels|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|b0cbb31791561ec267c644d2f3dd3ddfe4fcb106|feat(store): enhance inventory store with additional data handling for origins, providers, and stock kg maps|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|476784f0adcae7b2501231d15332fb867f3ee66c|feat(api): add summary documentation for inventory API service|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|fd5355152ec186b1a4413728198e38e8644e4824|feat(assembler): add inventory, origin, provider, and stock kg map assemblers for resource transformation|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|68bc03008b266f70684087e2948ca3229b11cfc9|feat(entity): add new entity classes for audit logs, distributor movements, inventory movements, and related models|24/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|58b6771b17373854955053dd771b719e4cab457f|fix(deps): downgrade json-server to version 0.17.4|23/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/commercial-management-distributor|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/iam|856e709a09f99a2053f60cd40acca852d7c3604a|refactor(main): simplify import paths for i18n, pinia, and router modules|24/05/2026|
|Regula-Frontend|feature/iam|2c8704b24794f7ce241a4c7a52883d8fa2ae013b|feat(styles): add Regula brand tokens and typography styles to enhance UI consistency|24/05/2026|
|Regula-Frontend|feature/iam|f848e45a9ebb71b4ed62145531108d64947fc377|feat(navbar): simplify app-navbar and enhance navigation for enterprise and distributor roles|24/05/2026|
|Regula-Frontend|feature/iam|0717c639adf3f2133b0e925c6d1f20515005e38b|refactor(i18n): update import paths for localization files|24/05/2026|
|Regula-Frontend|feature/iam|314a7061e38822e67c188e2368733d8732bfaa8b|refactor(pinia): move pinia.js to root directory for improved structure|24/05/2026|
|Regula-Frontend|feature/iam|f416863010055ea06418868cab9e6585f5078787|feat(router): add main router configuration with inventory routes and role selection|24/05/2026|
|Regula-Frontend|feature/iam|7eb357f04a3b98a9876b701a03df606d69c05905|feat(routes): add inventory route definitions for enterprise and distributor views|24/05/2026|
|Regula-Frontend|feature/iam|151a801f04ea81d8a16a206f41a035e021a6a2b6|feat(inventory): refactor inventory store usage and enhance data fetching in panels|24/05/2026|
|Regula-Frontend|feature/iam|e24f9e54af16ca3d248c59cb49648553ba8cc082|feat(distributor): refactor inventory store usage in distributor panels|24/05/2026|
|Regula-Frontend|feature/iam|b0cbb31791561ec267c644d2f3dd3ddfe4fcb106|feat(store): enhance inventory store with additional data handling for origins, providers, and stock kg maps|24/05/2026|
|Regula-Frontend|feature/iam|476784f0adcae7b2501231d15332fb867f3ee66c|feat(api): add summary documentation for inventory API service|24/05/2026|
|Regula-Frontend|feature/iam|fd5355152ec186b1a4413728198e38e8644e4824|feat(assembler): add inventory, origin, provider, and stock kg map assemblers for resource transformation|24/05/2026|
|Regula-Frontend|feature/iam|68bc03008b266f70684087e2948ca3229b11cfc9|feat(entity): add new entity classes for audit logs, distributor movements, inventory movements, and related models|24/05/2026|
|Regula-Frontend|feature/iam|58b6771b17373854955053dd771b719e4cab457f|fix(deps): downgrade json-server to version 0.17.4|23/05/2026|
|Regula-Frontend|feature/iam|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/iam|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/iam|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/iam|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/iam|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/iam|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/iam|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/iam|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/iam|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/iam|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/iam|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/iam|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/iam|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/iam|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/iam|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/iam|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/iam|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/iam|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/iam|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/iam|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/iam|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/iam|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/iam|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/iam|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/iam|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/iam|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/iam|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/iam|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/iam|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/iam|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/iam|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/iam|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/iam|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/iam|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/iam|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/iam|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/iam|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/iam|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/iam|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/iam|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/iam-authentication|846b5bbe3a4fc470763faf4ba2b7e32a16abb72b|feat(iam): build sign-in and sign-up views integrated with vue router.|30/05/2026|
|Regula-Frontend|feature/iam-authentication|c3972aa14595f88eb3f9da14694bb62639a7b6da|feat(iam): configure state management store for reactive authentication tracking.|30/05/2026|
|Regula-Frontend|feature/iam-authentication|914fb00b33a97b735d34d2dbbf577a6ebde77616|refactor(iam): relocate data assemblers from shared to iam infrastructure layer.|30/05/2026|
|Regula-Frontend|feature/iam-authentication|581b7dacc08af9cd2aee8ee0c7443bbe12b58c51|feat(iam): implement infrastructure api client, resources and data assemblers.|30/05/2026|
|Regula-Frontend|feature/iam-authentication|e4dc1d399094dd0ceecceb33b728ebcd51dc94e3|feat(iam): define user core entity and authentication domain commands.|30/05/2026|
|Regula-Frontend|feature/iam-authentication|856e709a09f99a2053f60cd40acca852d7c3604a|refactor(main): simplify import paths for i18n, pinia, and router modules|24/05/2026|
|Regula-Frontend|feature/iam-authentication|2c8704b24794f7ce241a4c7a52883d8fa2ae013b|feat(styles): add Regula brand tokens and typography styles to enhance UI consistency|24/05/2026|
|Regula-Frontend|feature/iam-authentication|f848e45a9ebb71b4ed62145531108d64947fc377|feat(navbar): simplify app-navbar and enhance navigation for enterprise and distributor roles|24/05/2026|
|Regula-Frontend|feature/iam-authentication|0717c639adf3f2133b0e925c6d1f20515005e38b|refactor(i18n): update import paths for localization files|24/05/2026|
|Regula-Frontend|feature/iam-authentication|314a7061e38822e67c188e2368733d8732bfaa8b|refactor(pinia): move pinia.js to root directory for improved structure|24/05/2026|
|Regula-Frontend|feature/iam-authentication|f416863010055ea06418868cab9e6585f5078787|feat(router): add main router configuration with inventory routes and role selection|24/05/2026|
|Regula-Frontend|feature/iam-authentication|7eb357f04a3b98a9876b701a03df606d69c05905|feat(routes): add inventory route definitions for enterprise and distributor views|24/05/2026|
|Regula-Frontend|feature/iam-authentication|151a801f04ea81d8a16a206f41a035e021a6a2b6|feat(inventory): refactor inventory store usage and enhance data fetching in panels|24/05/2026|
|Regula-Frontend|feature/iam-authentication|e24f9e54af16ca3d248c59cb49648553ba8cc082|feat(distributor): refactor inventory store usage in distributor panels|24/05/2026|
|Regula-Frontend|feature/iam-authentication|b0cbb31791561ec267c644d2f3dd3ddfe4fcb106|feat(store): enhance inventory store with additional data handling for origins, providers, and stock kg maps|24/05/2026|
|Regula-Frontend|feature/iam-authentication|476784f0adcae7b2501231d15332fb867f3ee66c|feat(api): add summary documentation for inventory API service|24/05/2026|
|Regula-Frontend|feature/iam-authentication|fd5355152ec186b1a4413728198e38e8644e4824|feat(assembler): add inventory, origin, provider, and stock kg map assemblers for resource transformation|24/05/2026|
|Regula-Frontend|feature/iam-authentication|68bc03008b266f70684087e2948ca3229b11cfc9|feat(entity): add new entity classes for audit logs, distributor movements, inventory movements, and related models|24/05/2026|
|Regula-Frontend|feature/iam-authentication|58b6771b17373854955053dd771b719e4cab457f|fix(deps): downgrade json-server to version 0.17.4|23/05/2026|
|Regula-Frontend|feature/iam-authentication|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/iam-authentication|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/iam-authentication|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/iam-authentication|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/iam-authentication|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/iam-authentication|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/iam-authentication|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/iam-authentication|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/iam-authentication|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/iam-authentication|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/iam-authentication|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/iam-authentication|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/iam-authentication|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/iam-authentication|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/iam-authentication|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/iam-authentication|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/iam-authentication|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/iam-authentication|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/iam-authentication|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/iam-authentication|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/iam-authentication|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/iam-authentication|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/iam-authentication|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/iam-authentication|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/iam-authentication|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/iam-authentication|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/iam-authentication|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/iam-authentication|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/iam-authentication|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/iam-authentication|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/iam-authentication|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/iam-authentication|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/iam-authentication|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/iam-authentication|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/distribution|3a83d71184901b44c6e7d8142d70e5f27ba2640a|feat: add enterprise distribution management views and routes for application|29/05/2026|
|Regula-Frontend|feature/distribution|eefd6fbb4e9dc6479f1e1f30ff6fdfa76e83b117|feat: implement distribution logistics management with delivery and deliverer entities|27/05/2026|
|Regula-Frontend|feature/distribution|07de9472b791b5f9ac1d5d226980059ab176d198|feat: implement distribution logistics management with delivery and deliverer entities|27/05/2026|
|Regula-Frontend|feature/distribution|c55cf2331175879c9cc8f09c014da4cac96a3501|feat: add commercial management bounded context|13/05/2026|
|Regula-Frontend|feature/distribution|5916838bcaa0e619eb810ce568d688bba728771b|feat: add operational analytics reports bounded context|13/05/2026|
|Regula-Frontend|feature/distribution|f4536d8bfa9507847c6abdf6c3d1e935c203f438|feat: add english debt management translations|12/05/2026|
|Regula-Frontend|feature/distribution|3ac06db7acc7c6668fc17194b784b48c67577de3|feat: add spanish debt management translations|12/05/2026|
|Regula-Frontend|feature/distribution|642a39cbd7e3f389fb63486442316577bf48acae|feat: add i18n to debt management view|12/05/2026|
|Regula-Frontend|feature/distribution|c796961c9d2d7644ed3385166bcb77c8c2b6e716|feat: update debt management routes|12/05/2026|
|Regula-Frontend|feature/distribution|d5e018d51db426876b6fd7365e729391bc9c16db|feat: update debt management navigation|12/05/2026|
|Regula-Frontend|feature/distribution|498d5c326d5046ffb518a85e4a237a2361f3afa6|feat: add distributor sales view|12/05/2026|
|Regula-Frontend|feature/distribution|dfd877265fb82572c4ded515e61351fba0ee05fc|feat: add distributor debts view|12/05/2026|
|Regula-Frontend|feature/distribution|b527d838430eb7972ccf8035432a8726523110a3|feat: add register sale dialog|12/05/2026|
|Regula-Frontend|feature/distribution|69406922cd3b3a8257da4c24a2a3b97fb2fdc880|feat: add register payment panel|12/05/2026|
|Regula-Frontend|feature/distribution|d12ef3fe37e446c827b3f407020ac22fe2f5b3d7|feat: add register debt panel|12/05/2026|
|Regula-Frontend|feature/distribution|399e990ed5cd676273e87fbef8734d424f352eaa|feat: add pending debts panel|12/05/2026|
|Regula-Frontend|feature/distribution|d39ea5f5894eede9736451c6bb920df84936e1c8|feat: add commercial history panel|12/05/2026|
|Regula-Frontend|feature/distribution|bb9b5643c6bd6f0c3bd04d73034dad961512fc9b|feat: update commercial store|12/05/2026|
|Regula-Frontend|feature/distribution|b37899e6d7717cbe629d4baa5accc5b61bdd7c04|feat: update commercial api|12/05/2026|
|Regula-Frontend|feature/distribution|b2bb6e42350f5cd70699dc3ff7c0aa7b95f86e11|feat: add commercial assembler|12/05/2026|
|Regula-Frontend|feature/distribution|5d893d79d6d4d45821b27ac9314d15e3f6cd5107|feat: add sale entity|12/05/2026|
|Regula-Frontend|feature/distribution|280fc4d0a74a6b94822b68bb4e597a90f27ed461|feat: add debt movement entity|12/05/2026|
|Regula-Frontend|feature/distribution|9db813ec4328e9c1d5fdb17f82f2f6a66a5f3e4b|feat: add cylinder type entity|12/05/2026|
|Regula-Frontend|feature/distribution|5afac19e3e6d9053f5fe329fedca1cd3e7e304c4|feat: add client entity|12/05/2026|
|Regula-Frontend|feature/distribution|9193c33a463911e2aaaf68086aa4b895ca250ca6|feat(reports): implement analytics store and enhance report generation logic|12/05/2026|
|Regula-Frontend|feature/distribution|b1ecd1915a6113b451429df58ff006adf3ce1491|feat: add distributor sales and debt management views|12/05/2026|
|Regula-Frontend|feature/distribution|0277fc7026362af42ee401630a4d6e5e64de9213|feat(reports): improve code readability in generate report view|12/05/2026|
|Regula-Frontend|feature/distribution|64c502c98bd627b14ad0904950aa43dfb72a3286|feat(reports): add generate report view and localization support|12/05/2026|
|Regula-Frontend|feature/distribution|e539cb3bf3a909e61b5180899a4a1483a9ea6845|feat: add distributor commercial sales module|12/05/2026|
|Regula-Frontend|feature/distribution|a8e0924eda9ef72a95621ba9534db7ee1fa24220|feat(security): implement i18n for active alerts and history views|11/05/2026|
|Regula-Frontend|feature/distribution|2c7bd6f7fd20bae74c15ec07e6bf492ce7a9a29e|feat(i18n): config translation support|11/05/2026|
|Regula-Frontend|feature/distribution|ccce051d019f4253881550070b8523f121777fb7|feat(i18n): add translation support for navbar labels|11/05/2026|
|Regula-Frontend|feature/distribution|75ad61e674ff95816c5f74bda127a653705a8053|feat(routing): add security hub container with nested child routes|11/05/2026|
|Regula-Frontend|feature/distribution|9e4b33dba08a4a4e1f838c71080b703624ca23ce|feat(presentation): add operational security management views|11/05/2026|
|Regula-Frontend|feature/distribution|94eba50508b10eeb34191d272254cc2a3393b4a2|feat(presentation): add security routes for operational security|11/05/2026|
|Regula-Frontend|feature/distribution|288754dd874dd91665ec8477f79466b6a93c1d16|feat(infrastructure): add security API and assemblers|11/05/2026|
|Regula-Frontend|feature/distribution|df807758e72edc22b61beeb55bb553b7c475eeb6|feat(domain): add operational-security domain entities|11/05/2026|
|Regula-Frontend|feature/distribution|7f32e16b78e75e7d076ee5783ac1e30cb5f60ccb|feat(store): add Pinia security store for operations|11/05/2026|
|Regula-Frontend|feature/distribution|20480336b0020b1d6cb1628bf18c5ac852da2f2f|chore(config): update json server|11/05/2026|
|Regula-Frontend|feature/distribution|3efb97d4e674c1e9a3ce7d48bec9d832fc9c8f79|fix: json-server; update lockfile & remove BOM|11/05/2026|
|Regula-Frontend|feature/distribution|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/distribution|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/distribution|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/distribution|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/distribution|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/distribution|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/distribution|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/distribution|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/distribution|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/distribution|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/distribution|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/distribution|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/distribution|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/distribution|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/distribution|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/distribution|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/distribution|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/distribution|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/distribution|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/distribution|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/distribution|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/distribution|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/distribution|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/distribution|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/distribution|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/distribution|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/distribution|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/distribution|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/distribution|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/distribution|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/distribution|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/distribution|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/distribution|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/distribution|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/distribution|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/distribution|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/distribution|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/distribution|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/distribution|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/distribution|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/report-graphics|b0cbb31791561ec267c644d2f3dd3ddfe4fcb106|feat(store): enhance inventory store with additional data handling for origins, providers, and stock kg maps|24/05/2026|
|Regula-Frontend|feature/report-graphics|476784f0adcae7b2501231d15332fb867f3ee66c|feat(api): add summary documentation for inventory API service|24/05/2026|
|Regula-Frontend|feature/report-graphics|fd5355152ec186b1a4413728198e38e8644e4824|feat(assembler): add inventory, origin, provider, and stock kg map assemblers for resource transformation|24/05/2026|
|Regula-Frontend|feature/report-graphics|68bc03008b266f70684087e2948ca3229b11cfc9|feat(entity): add new entity classes for audit logs, distributor movements, inventory movements, and related models|24/05/2026|
|Regula-Frontend|feature/report-graphics|d999b27988e7fede64721005a98c912d36cb9d00|Merge branch 'refs/heads/develop' into feature/report-graphics|23/05/2026|
|Regula-Frontend|feature/report-graphics|58b6771b17373854955053dd771b719e4cab457f|fix(deps): downgrade json-server to version 0.17.4|23/05/2026|
|Regula-Frontend|feature/report-graphics|9193c33a463911e2aaaf68086aa4b895ca250ca6|feat(reports): implement analytics store and enhance report generation logic|12/05/2026|
|Regula-Frontend|feature/report-graphics|0277fc7026362af42ee401630a4d6e5e64de9213|feat(reports): improve code readability in generate report view|12/05/2026|
|Regula-Frontend|feature/report-graphics|64c502c98bd627b14ad0904950aa43dfb72a3286|feat(reports): add generate report view and localization support|12/05/2026|
|Regula-Frontend|feature/report-graphics|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/report-graphics|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/report-graphics|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/report-graphics|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/report-graphics|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/report-graphics|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/report-graphics|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/report-graphics|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/report-graphics|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/report-graphics|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/report-graphics|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/report-graphics|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/report-graphics|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/report-graphics|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/report-graphics|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/report-graphics|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/report-graphics|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/report-graphics|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/report-graphics|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/report-graphics|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/report-graphics|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/report-graphics|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/report-graphics|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/report-graphics|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/report-graphics|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/report-graphics|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/report-graphics|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/report-graphics|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/report-graphics|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/report-graphics|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/report-graphics|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/report-graphics|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/report-graphics|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/report-graphics|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/report-graphics|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/report-graphics|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/report-graphics|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/report-graphics|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/report-graphics|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/report-graphics|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/inventory-and-cylinder-tracking|856e709a09f99a2053f60cd40acca852d7c3604a|refactor(main): simplify import paths for i18n, pinia, and router modules|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|2c8704b24794f7ce241a4c7a52883d8fa2ae013b|feat(styles): add Regula brand tokens and typography styles to enhance UI consistency|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|f848e45a9ebb71b4ed62145531108d64947fc377|feat(navbar): simplify app-navbar and enhance navigation for enterprise and distributor roles|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|0717c639adf3f2133b0e925c6d1f20515005e38b|refactor(i18n): update import paths for localization files|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|314a7061e38822e67c188e2368733d8732bfaa8b|refactor(pinia): move pinia.js to root directory for improved structure|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|f416863010055ea06418868cab9e6585f5078787|feat(router): add main router configuration with inventory routes and role selection|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|7eb357f04a3b98a9876b701a03df606d69c05905|feat(routes): add inventory route definitions for enterprise and distributor views|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|151a801f04ea81d8a16a206f41a035e021a6a2b6|feat(inventory): refactor inventory store usage and enhance data fetching in panels|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|e24f9e54af16ca3d248c59cb49648553ba8cc082|feat(distributor): refactor inventory store usage in distributor panels|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|b0cbb31791561ec267c644d2f3dd3ddfe4fcb106|feat(store): enhance inventory store with additional data handling for origins, providers, and stock kg maps|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|476784f0adcae7b2501231d15332fb867f3ee66c|feat(api): add summary documentation for inventory API service|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|fd5355152ec186b1a4413728198e38e8644e4824|feat(assembler): add inventory, origin, provider, and stock kg map assemblers for resource transformation|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|68bc03008b266f70684087e2948ca3229b11cfc9|feat(entity): add new entity classes for audit logs, distributor movements, inventory movements, and related models|24/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|58b6771b17373854955053dd771b719e4cab457f|fix(deps): downgrade json-server to version 0.17.4|23/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/inventory-and-cylinder-tracking|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

|**Repository**|**Branch**|**Commit ID**|**Commit Message**|**Fecha**|
| :- | :- | :- | :- | :- |
|Regula-Frontend|feature/operational-analytics|c0d738970db2a5137993abaf06a14922a623d943|chore: delete i18n in public.|10/05/2026|
|Regula-Frontend|feature/operational-analytics|5bcc81ac7ebe226771e367e66cd96200493a7112|Merge branch 'feature/inventory-management' into develop|10/05/2026|
|Regula-Frontend|feature/operational-analytics|f671e693b6b21c23f65c1dc2f4edbaa5e49985aa|feat(view): update enterprise inventory view with new components and data handling|10/05/2026|
|Regula-Frontend|feature/operational-analytics|2ee4da13542be733048791796f72f935b8f3d94d|feat(seed): create seed script for inventory history with enterprise and distributor movements|10/05/2026|
|Regula-Frontend|feature/operational-analytics|945539241c98c9ae8dae5e9003f2faf2dbf6a4b6|feat(deps): add json-server to dependencies and create seed script for inventory history|10/05/2026|
|Regula-Frontend|feature/operational-analytics|59686a0e62ffdec2bc21137c3917186d7ecbad84|feat(store): add inventory UI store for managing section keys|10/05/2026|
|Regula-Frontend|feature/operational-analytics|909517758a896341b35ab42f5a632b56167e305e|feat(store): implement inventory store with stock and movement fetching|10/05/2026|
|Regula-Frontend|feature/operational-analytics|745da975894d0fe1d193ff4c065b3ed309a49667|feat(config): add alias for src directory and set server port in vite.config.js|10/05/2026|
|Regula-Frontend|feature/operational-analytics|ccb6d2e0b7d1136d6c1ff252e4c45fe56a09c5be|feat(deps): move json-server to devDependencies in package.json|10/05/2026|
|Regula-Frontend|feature/operational-analytics|ed4ec6518fb732069bc035f88c5cd2b8d0cbfab7|feat(ui): add inventory stock table and placeholder components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|8368e5f0cf0f7e3ccb15142267286924ec3c1306|feat(ui): implement navigation presets for enterprise and distributor roles|10/05/2026|
|Regula-Frontend|feature/operational-analytics|3cab083dac76610c0ec3eb2ec343762bbc2b1402|feat(ui): enhance app navbar and sidebar with inventory management features|10/05/2026|
|Regula-Frontend|feature/operational-analytics|8f6763ef86225c779cb8211d40bf610d06704b8d|feat(ui): integrate PrimeVue with toast and tooltip services in main.js|10/05/2026|
|Regula-Frontend|feature/operational-analytics|13ce0319c19fa2dc5ee8a07b821639738b026686|feat(ui): update index.html and add base styles for Regula app|10/05/2026|
|Regula-Frontend|feature/operational-analytics|e2bae69a36c7ee8dbe682af3042f74544752f7d6|feat(ui): add toast notification component to app layout|10/05/2026|
|Regula-Frontend|feature/operational-analytics|ce439beac79bade9f46cf2fa8882547bef07d3a9|feat(ui): add role selection view for enterprise and distributor interfaces|10/05/2026|
|Regula-Frontend|feature/operational-analytics|9ee4dd3bc794a85d46533d6ec65cd5b8b0f5b18e|feat(layout): implement app shell layout with responsive navbar and sidebar|10/05/2026|
|Regula-Frontend|feature/operational-analytics|837d76f691d23e871a7aa754e37438ddd0697086|feat(ui): add enterprise inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/operational-analytics|195c2b451d1b03decbaf91fc800f70442451ff45|feat(ui): add distributor inventory view with stock, entry, exit, and history panels|10/05/2026|
|Regula-Frontend|feature/operational-analytics|a5e747ea8ab23e90bc559054365592e649add8aa|feat(ui): add inventory shell tabs and stock card components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|98bf67a74dbbd4b53a98a787aaee57862a2d3283|feat(ui): add inventory distributor and enterprise stock panels|10/05/2026|
|Regula-Frontend|feature/operational-analytics|b473399cc4864887ba603be5610920198463d247|feat(ui): add enterprise register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|70d429d80a1cc1de0b96cded7c3c04e2e7daa8d6|feat(ui): add enterprise audit and movement history panel components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|be253cc19d08fe45060a0b0bd935239448881cf8|feat(ui): add distributor register entry and exit panel components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|4796d53b8de17372bc47662118a87b74402e48a0|feat(ui): add cylinder type picker and distributor movement history panel components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|95eebd10373f5a20fb59c90c320c1abc6f578ce5|feat(styles): add Regula design tokens and tooltip styles for consistent UI|10/05/2026|
|Regula-Frontend|feature/operational-analytics|d5d9a9f378999ecd25c6baa499ee51f31f70e086|feat(shell): add shell presets utility for enhanced shell configuration|10/05/2026|
|Regula-Frontend|feature/operational-analytics|970b44764c9becb2fbdd01147b196b6258f3e99f|feat(ui): add basic structure for app navbar and sidebar components|10/05/2026|
|Regula-Frontend|feature/operational-analytics|5541d24cb20c7367aa2f262da536bfc76f4c0faa|feat(store): create inventory store for state management|10/05/2026|
|Regula-Frontend|feature/operational-analytics|010715caa87e302287c6d03157cf5a8e2d31b486|feat(ui): add inventory UI store for state management|10/05/2026|
|Regula-Frontend|feature/operational-analytics|6fb9ed0f85846a7c7e6061cf4492969b72c6d347|feat(helper): add CSV download and HTML print utilities|10/05/2026|
|Regula-Frontend|feature/operational-analytics|9d97d55846e5f082dba66589c435afe5d9ba88d1|feat(api): implement InventoryApi and InventoryStockAssembler for inventory management|10/05/2026|
|Regula-Frontend|feature/operational-analytics|035ae0d44012cf5b0b96b8b3e3657894d040e5a5|feat(domain): add DistributorStockCard and GasCylinderStockRow entities|10/05/2026|
|Regula-Frontend|feature/operational-analytics|885e1a9cdcddf22f983fee81df094abb973d1c2e|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/operational-analytics|d9ca4ba621d32f063ba772c7fac72cd92f8151b5|chore: implement base API and router setup for inventory management|10/05/2026|
|Regula-Frontend|feature/operational-analytics|57a8550a97e80f4fd73110b207260b1b0153b526|chore: add content translate.|10/05/2026|
|Regula-Frontend|feature/operational-analytics|8eed5a198b48495aac186af0f2772ac7428578aa|chore: add base API and endpoint files|10/05/2026|
|Regula-Frontend|feature/operational-analytics|f48408ba6e5979f1e3f41df0189c90e2f9428088|chore: add localization files for English and Spanish|10/05/2026|
|Regula-Frontend|feature/operational-analytics|26440c798c81f915f2f5d45c85f4758da65059e5|chore: correction.|08/05/2026|
|Regula-Frontend|feature/operational-analytics|b220aadf8e26fa2e0be27de8ee8c3b1a7c7891c9|chore: initial commit.|08/05/2026|

## 5.2.2.5. Execution Evidence for Sprint Review
Durante el Sprint 2, el equipo logró desplegar y dejar operativas las principales vistas de la Web Application de Regula, integradas con los Web Services internos y con experiencia consistente entre el Landing Page y la aplicación. La navegación parte de la selección de rol (empresa / distribuidor) y del flujo de autenticación (sign-in / sign-up), y desde allí el usuario accede a los módulos funcionales construidos en este Sprint: gestión de inventario, gestión comercial (ventas y deudas), logística de distribución, seguridad y alertas, y reportes/analytics. Todas las vistas aplican responsive web design, internacionalización (English / Latin American Spanish) y atributos ARIA para accesibilidad. A continuación se presentan los screenshots de las vistas más representativas junto con su explicación, y al final el enlace al video de navegación del producto.


# Execution Evidence for Sprint Review

## 1. Role Selection View

Vista inicial donde el visitante elige el tipo de perfil (**Enterprise** / **Distributor**), que condiciona la navegación y los módulos disponibles.

> **Capturas de pantalla:**

![1. Role Selection View.png](assets/images/cap-05/1.%20Role%20Selection%20View.png)

---

## 2. Sign-in / Sign-up (IAM)

Vistas de autenticación integradas con **Vue Router** y el store de estado de autenticación. Permiten el acceso seguro a la aplicación.

> **Capturas de pantalla:**

![2. Sign-in  Sign-up (IAM).png](assets/images/cap-05/2.%20Sign-in%20%20Sign-up%20%28IAM%29.png)
---

## 3. Enterprise Inventory View

Tablero de inventario para la empresa, con paneles de stock, entradas, salidas e historial de movimientos, además del registro de auditoría.

> **Capturas de pantalla:**

![3. Enterprise Inventory View .png](assets/images/cap-05/3.%20Enterprise%20Inventory%20View%20.png)
![3. Enterprise Inventory View  (2).png](assets/images/cap-05/3.%20Enterprise%20Inventory%20View%20%20%282%29.png)
![3. Enterprise Inventory View  (3).png](assets/images/cap-05/3.%20Enterprise%20Inventory%20View%20%20%283%29.png)
![3. Enterprise Inventory View  (4).png](assets/images/cap-05/3.%20Enterprise%20Inventory%20View%20%20%284%29.png)
![3. Enterprise Inventory View  (5).png](assets/images/cap-05/3.%20Enterprise%20Inventory%20View%20%20%285%29.png)

---

## 4. Distributor Inventory View

Vista equivalente para el distribuidor, con stock por tipo de balón (**cylinder type**), registro de entradas/salidas e historial de movimientos.

> **Capturas de pantalla:**

![4. Distributor Inventory View.png](assets/images/cap-05/4.%20Distributor%20Inventory%20View.png)
![4. Distributor Inventory View (2).png](assets/images/cap-05/4.%20Distributor%20Inventory%20View%20%282%29.png)
![4. Distributor Inventory View (3).png](assets/images/cap-05/4.%20Distributor%20Inventory%20View%20%283%29.png)
![4. Distributor Inventory View (4).png](assets/images/cap-05/4.%20Distributor%20Inventory%20View%20%284%29.png)

---

## 5. Commercial Management (Sales & Debts)

Vistas de ventas y deudas del distribuidor: tabla de ventas, panel resumen de ventas, diálogo de registro de venta, panel de registro de pago, registro de deuda, deudas pendientes e historial comercial.

> **Capturas de pantalla:**

![5. Commercial Management (Sales & Debts).png](assets/images/cap-05/5.%20Commercial%20Management%20%28Sales%20%26%20Debts%29.png)
![5. Commercial Management (Sales & Debts) (2).png](assets/images/cap-05/5.%20Commercial%20Management%20%28Sales%20%26%20Debts%29%20%282%29.png)


## 6. Distribution Logistics

Vistas de gestión de distribución (**delivery** y **deliverer**), que soportan la operación logística de entrega.

> **Capturas de pantalla:**

![6. Distribution Logistics.png](assets/images/cap-05/6.%20Distribution%20Logistics.png)
![6. Distribution Logistics (2).png](assets/images/cap-05/6.%20Distribution%20Logistics%20%282%29.png)
![6. Distribution Logistics (3).png](assets/images/cap-05/6.%20Distribution%20Logistics%20%283%29.png)
![6. Distribution Logistics (4).png](assets/images/cap-05/6.%20Distribution%20Logistics%20%284%29.png)
---

## 7. Operational Security & Alerts

Vistas de gestión de seguridad operativa, alertas de empresa, estado de almacenes e historial de alertas.

> **Capturas de pantalla:**

![7. Operational Security & Alerts .png](assets/images/cap-05/7.%20Operational%20Security%20%26%20Alerts%20.png)
![7. Operational Security & Alerts  (2).png](assets/images/cap-05/7.%20Operational%20Security%20%26%20Alerts%20%20%282%29.png)
![7. Operational Security & Alerts  (3).png](assets/images/cap-05/7.%20Operational%20Security%20%26%20Alerts%20%20%283%29.png)
![7. Operational Security & Alerts  (4).png](assets/images/cap-05/7.%20Operational%20Security%20%26%20Alerts%20%20%284%29.png)
![7. Operational Security & Alerts  (5).png](assets/images/cap-05/7.%20Operational%20Security%20%26%20Alerts%20%20%285%29.png)

---

## 8. Reports & Analytics

Vista de generación de reportes y tablero de analytics (incluyendo **security trends**), con soporte de descarga (**CSV**) e impresión.

> **Capturas de pantalla:**

![8. Reports & Analytics.png](assets/images/cap-05/8.%20Reports%20%26%20Analytics.png)

---

# Video de navegación (Execution Evidence)

A continuación se incluye el screenshot del video y el enlace en el que se demuestra y explica la visualización y navegación logradas durante el Sprint 2.

| Elemento       | Información            |
|----------------|------------------------|
| imagen            | ![Video de navegación (Execution Evidence) .png](assets/images/cap-05/Video%20de%20navegaci%C3%B3n%20%28Execution%20Evidence%29%20.png) |
| **Archivo**    | https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a649_upc_edu_pe/IQDVSGZAIa-8RoS6LXjGdbn9AQTJOE-z0Eoldx9MYBHf-7I?e=hJiTo5&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D   |
| **Plataforma** | Microsoft Stream       |
| **Duración**   | **2:42**               |
