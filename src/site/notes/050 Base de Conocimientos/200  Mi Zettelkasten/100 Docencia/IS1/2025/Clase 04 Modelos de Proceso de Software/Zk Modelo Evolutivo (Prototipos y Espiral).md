---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Modelo Evolutivo (Prototipos y Espiral)/","tags":["digitalGarden","modeloDeProceso"]}
---

## Modelo Evolutivo (Prototipos y Espiral)

### Definición

Es un enfoque de desarrollo de software evolutivo basado en la creación de prototipos y la mejora progresiva del sistema. Se centra en la adaptabilidad y la gestión de riesgos, permitiendo ajustar los requerimientos a medida que se avanza en el desarrollo. Dentro de este enfoque, el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Modelo de Prototipos\|Modelo de Prototipos]] permite construir versiones preliminares del software para evaluar y refinar requisitos, mientras que el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Modelo en Espiral\|Modelo en Espiral]], propuesto por Barry Boehm en 1986, introduce una estructura iterativa con un fuerte enfoque en la evaluación de riesgos ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman, 2013]]).

----
### Fases Principales
Conforme a [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman (2013]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]], las principales fases con las siguientes:

**Identificación de Requerimientos**
Se determinan las necesidades iniciales del sistema basándose en la retroalimentación del usuario.
   
**Diseño Inicial del Prototipo**
Creación de un modelo preliminar que represente aspectos clave del sistema.

**Evaluación del Prototipo**
Se presenta el prototipo a los usuarios para obtener retroalimentación y refinar los requisitos.

**Desarrollo Iterativo**
Se ajusta y mejora el prototipo en ciclos sucesivos hasta alcanzar la versión final.

**Pruebas y Validación**
Evaluación del software desarrollado para garantizar su funcionalidad y calidad.

**Implementación y Entrega**
Se pone en producción el sistema final, asegurando que cumpla con los requisitos establecidos.

**Mantenimiento y Evolución**
Se realizan mejoras y correcciones en respuesta a cambios en el entorno y nuevas necesidades del usuario.

**Iteración**
Repetición del proceso para agregar nuevos incrementos hasta completar el sistema.

**Mantenimiento**
- Corrección de errores, actualización del software y adaptación a nuevos requerimientos.

----
### Ventajas
De acuerdo a [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Pfleeger (2006)]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]] se destacan las siguientes:

- Retroalimentación temprana: Los usuarios pueden evaluar y sugerir mejoras desde las primeras versiones del software.
- Mayor flexibilidad: Permite realizar cambios en los requisitos durante el desarrollo.
- Entrega rápida de software funcional: Se puede poner en producción una versión operativa del sistema antes de completar todo el desarrollo.
 
----
### Desventajas
En cuanto a los inconvenientes, [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman (2013]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]], indican:

- Complejidad en la gestión de versiones: Requiere una administración adecuada para evitar conflictos entre múltiples versiones en desarrollo.
- Dependencia de un buen diseño inicial: Si la arquitectura no está bien definida desde el principio, pueden surgir problemas de escalabilidad y mantenimiento.
- Mayor necesidad de coordinación: Al haber entregas frecuentes, se requiere una comunicación constante con los interesados del proyecto.

----
### Aplicaciones
Para [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Pfleeger (2006)]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]], algunas aplicaciones de este modelo:

- Proyectos con entregas continuas: Ideal para desarrollos donde se requiere la liberación frecuente de nuevas funcionalidades.
- Aplicaciones web y servicios en la nube: Modelos de negocio basados en SaaS (Software as a Service) suelen beneficiarse de este enfoque.
- Sistemas con requisitos evolutivos: Cuando no se pueden definir completamente los requerimientos desde el inicio, el modelo incremental permite ajustarlos en el tiempo.

----
### Conclusión
Es un enfoque efectivo cuando se requiere flexibilidad y entrega continua de valor al usuario. Su enfoque iterativo permite minimizar riesgos y adaptarse a cambios en los requisitos. Sin embargo, requiere una buena planificación y gestión para evitar problemas de integración y control de versiones. Es particularmente útil en proyectos de software moderno, como aplicaciones web y servicios en la nube, donde la evolución constante es un factor clave de éxito. Además, la fase de mantenimiento garantiza la continuidad y adaptabilidad del software a largo plazo.
