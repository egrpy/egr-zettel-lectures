---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Secuencia)/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Modelo Conceptual del UML (Diagrama de Secuencia)

El diagrama de secuencia es un tipo de diagrama dinámico que muestra la secuencia temporal de mensajes entre objetos. Se utiliza para modelar interacciones entre objetos en el tiempo, ayudando a entender cómo se comportan los sistemas dinámicamente.

| Tipos                                            | Objetivo                                                                               |
| ------------------------------------------------ | -------------------------------------------------------------------------------------- |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Dinámico]] | Describe la secuencia temporal de mensajes entre los participantes (actores, objetos). |

----
### Visualización
#### Escenario Elemental
**Figura**
_Ejemplo de Diagrama de Secuencia Simple_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
skinparam linetype ortho
scale 1

actor Usuario
note top: Actor

rectangle ":Sistema" as Sistema
note right: Participante / Objeto

rectangle ":BaseDeDatos" as BaseDeDatos
rectangle ":Objeto" as Objeto

' Mensaje horizontal derecha (Usuario a Sistema)
Usuario -r- Sistema : 1: Solicita datos() <&arrow-right>

' Mensaje vertical abajo (Sistema a BaseDeDatos)
Sistema -d- BaseDeDatos : 2: Consulta datos() <&arrow-bottom>

' Mensaje vertical abajo (BaseDeDatos a Objeto)
BaseDeDatos -d- Objeto : 3: Calcular() <&arrow-bottom>

' Mensaje vertical arriba (Objeto a BaseDeDatos, retorno)
Objeto --u- BaseDeDatos : 4: Retorno <&arrow-top>

' Mensaje horizontal izquierda (Sistema a Usuario, retorno)
Sistema --l- Usuario : 5: Muestra datos() <&arrow-left>

@enduml
```

#### Escenario Avanzado
**Figura**
_Ejemplo de Diagrama de Secuencia más Complejo_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho

Title Prestar Libro

actor Usuario as "Usuario"
actor Bibliotecario as "Bibliotecario"

participant GUIBuscarLibro as ":GUIBuscarLibro"
participant GUIRegistrarPréstamo as ":GUIRegistrarPréstamo"
participant Libro as ":libro"
participant Prestamos as ":prestamos"

Usuario ->> Bibliotecario: solicitar libro
Bibliotecario ->> GUIBuscarLibro: buscarLibro()
GUIBuscarLibro ->> Libro: verLibros()
Libro -->> GUIBuscarLibro: listaLibros
GUIBuscarLibro -->> Bibliotecario: mostrar listaLibros

alt libro disponible
  Bibliotecario ->> GUIRegistrarPréstamo: registrarPréstamo()
  create Prestamos
  GUIRegistrarPréstamo ->> Prestamos: registrarPréstamo()
  Prestamos -->> GUIRegistrarPréstamo: confirmarPréstamo()
  GUIRegistrarPréstamo -->> Bibliotecario: mostrar confirmación
  Bibliotecario ->> Usuario: entregar libro físico
else libro no disponible
  GUIBuscarLibro -->> Bibliotecario: mostrar no disponible
  Bibliotecario ->> Usuario: notificar no disponible
end
@enduml
```

### Características Relevantes

| Elementos más Frecuentes                         | Relaciones                                                                                          | Otros                                                                    |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Participantes (que pueden ser actores u objetos) | Mensajes (ilustran interacciones entre participantes, representan operaciones o llamadas a métodos. | Utilizado para modelar interacciones con énfasis temporal entre objetos. |

_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                                      | Escenarios                                    |
| ----------------------------------------------------------------- | --------------------------------------------- |
| Análisis de comportamiento, diseño de protocolos de comunicación. | Desarrollo de software, modelado de sistemas. |
