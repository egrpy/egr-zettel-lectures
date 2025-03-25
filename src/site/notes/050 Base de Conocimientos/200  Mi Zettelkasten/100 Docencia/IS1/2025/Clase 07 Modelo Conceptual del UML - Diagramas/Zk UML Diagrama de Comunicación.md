---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk UML Diagrama de Comunicación/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Diagrama de Comunicación

El diagrama de comunicación es un tipo de diagrama dinámico que describe la estructura de las interacciones entre objetos, enfocándose en la organización de los mensajes y las conexiones entre los participantes. Aunque similar al diagrama de secuencia, se centra más en la estructura de las interacciones.

| Tipos                                                       | Objetivo                                                                                                       |
| ----------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Dinámico]] | Describe la estructura estática de un sistema, incluyendo clases, atributos, métodos y relaciones entre ellas. |

----
### Visualización
#### Escenario Elemental
**Figura**
_Ejemplo de Diagrama de Comunicación Simple_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

Title Buscar Libro
!$left="←"
!$right="→"
!$up="↑"
!$down="↓"

Actor Usuario
rectangle ":GUIBuscarLibro" as GUIBuscarLibro
rectangle ":libro" as libro

Usuario --r- GUIBuscarLibro : 1: buscarLibro() $right\n4: mostrarResultado() $left
GUIBuscarLibro --r- libro : 2: verLibros() $right\n3: listaLibros() $left
@enduml

```

#### Escenario Avanzado
**Figura**
_Ejemplo de Diagrama de Comunicación más Complejo_
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

!$left="←"
!$right="→"
!$up="↑"
!$down="↓"

Actor Usuario
rectangle ":GUIBuscarLibro" as GUIBuscarLibro
rectangle ":libro" as libro
rectangle ":GUIRegistrarPréstamo" as GUIRegistrarPréstamo
rectangle ":prestamos" as prestamos

Usuario --d- GUIBuscarLibro : 1: buscarLibro() $down\n4: mostrarListaLibros() $up
GUIBuscarLibro --d- libro : 2: verLibros() $down\n3: listaLibros() $up

Usuario --r- GUIRegistrarPréstamo : 5: solicitarPréstamo() $right\n8: notificarPréstamo() $left
GUIRegistrarPréstamo --d- prestamos : 6: registrarPréstamo() $down\n7: confirmarPréstamo() $up

@enduml
```

----
### Características Relevantes

| Elementos más Frecuentes                         | Relaciones                                                                                                                                              | Otros                                                                    |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Participantes (que pueden ser actores u objetos) | Vínculos (un solo vínculo entre dos participantes); Mensajes (ilustran interacciones entre participantes, representan operaciones o llamadas a métodos. | Utilizado para modelar la estructura de las interacciones entre objetos. |

_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                     | Escenarios                                    |
| ------------------------------------------------ | --------------------------------------------- |
| Diseño de interfaces, análisis de interacciones. | Desarrollo de software, modelado de sistemas. |

----
### Notas Adicionales
Anteriormente, este diagrama era conocido como **Diagrama de Colaboración** en versiones anteriores del UML. El nombre cambió a **Diagrama de Comunicación** en UML 2.0 para enfatizar su enfoque en la estructura de las interacciones entre los participantes.
