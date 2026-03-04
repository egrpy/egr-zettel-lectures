---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Ingeniería del Software 1/Clase 01 Presentación/Zk Ingeniería del Software 1 Presentación/","tags":["#definir"]}
---

## Ingeniería del Software 1 Presentación

**Figura**
_Recorrido de Conceptual de Ingeniería de Software_
```plantuml
!pragma layout smetana
'skinparam style strictuml
'skinparam classAttributeIconSize 0
'skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
'skinparam linetype ortho
'scale 1

'skinparam defaultFontName Arial

title Ingeniería del Software 1 - Estructura del Curso

' Estilos por estereotipo
skinparam rectangle {
    BackgroundColor<<fundamento>> #E8F5E9
    BorderColor<<fundamento>> #4CAF50
    BackgroundColor<<paradigma>> #E3F2FD
    BorderColor<<paradigma>> #2196F3
    BackgroundColor<<sdlc>> #FFF9C4
    BorderColor<<sdlc>> #FFC107
    BackgroundColor<<gestion>> #F3E5F5
    BorderColor<<gestion>> #9C27B0
}

rectangle "NIVEL 1: FUNDAMENTOS" <<fundamento>> {
  component "IS & Complejidad" as F1
  component "Proceso & Modelado" as F2
}

note left of F1
  Ingeniería del Software
  Complejidad del Software
  Costos (Directo, Indirecto, Ocultos)
end note

note right of F2
  Proceso del Software
  Modelos: Cascada, Incremental,
  Evolutivo, Espiral
  Modelos ágiles y contemporáneos
  ¿Por qué modelar?
  Principios y niveles del modelado
end note

rectangle "NIVEL 2: PARADIGMA OO" <<paradigma>> {
  component "Conceptos OO" as OO1
  component "Elementos OO" as OO2
}

note right of OO1
  Abstracción
  Herencia
  Polimorfismo
  Encapsulamiento
end note

note right of OO2
  Clases y objetos
  Atributos
  Operaciones / Métodos
  Mensajes
end note

rectangle "NIVEL 3: SDLC -  SOFTWARE DEVELOPMENT LIFE CYCLE\nCICLO DE VIDA DEL DESARROLLO DEL SOFTWARE" <<sdlc>> {

  package "Comprensión (¿Qué?)" {
    component "Elicitación de\nrequerimientos" as REQ
    component "Análisis" as ANA
  }

  package "Construcción (¿Cómo?)" {
    component "Diseño del sistema" as DIS_S
    component "Diseño de objetos" as DIS_O
    component "Implementación" as IMP
  }

  package "Validación (¿Funciona?)" {
    component "Pruebas" as TEST
  }

  REQ -right-> ANA
  ANA -right-> DIS_S
  DIS_S -right-> DIS_O
  DIS_O -right-> IMP
  IMP -right-> TEST
}

rectangle "NIVEL 4: GESTIÓN" <<gestion>> {
  component "Comunicación" as COM
  component "Rationale" as RAT
  component "Configuración" as CONF
  component "Proyectos" as PM

  COM -[hidden]right- RAT
  RAT -[hidden]right- CONF
  CONF -[hidden]right- PM
}

' Relaciones entre niveles
F1 -[#green,bold]down-> OO1 : requiere\ncomprender
F2 -[#green,bold]down-> OO2 : aplica\ntécnicas

OO1 -[#blue,bold]down-> REQ : se\nutiliza en
OO2 -[#blue,bold]down-> ANA : modela\ncon

REQ ..down..> COM : usa
ANA ..down..> RAT : genera
IMP ..down..> CONF : requiere
TEST ..down..> PM : reporta

' Anotaciones globales
note right of F1
  Cap. 1: Base conceptual
  de la disciplina
end note

note right of OO1
  Cap. 2: Paradigma fundamental
end note

note right of REQ
  Cap. 4–11: Actividades
  centrales del desarrollo
end note

note bottom of COM
  Cap. 3, 12–14: Soporte
  transversal al SDLC
end note

note right
  Flujo de aprendizaje: de lo conceptual (niveles 1–2)
  a lo práctico (niveles 3–4).
  UML: notación común en todos los niveles.
end note

@enduml
```
*Nota*: La visualización con smetama es ligeramente distinta a sin ella