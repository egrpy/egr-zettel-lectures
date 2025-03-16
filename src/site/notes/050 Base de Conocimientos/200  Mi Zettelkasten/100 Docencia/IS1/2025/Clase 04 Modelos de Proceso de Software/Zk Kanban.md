---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Kanban/","tags":["digitalGarden","kanban"]}
---

## Kanban

### Definición
Kanban es un sistema visual para gestionar el flujo de trabajo, enfocado en la entrega continua y la mejora continua del proceso. No establece roles fijos ni ceremonias o procesos obligatorios, lo que lo hace flexible y adaptable a diferentes contextos.
 
### Principios

**Visualización del Trabajo**
Se utiliza un **tablero Kanban** para la visualización de las tareas. Este tablero es una herramienta efectiva para visualizar todas las tareas de un proyecto. Cada tablero típicamente incluye columnas como "Pendiente", "En curso" y "Terminado", donde las tareas se representan como tarjetas con información asociada, como el título de la tarea y la fecha de entrega

**Limitación del Trabajo en Progreso (WIP)**
Los límites del trabajo en proceso (WIP) son cruciales para evitar sobrecargas y mantener un ritmo de trabajo óptimo. Estos límites restringen la cantidad máxima de tareas que un equipo puede trabajar simultáneamente, lo que ayuda a evitar cuellos de botella y a mantener un flujo continuo de trabajo. La implementación de los límites WIP permite a los equipos enfocarse en las tareas actuales y terminarlas más rápido, además de detectar y resolver bloqueos en el proceso de trabajo.

**Mantenimiento del Flujo Continuo**
Se busca mantener un flujo continuo de trabajo sin interrupciones.
La fabricación de flujo continuo (FFC) es una metodología que busca mantener un movimiento constante e ininterrumpido de materiales a través de la línea de producción. Este enfoque se basa en la filosofía de la fabricación esbelta y el Sistema de Producción de Toyota, y se caracteriza por minimizar paradas, cuellos de botella y desperdicio dentro del proceso de fabricación. En el contexto de los tableros Kanban, el objetivo es mantener un flujo continuo de trabajo sin interrupciones, asegurando que las tareas avancen sin obstáculos significativos.


**Mejora Continua**
Se fomenta la **reflexión periódica** para mejorar el proceso. Es un proceso continuo de realización de mejoras incrementales en procesos, productos o servicios para lograr una mayor eficiencia, calidad y rendimiento general. Para fomentar la mejora continua, es importante centrarse en los procesos subyacentes y no solo en los resultados. Esto permite identificar ineficiencias y áreas de mejora, y optimizar los procesos para obtener mejores resultados de forma natural. La reflexión periódica y la adaptación constante son fundamentales para mantener un flujo de trabajo eficiente y mejorar continuamente

### Ventajas

**Flexibilidad**
No requiere roles fijos ni ceremonias obligatorias. En su lugar, se enfocan en la adaptabilidad y la flexibilidad para ajustar los planes según sea necesario. Esto permite que los equipos puedan responder rápidamente a cambios inesperados y mantenerse alineados con los requisitos cambiantes del proyecto.

**Mejora Continua**
Promueve la reflexión constante para identificar oportunidades de mejora y desarrollar estrategias para mejorar el proceso. Esto se logra mediante la participación activa de los miembros del equipo, quienes son los más indicados para identificar oportunidades de mejora debido a su conocimiento profundo de los productos, servicios y procesos

**Priorización**
Permite a los equipos priorizar tareas según su importancia y urgencia, asegurando que los esfuerzos se orienten hacia aquellas actividades que proporcionen el mayor valor al cliente y al proyecto. La priorización ayuda a los equipos a centrarse en las tareas más valiosas y cruciales, evitando el desperdicio de tiempo y recursos en actividades menos relevantes

### Desventajas

**Cuellos de Botella y Producción Insuficiente**
Puede generar cuellos de botella y producción insuficiente ante cambios repentinos en la demanda.

**Confusión por Exceso de Etiquetas**
El uso excesivo de etiquetas puede causar desorganización.

**Rigidez del Sistema**
Puede ser rígido en ciertos contextos, dificultando la adaptación a cambios rápidos.

**Limitaciones en Proyectos Complejos**
No es adecuado para proyectos complejos que requieren planificación detallada.

**Dificultades en la Colaboración del Equipo**
Puede haber desafíos en la colaboración si no hay estructura clara.

**Sobrecarga de Información**
Los tableros pueden sobrecargar de información, dificultando la priorización.

**Dificultad para Predecir el Progreso a Largo Plazo**
No es ideal para rastrear el progreso a largo plazo.

**Dependencia de la Disciplina del Equipo**
Su efectividad depende de la autodisciplina del equipo.

**No Adecuado para Todos los Proyectos**
No es la mejor opción para proyectos que requieren cambios constantes o estructura rígida.

[Wikipedia: Kanban (development)](https://en.wikipedia.org/wiki/Kanban_\(development\))
[(Project Managers, 2023)](https://projectmanagers.net/kanban-boards-top-10-cons-disadvantages-limitations/)

### Esquema Gráfico
**Figura**
_Esquema Gráfico Kanban_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
'left to right direction
skinparam linetype ortho

class Kanban {
}

package "Tablero" as TableroKanban {
	class Pendiente
	class "En Curso"
	class Terminado
	  
	Pendiente -r-> "En Curso"
	"En Curso" -r-> Terminado
	
	object "Tarea 1"
	object "Tarea 2"
	object "Tarea i"
	object "Tarea n"

	Pendiente --> "Tarea 1"
	Pendiente --> "Tarea 2"
	"En Curso" --> "Tarea i"
	Terminado --> "Tarea n"
}

package Principios {
	note as N1
		- Visualización del Trabajo
		- Limitación del Trabajo en Progreso (WIP)
		- Mantenimiento del Flujo Continuo
		- Mejora Continua
	end note
}

package Ventajas {
	note as N2
		- Flexibilidad
		- Mejora Continua
		- Priorización
	end note
}

package Desventajas {
	note as N3
		- Cuellos de Botella y Producción Insuficiente
		- Confusión por Exceso de Etiquetas
		- Rigidez del Sistema
		- Limitaciones en Proyectos Complejos
		- Dificultades en la Colaboración del Equipo
		- Sobrecarga de Información
		- Dificultad para Predecir el Progreso a Largo Plazo
		- Dependencia de la Disciplina del Equipo
		- No Adecuado para Todos los Proyectos
	end note
}

Kanban -u- Principios
Kanban -d- TableroKanban
Kanban -r- Ventajas
Kanban -l- Desventajas
 @enduml
```
Fuente: Elaboración propia.