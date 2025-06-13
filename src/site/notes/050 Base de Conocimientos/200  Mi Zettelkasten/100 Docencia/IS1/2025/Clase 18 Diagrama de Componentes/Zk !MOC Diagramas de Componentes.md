---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 18 Diagrama de Componentes/Zk !MOC Diagramas de Componentes/","tags":["digitalGarden","moc","UML","diagramaDeComponentes"]}
---

## MOC Diagramas de Componentes

El objetivo de esta clase es profundizar sobre el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Componentes)\|diagrama de componentes]] del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 06 Introducción al UML/Zk Modelo Conceptual del UML\|Zk Modelo Conceptual del UML]], de manera que el estudiante comprenda su propósito y la utilidad como herramienta para modelar la arquitectura física y lógica de sistemas software, identificando módulos reutilizables, interfaces y dependencias. Se busca que el alumno sea capaz de reconocer cuándo y cómo emplear diagramas de componentes para documentar, analizar y comunicar la estructura de implementación de sistemas complejos, facilitando la integración y el mantenimiento en proyectos de ingeniería de software.

### Introducción
A modo de introducción, se analizará la [[Zk Diagrama de Componentes (Analogía del Ensamblaje Modular)\|Analogía del Ensamblaje Modular]], donde los componentes se asemejan a piezas intercambiables en un sistema físico, conectadas mediante interfaces bien definidas, para ilustrar la importancia de la modularidad y la separación de responsabilidades.

### Desarrollo
- [[Zk Diagrama de Componentes (Definición y Objetivo)\|Definición y Objetivos]]. Breve introducción sobre qué es un diagrama de componentes UML, su función principal en la visualización de la estructura física del software (componentes, artefactos, interfaces) y su papel en la documentación de la arquitectura de implementación[[](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_35495c5e-566e-4c50-a40e-f6d91e60822d/ed559439-bdb9-4e0a-87f5-d5417c54b71b/uug.pdf)].
    
- [[Zk Diagrama de Componentes (Elementos y Notación)\|Elementos y Notación]]. Descripción de los elementos principales:
    
    - **Componente**: módulo físico o lógico del sistema (bibliotecas, ejecutables, servicios, etc.), representado por un rectángulo con una pestaña.
        
    - **Interfaz**: contratos explícitos que definen los servicios ofrecidos o requeridos por un componente.
        
    - **Relaciones**: dependencias, ensamblajes y conexiones entre componentes e interfaces[[](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_35495c5e-566e-4c50-a40e-f6d91e60822d/ed559439-bdb9-4e0a-87f5-d5417c54b71b/uug.pdf)].
        
- [[Zk Diagrama de Componentes (Principios de Modularidad y Acoplamiento)\|Principios de Modularidad y Acoplamiento]]. Explicación de los principios de bajo acoplamiento y alta cohesión en el diseño de componentes, y cómo estos principios favorecen la mantenibilidad, la escalabilidad y la reutilización del software[[](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_35495c5e-566e-4c50-a40e-f6d91e60822d/ed559439-bdb9-4e0a-87f5-d5417c54b71b/uug.pdf)].
    
- [[Zk Diagrama de Componentes (Integración con Otros Diagramas UML)\|Integración con Otros Diagramas UML]]. Relación con diagramas de despliegue (para mostrar la distribución física), diagramas de clases (para detallar la implementación interna de los componentes) y diagramas de paquetes (para la organización lógica de los módulos)[[](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_35495c5e-566e-4c50-a40e-f6d91e60822d/b7cd29a8-e8d4-4909-a83d-7c922678172c/Prentice-Object-Oriented-Software-Engineering-Using-UML-Patterns-and-Java-3rd-2012.pdf)][[](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/collection_35495c5e-566e-4c50-a40e-f6d91e60822d/ed559439-bdb9-4e0a-87f5-d5417c54b71b/uug.pdf)].
    
- Ejemplos:
    
    - [[Zk Diagrama de Componentes (Ejemplo - Sistema de Gestión de Pedidos)\|Sistema de Gestión de Pedidos]]: identificación de componentes principales (UI, lógica de negocio, acceso a datos) y sus interfaces.
        
    - [[Zk Diagrama de Componentes (Ejemplo - Aplicación Web Multicapa)\|Aplicación Web Multicapa]]: representación de componentes como servicios, controladores, repositorios, etc.
- Ejemplos:
	- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 17 Diagrama de Paquetes/Zk Diagrama de Paquetes (Ejemplo - Diagrama de Alto Nivel)\|Diagrama de Alto Nivel]]
	- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 17 Diagrama de Paquetes/Zk Diagrama de Paquetes (Ejemplo - Diagrama de Detallado para Análisis de Dependencias)\|Diagrama de Detallado para Análisis de Dependencias]]


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