---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores, Uso de la Relación de Generalización para Casos de Uso con Usuarios Multiples pero no Concurrentes)/","tags":["digitalGarden","diagramaCasosDeUso","casosDeUso"]}
---

## Uso de la Relación de Generalización para Casos de Uso con Usuarios Múltiples pero No Concurrentes

Una de las aplicaciones más frecuentes de la relación de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Relaciones)#Generalización\|generalización]] entre [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] en los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)]] se presenta cuando una funcionalidad puede ser empleada por diversos actores, sin que sea necesario que todos interactúen simultáneamente con el sistema. En este contexto, cada actor puede acceder de manera independiente a los servicios ofrecidos por el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Sujeto)\|sujeto]], sin depender de la presencia o intervención de los demás actores. Esta característica permite modelar de forma eficiente escenarios en los que diferentes tipos de usuarios comparten funcionalidades, pero los ejercen de manera autónoma y no concurrente. En estos casos se recomienda [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Relaciones)#Generalización\|generalizar]] estos actores en un actor común. Este actor generalizado se asocia entonces con el caso de uso en cuestión.

**Figura**
_Ejecución de Caso de Uso por Varios Actores no Simultáneos
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
left to right direction
'top to bottom direction
skinparam linetype ortho
scale 1

actor Actor1
actor Actor2
actor Actor3
actor ActorGeneral

Actor1 --|> ActorGeneral
Actor2 --|> ActorGeneral
Actor3 --|> ActorGeneral

ActorGeneral -- (Caso de Uso)

@enduml
```
_Nota:_ En este ejemplo tanto el Actor1, Actor2 como el Actor3 pueden ejecutar el Caso de Uso, pero no necesariamente de manera concurrente, es decir estar presentes para su uso.

Es fundamental distinguir entre la ejecución independiente de un caso de uso y la ejecución concurrente:
- La ejecución **independiente** implica que **cada actor puede iniciar y completar el caso de uso por sí mismo**, sin requerir la presencia o interacción simultánea de otros.

- La ejecución **concurrente**, por otro lado, implica que **los actores deben actuar juntos** en tiempo real para completar el caso de uso.

### Ventajas

| Ventaja            | Descripción                                                                                     |
| ------------------ | ----------------------------------------------------------------------------------------------- |
| Claridad           | Reduce la complejidad del diagrama y facilita la comprensión de quién puede realizar la acción. |
| Mantenibilidad     | Simplifica la adición de nuevos actores ejecutores.                                             |
| Semántica Correcta | Evita la interpretación errónea de ejecución simultánea.                                        |

### Ejemplo

En el contexto de un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Sujeto)\|sujeto]] como un Smart TV, los padres (Padre, Madre) pueden configurar el televisor de forma independiente. En lugar de asociar cada padre directamente con el caso de uso "Configurar Smart TV", se generalizan bajo el actor "Tutor".

**Figura**
_Padre o Madre Pueden Configurar el Smart TV_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
left to right direction
skinparam conditionStyle InsideDiamond
skinparam linetype ortho

actor Tutor
actor Padre
actor Madre

Padre --|> Tutor
Madre --|> Tutor

rectangle "Smart TV" {
  (Configurar TV) as UC6
  (Control Parental) as UC7
}

Tutor --> UC6
UC6 <.. UC7 : <<extend>>

@enduml
```
_Nota:_ En el ejemplo, el padre o la madre pueden configurar el Smart TV.

### Caso Mixto

Es posible encontrar escenarios donde múltiples actores participan en un caso de uso de forma independiente, pero además se requiere la presencia de otro u otros actores para su ejecución. Por ejemplo, retomando el caso del Smart TV, si este presenta un desperfecto, se necesita la intervención de un técnico de reparación a domicilio (Caso de Uso: Diagnosticar Desperfecto). Para que el técnico pueda realizar su trabajo, el padre o la madre deben estar presentes durante el diagnóstico.

**Figura**
_Diagnóstico de Desperfacto de Smart TV_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
left to right direction
skinparam conditionStyle InsideDiamond
skinparam linetype ortho

actor Tutor
actor Padre
actor Madre
actor "Técnico TV" as Tecnico

Padre --|> Tutor
Madre --|> Tutor

rectangle "Smart TV" {
  (Diagnosticar Desperfecto) as Diagnosticar
}

Tutor -- Diagnosticar
Tecnico -- Diagnosticar

note left of Tutor : Debe estar presente\nPadre o Madre
note right of Tecnico : Realiza el diagnóstico

@enduml
```
