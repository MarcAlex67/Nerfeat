# Nerfeat
Aplicación web de gimnasio y comida

----

## Índice de Contenidos

* 1. [Introducción](#1-introducción)
* 2. [Briefing de Ideas](#2-briefing-de-ideas)
* 3. [Arquitectura del Software](#3-arquitectura-del-software)
* 4. [Tecnologías Utilizadas](#4-tecnologías-utilizadas)
* 5. [Infraestructura de Red](#5-infraestructura-de-red)
  * 5.1. [Diagrama de Red](#51-diagrama-de-red)
  * 5.2. [Mapa Físico](#52-mapa-físico)
  * 5.3. [Mapa Lógico](#53-mapa-lógico)
* 6. [Desarrollo Web](#6-desarrollo-web)
  * 6.1. [Diseño](#61-diseño)
  * 6.2. [Mockups](#62-mockups)
  * 6.3. [Mapa de Navegabilidad](#63-mapa-de-navegabilidad)
* 7. [Base de Datos](#7-base-de-datos)
* 8. [Servicios e Infraestructura](#8-servicios-e-infraestructura)
  * 8.1. [DNS](#81-dns)
  * 8.2. [DHCP](#82-dhcp)
  * 8.3. [Servidor Web (Apache)](#83-servidor-web-apache)
  * 8.4. [Cortafuegos (Firewall)](#84-cortafuegos-firewall)
  * 8.5. [Copias de Seguridad (Backups)](#85-copias-de-seguridad-backups)
* 9. [Guías de Usuario](#9-guías-de-usuario)
* 10. [Conclusiones](#10-conclusiones)
* 11. [Bibliografía](#11-bibliografía)

---

## Índice de Contenidos

<details>
<summary><h2>1. Introducción</h2></summary>
<br>

Desarrollo de una plataforma web orientada a personas sedentarias que buscan un cambio de estilo de vida. La aplicación integra dos pilares fundamentales:
* **Área de Actividad Física:** Seguimiento visual y progresivo del entrenamiento muscular.
* **Área de Nutrición Inteligente:** Escáner de alimentos que alimenta un historial de ingredientes y una IA "Chef" personal capaz de generar recetas personalizadas en función de los productos escaneados.
</details>

<details>
<summary><h2>2. Briefing de Ideas</h2></summary>
<br>

---

## Justificación

En la actualidad, muchas personas que entrenan tienen dificultades para mantener una relación clara entre la intensidad de sus entrenamientos y sus necesidades nutricionales. Las aplicaciones existentes suelen ofrecer estas funciones de forma separada. 

**NerfEat** nace para unificar en un solo ecosistema el análisis del progreso muscular con el reconocimiento inteligente de alimentos y la generación de dietas adaptadas, facilitando la adherencia a un estilo de vida saludable mediante la automatización de procesos.

---

## Objetivos del Proyecto

### Objetivo General
Desarrollar una aplicación móvil/web funcional que ayude a gente que le cuesta o a gente princpiantes a mejorar su salud tanto ayundándolos a comer bien y hacer una rutina de ejercicios para los diferentes grupos musculares

### Objetivos Específicos
- **Ranking y Progreso Muscular:**
  - Desarrollar un mapa corporal interactivo que cuantifique el volumen de trabajo asignado a cada grupo muscular.
  - Integrar métricas temporales semanal, mensual, anual para poder evaluar el equilibrio entre el entrenamiento de distintas zonas musculares y prevenir lesiones.
- **Escáner de Alimentos:**
  - Integrar un modelo de visión por ordenador para identificar ingredientes y alimentos empaquetados o preparados a través de la cámara del dispositivo.
  - Conectar la detección con una base de datos nutricional para extraer calorías (proteínas, carbohidratos, grasas,etc).
- **("Chef Personal"):**
  - Diseñar un algoritmo que procese la despensa virtual creada mediante los escaneos previos del usuario.
  - Proponer recetas personalizadas en tiempo real ajustadas al objetivo del usuario (ganancia muscular, déficit calórico o mantenimiento).

---

## Público Objetivo

- **Deportistas y entusiastas del fitness** que buscan mejorar su rendimiento y composición corporal.
- **Personas con poco tiempo libre** que quieren organizar sus comidas rápidamente a base de los ingredientes que ya tienen en casa.
- **Usuarios principiantes en el gimnasio** que necesitan guía una visual sobre qué grupos musculares se están trabajando y aprender a cómo alimentarse adecuadamente.

---

## Módulos del Ciclo Relacionados

- **Programación / Desarrollo Web o Móvil:** Aplicación de lenguajes como Python o JavaScript para la lógica de la aplicación y la interfaz de usuario.
- **Bases de Datos:** Diseño e implementación de modelos relacionales o no relacionales para almacenar el historial de escaneos, usuarios y planes de entrenamiento.
- **Sistemas de Gestión Empresarial / Acceso a Datos:** Integración de APIs externas y despliegue de modelos de Machine Learning.

---

## Requisitos y Materiales

### Materiales Físicos (Hardware)
- Ordenador de desarrollo .
- Dispositivo móvil para pruebas del escáner y la interfaz.

### Materiales Lógicos (Software y Herramientas)
- **IDE & Entorno:** Visual Studio Code / Android Studio
- **Frontend / Backend:** Flutter o React Native / Node.js o Python (FastAPI/Flask)
- **Base de Datos:** Firebase / PostgreSQL
- **Librerías de IA & APIs:** OpenCV, Google Vision API, OpenAI API, TensorFlow/PyTorch

---

## Recursos y Referencias

### Documentación Técnica y APIs
- Open Food Facts API - Una base de datos abierta para los productos alimenticios.
- OpenAI API Documentation - Una guía de integración para modelos de lenguaje.
- Google Cloud Vision API - Un reconocimiento de imágenes.

### Bibliografía
- *National Strength and Conditioning Association (NSCA):* Principios del entrenamiento de fuerza y acondicionamiento físico.
</details>

<details>
<summary><h2>3. Arquitectura del Software</h2></summary>
<br>

*Estructura general del sistema, patrones de diseño aplicados (e.g., MVC, Microservicios, Cliente-Servidor) y componentes principales.*
</details>

<details>
<summary><h2>4. Tecnologías Utilizadas</h2></summary>
<br>

*Lista detallada de lenguajes de programación, frameworks, librerías, APIs de IA y herramientas de desarrollo.*
</details>

<details>
<summary><h2>5. Infraestructura de Red</h2></summary>
<br>

### 5.1. Diagrama de Red
*Esquema global de la red donde se despliega la plataforma.*

### 5.2. Mapa Físico
*Ubicación, conexiones y hardware de los equipos de la infraestructura.*

### 5.3. Mapa Lógico
*Direccionamiento IP, subredes, VLANs y segmentación.*
</details>

<details>
<summary><h2>6. Desarrollo Web</h2></summary>
<br>

### 6.1. Diseño
*Guía de estilo, paleta de colores, tipografías y componentes de interfaz.*

### 6.2. Mockups
*Prototipos visuales de la aplicación (pantalla de progreso muscular, escáner e interfaz del Chef IA).*

### 6.3. Mapa de Navegabilidad
*Diagrama de flujo de usuario y experiencia de navegación entre páginas.*
</details>

<details>
<summary><h2>7. Base de Datos</h2></summary>
<br>

*Diseño del modelo entidad-relación, esquemas relacionales y tablas (usuarios, ejercicios, registro muscular, historial de escaneos y recetas).*
</details>

<details>
<summary><h2>8. Servicios e Infraestructura</h2></summary>
<br>

Explicación sencilla y conceptual de los servicios desplegados en la red para el soporte de la aplicación:

* **8.1. DNS:** Funciona como la "agenda telefónica" de la red. Traduce la dirección web fácil de recordar a la dirección IP numérica del servidor.
* **8.2. DHCP:** Asigna automáticamente una dirección IP a cada dispositivo que se conecta a la red, evitando conflictos y configuraciones manuales.
* **8.3. Servidor Web (Apache):** Encargado de procesar las peticiones de los usuarios desde sus navegadores y entregar las páginas web e interfaces.
* **8.4. Cortafuegos (Firewall):** Actúa como el guardia de seguridad de la red. Filtra el tráfico permitiendo solo conexiones seguras y autorizadas.
* **8.5. Copias de Seguridad (Backups):** Realiza respaldos periódicos y automáticos de la base de datos y archivos para recuperar información ante fallos.
</details>

<details>
<summary><h2>9. Guías de Usuario</h2></summary>
<br>

*Manuales de instalación, despliegue y uso de la aplicación tanto para administradores como para usuarios finales.*
</details>

<details>
<summary><h2>10. Conclusiones</h2></summary>
<br>

*Evaluación de los objetivos alcanzados, rendimiento del sistema, limitaciones y posibles líneas futuras de desarrollo.*
</details>

<details>
<summary><h2>11. Bibliografía</h2></summary>
<br>

*Referencias bibliográficas, documentación de las herramientas utilizadas y recursos externos.*
</details>
