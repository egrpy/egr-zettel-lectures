---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk !MOC Diagramas de Estados/","tags":["digitalGarden","moc","UML","diagramaDeClases"]}
---

## MOC Diagramas de Estados

En la clase, se estudiará cómo utilizar el diagrama de estados en UML para modelar el comportamiento dinámico de un sistema de software, centrándose en los diferentes estados que puede asumir un objeto a lo largo de su vida y en los eventos que provocan transiciones entre ellos. Se abordarán conceptos como estados, transiciones, eventos y acciones internas.

De este modo, se preparará al estudiante para emplear el diagrama de estados en el diseño de sistemas que respondan adecuadamente a estímulos internos y externos, asegurando un comportamiento controlado, predecible y coherente a lo largo del ciclo de vida del software.

### Introducción
A modo de introducción analizaremos el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Introducción, Ejemplo,  Estado Civil de las Personas de Paraguay)\|Estado Civil de las Personas de Paraguay]], de manera a comprender la esencia por detrás de este diagrama.

### Desarrollo
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)\|Diagrama de Estados (Elementos y Relaciones)]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados y el SDLS\|Diagrama de Estados y el SDLS]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Relación con Otros Diagramas)\|Diagrama de Estados (Relación con Otros Diagramas)]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Ejercicios y Ejemplos)\|Ejemplos]]

----
### Referencias y Citaciones

OMG. (2017, diciembre). _About the Unified Modeling Language Specification Version 2.5.1_. [https://www.omg.org/spec/UML](https://www.omg.org/spec/UML) 
Citación Parentética: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|(OMG, 2017)]]
Citación Parentética Múltiple: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]
Citación Narrativa: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG (2017)]]

Booch, G., Rumbaugh, J., y Jacobson, I. (2006). _El lenguaje Unificado de Modelado: Guía del Usuario_ (J. J. García Molina & J. Sáez Martínez, Trads.). Addison-Wesley.
Citación Parentética: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]]
Citación Parentética Múltiple: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]
Citación Narrativa: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al. (2006)]]

Rumbaugh, J., Booch, G., y Jacobson, I. (2000). _El lenguaje unificado de modelado: Manual de referencia_.
Citación Parentética: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al.,2000)]]
Citación Parentética Múltiple: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al.,2000]]
Citación Narrativa: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000)]]

Pressman, R. S. (2013). _Ingeniería del Software: Un Enfoque Práctico_ (Séptima edición). McGraw-Hill Education.
Citación Parentética: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|(Pressman, 2013)]]
Citación Parentética: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]
Citación NArrativa: [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman (2013)]]


## Bibliografía Adicional
Blankenhorn, K., y Jeckle, M. (2004). A UML Profile for GUI Layout. En M. Weske y P. Liggesmeyer (Eds.), _Object-Oriented and Internet-Based Technologies_ (Vol. 3263, pp. 110-121). Springer Berlin Heidelberg. [https://doi.org/10.1007/978-3-540-30196-7_9](https://doi.org/10.1007/978-3-540-30196-7_9)

Cabot, Sagrera, Jordi. Ingeniería del software, Editorial UOC, 2013. ProQuest Ebook Central, [(https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3219169)](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3219169).

Campderrich, Falgueras, Benet. Ingeniería del software, Editorial UOC, 2003. ProQuest Ebook 
Central, [https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3206903](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3206903).

Casas, Roma, Jordi, and i Caralt,Jordi Conesa. Diseño conceptual de bases de datos en UML, Editorial UOC, 2014. ProQuest Ebook Central, [https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3222912](https://ebookcentral.proquest.com/lib/biblioucsp/detail.action?docID=3222912).