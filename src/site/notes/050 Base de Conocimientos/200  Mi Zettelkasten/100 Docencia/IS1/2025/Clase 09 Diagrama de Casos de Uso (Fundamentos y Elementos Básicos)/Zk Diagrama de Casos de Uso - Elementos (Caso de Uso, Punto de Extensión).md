---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso, Punto de Extensión)/","tags":["digitalGarden","diagramaCasosDeUso"]}
---

## Punto de Extensión de Caso de Uso

Un **punto de extensión** es una ubicación específica dentro del flujo de un caso de uso base donde se puede insertar un comportamiento adicional definido por otro caso de uso mediante la relación `<<extend>>`. Estos puntos permiten modelar funcionalidades opcionales o condicionales sin modificar el flujo principal del caso base. Se documenta en la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso, Especificación) Ejemplo\|especificación textual]] del caso de uso base.

### Propósito

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



### Propósito

| Propósito    | Explicación                                                             |
| ------------ | ----------------------------------------------------------------------- |
| Modularidad  | Separar funcionalidades opcionales o condicionales del flujo principal. |
| Flexibilidad | Permitir que el caso base funcione independientemente de la extensión.  |
| Claridad     | Evitar sobrecargar el caso base con variantes poco frecuentes.          |


</div></div>


### Ejemplo

#### El Diagrama de Casos de Uso
**Figura**
_Ejemplo de Relación de Dependencia Extend _
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
	actor Cliente	
	rectangle "Sistema" {
		(Realizar Compra) <.. (Aplicar Descuento) : <<extend>>
	}
	Cliente -- (Realizar Compra)
@enduml
```
_Nota:_ Una limitación del diagrama es que no indica en qué paso del flujo principal se extiende a `Aplicar Descuento`.

#### La Especificación del Caso de Uso (Base)

##### Opción 1
>[!example] Especificación del Caso de Uso
> #### Identificación
>- **Nombre:** Realizar Compra
>- **Actor(es):** Cliente
>- **Precondiciones:**
>- ...
>- 
>#### Escenario
>- ...
> 
>#### Flujo Principal (Normal)
>1. Paso 1
>2. Paso 2
>...
>j. Si se cumple <condición> entonces ver Caso de Uso **Aplicar Descuento**
>
>#### Flujos Alternativos
>- ...
>
>#### Excepciones
>- ...
>#### Poscondiciones
>- ...

##### Opción 2
>[!example] Especificación del Caso de Uso
> #### Identificación
>- **Nombre:** Realizar Compra
>- **Actor(es):** Cliente
>- **Precondiciones:**
>- ...
>- 
>#### Escenario
>- ...
> #### Puntos de Extensión
> PE1: Luego del Paso i, si se cumple la <condición>
> PE2: ...
> 
>#### Flujo Principal (Normal)
>1. Paso 1
>2. Paso 2
>...
>i. Paso i
>j. Si se cumple <condición> entonces ver Caso de Uso **Aplicar Descuento**
>...
>
>#### Flujos Alternativos
>- ...
>
>#### Excepciones
>- ...
>#### Poscondiciones
>- ...

**Ventaja**: La especificación textual precisa dónde y cómo se invoca el caso incluido.
