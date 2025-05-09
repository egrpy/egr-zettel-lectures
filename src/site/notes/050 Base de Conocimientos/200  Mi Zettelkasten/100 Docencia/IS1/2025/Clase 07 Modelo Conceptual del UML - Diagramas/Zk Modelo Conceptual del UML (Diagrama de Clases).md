---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Clases)/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Modelo Conceptual del UML (Diagrama de Clases)



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 13 Diagrama de Clases (Fundamentos, Elementos, Relaciones, etc.)/Zk Diagrama de Clases (Introducción, Definición, Características y sus Usos)/#definicion" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Definición

Un **diagrama de clases** es una representación gráfica que muestra las clases de un sistema, sus atributos, operaciones (métodos) y las relaciones estáticas entre ellas. Es el diagrama [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Estructurales)\|estructural]] más utilizado en UML y sirve como base para el análisis y diseño orientado a objetos ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]).


</div></div>


### Tipo

| Tipo                                                    | Objetivo                                                                                                       |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Estructurales)\|Estructural]] | Describe la estructura estática de un sistema, incluyendo clases, atributos, métodos y relaciones entre ellas. |

----
### Visualización
#### Escenario Elemental

**Figura**
_Ejemplo de Diagrama de Clases Simple_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

Title Préstamos de Libros de la Biblioteca

class Libro {
  - id: Integer
  - título: String
  - editorial: String
}

class Autor {
  - id: Integer
  - nombre: String
}

class Usuario {
  - id: Integer
  - nombre: String
}

class Prestamo {
  - id: Integer
  - fechaPrestamo: Date
  - fechaDevolucion: Date
}

Libro "1..*" -- "*" Autor : escribe
Usuario "0..*" -- "0..*" Prestamo : presta
Libro "0..*" -- "0..*" Prestamo : prestado

@enduml
```

#### Escenario Avanzado
**Figura**
_Ejemplo de Diagrama de Clases con Mayor Complejidad_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

class Libro {
  - id: Integer
  - título: String
  - ISBN: String
  - editorial: Editorial
  - genero: Genero
}

class Autor {
  - id: Integer
  - nombre: String
  - nacionalidad: String
}

class Usuario {
  - id: Integer
  - nombre: String
  - direccion: Direccion
  - telefono: String
}

class Prestamo {
  - id: Integer
  - libro: Libro
  - usuario: Usuario
  - fechaPrestamo: Date
  - fechaDevolucion: Date
  - estado: EstadoPrestamo
}

class Editorial {
  - id: Integer
  - nombre: String
  - direccion: Direccion
}

class Genero {
  - id: Integer
  - nombre: String
  - descripcion: String
}

class Direccion {
  - calle: String
  - ciudad: String
  - codigoPostal: String
}

enum EstadoPrestamo {
  PRESTADO
  DEVUELTO
  ATRASADO
}

Libro "1..*" -- "*" Autor : escribe
Usuario "0..*" -- "0..*" Prestamo : presta
Libro "0..*" -- "0..*" Prestamo : prestado
Libro "1" -- "1" Editorial : publicadoPor
Libro "1" -- "1" Genero : perteneceA
Usuario "1" -- "1" Direccion : viveEn
Editorial "1" -- "1" Direccion : ubicadaEn
Prestamo "1" -- "1" Libro : tiene
Prestamo "1" -- "1" Usuario : realizadoPor
Prestamo "1" -- "1" EstadoPrestamo : estadoActual

@enduml
```

----
### Elementos y Relaciones más Comunes

| Elementos más                | Relaciones                                   | Otros                                                                                                                                    |
| ---------------------------- | -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Clases, interfaces, paquetes | Asociaciones, dependencias, generalizaciones | - Fundamental en el diseño de software.<br>- Utilizado para visualizar la estructura del sistema<br>- Deben llevar un nombre descriptivo |
_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                                                | Escenarios                                             |
| --------------------------------------------------------------------------- | ------------------------------------------------------ |
| Modelado de sistemas de información, de persistencia de datos, entre otros. | Análisis de requisitos, definición de funcionalidades. |
