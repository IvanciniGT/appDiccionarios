Aquí tienes los requisitos ajustados a los nuevos casos de uso que mencionaste:

---

# Requisitos - Aplicación de Diccionarios

Estos son los requisitos de la aplicación de diccionarios, utilizada en los videos y formaciones de **Iván Osuna Ayuste**, y está protegido bajo la licencia **Creative Commons BY-NC-SA** y las leyes de **Copyright ©**. [Ver más...](#copyright-y-licencia)

© 2024 Iván Osuna Ayuste. Todos los derechos reservados.

## 1. Introducción

### 1.1 Propósito
Este documento describe los requisitos funcionales y no funcionales de la aplicación de diccionarios. Está diseñado para proporcionar una guía clara sobre las funcionalidades que se implementarán, así como los criterios que deben cumplirse para que el sistema cumpla con las expectativas de los usuarios finales.

### 1.2 Alcance
El proyecto es una aplicación de diccionarios que permite a los usuarios realizar búsquedas de palabras y a los editores gestionar diccionarios, palabras e idiomas. La aplicación está orientada a la formación y a la creación de contenido educativo para **Iván Osuna**.

## 2. Definiciones Clave

### 2.1 Idioma
Un **Idioma** representa el lenguaje al que pertenecen las palabras o significados dentro de la aplicación. Cada idioma tiene un código único, como `es` para español o `en` para inglés. Además, cada idioma puede estar asociado a varios diccionarios. En algunos contextos, los idiomas pueden tener un icono que los representa visualmente, aunque esto no es necesario en todos los casos.

### 2.2 Diccionario
Un **Diccionario** es un conjunto de palabras asociadas a un idioma específico. Cada diccionario tiene un nombre único y contiene una lista de palabras. Las palabras en el diccionario están asociadas a significados y variantes, permitiendo su búsqueda y gestión.

### 2.3 Tipo Morfológico
El **Tipo Morfológico** describe la categoría gramatical o morfológica de una palabra o de sus variantes. Esto incluye categorías como sustantivos, verbos o adjetivos. Cada tipo morfológico tiene una descripción detallada para aclarar su función dentro del idioma.

### 2.4 Palabra
Una **Palabra** es una entidad central en la aplicación de diccionarios, que puede tener múltiples significados y variantes. Cada palabra está asociada a un diccionario y puede tener varias formas morfológicas. Las palabras pueden ser buscadas por los usuarios y gestionadas por los editores.

### 2.5 Contexto
El **Contexto** define el escenario en el que un significado de una palabra es aplicable. Cada significado puede tener varios contextos que ayudan a desambiguar su uso en diferentes situaciones. Un contexto también incluye una descripción detallada de cómo se usa la palabra en ese contexto específico.

### 2.6 Significado
Un **Significado** es la definición de una palabra en un contexto determinado. Las palabras pueden tener múltiples significados, cada uno con su posición en la lista de significados, morfología asociada, contexto de uso, ejemplos y posibles sinónimos. Los significados ayudan a los usuarios a entender las diferentes formas en que una palabra puede ser utilizada.

### 2.7 Variante
Una **Variante** es una forma morfológica alternativa de una palabra. Las variantes están asociadas a un tipo morfológico específico, como un verbo conjugado o un adjetivo en plural. Estas variantes permiten que una palabra tenga múltiples formas, adaptadas a distintas estructuras gramaticales o contextos.

## 3. Requisitos Funcionales

### 3.1 Requisitos Funcionales de Búsqueda de Palabras (CU01)
#### RF01: Búsqueda Exacta
El sistema debe permitir a los usuarios buscar palabras específicas dentro de un diccionario (case-insensitive, acentos-insensitive, plural-insensitive).
- **Entrada**: Texto de la palabra.
- **Salida**: Palabra encontrada con sus significados y variantes.
- **Caso de uso asociado**: UC01

#### RF02: Búsqueda por Prefijo
El sistema debe permitir a los usuarios buscar palabras que comiencen con un conjunto específico de letras (case-insensitive, acentos-insensitive, plural-insensitive).
- **Entrada**: Prefijo de la palabra.
- **Salida**: Lista de palabras que comienzan con ese prefijo.
- **Caso de uso asociado**: UC02

#### RF03: Búsqueda por Similitud
El sistema debe permitir a los usuarios buscar palabras similares basadas en un algoritmo específico (por ejemplo, Levenshtein).
- **Entrada**: Texto de la palabra.
- **Salida**: Lista de palabras similares.
- **Caso de uso asociado**: UC03

### 3.2 Requisitos Funcionales de Gestión de Diccionarios (CU02)
#### RF04: Crear Diccionario
El sistema debe permitir al editor crear nuevos diccionarios.
- **Entrada**: Nombre del diccionario, idioma asociado.
- **Salida**: Diccionario creado.
- **Caso de uso asociado**: UC11

#### RF05: Modificar Diccionario
El sistema debe permitir al editor modificar los detalles de un diccionario existente.
- **Entrada**: Nombre del diccionario, idioma.
- **Salida**: Diccionario actualizado.
- **Caso de uso asociado**: UC11

#### RF06: Eliminar Diccionario
El sistema debe permitir al editor eliminar un diccionario si no está en uso.
- **Entrada**: Nombre del diccionario.
- **Salida**: Diccionario eliminado.
- **Caso de uso asociado**: UC11

#### RF07: Recuperar Diccionario(s)
El sistema debe permitir al editor consultar o listar diccionarios en el sistema.
- **Entrada**: Parámetros de búsqueda (opcional).
- **Salida**: Diccionarios recuperados.
- **Caso de uso asociado**: UC12

### 3.3 Requisitos Funcionales de Gestión de Palabras (CU03)
#### RF08: Crear Palabra
El sistema debe permitir al editor agregar nuevas palabras a un diccionario.
- **Entrada**: Texto de la palabra, significados, variantes.
- **Salida**: Palabra agregada al diccionario.
- **Caso de uso asociado**: UC13

#### RF09: Modificar Palabra
El sistema debe permitir al editor modificar una palabra existente en un diccionario.
- **Entrada**: Texto de la palabra, significados actualizados, variantes.
- **Salida**: Palabra modificada.
- **Caso de uso asociado**: UC13

#### RF10: Eliminar Palabra
El sistema debe permitir al editor eliminar una palabra de un diccionario.
- **Entrada**: Texto de la palabra.
- **Salida**: Palabra eliminada.
- **Caso de uso asociado**: UC13

#### RF11: Recuperar Palabra(s)
El sistema debe permitir al editor consultar o listar palabras en el sistema.
- **Entrada**: Parámetros de búsqueda (opcional).
- **Salida**: Palabras recuperadas.
- **Caso de uso asociado**: UC14

### 3.4 Requisitos Funcionales de Gestión de Idiomas (CU04)
#### RF12: Crear Idioma
El sistema debe permitir al editor agregar nuevos idiomas.
- **Entrada**: Nombre del idioma, código de idioma.
- **Salida**: Idioma agregado al sistema.
- **Caso de uso asociado**: UC15

#### RF13: Modificar Idioma
El sistema debe permitir al editor modificar los detalles de un idioma existente.
- **Entrada**: Nombre del idioma, código de idioma.
- **Salida**: Idioma modificado.
- **Caso de uso asociado**: UC15

#### RF14: Eliminar Idioma
El sistema debe permitir al editor eliminar un idioma siempre y cuando no tenga diccionarios asociados.
- **Entrada**: Nombre del idioma.
- **Salida**: Idioma eliminado.
- **Caso de uso asociado**: UC15

#### RF15: Recuperar Idiomas
El sistema debe permitir al editor consultar o listar idiomas en el sistema.
- **Entrada**: Parámetros de búsqueda (opcional).
- **Salida**: Idiomas recuperados.
- **Caso de uso asociado**: UC16

### 3.5 Requisitos Funcionales de Administración (CU05)
#### RF16: Exportar Diccionarios
El sistema debe permitir al administrador exportar diccionarios.
- **Entrada**: Parámetros de exportación (idioma, nombre del diccionario).
- **Salida**: Archivo con el diccionario exportado.
- **Caso de uso asociado**: UC21

#### RF17: Importar Diccionarios
El sistema debe permitir al administrador importar diccionarios desde un archivo.
- **Entrada**: Archivo del diccionario.
- **Salida**: Diccionario importado al sistema.
- **Caso de uso asociado**: UC22

## 4. Requisitos No Funcionales

### RNF01: Seguridad
El acceso al sistema debe estar restringido por roles (usuario, editor y administrador) y debe garantizarse la autenticación mediante un sistema de seguridad basado en tokens (JWT).

### RNF02: Escalabilidad
El sistema debe ser escalable horizontalmente, permitiendo agregar más servidores en caso de aumento de carga.

## 5. Relación entre Casos de Uso y Requisitos

| Código del Caso de Uso | Descripción del Caso de Uso                      | Requisitos Relacionados            |
|------------------------|-------------------------------------------------|------------------------------------|
| **UC01**               | Búsqueda exacta de palabras                     | RF01                              |
| **UC02**               | Búsqueda por prefijo                            | RF02                              |
| **UC03**               | Búsqueda por similitud                          | RF03                              |
| **UC11**               | Gestionar diccionario                           | RF04, RF05, RF06                  |
| **UC12**               | Recuperar diccionario(s)                        | RF07                              |
| **UC13**               | Gestionar palabras                              | RF08, RF09, RF10                  |
| **UC14**               | Recuperar palabra(s)                            | RF11                              |
| **UC15**               | Gestionar idioma                                | RF12, RF13, RF14                  |
| **UC16**               | Recuperar idiomas                               | RF15                              |
| **UC21**               | Exportar diccionarios                           | RF16                              |
| **UC22**               | Importar diccionarios                           | RF17                              |

### Diagrama UML 

```mermaid
graph LR
    CU01[Búsqueda exacta de palabras]
    CU02[Búsqueda por prefijo]
    CU03[Búsqueda por similitud]
    CU11[Gestionar diccionario]
    CU12[Recuperar diccionario(s)]
    CU13[Gestionar palabras]
    CU14[Recuperar palabra(s)]
    CU15[Gestionar idioma]
    CU16[Recuperar idiomas]
    CU21[Exportar diccionarios]
    CU22[Importar diccionarios]

    RF01[RF01: Búsqueda exacta]
    RF02[RF02: Búsqueda por prefijo]
    RF03[RF03: Búsqueda por similitud]
    RF04[RF04: Crear diccionario]
    RF05[RF05: Modificar diccionario]
    RF06[RF06: Eliminar diccionario]
    RF07[RF07: Recuperar diccionario(s)]
    RF08[RF08: Crear palabra]
    RF09[RF09: Modificar palabra]
    RF10[RF10: Eliminar palabra]
    RF11[RF11: Recuperar palabra(s)]
    RF12[RF12: Crear idioma]
    RF13[RF13: Modificar idioma]
    RF14[RF14: Eliminar idioma]
    RF15[RF15: Recuperar idiomas]
    RF16[RF16: Exportar diccionarios]
    RF17[RF17: Importar diccionarios]

    CU01 --> RF01
    CU02 --> RF02
    CU03 --> RF03
    CU11 --> RF04
    CU11 --> RF05
    CU11 --> RF06
    CU12 --> RF07
    CU13 --> RF08
    CU13 --> RF09
    CU13 --> RF10
    CU14 --> RF11
    CU15 --> RF12
    CU15 --> RF13
    CU15 --> RF14
    CU16 --> RF15
    CU21 --> RF16
    CU22 --> RF17
```

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

---

Este documento ahora refleja fielmente los casos de uso y requisitos ajustados según la nueva estructura definida.