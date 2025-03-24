---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk UML Diagrama de Actividades/","tags":["digitalGarden","modeloConceptualUML"]}
---

## Diagrama de Actividades

El diagrama de actividades es un tipo de diagrama dinámico que muestra el flujo de trabajo y las actividades que se realizan en un proceso. Se utiliza para modelar procesos empresariales y flujos de trabajo, ayudando a entender cómo se realizan las tareas dentro del sistema.

| Tipos                                                       | Objetivo                                                                                         |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|Dinámico]] | Describe procesos y flujos de trabajo, mostrando cómo se realizan las tareas dentro del sistema. |

----
### Visualización
#### Escenario Elemental
**Figura**
_Ejemplo de Diagrama de Actividades Simple
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho
skinparam conditionStyle InsideDiamond

Title Buscar Libro
start
:Buscar libro;
if (Libro disponible?) then (Sí)
  :Prestar libro;
else (No)
  :Notificar no disponible;
endif
stop
@enduml
```

#### Escenario Avanzado
**Figura**
_Ejemplo de Diagrama de Actividades más Complejo_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho
skinparam conditionStyle InsideDiamond

start
:Buscar libro;
if (Libro disponible?) then (Sí)
  :Verificar préstamos pendientes;
  if (Préstamos permitidos?) then (Sí)
    :Prestar libro;
    :Actualizar registro de préstamos;
  else (No)
    :Notificar límite de préstamos alcanzado;
  endif
else (No)
  :Notificar no disponible;
endif
stop
@endumlm
@enduml
```

**Figura**
_Ejemplo de Diagrama de Actividades por Calles (Swimlines)_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho
skinparam conditionStyle InsideDiamond

|#Strategy|Usuario|
start
:Buscar libro;
|#pink|Bibliotecario|
if (Libro disponible?) then (Sí)
	:Verificar préstamos pendientes;
	if (Préstamos permitidos?) then (Sí)
	    :Prestar libro;
	    :Actualizar registro de préstamos;
	    |Usuario|
	    :Recibir libro;
	  else (No)
		|Bibliotecario|
	    :Notificar límite de préstamos alcanzado;
	    |Usuario|
	    :Recibir notificación;
	  endif
else (No)
	|Bibliotecario|
	:Notificar no disponible;
	|Usuario|
	:Recibir notificación;
endif
|Bibliotecario|
stop
@enduml
```

**Figura**
_Ejemplo de Diagrama de Actividades con Flujos Paralelos_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho
skinparam conditionStyle InsideDiamond

start
:Verificar disponibilidad;
if (Disponible?) then (Sí)
  fork
    :Generar recibo;
    :Preparar entrega;
  fork again
    :Notificar al Usuario;
  end fork
  :Entregar Libro;
else (No)
  :Notificar no disponible;
endif
stop
@enduml

```


### Características Relevantes

| Elementos más Frecuentes                                                                       | Relaciones                       | Otros                                                                                                  |
| ---------------------------------------------------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------ |
| Actividades, nodos de decisión, nodos de inicio y fin, calles, divisiones y uniones de flujos. | Flujo de control de actividades. | Utilizado para modelar procesos como algoritmos, procedimientos empresariales, flujos de trabajo, etc. |
_Nota_: La lista de elementos y relaciones son los más frecuentemente utilizados.

----
### Ejemplos de Uso

| Aplicaciones                                              | Escenarios                                    |
| --------------------------------------------------------- | --------------------------------------------- |
| Modelado de procesos empresariales, diseño de algoritmos. | Desarrollo de software, gestión de proyectos. |
