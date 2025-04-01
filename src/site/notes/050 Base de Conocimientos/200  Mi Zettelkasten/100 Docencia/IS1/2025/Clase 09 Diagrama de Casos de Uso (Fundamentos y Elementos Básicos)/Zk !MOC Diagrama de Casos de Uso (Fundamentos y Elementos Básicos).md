---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk !MOC Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/","tags":["digitalGarden","moc","UML","casosDeUso"]}
---


## MOC Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)

### Introducción

En el análisis del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 06 Introducción al UML/Zk Modelo Conceptual del UML\|Modelo Conceptual del UML]], exploramos las características generales del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|Diagrama de Casos de Uso]]. En esta clase, profundizaremos en su estudio para que, al finalizar las sesiones previstas, puedan interpretar y elaborar diagramas de casos de uso con una aplicación precisa de su semántica y sintaxis.

El objetivo principal es que adquieran las herramientas necesarias para modelar interacciones entre actores y sistemas, capturando los requisitos funcionales y definiendo el alcance del sistema.

#### Ejercicio

>[!Todo] [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Ejercicio de Clase 01.1\|Desarrollar el ejercicio 1.1]]

----
### Desarrollo

#### Visualización Preliminar

Para comenzar, utilizaremos una [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Un Mapa de Aventuras\|historia conceptual]] que nos permitirá visualizar qué es un diagrama de casos de uso. Esta analogía facilita la comprensión inicial al relacionar los elementos del diagrama con un "mapa de aventuras".

#### El Diagrama

Según la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Diagrama UML - Definición\|definición de diagrama]] y el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 06 Introducción al UML/Zk Modelo Conceptual del UML\|Modelo Conceptual del UML]], la construcción de diagramas se basa en [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Tipos de Elementos)\|elementos]] y las [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Relaciones)\|relaciones]] entre ellos.

Para entender completamente el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|Diagrama de Casos de Uso]], analizaremos por separado los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Tipos de Elementos)\|elementos]]  y las [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Relaciones)\|relaciones]] que lo componen. Sin embargo, dado que los elementos y las relaciones están intrínsecamente conectados, en algunos casos será necesario abordar las relaciones al presentar los elementos, con el fin de contextualizar su uso y dar sentido a cada componente en su entorno funcional.

Este enfoque permite comprender cómo los actores, casos de uso y el sistema sujeto de estudio se integran y colaboran para modelar interacciones significativas, manteniendo la coherencia entre los conceptos fundamentales del UML.

##### [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos\|Elementos]]

- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|Actores]]: Representan a las entidades externas que interactúan con el sistema.
	- Ejemplo: [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk UML - Actores - Roles - Equipo de Fútbol\|Actores y Roles en un Equipo de Fútbol]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Sujeto)\|Sujeto (Sistema)]]: El sistema o subsistema sujeto del análisis.
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|Caso de Uso]]: Las funcionalidades específicas ofrecidas por el sujeto.
	- Ejemplo: [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk UML - Actores - Roles - Casos de Uso - Equipo de Fútbol\|Roles, Actores y Casos de Uso en un Equipo de Fútbol]]

>[!Todo] [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Ejercicio de Clase 01.2\|Desarrollar el ejercicio 1.2]]

##### [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Relaciones\|Relaciones]]
Conexiones entre actores y casos de uso, así como entre los propios casos.


----
### Conclusión

----
## Referencias
[[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|(OMG, 2017)]]
OMG. (2017, diciembre). _About the Unified Modeling Language Specification Version 2.5.1_. [https://www.omg.org/spec/UML](https://www.omg.org/spec/UML) 

[[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]]
Booch, G., Rumbaugh, J., y Jacobson, I. (2006). _El lenguaje Unificado de Modelado: Guía del Usuario_ (J. J. García Molina & J. Sáez Martínez, Trads.). Addison-Wesley.

[[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al.,2000)]]
Rumbaugh, J., Booch, G., y Jacobson, I. (2000). _El lenguaje unificado de modelado: Manual de referencia_.

Blankenhorn, K., y Jeckle, M. (2004). A UML Profile for GUI Layout. En M. Weske y P. Liggesmeyer (Eds.), _Object-Oriented and Internet-Based Technologies_ (Vol. 3263, pp. 110-121). Springer Berlin Heidelberg. [https://doi.org/10.1007/978-3-540-30196-7_9](https://doi.org/10.1007/978-3-540-30196-7_9)

Cabot, Sagrera, Jordi. Ingeniería del software, Editorial UOC, 2013. ProQuest Ebook Central, [](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3219169).

Campderrich, Falgueras, Benet. Ingeniería del software, Editorial UOC, 2003. ProQuest Ebook 
Central, [](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3206903).

Casas, Roma, Jordi, and i Caralt,Jordi Conesa. Diseño conceptual de bases de datos en UML, Editorial UOC, 2014. ProQuest Ebook Central, [](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3222912).
