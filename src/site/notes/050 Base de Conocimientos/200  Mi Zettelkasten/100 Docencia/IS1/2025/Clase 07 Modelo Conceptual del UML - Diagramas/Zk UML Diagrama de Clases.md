---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk UML Diagrama de Clases/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Diagrama de Clases

El diagrama de clases es un tipo de diagrama estructural que se utiliza para modelar la estructura estática de un sistema, mostrando las clases, sus atributos, métodos y las relaciones entre ellas. Es fundamental para diseñar y comprender la arquitectura de un sistema de software.

| Tipos                                                          | Objetivo                                                                                                       |
| -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Estructural]] | Describe la estructura estática de un sistema, incluyendo clases, atributos, métodos y relaciones entre ellas. |

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
### Características Relevantes

| Elementos más Frecuentes     | Relaciones                                   | Otros                                                                                                                                    |
| ---------------------------- | -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Clases, interfaces, paquetes | Asociaciones, dependencias, generalizaciones | - Fundamental en el diseño de software.<br>- Utilizado para visualizar la estructura del sistema<br>- Deben llevar un nombre descriptivo |
_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                                                | Escenarios                                             |
| --------------------------------------------------------------------------- | ------------------------------------------------------ |
| Modelado de sistemas de información, de persistencia de datos, entre otros. | Análisis de requisitos, definición de funcionalidades. |
