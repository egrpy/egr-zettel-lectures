---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Captura de Requerimientos - Profundizando Conceptos/","tags":["digitalGarden"]}
---

## Captura de Requerimientos - Profundizando Conceptos

La **captura de requerimientos** (también denominada elicitación de requerimientos) constituye la actividad central de la ingeniería de requerimientos donde se descubren, extraen y articulan las necesidades, expectativas y restricciones de los stakeholders para un sistema de software. Esta actividad trasciende la simple recolección de información, involucrando procesos complejos de comunicación, negociación y traducción entre dominios de conocimiento heterogéneos (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]).

### Definición Multidimensional

[[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|Bruegge y Dutoit (2010)]] definen la elicitación como "el proceso de definir el sistema en términos del universo de discurso usando únicamente el vocabulario natural del dominio de aplicación" [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|(p. 123)]]. Esta definición subraya la **complejidad semántica** del proceso, donde el analista debe construir un puente lingüístico entre el mundo del usuario y el mundo técnico del desarrollo.

[[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]] amplía esta perspectiva al caracterizar la elicitación como "el proceso de trabajar con clientes y usuarios del sistema para descubrir el dominio de aplicación, qué servicios debe proporcionar el sistema y las restricciones operacionales del sistema" [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|(p. 85)]]. Esta caracterización enfatiza el aspecto **colaborativo** y **exploratorio** del proceso.

### Naturaleza Sociotécnica

La captura de requerimientos emerge como una actividad fundamentalmente [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Sistemas Sociotécnicos\|sociotécnica]] que involucra la intersección entre sistemas humanos y sistemas técnicos. Según la perspectiva sistémica, los requerimientos no existen como entidades preexistentes esperando ser descubiertas, sino que se **construyen socialmente** a través de procesos de interacción entre múltiples actores ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Principios Sistémicos Aplicados a la Ingeniería de Requerimientos\|Principios Sistémicos Aplicados a la Ingeniería de Requerimientos]]).

### El Problema de la Comunicación

[[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman (2013)]] identifica tres problemas fundamentales en la captura de requerimientos:

1. **Problema del alcance**: Los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 07 Administración de Proyectos/Zk Stakeholder\|stakeholders]] tienen dificultades para definir límites claros del sistema
2. **Problema del entendimiento**: Los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 07 Administración de Proyectos/Zk Stakeholder\|stakeholders]] no comprenden completamente sus propias necesidades
3. **Problema de la volatilidad**: Los requerimientos cambian durante el proceso de desarrollo

Estos problemas evidencian la **naturaleza emergente** del conocimiento sobre requerimientos y la necesidad de enfoques iterativos y adaptativos. Ver también [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 09 Gestión de Comunicación en Proyectos/Zk Comunicación en Proyectos - Fundamentos\|Comunicación en la Gestión de Proyectos]] y más específicamente [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 09 Gestión de Comunicación en Proyectos/Zk Comunicación en Proyectos - Comunicación e Ingeniería de Requerimientos\|Comunicación e Ingeniería de Requerimientos]].

### Contexto de la Captura de Requerimientos

#### Contexto Sistémico

Desde la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 02 Introducción a la Teoría General de Sistemas/Zk Enfoque de Sistemas\|Teoría General de Sistemas]], el contexto puede conceptualizarse como un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 06 Sistemas, Fundamentos, Propiedades, Principios Básicos/Zk Sistemas (Complejidad de los Sistemas)\|sistema complejo]] con [[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Propiedades Emergentes\|propiedades emergentes]]. Los requerimientos emergen de las interacciones entre los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 07 Elementos de un Sistema (Corriente de Entrada)/Zk Sistemas (Elementos)\|elementos del sistema]], no de los elementos individualmente considerados.

#### Contexto Organizacional

Constituye el espacio conceptual donde opera el sistema propuesto (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]):

- **Actores primarios**: Usuarios directos del sistema
- **Actores secundarios**: Sistemas externos o roles de apoyo
- **Procesos de negocio**: Actividades organizacionales que el sistema debe soportar
- **Restricciones del dominio**: Limitaciones impuestas por el contexto operacional

### Tipos de Requerimientos

#### Requerimientos Funcionales

Los requerimientos funcionales establecen lo que el sistema debe realizar, sin considerar la forma en que esto se implementa. Según el autor [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]], estos requerimientos engloban las prestaciones que debe brindar el sistema, su respuesta ante entradas determinadas y el comportamiento esperado en circunstancias específicas. Presentan las siguientes características:

- Especifican funcionalidades observables externamente
- Son independientes de la implementación tecnológica
- Deben ser verificables y trazables

#### Requerimientos No Funcionales

Los requerimientos no funcionales establecen restricciones y condiciones sobre la operación de los servicios o funciones del sistema, se describen como limitaciones que condicionan los servicios ofrecidos por el sistema [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|(Pressman, 2013)]].

Según [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]] pueden clasificarse en:

- **Requerimientos de producto**: Incluyen atributos como usabilidad, eficiencia y confiabilidad.
- **Requerimientos organizacionales**: Derivan de procesos internos, estándares y políticas vigentes.
- **Requerimientos externos**: Están relacionados con normas legales, principios éticos y necesidades de interoperabilidad.

Esta clasificación ayuda a identificar distintas fuentes y ámbitos de los requisitos no funcionales, facilitando su detección y gestión en el proceso de desarrollo.

#### Pseudorequerimientos

Los seudorrequerimientos (en inglés, pseudo-requirements), también llamados restricciones o requisitos impuestos, son requerimientos que no son funcionales ni no funcionales en el sentido clásico, sino condiciones o limitaciones impuestas por factores externos al sistema, como políticas organizacionales, normativas legales, tecnologías preestablecidas o decisiones estratégicas previas. Pueden referirse a cuestiones como el lenguaje de programación, plataforma tecnológica, uso obligatorio de ciertos estándares, cumplimiento de normativas regulatorias, protección de datos, entre otros (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]).

Los seudorrequerimientos / restricciones / requisitos impuestos: limitan la solución desde fuera del sistema, por ejemplo, “todo el software debe estar en Java”, o “el sistema deberá ejecutarse en AWS según política corporativa”. Estos últimos no suelen afectar directamente la percepción del usuario sobre el sistema (son invisibles desde el uso, aunque críticos para los equipos de desarrollo) (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]).

En la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 02 Introducción a la Teoría General de Sistemas/Zk Enfoque de la Teoría General de Sistemas\|Teoría General de Sistemas]] las restricciones son componentes estructurales  para definir la viabilidad y el alcance de un sistema [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Johansen Bertoglio, 2013) Introducción a la Teoría General de Sistemas\|(Johansen, 2013)]].

Reconocer y separar los pseudorequisitos es fundamental para una ingeniería de requisitos profesional, tanto desde la perspectiva metodológica clásica como sistémica.

### Actividades y Herramientas para Captura de Requerimientos

#### Identificación de Stakeholders

La identificación de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 07 Administración de Proyectos/Zk Stakeholder\|Stakeholders]] constituye la actividad fundacional, donde se propone el análisis de (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]):

- **Círculo interno**: Usuarios directos, desarrolladores
- **Círculo medio**: Gerentes, patrocinadores, mantenedores
- **Círculo externo**: Reguladores, competidores, sociedad

#### Técnicas de Captura de Requerimientos

##### Entrevistas Estructuradas y Semiestructuradas

Las entrevistas permiten exploración profunda de necesidades individuales, se  distinguen entre:

- **Entrevistas cerradas**: Con preguntas predefinidas para información específica
- **Entrevistas abiertas**: Exploratorias para descubrir necesidades latentes
- **Entrevistas semiestructuradas**: Híbridas que combinan estructura con flexibilidad

##### Observación Etnográfica

La observación directa revela prácticas implícitas y conocimiento tácito. [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]] destaca que la observación directa ayuda a entender aspectos detallados de los procesos que los participantes consideran obvios y que no mencionarían en una conversión, entrevista o encuesta [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|(p. 92)]].

##### Casos de Uso como Técnica de Captura de Requerimientos

Los casos de uso operan simultáneamente como técnica de captura de requerimientos y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso, Especificación)\|herramienta de especificación]]. El proceso de identificación de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso, Escenarios)\|escenarios]] facilita el descubrimiento de [[050 Base de Conocimientos/100 Temporales/Zk Temp Requerimientos Funcionales\|Zk Requerimientos Funcionales]] de manera sistemática ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al., 2006]]; Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]).

La captura de requerimientos se materializa típicamente a través de **modelos conceptuales**, siendo los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|diagramas de casos]] de uso una herramienta fundamental. Como señalan [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2007)]], "los casos de uso proporcionan una forma de comunicar los requisitos del sistema a todos los stakeholders usando un vocabulario común" [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|(p. 70)]].

La [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones\|relación]] entre [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|casos de uso]] refleja directamente el proceso de elicitación: los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] representan las fuentes de requerimientos ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 07 Administración de Proyectos/Zk Stakeholder\|stakeholders]]), mientras que los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|casos de uso]] capturan las **funcionalidades deseadas** desde la perspectiva del usuario.

### Relación con el Proceso de Desarrollo

La captura de requerimientos es parte esencial para todos los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Modelos de Proceso de Software\|modelos de procesos]] (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]).

#### Administración de Requerimientos

Los requerimientos capturados requieren **gestión continua** a través de:

- **Trazabilidad**: Conexión entre requerimientos y artefactos de desarrollo
- **Control de cambios**: Gestión formal de modificaciones
- **Validación**: Verificación de corrección y completitud

## Perspectiva de Ingeniería del Software

La captura de requerimientos constituye una disciplina técnica dentro de la ingeniería del software, requiriendo (Bruegge y Dutoit, [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2002) Ingeniería del Software Orientada a Objetos\|2002]], [[050 Base de Conocimientos/900 Biblioteca/Zk Lib (Bruegge y Dutoit, 2010) Object Oriented Software Engineering -  Using UML, patterns, and Java (3rd ed). Prentice Hall.\|2010]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011]]).:

- **Métodos sistemáticos** para la exploración de dominios complejos
- **Herramientas de modelado** para representar conocimiento
- **Procesos de validación** para asegurar corrección
    
### Desafíos Contemporáneos

#### Sistemas Distribuidos y Ágiles

Los enfoques ágiles plantean desafíos particulares para la captura tradicional de requerimientos. Beck et al. (2001) en el Manifiesto Ágil priorizan "individuos e interacciones sobre procesos y herramientas", sugiriendo enfoques más **colaborativos** y **emergentes**.

#### Sistemas Sociotécnicos Complejos

Los sistemas contemporáneos operan en entornos **sociotécnicos complejos** donde los requerimientos emergen de **redes de interacción** entre múltiples stakeholders con objetivos potencialmente conflictivos.
