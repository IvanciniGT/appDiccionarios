# Documentación del Backend de la Aplicación de Diccionarios

Este repositorio contiene la **documentación** del **Backend de la Aplicación de Diccionarios** utilizada en los cursos y formaciones de **Iván Osuna**.

Incluye modelos UML, ejemplos de código y explicaciones detalladas sobre cómo estructurar un backend RESTful utilizando una arquitectura en capas y buenas prácticas de desarrollo.

## Descripción

La documentación cubre cómo estructurar un backend para la gestión de diccionarios, palabras, significados, variantes morfológicas y otros elementos relacionados.

Se incluyen diagramas UML, ejemplos de código y explicaciones detalladas sobre cómo implementar cada capa de la arquitectura.

### Casos de uso

![Casos de uso](https://github.com/IvanciniGT/appDiccionarios/blob/master/resources/casos-uso.png)

Pulsa aquí para ver el detalle de los [Casos de uso](https://github.com/IvanciniGT/appDiccionarios/blob/master/casos-uso.md)

### Arquitectura en capas del backend

Para el backend se han definido las siguientes capas:

```mermaid
---
title: Capas del sistema - APIs
---
graph TD

    B[<a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-controlador.md">Capa de Controlador</a>]
    B -->C[<a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-servicio.md">Capa de Negocio</a>]
    C -->D[<a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-dominio.md">Capa de Dominio</a>]
    E[Módulo de <BR>Exportación/Importación] --> D

```

## Propósito

El objetivo de este proyecto es servir como un recurso educativo para los estudiantes y desarrolladores que participan en los cursos y videos de **Iván Osuna**. A través de esta documentación, los usuarios aprenderán:

- Cómo diseñar un backend RESTful completo.
- La estructura típica de un backend en capas.
- Buenas prácticas para el manejo de entidades relacionadas con diccionarios y palabras.

## Uso

Puedes utilizar esta documentación como guía para desarrollar tus propias aplicaciones backend o para complementar los cursos en los que se utiliza como material didáctico.

1. **Navega por la documentación**: Examina las distintas capas de la arquitectura (controlador, servicio, DTOs) y los ejemplos detallados.
2. **Aplica los conceptos**: Implementa lo aprendido en tus propios proyectos o sigue los ejemplos mostrados en los cursos.

## Contribución

Por ahora, este repositorio está limitado a documentación, pero si deseas contribuir con mejoras o correcciones en el contenido, puedes hacerlo de la siguiente manera:

1. Haz un fork del repositorio.
2. Realiza los cambios en tu propio fork.
3. Envía un **Pull Request** con tus sugerencias o mejoras.

---

## Contacto

Para consultas o más información:

- **Iván Osuna**
- Email: [ivan.osuna.ayuste@gmail.com](mailto:ivan.osuna.ayuste@gmail.com)

---
## Copyright y Licencia

**© 2024 Iván Osuna Ayuste. Todos los derechos reservados**.

Este material, este documento y su contenido están licenciados bajo la licencia [Licencia Creative Commons Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

![Licencia CC BY-NC-SA](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)

 **Queda expresamente prohibido el uso en formaciones comerciales** por terceros sin autorización expresa del autor.

 ---
<p align="center">
    <strong>README.md</strong> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-controlador.md">Capa de Controlador</a> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-servicio.md">Capa de Negocio</a> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-dominio.md">Capa de Dominio</a>
</p>
