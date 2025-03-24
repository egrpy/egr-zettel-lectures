---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk UML Diagrama de Objetos/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Diagrama de Objetos

El diagrama de objetos es un tipo de diagrama estructural que muestra instancias de clases y sus relaciones en un momento específico. Se utiliza para visualizar escenarios de ejecución o pruebas de sistemas, ayudando a entender cómo se comportan los objetos en tiempo de ejecución.

| Tipos                                                          | Objetivo                                                                                    |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Estructural]] | Describe un momento específico del sistema, mostrando instancias de clases y sus relaciones |

----
### Visualización
#### Escenario Elemental
**Figura**
_Ejemplo de Diagrama de Objetos Simple
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

Title Préstamos de Líbros de la Biblioteca

object Libro1 {
  id = 1
  título = "Harry Potter"
  editorial = "Bloomsbury"
}

object Libro2 {
  id = 2
  título = "El Señor de los Anillos"
  editorial = "Allen & Unwin"
}

object Autor1 {
  id = 1
  nombre = "J.K. Rowling"
}

object Autor2 {
  id = 2
  nombre = "J.R.R. Tolkien"
}

object Usuario1 {
  id = 1
  nombre = "Juan"
}

Libro1 -- Autor1 : escritoPor
Libro2 -- Autor2 : escritoPor
Usuario1 -- Libro1 : presta
Usuario1 -- Libro2 : presta
@enduml
```

#### Escenario Complejo
**Figura**
_Ejemplo de Diagrama de Objetos con Mayor Complejidad_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

Title Préstamos de Líbros de la Biblioteca

object Libro1 {
  id = 1
  título = "Harry Potter"
  ISBN = "9780747532743"
  editorial = Editorial1
  genero = Genero1
}

object Libro2 {
  id = 2
  título = "El Señor de los Anillos"
  ISBN = "9780261102385"
  editorial = Editorial2
  genero = Genero2
}

object Autor1 {
  id = 1
  nombre = "J.K. Rowling"
  nacionalidad = "Británica"
}

object Autor2 {
  id = 2
  nombre = "J.R.R. Tolkien"
  nacionalidad = "Británica"
}

object Usuario1 {
  id = 1
  nombre = "Juan"
  direccion = Direccion1
  telefono = "+1234567890"
}

object Editorial1 {
  id = 1
  nombre = "Bloomsbury"
  direccion = Direccion2
}

object Editorial2 {
  id = 2
  nombre = "Allen & Unwin"
  direccion = Direccion3
}

object Genero1 {
  id = 1
  nombre = "Fantasía"
  descripcion = "Libros de fantasía"
}

object Genero2 {
  id = 2
  nombre = "Aventuras"
  descripcion = "Libros de aventuras"
}

object Direccion1 {
  calle = "Calle Principal"
  ciudad = "Ciudad A"
  codigoPostal = "12345"
}

object Direccion2 {
  calle = "Calle Editorial"
  ciudad = "Ciudad B"
  codigoPostal = "67890"
}

object Direccion3 {
  calle = "Calle Impresión"
  ciudad = "Ciudad C"
  codigoPostal = "34567"
}

Libro1 -- Autor1 : escritoPor
Libro2 -- Autor2 : escritoPor
Usuario1 -- Libro1 : presta
Usuario1 -- Libro2 : presta
Libro1 -- Editorial1 : publicadoPor
Libro2 -- Editorial2 : publicadoPor
Libro1 -- Genero1 : perteneceA
Libro2 -- Genero2 : perteneceA
Usuario1 -- Direccion1 : viveEn
Editorial1 -- Direccion2 : ubicadaEn
Editorial2 -- Direccion3 : ubicadaEn

@enduml
```

----
### Características Relevantes

| Elementos más Frecuentes              | Relaciones                 | Otros                                                                                                              |
| ------------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Objetos, que son instancias de clases | Asociaciones entre objetos | - Utilizado para visualizar escenarios de ejecución o pruebas de sistemas.<br>- Deben llevar un nombre descriptivo |
_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                                  | Escenarios                                        |
| ------------------------------------------------------------- | ------------------------------------------------- |
| Visualización de escenarios de ejecución, pruebas de sistemas | Análisis de comportamiento en tiempo de ejecución |
