---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Introducción)/","tags":["digitalGarden"]}
---

## Diagramas de Interacción (Introducción)

Los **diagramas de interacción** en UML son una familia de diagramas de **comportamiento** destinados a modelar cómo los **objetos** de un sistema **colaboran** a través del **intercambio de mensajes** para lograr un objetivo común. Estos diagramas permiten visualizar la dinámica de las interacciones, mostrando tanto la secuencia como la estructura de los intercambios entre los participantes del sistema ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]).

### Usos de los Diagramas de Interacción

Los diagramas de interacción se utilizan fundamentalmente para [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]]:

- Analizar y documentar el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagramas UML 2.5.1 (Dinámicos)\|comportamiento dinámico]] de un sistema.
- Comprender y comunicar cómo los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Objetos)\|objetos]] cooperan para ejecutar [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk UML Casos de Uso - Definición\|procesos o casos de uso]].
- Identificar posibles problemas de comunicación, cuellos de botella y optimizar la arquitectura de software.
- Facilitar el diseño, la validación y la mejora de sistemas complejos, especialmente en etapas de análisis y diseño orientado a objetos.

### Tipos de diagramas de interacción en UML

Según la [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|Especificación del UML del OMG (2017)]] los diagramas más utilizados para modelar interacción de objetos son:

| Diagrama                                                                             | Descripción breve                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Diagrama de Secuencia)\|Diagrama de Secuencia]]       | Se centra en la **dimensión** **temporal** de las interacciones.<br><br>Muestra cómo los objetos se comunican a través de mensajes en un **orden cronológico**, permitiendo analizar el flujo de eventos y la secuencia exacta en que ocurren ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2027]]).                                                                                                               |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Diagrama de Comunicación)\|Diagrama de Comunicación]] | Enfatiza la **estructura y las relaciones** entre los objetos participantes.<br><br>Representa cómo los objetos están **conectados** y cómo se envían mensajes entre ellos, priorizando la organización espacial y las conexiones sobre el orden temporal ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]).<br><br> En versiones anteriores del UML este diagrama era conocido como Diagrama de Colaboración. |

>[!Nota] Nota
>En versiones anteriores del UML, este diagrama era conocido como **Diagrama de Colaboración**. El nombre cambió a **Diagrama de Comunicación** en UML 2.0 para enfatizar su enfoque en la estructura de las interacciones entre los participantes.
{ #3d4f56}


### Diagramas de Interacción y el SDLC

Ver [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 14 Diagramas de Interacción/Zk Diagramas de Interacción (Diagramas de Interacción y el SDLS)\|Diagramas de Interacción y el SDLS]].
