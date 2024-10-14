

# Documento de Requisitos - Aplicación de Diccionarios

## 1. Introducción

### 1.1 Propósito
Este documento describe los requisitos funcionales y no funcionales de la aplicación de diccionarios. Está diseñado para proporcionar una guía clara sobre las funcionalidades que se implementarán, así como los criterios que deben cumplirse para que el sistema cumpla con las expectativas de los usuarios finales.

### 1.2 Alcance
El proyecto es una aplicación de diccionarios que permite a los usuarios realizar búsquedas de palabras y a los editores gestionar diccionarios, palabras e idiomas. La aplicación está orientada a la formación y a la creación de contenido educativo para **IOChannel**.

## 2. Requisitos Funcionales

### 2.1 Búsqueda de Palabras
#### 2.1.1 Requisito: Búsqueda Exacta
El sistema debe permitir a los usuarios buscar palabras específicas dentro de un diccionario.
- **Entrada**: Texto de la palabra.
- **Salida**: Palabra encontrada con sus significados y variantes.

#### 2.1.2 Requisito: Búsqueda por Prefijo
El sistema debe permitir a los usuarios buscar palabras que comiencen con un conjunto específico de letras.
- **Entrada**: Prefijo de la palabra.
- **Salida**: Lista de palabras que comienzan con ese prefijo.

#### 2.1.3 Requisito: Búsqueda por Similitud
El sistema debe permitir a los usuarios buscar palabras similares basadas en un algoritmo específico (por ejemplo, Levenshtein).
- **Entrada**: Texto de la palabra.
- **Salida**: Lista de palabras similares.

### 2.2 Gestión de Diccionarios (Editor)
#### 2.2.1 Requisito: Crear Diccionario
El sistema debe permitir al editor crear nuevos diccionarios.
- **Entrada**: Nombre del diccionario, idioma asociado.
- **Salida**: Diccionario creado.

#### 2.2.2 Requisito: Modificar Diccionario
El sistema debe permitir al editor modificar los detalles de un diccionario existente.
- **Entrada**: Nombre del diccionario, idioma.
- **Salida**: Diccionario actualizado.

#### 2.2.3 Requisito: Eliminar Diccionario
El sistema debe permitir al editor eliminar un diccionario si no está en uso.
- **Entrada**: Nombre del diccionario.
- **Salida**: Diccionario eliminado.

### 2.3 Gestión de Palabras (Editor)
#### 2.3.1 Requisito: Crear Palabra
El sistema debe permitir al editor agregar nuevas palabras a un diccionario.
- **Entrada**: Texto de la palabra, significados, variantes.
- **Salida**: Palabra agregada al diccionario.

#### 2.3.2 Requisito: Modificar Palabra
El sistema debe permitir al editor modificar una palabra existente en un diccionario.
- **Entrada**: Texto de la palabra, significados actualizados, variantes.
- **Salida**: Palabra modificada.

#### 2.3.3 Requisito: Eliminar Palabra
El sistema debe permitir al editor eliminar una palabra de un diccionario.
- **Entrada**: Texto de la palabra.
- **Salida**: Palabra eliminada.

### 2.4 Gestión de Idiomas (Editor)
#### 2.4.1 Requisito: Crear Idioma
El sistema debe permitir al editor agregar nuevos idiomas.
- **Entrada**: Nombre del idioma, código de idioma.
- **Salida**: Idioma agregado al sistema.

#### 2.4.2 Requisito: Modificar Idioma
El sistema debe permitir al editor modificar los detalles de un idioma existente.
- **Entrada**: Nombre del idioma, código de idioma.
- **Salida**: Idioma modificado.

#### 2.4.3 Requisito: Eliminar Idioma
El sistema debe permitir al editor eliminar un idioma siempre y cuando no tenga diccionarios asociados.
- **Entrada**: Nombre del idioma.
- **Salida**: Idioma eliminado.


## 3. Requisitos No Funcionales

### 3.2 Seguridad
El acceso al sistema debe estar restringido por roles (usuario y editor) y debe garantizarse la autenticación mediante un sistema de seguridad basado en tokens (JWT).

### 3.3 Escalabilidad
El sistema debe ser escalable horizontalmente, permitiendo agregar más servidores en caso de aumento de carga.


## 4. Suposiciones y Dependencias

- Se asume que el sistema usará una base de datos relacional para almacenar los diccionarios, palabras e idiomas. No obstante, se debe diseñar de manera que sea independiente del tipo de base de datos. El día de mañana, si se decide cambiar a una base de datos NoSQL, el sistema debería poder adaptarse sin problemas.
