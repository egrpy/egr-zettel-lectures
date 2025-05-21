---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 15 Diagrama de Actividades/Zk Diagrama de Actividades (Introducción)/","tags":["digitalGarden"]}
---

## Diagrama de Actividades (Introducción)

El **diagrama de actividades** en UML es una herramienta de modelado que permite describir el comportamiento **dinámico** de un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 05 Sistemas, Subsistemas, Suprasistemas/Zk !MOC Sistemas, Subsistemas y Suprasistemas\|sistema]] (en el sentido amplio), enfocándose en la representación de **flujos de trabajo** y **procesos**, tanto de **sistemas de software** como de **organizaciones**. Estos diagramas muestran la **secuencia** y **condiciones** de las **actividades**, así como las **decisiones**, **bifurcaciones**, **concurrencia** y **sincronización** de tareas dentro de un proceso. Su notación gráfica es similar a los diagramas de flujo tradicionales, pero con capacidades extendidas para modelar actividades concurrentes y flujos de datos, lo que los hace especialmente útiles en el análisis y diseño de sistemas complejos ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]).

### Ejemplo Simple

**Figura**
_Ejemplo Genérico de un Diagrama de Actividades_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

start

:Actividad 1;
:Actividad 2;

if (condición) then (Sí)
  split
    :Actividad 3;
    :Actividad 4;
  split again
    :Actividad 5;
  split again
    :Actividad 6;
  end split

  :Actividad 7;
  :Actividad 8;

elseif (No)
  if (Otra Condición) then (Sí)
    :Actividad 9;
    :Actividad 10;
  else (No)
    stop
  endif
endif

:Actividad 11;
stop
@enduml
```

### Casos de Uso del Diagrama de Actividades

Los diagramas de actividades se utilizan fundamentalmente para ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]):

- Modelar **procesos** de negocio y flujos de trabajo organizacionales, representando cómo se desarrolla una tarea desde el inicio hasta su finalización.

- Especificar el **comportamiento** interno de un caso de uso, detallando los pasos que lo componen y las posibles ramificaciones de su ejecución.

- Describir la **lógica** de control de operaciones complejas, incluyendo decisiones, ciclos, concurrencia y sincronización de actividades.

- Representar la **interacción** entre diferentes roles, sistemas o componentes, especialmente cuando se requiere visualizar la responsabilidad de cada uno en el proceso.

- **Documentar** procedimientos operativos, algoritmos o procesos que involucren múltiples pasos y condiciones.

### Relación con Otros Diagramas

Los diagramas de actividades están estrechamente relacionados con otros diagramas de UML, como los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|diagramas de casos de uso]], los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Introducción)\|diagramas de interacción]] y los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Estados)\|diagramas de estado]]. A continuación, se describen algunas de las relaciones entre estos diagramas ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]):

| Diagrama     | Explicación                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Casos de Uso | Los diagramas de actividades se utilizan en conjunto con los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|diagramas de casos]] de uso para modelar los flujos de trabajo de los usuarios en un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 05 Sistemas, Subsistemas, Suprasistemas/Zk !MOC Sistemas, Subsistemas y Suprasistemas\|sistema]], proporcionan una visión más detallada de los procesos que se llevan a cabo dentro de un caso de uso.                                                                                                                                                                                                                                                                                                                                                              |
| Interacción  | Los diagramas de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Diagrama de Secuencia)\|secuencia]] y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Diagrama de Comunicación)\|comunicación]] se utilizan para modelar la interacción entre los objetos en un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 05 Sistemas, Subsistemas, Suprasistemas/Zk !MOC Sistemas, Subsistemas y Suprasistemas\|sistema]]. Los diagramas de actividades pueden utilizarse para modelar las actividades que se llevan a cabo dentro de los métodos de un objeto, o de todo un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|caso de uso]]. Por lo tanto, los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Introducción)\|diagramas de interacción]] y los diagramas de actividades pueden utilizarse juntos para proporcionar una visión completa de cómo funciona un sistema. |
| Estados      | Los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Estados)\|diagramas de estado]] se utilizan para modelar el comportamiento de un objeto en diferentes estados. Los diagramas de actividades pueden utilizarse para modelar las actividades que se llevan a cabo durante la transición entre estados en un diagrama de estado. Por lo tanto, los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Estados)\|diagramas de estado]] y los diagramas de actividades pueden utilizarse juntos para proporcionar una visión completa del comportamiento de un objeto en un sistema.                                                                                                                                                                   |

### Tipos de Diagramas de Actividades
Se distinguen dos tipos o configuración del diagrama de actividades ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]):

| Tipo                                                         | Explicación                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Diagrama de Actividades                                      | Representan el flujo de acciones y decisiones sin distinguir responsables. Son útiles para procesos lineales o de baja complejidad. Ver [[#Ejemplo Simple\|Ejemplo]].                                                                                                                                                                             |
| Diagrama de Actividades con Particiones (Calles o Swimlanes) | Dividen el diagrama en regiones, denominadas particiones o calles, que agrupan las actividades según el responsable (por ejemplo, un actor, un sistema o una unidad organizacional, etc.). Esta configuración facilita identificar claramente quién ejecuta cada paso del proceso. Ver [[#Ejemplo con Particiones (Calles o Swimlanes)\|Ejemplo]] |

_Nota_: En realidad no son tipos propiamente dicho, pero por su semántica los exponemos como tal. Las particiones realmente son un tipo de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 15 Diagrama de Actividades/Zk Diagrama de Actividades (Elementos)\|elemento]] del diagrama de actividades.

### Ejemplo con Particiones (Calles o Swimlanes)

**Figura**
__Ejemplo Genérico de un Diagrama de Actividades con Particiones__
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

|Partición 1|

start
  
:Actividad 1;

If (Condición) then (si)
	|Sistema|
	:Actividad 2;
	:Actividad 3;
	Stop
else (no)
	|Organización|

	:Actividad 4;
	:Actividad 5;
	
	if (Otra Condición) then (si)
		:Actividad 6;
	else (no)

	endif

endif

stop
@enduml
```

