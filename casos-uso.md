# Casos de Uso - Aplicación de Diccionarios

Estos son los casos de uso de la aplicación de diccionarios, utilizada en los videos y formaciones de **Iván Osuna Ayuste**, y está protegido bajo la licencia **Creative Commons BY-NC-SA** y las leyes de **Copyright ©**. [Ver más...](#copyright-y-licencia)

© 2024 Iván Osuna Ayuste. Todos los derechos reservados.

## Introducción

Este documento describe los casos de uso principales para los dos tipos de usuarios de la aplicación de diccionarios: **Usuario** y **Editor de Diccionarios**. Cada actor tiene acceso a diferentes funcionalidades dentro del sistema.

## Actores:
- **Usuario**: Puede buscar palabras dentro de los diccionarios mediante diferentes tipos de búsqueda.
- **Editor de Diccionarios**: Además de buscar palabras, puede editar y gestionar los diccionarios, palabras e idiomas.

## Diagrama de Casos de Uso

![Casos de uso](https://github.com/IvanciniGT/appDiccionarios/blob/master/resources/casos-uso.png)

## Descripción de Casos de Uso

### **CU01: Buscar palabras**
El **Usuario** puede buscar palabras dentro de los diccionarios con las siguientes opciones:

- **Búsqueda exacta** (RF01): Buscar una palabra tal como está escrita.
- **Búsqueda por prefijo** (RF02): Buscar palabras que comienzan con un conjunto específico de letras.
- **Búsqueda por similitud** (RF03): Buscar palabras similares basadas en ciertas reglas (ej. Levenshtein, Jaccard, etc.).

### **CU02: Editar idiomas**
El **Editor de Diccionarios** puede crear, modificar o eliminar idiomas del sistema, asegurando que los diccionarios estén siempre asociados a un idioma válido.
- **Crear Idioma** (RF10)
- **Modificar Idioma** (RF11)
- **Eliminar Idioma** (RF12)

### **CU03: Editar diccionarios**
El **Editor de Diccionarios** tiene la capacidad de crear nuevos diccionarios, modificar los existentes o eliminar aquellos que ya no sean necesarios.
- **Crear Diccionario** (RF04)
- **Modificar Diccionario** (RF05)
- **Eliminar Diccionario** (RF06)

### **CU04: Editar palabras**
El **Editor de Diccionarios** puede agregar, modificar o eliminar palabras dentro de un diccionario. Cada palabra puede tener variantes, significados y estar asociada a un idioma específico.
- **Crear Palabra** (RF07)
- **Modificar Palabra** (RF08)
- **Eliminar Palabra** (RF09)

## Notas adicionales
- El sistema debe garantizar que los editores no eliminen diccionarios o palabras que aún estén en uso.
- Los usuarios pueden realizar búsquedas, pero no pueden modificar el contenido de los diccionarios.

---
## Copyright y Licencia

**© 2024 Iván Osuna Ayuste. Todos los derechos reservados**.

Este material, este documento y su contenido están licenciados bajo la licencia [Licencia Creative Commons Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

![Licencia CC BY-NC-SA](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)

 **Queda expresamente prohibido el uso en formaciones comerciales** por terceros sin autorización expresa del autor.

 ---
 <p align="center">
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/casos-uso.md">Casos de uso</a> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-controlador.md">Capa de Controlador</a> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-servicio.md">Capa de Negocio</a> |
    <a href="https://github.com/IvanciniGT/appDiccionarios/blob/master/capa-dominio.md">Capa de Dominio</a>
</p>
