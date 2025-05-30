---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso)/","tags":["digitalGarden","diagramaCasosDeUso","relaciones"]}
---

## Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso)

En un diagrama de casos de uso, los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] se relacionan con el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Sujeto)\|sujeto]] a través de las funcionalidades representadas por los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|casos de uso]]. Estas relaciones se modelan mediante [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Relaciones)#Asociación\|asociaciones]], que indican cómo los actores interactúan o se comunican con los casos de uso ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006, p. 244]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017, sección 18]]). 

### Asociación entre Actores y Casos de Uso

#### Representación Gráfica

En UML, una asociación entre un actor y un caso de uso se representa como una línea simple que conecta ambos elementos. Esta línea indica que el actor participa en el caso de uso, ya sea iniciándolo o colaborando en su ejecución.

Figura
_Ejemplo de Representación Gráfica de Asociación Entre Actor y Caso de Uso_
```plantuml
@startuml
!pragma layout smetana
	skinparam style strictuml
	skinparam classAttributeIconSize 0
	skinparam BackgroundColor LightGray
	left to right direction
	'top to bottom direction
	skinparam linetype ortho

	scale 1.3
	
	actor Estudiante
	actor Cajero
	
	rectangle "Sistema Universidad" {
		usecase "Verificar Saldo" as UC1
		usecase "Pagar Cuota" as UC2
	}
	
	Estudiante -[#red]- UC1
	Estudiante -[#red]- UC2 : Paga
	UC2 -[#red]- Cajero :Cobra

	note as N1
		El color rojo de las
		asociaciones, son al
		solo efecto resaltar
		en este ejemplo.
	end note
@enduml
```
{ #195d41}


#### Ejemplos Prácticos

>[!Example] Ejemplo 1
>Estudiante realiza el pago de su cuota de la universidad desde una boca de cobranza externa.
>- Si bien el Estudiante paga su cuota, y transacción debe registrarse en el Sistema Universidad (SU), en este caso el Estudiante interactúa con el Sistema de la Boca de Cobranza (SBC), no con SU.
>- El SBC es el actor primario que interactúa con SU.

**Figura**
_Pago de Cuota de Universidad Vía Boca de Cobranza (Externa)_
```plantuml
@startuml
!pragma layout smetana
	skinparam style strictuml
	skinparam classAttributeIconSize 0
	skinparam BackgroundColor LightGray
  left to right direction
	'top to bottom direction
	skinparam linetype ortho

  rectangle "Sistema Universidad" {
    usecase "Procesar Pago de\nBoca de Cobranza" as UC
  }
  
  actor "Boca de Cobranza" as BC 
  note bottom of BC : Actor Primario
  
  BC -- UC : Transacción de Pago de\nCuota de un Estudiante
  note "El estudiante no interactúa\ndirectamente con el Sistema Universidad" as N1
@enduml
```

> [!Example] Ejemplo 2 
> Estudiante realiza el pago de su cuota de la universidad en una Caja de la universidad.
> - El Estudiante inicia el proceso de pago de su cuota en SU, por tanto es el actor primario
> - El Cajero, es un actor secundario, que interactúa con SU para Registrar Pago de Cuota.

**Figura**
_Pago de Cuota Vía Caja Interna de la Universidad_
```plantuml
@startuml
  !pragma layout smetana
  skinparam style strictuml
  skinparam classAttributeIconSize 0
  skinparam BackgroundColor LightGray
  left to right direction
  'top to bottom direction
  skinparam linetype ortho

  scale 1.5
  rectangle "Sistema Universidad" {
    usecase "Procesar Pago\nen Caja" as UC
  }

  actor Estudiante
  actor Cajero

  Estudiante -- UC : Paga Cuota
  UC -- Cajero : Registra Pago
@enduml
```

----
#### Algunas Notaciones Adicionales

Las siguiente notaciones pueden enriquecer la semántica de las asociaciones entre los actores y los casos de uso. Todas ellas son opcionales.

1. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso, Multiplicidad)\|Multiplicidad]]
2. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso, Nombre)\|Nombre de la Asociación (Opcional)]]
3. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso, Nombre)\|Nombre de la Asociación]]
4. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores y Casos de Uso, Navegabilidad)\|Sentido de la Navegación Asociación]]
5. Otros, UML proporciona múltiples mecanismos y notaciones para aumentar el entendimiento de los modelos.

#### Aspectos Avanzados

1. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Actores, Uso de la Relación de Generalización para Casos de Uso con Usuarios Multiples pero no Concurrentes)\|Casos de Uso con Varios Actores no Concurrentes]]. Se refiere al caso en que varios actores pueden usar el caso de uso pero no se requiere que todos estén presentes. 
