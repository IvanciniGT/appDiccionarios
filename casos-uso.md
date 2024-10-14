
# Casos de Uso - Aplicación de Diccionarios

## Introducción

Este documento describe los casos de uso principales para los dos tipos de usuarios de la aplicación de diccionarios: **Usuario** y **Editor de Diccionarios**. Cada actor tiene acceso a diferentes funcionalidades dentro del sistema.

### Actores:
- **Usuario**: Puede buscar palabras dentro de los diccionarios mediante diferentes tipos de búsqueda.
- **Editor de Diccionarios**: Además de buscar palabras, puede editar y gestionar los diccionarios, palabras e idiomas.

## Diagrama de Casos de Uso

![Casos de uso](https://github.com/IvanciniGT/appDiccionarios/blob/master/resources/casos-uso.png)

## Descripción de Casos de Uso

### **1. Buscar palabras**
El **Usuario** puede buscar palabras dentro de los diccionarios con las siguientes opciones:

- **Búsqueda exacta**: Buscar una palabra tal como está escrita.
- **Búsqueda por prefijo**: Buscar palabras que comienzan con un conjunto específico de letras.
- **Búsqueda por similitud**: Buscar palabras similares basadas en ciertas reglas (ej. Levenshtein, Jaccard, etc.).

### **2. Editar idiomas**
El **Editor de Diccionarios** puede crear, modificar o eliminar idiomas del sistema, asegurando que los diccionarios estén siempre asociados a un idioma válido.

### **3. Editar diccionarios**
El **Editor de Diccionarios** tiene la capacidad de crear nuevos diccionarios, modificar los existentes o eliminar aquellos que ya no sean necesarios.

### **4. Editar palabras**
El **Editor de Diccionarios** puede agregar, modificar o eliminar palabras dentro de un diccionario. Cada palabra puede tener variantes, significados y estar asociada a un idioma específico.

## Notas adicionales
- El sistema debe garantizar que los editores no eliminen diccionarios o palabras que aún estén en uso.
- Los usuarios pueden realizar búsquedas, pero no pueden modificar el contenido de los diccionarios.
