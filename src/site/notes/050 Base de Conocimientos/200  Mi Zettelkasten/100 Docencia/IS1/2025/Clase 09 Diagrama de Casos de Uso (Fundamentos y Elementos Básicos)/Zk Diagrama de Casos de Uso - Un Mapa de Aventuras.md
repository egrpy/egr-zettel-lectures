---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Un Mapa de Aventuras/","tags":["digitalGarden","diagramaCasosDeUso"]}
---

## Diagrama de Casos de Uso - Un Mapa de Aventuras

Imaginemos un **mapa de aventuras**, donde los **actores**, nuestros protagonistas, exploran un mundo llamado **sistema**. Cada acción que realizan, desde buscar ayuda hasta rescatar a un prisionero, representa una pequeña **aventura**, también conocida como **caso de uso**, con su propio inicio, desarrollo y desenlace. El **diagrama de casos de uso** es este mapa, que conecta todas las aventuras y muestra los caminos posibles, así como los **objetivos** que los actores pueden alcanzar dentro del sistema.

**Figura**
_Un Mapa de Aventuras_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
left to right direction
skinparam conditionStyle InsideDiamond
skinparam linetype ortho

actor "Aventurero" as aventurero
actor "Guía" as guia

rectangle "Mundo de Aventuras (Sistema)" {
  usecase "Buscar Ayuda" as UC2
  usecase "Encontrar un Tesoro" as UC1
  usecase "Descubrir un Secreto" as UC4
  usecase "Recolectar Recursos" as UC5
  usecase "Defender el Reino" as UC6
  usecase "Construir un Puente" as UC7
  usecase "Buscar Lianas" as UC8
  usecase "Rescatar un Prisionero" as UC9
}

aventurero --> UC1
aventurero --> UC2
'aventurero --> UC4
aventurero --> UC5
'aventurero --> UC6
aventurero --> UC7
'aventurero --> UC8


guia <-- UC2

UC1 ..> UC6
UC5 <.. UC7
UC1 ..> UC4
UC5 <.. UC6
UC6 ..> UC9
UC7 ..> UC8

@enduml
```
_Nota:_ Cada caso de uso tiene su historia, un inicio un desarrollo y desenlace.

**Figura**
_Las Aventuras de un Estudiante al Cursar Ingeniería del Software_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
left to right direction
'top to bottom direction
skinparam linetype ortho

actor Estudiante1 as "Estudiante:1"
actor Estudiante2 as "Estudiante:2"
rectangle "Aventuras de un Estudiante\nal Cursar Ingeniería del Software" {
  usecase "Inscribirse a la Asignatura" as UC1
  usecase "Asistir a Clases" as UC2
  usecase "Estudiar" as UC9
  usecase "Hacer Tareas" as UC3
  usecase "Entregar Tareas" as UC4
  usecase "Estudiar para Parcial" as UC5
  usecase "Rendir Examen Parcial" as UC6
  usecase "Estudiar para Final" as UC7
  usecase "Rendir Examen Final" as UC8
}
Estudiante1 --> UC1 : Inicia la aventura
Estudiante1 --> UC2 : Asiste a clases
Estudiante1 --> UC3 : Realiza tareas

Estudiante2 -u-> UC6 : Rinde parcial
Estudiante2 -u-> UC8 : Rinde final

UC2 ..> UC9
UC3 ..> UC4
UC3 ..> UC9
UC9 <|-- UC5
UC9 <|-- UC7
UC5 ..> UC6
UC7 ..> UC8
@enduml
```

A partir de estos ejemplos introductorios, podemos extraer algunas ideas que nos servirán para comprender mejor el **Diagrama de Casos de Uso**.

| **Idea**                                            | **Analogía**                             |
| --------------------------------------------------- | ---------------------------------------- |
| Un sistema tiene **actores** que interactúan con él | Aventureros que exploran un mundo        |
| Cada acción relevante es un **caso de uso**         | Cada misión es una aventura              |
| Los casos de uso tienen un inicio y un fin          | Cada aventura tiene su propia historia   |
| Los actores pueden compartir casos de uso           | Aventureros pueden seguir mismos caminos |
| Algunos casos de uso dependen de otros              | Algunas misiones requieren pasos previos |

El **diagrama de casos de uso** es una herramienta poderosa que nos permite visualizar cómo los actores interactúan con un sistema para alcanzar objetivos específicos. A través de la analogía del "mapa de aventuras", hemos explorado cómo cada caso de uso representa una pequeña historia con un inicio, desarrollo y desenlace, conectando las interacciones y objetivos dentro del sistema.

Estos ejemplos iniciales nos invitan a reflexionar sobre cómo modelar sistemas no solo desde la perspectiva técnica, sino también desde el punto de vista narrativo y funcional. A medida que avancemos en el estudio de los elementos y relaciones en UML, podremos refinar estos diagramas para capturar con mayor precisión la complejidad y riqueza de los sistemas que modelamos. En definitiva, cada diagrama es un mapa que guía tanto a los desarrolladores como a los usuarios hacia una comprensión compartida del sistema.