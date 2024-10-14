# Casos de Uso - Aplicación de Diccionarios

Estos son los casos de uso de la aplicación de diccionarios, utilizada en los videos y formaciones de **Iván Osuna Ayuste**, y está protegido bajo la licencia **Creative Commons BY-NC-SA** y las leyes de **Copyright ©**. [Ver más...](#copyright-y-licencia)

© 2024 Iván Osuna Ayuste. Todos los derechos reservados.

## Introducción

Este documento describe los casos de uso principales para los dos tipos de usuarios de la aplicación de diccionarios: **Usuario** y **Editor de Diccionarios**. Cada actor tiene acceso a diferentes funcionalidades dentro del sistema.

## Actores:
- **Usuario**: Puede buscar palabras dentro de los diccionarios mediante diferentes tipos de búsqueda.
- **Editor de Diccionarios**: Además de buscar palabras, puede editar y gestionar los diccionarios, palabras e idiomas.
- **Administrador**: Puede realizar tareas administrativas como exportar e importar diccionarios.

## Diagrama de Casos de Uso

![Casos de uso](https://github.com/IvanciniGT/appDiccionarios/blob/master/resources/casos-uso.svg)

## Descripción de Casos de Uso

### **CU01: Buscar palabras**
El **Usuario** puede buscar palabras dentro de los diccionarios con las siguientes opciones:

- **UC01: Búsqueda exacta de palabras** (RF01): Buscar una palabra tal como está escrita (case-insensitive, acentos-insensitive, plural-insensitive... y otros que se consideren en el futuro).
- **UC02: Búsqueda por prefijo** (RF02): Buscar palabras que comienzan con un conjunto específico de letras (case-insensitive, acentos-insensitive, plural-insensitive... y otros que se consideren en el futuro).
- **UC03: Búsqueda por similitud** (RF03): Buscar palabras similares basadas en ciertas reglas (ej. Levenshtein, etc.).

### **CU02: Editar diccionarios**
El **Editor de Diccionarios** puede gestionar los diccionarios con las siguientes acciones:

- **UC11: Gestionar diccionario** (RF04, RF05, RF06): Crear, modificar o eliminar diccionarios en el sistema.
- **UC12: Recuperar diccionario(s)**: Consultar o listar diccionarios en el sistema.

### **CU03: Editar palabras**
El **Editor de Diccionarios** puede gestionar las palabras con las siguientes acciones:

- **UC13: Gestionar palabras** (RF07, RF08, RF09): Crear, modificar o eliminar palabras en el sistema.
- **UC14: Recuperar palabra(s)**: Consultar o listar palabras en el sistema.

### **CU04: Editar idiomas**
El **Editor de Diccionarios** puede gestionar los idiomas con las siguientes acciones:

- **UC15: Gestionar idioma** (RF10, RF11, RF12): Crear, modificar o eliminar idiomas en el sistema.
- **UC16: Recuperar idiomas**: Consultar o listar idiomas en el sistema.

### **CU05: Administrar diccionarios (Administrador)**
El **Administrador** puede realizar acciones administrativas:

- **UC21: Exportar diccionarios**: Exportar diccionarios del sistema.
- **UC22: Importar diccionarios**: Importar diccionarios al sistema.

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
