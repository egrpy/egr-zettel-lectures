---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 03 Sinergia y Recursividad/Zk Sinergia en Acción (Ciclo de Vida del Agua)/","tags":["digitalGarden","sinergia"]}
---

## Sinergia en Acción

La [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 03 Sinergia y Recursividad/Zk Sinergia en la Teoría General de Sistemas\|sinergia]] juega un papel fundamental en el contexto de la compresión de la dinámica interna que se desarrolla en un sistemas. Utilizaremos un ejemplo cotidiano para ilustrar cómo las variables interactúan y se refuerzan mutuamente.

## Ciclo de Vida del Agua

### Variables
- Aguas Superficiales (lagos, estanques, océanos, etc.)
- Evaporación (evaporación de las aguas)
- Lluvia (agua evaporada que vuelve a caer)
- Corrientes de Agua (rios, arroyos, etc.)

### Relación de Variables

| Variables                                | Comentarios                                                                                                                                                                                                     |
| ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aguas Superficiales y Evaporación        | La cantidad de agua en las Aguas Superficiales influye positivamente en la evaporación. Cuanto más agua en las Aguas Superficiales, más evaporación ocurre.                                                     |
| Evaporación y Lluvias                    | La cantidad de agua en las Aguas Superficiales influye positivamente en la Evaporación. Cuanto más agua en las Aguas Superficiales, más Evaporación ocurre.                                                     |
| Lluvia y Corrientes de Agua              | La Lluvia influye positivamente en las Corrientes de Agua.<br>Más Lluvia significa más agua disponible para las Corrientes de Agua.                                                                             |
| Corrientes de Agua y Evaporación         | La cantidad de agua en las Corrientes de Agua influye positivamente en la Evaporación, aunque en menor medida que las Aguas Superficiales<br>Cuanto más agua en las Corrientes de Agua, más Evaporación ocurre. |
| Corrientes de Agua y Aguas Superficiales | Las Corrientes de Agua influyen positivamente en las Aguas Superficiales.<br>Las Corrientes de Agua, finalmente desembocan en las Aguas Superficiales, aumentando su volumen.                                   |

```plantuml
@startuml
!pragma layout smetana
skinparam Rectangle {
    BackgroundColor White
    BorderColor White
    FontColor green
}

skinparam defaultTextAlignment center
skinparam ArrowColor blue

rectangle "Aguas Superficiales" as AS
rectangle "Evaporación" as EV
rectangle "Lluvia" as LL
rectangle "Corrientes de Agua" as CA

AS --> EV 
CA --> EV 
EV --> LL 
LL --> CA 
CA --> AS 
```
Figura
_Interacción de Variables del Cliclo de Vida del Agua_
Nota: Elaboración Propia

Este ejemplo muestra cómo las variables en un sistema, **interactúan** de manera **sinérgica**, para crear un **efecto mayor que la suma de sus partes**. Además, ilustra cómo estos efectos pueden ser recursivos, donde el cambio en una variable puede influir en otras y eventualmente volver a influir en sí misma a través de un ciclo de retroalimentación.