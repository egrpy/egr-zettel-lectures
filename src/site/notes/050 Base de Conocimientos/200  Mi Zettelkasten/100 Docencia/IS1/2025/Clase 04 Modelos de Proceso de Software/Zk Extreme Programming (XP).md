---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Extreme Programming (XP)/","tags":["digitalGarden","xp"]}
---

## Extreme Programming (XP)

### Definición
Extreme Programming es una metodología ágil que enfatiza la programación en pareja, la integración continua y la entrega continua de software funcional. Se centra en la simplicidad, la comunicación y la retroalimentación constante [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Beck, 2004) Extreme Programming Explained - Embrace Change\|(Beck, 2004)]].

### Principios

**Programación en Pareja** 
Dos desarrolladores trabajan juntos en una sola tarea.

**Integración Continua**
El código se integra frecuentemente para detectar errores temprano.

**Entrega Continua**
Se entrega software funcional al cliente de manera regular.

**Refactorización**
La [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Refactorización\|refactorización]] se refiere la mejora continua del código para mantener su simplicidad.

Figura
_Principios de XP_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho

package "Principios de XP" {
    class Pareja  #transparent;line:red;text:red {
        +desarrollador1: String
        +desarrollador2: String
        +colaborar()
    }
    
    class Tarea {
        +descripcion: String
        +completar()
    }
    
    class "Integración Continua" #transparent;line:red;text:red {
        +subirCódigo()
        +detectarErroresTemprano()
    }
    
    class "Entrega Continua" #transparent;line:red;text:red {
        +entregarSoftware()
    }
    
    class "Refactorización" #transparent;line:red;text:red {
        +mejorarContinuamente()
        +mantenerSimplicidad()
    }
    
    class Código {
    }
    
    class Cliente {
    }
    
    Pareja *-u- "Desarrollador 1" : Forma parte
    Pareja *-u- "Desarrollador 2" : Forma parte
    
    Pareja --r--> Tarea : Trabaja en
    Tarea --> Código : Genera
    Pareja -r-> "Integración Continua" : Sube\nCódigo
    
    Código <--> "Integración Continua" : Integra y\nAjusta

    
    "Integración Continua" --> "Entrega Continua" : Prepara\nEntrega
    "Entrega Continua" -r-> Cliente : Entrega\nSoftware
    
    Código <--> "Refactorización" : Refactoriza\ny Mejora

}
@enduml
```
Fuente: Elaboración Propia

### Ventajas   
**Calidad del Código**
La programación en pareja y la refactorización mejoran la calidad del código.

**Flexibilidad**
Permite adaptarse rápidamente a cambios en los requisitos.        

**Retroalimentación**
La entrega continua proporciona retroalimentación temprana del cliente.

### Referencias
Ver [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Beck, 2004) Extreme Programming Explained - Embrace Change\|(Beck, 2004)]]
