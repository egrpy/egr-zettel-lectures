---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk UML Diagrama de Estados/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Diagrama de Estados

El diagrama de estados es un tipo de diagrama dinámico que describe los estados que puede tener un objeto y las transiciones entre ellos. Se utiliza para modelar el comportamiento de objetos que cambian de estado en respuesta a eventos.

| Tipos                                                       | Objetivo                                                                       |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------ |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Dinámico]] | Describe los estados que puede tener un objeto y las transiciones entre ellos. |

----
### Visualización
#### Escenario Elemental
**Figura**
_Ejemplo de Diagrama de Estados Simple_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho

Title Estados de Libros

state "Disponible" as disponible
state "Prestado" as prestado
state "Reservado" as reservado

[*] --> disponible
disponible --> prestado : Prestar
prestado --> disponible : Devolver
disponible --> reservado : Reservar
reservado --> disponible : Cancelar reserva
@enduml

```

#### Escenario Avanzado
**Figura**
_Ejemplo de Diagrama de Estados más Complejo_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho

title Estados de Libros

state "Disponible" as disponible
state "Prestado" as prestado
state "Reservado" as reservado
state "Atrasado" as atrasado

[*] --> disponible
disponible --> prestado : [usuario tiene menos de 3 préstamos pendientes]\nPrestar
prestado --> disponible : [devolución a tiempo]\nDevolver
prestado --> atrasado : [vencer fecha de devolución]\nVencer fecha de devolución /\nenviar notificación
atrasado --> disponible : [devolución con penalización]\nDevolver con penalización /\ncobrar multa
disponible --> reservado : [hay disponibilidad]\nReservar /\nenviar confirmación
reservado --> disponible : [cancelar reserva] Cancelar reserva\n / \nnotificar cancelación

@enduml

@enduml
```

----
### Características Relevantes

| Elementos más Frecuentes | Relaciones                 | Otros                                                                                                              |
| ------------------------ | -------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Estados, eventos         | Transiciones entre estados | Utilizado para modelar el comportamiento de objetos o grupos de este que cambian de estado en respuesta a eventos. |
_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                                                     | Escenarios                                               |
| -------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Modelado de sistemas de gestión de estado, diseño de protocolos de comunicación. | Desarrollo de software, modelado de sistemas de control. |
