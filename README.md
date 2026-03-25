# MetaMapa – Plataforma de Mapeo Colaborativo 🌍

MetaMapa es una plataforma distribuida orientada a la **recolección, integración y visualización de información geolocalizada de forma colaborativa**.

El sistema permite consolidar datos provenientes de múltiples fuentes (datasets, usuarios y APIs externas), garantizando su disponibilidad, trazabilidad y validación mediante mecanismos de agregación.

---

## 🚀 Funcionalidades principales

* Registro y visualización de hechos geolocalizados
* Creación y gestión de colecciones de información para agruparla en temáticas
* Búsqueda y filtrado avanzado (categoría, fecha, ubicación, etc.)
* Integración con múltiples fuentes de datos:
  * Estáticas (Archivos CSV)
  * Dinámicas (Usuarios)
  * Externas (APIs externas que proveen eventos)
* Carga colaborativa de información
* Normalización y deduplicación de información
* Generación de estadísticas y exportación CSV
* Gestión de solicitudes de eliminación con detección de spam
* Visualización en mapa

---

## 🏗️ Arquitectura

El sistema fue diseñado bajo una **arquitectura orientada a servicios**, evolucionando desde un enfoque monolítico hacia una solución distribuida.

### Componentes principales:

* Servicio de fuentes estáticas (ingestión de datasets CSV)
* Servicio de fuentes dinámicas (contenido generado por usuarios)
* Servicio de fuentes proxy (integración con APIs externas)
* Servicio agregador (consolidación, normalización y deduplicación)
* Servicio de Autenticación y Autorizacion 
* Servicio de Administración y Vizualización de Datos (maneja las API para funciones de los administradores)
* Servicio Público (encargado de la las APIs para ver y filtrar hechos y otros datos por parte de los usuarios)
* Servicio Normalizador (encargado de normalizar los datos obtenidos de las distintas fuentes)
* Servicio de Estadisticas (encargado de realizar constantemente estadísticas establecidas en base de todos los hechos recopilados)
* Cliente web desacoplado (arquitectura MVC)

---

## ⚙️ Tecnologías utilizadas

* Backend: Java usando SpringBoot
* APIs: REST y GraphQL
* Base de datos: Relacional (con ORM) usando MySQL
* Frontend: HTML, Tailwind CSS, JavaScript
* Contenerización: Docker
* Infraestructura: DigitalOcean
* Autenticacion: Keycloack
* Observabilidad: Prometheus, Loki, Grafana y Zipkin
---

## 🔄 Procesamiento de datos

El sistema implementa un pipeline completo de procesamiento:

* Importación de datasets masivos (CSV)
* Integración con APIs externas
* Normalización de datos inconsistentes
* Eliminación de duplicados
* Aplicación de algoritmos de consenso
* Generación periódica de estadísticas

---

> ⚠️ Actualmente el sistema no se encuentra desplegado en línea debido a limitaciones del plan gratuito de infraestructura.

---

## 👩‍💻 Mi contribución

Participé activamente en el diseño e implementación del sistema, destacando:

* Desarrollo de **fuente de datos estática** (procesamiento de datasets CSV)
* Implementación del **servicio de autenticación y seguridad**
* Participación en el **servicio agregador** (integración y procesamiento de datos)
* Diseño y definición de la **API REST**
* Implementación de la **persistencia de datos** en servicios
* Desarrollo y diseño del **frontend (UI/UX)**
* Implementación de **observabilidad del sistema**
* Despliegue de la aplicación en **DigitalOcean**
* **Dockerización** completa del proyecto
* Participación en el **diseño de arquitectura y modelo del sistema**

---

## 📌 Contexto académico

Proyecto desarrollado como Trabajo Práctico Integrador en la materia
**Diseño de Sistemas de Información **.

## 🚀 Documentación

Link a Carpeta de Drive con la siguiente documentación: 
* Wireframes del frontend
* Datos para los casos de prueba
* Casos de Uso
* Diagrama de Clases por servicio
* Diagrama de componentes
* Diagrama de Despliegue
* Diagramas de Entidad Relación de las Bases de Datos usadas
* Documentación de las APIs de cada servicio
* Decisiones de Diseño tomadas
* Demo del funcionamiento en fotos y dos videos mostrando el panel del Administrador y otro con la busqueda y filtros de hechos 

---

## 📬 Contacto

* GitHub: https://github.com/MilagrosLu
* LinkedIn: https://www.linkedin.com/in/milagros-salafia-75b8622b5/
