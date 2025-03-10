---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelo Incremental/","tags":["digitalGarden","modeloDeProceso"]}
---

## Modelo Incremental

### Definición

Es un enfoque de desarrollo de software basado en la entrega de pequeños incrementos funcionales. Cada incremento pasa por un ciclo de desarrollo, prueba y entrega, permitiendo mejorar el sistema de manera progresiva. En cada iteración se agregan nuevas funcionalidades sin afectar lo ya construido [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|(Pressman, 2013]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville, 2011)]]. Fue propuesto por Harlan Mills en el año 1980.

----
### Fases Principales
Según [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Pfleeger (2006)]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]] se distinguen las siguiente fases para este modelo:

#### Análisis de Requerimientos
- Identificación de las funcionalidades a desarrollar en cada incremento
   
#### Diseño Inicial
- Definición de la arquitectura del sistema para soportar el desarrollo incremental.

#### Implementación del Primer Incremento
- Desarrollo de una versión básica funcional del software.

#### Pruebas y Validación
- Evaluación del incremento desarrollado para asegurar su calidad.

#### Entrega y Retroalimentación
- Liberación del incremento al usuario y recopilación de comentarios.

#### Iteración
- Repetición del proceso para agregar nuevos incrementos hasta completar el sistema.

#### Mantenimiento
- Corrección de errores, actualización del software y adaptación a nuevos requerimientos.

----
### Ventajas
Según [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Pfleeger (2006)]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]]:
- Alta adaptabilidad: Permite incorporar cambios y ajustar requisitos durante el desarrollo.
- Mejor comprensión de requerimientos: La interacción con el usuario ayuda a identificar necesidades reales del sistema.
- Gestión efectiva de riesgos: Especialmente en el Modelo en Espiral, donde se evalúan y mitigan riesgos en cada iteración.

----
### Desventajas
Según [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|Pressman (2013)]z] y [[Zk Lit (Sommerville, 2011) Ingeniería del Software]]:
- Complejidad en la gestión de versiones: Requiere una administración adecuada para evitar conflictos entre múltiples versiones en desarrollo.
- Dependencia de un buen diseño inicial: Si la arquitectura no está bien definida desde el principio, pueden surgir problemas de escalabilidad y mantenimiento.
- Mayor necesidad de coordinación: Al haber entregas frecuentes, se requiere una comunicación constante con los interesados del proyecto.

----
### Aplicaciones
Según [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pfleeger, 2006) Software Engineering Theory and Practice\|Pfleeger (2006)]] y [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Sommerville, 2011) Ingeniería del Software\|Sommerville (2011)]]:
- Desarrollo de producto mínimo viable (MVP): Ideal para probar conceptos y recibir retroalimentación rápida del mercado.
- Proyectos en la industria aeroespacial: La necesidad de control estricto y la mitigación de riesgos hacen que el modelo en espiral sea una elección adecuada.
- Software con requisitos poco definidos: Cuando no se pueden establecer especificaciones detalladas desde el inicio, el modelo evolutivo permite ajustarlas progresivamente.

----
### Conclusión
Ofrece una metodología flexible y centrada en la retroalimentación continua, lo que lo hace ideal para entornos donde los requisitos pueden cambiar frecuentemente. Sin embargo, su implementación requiere una comunicación efectiva con los usuarios y una planificación adecuada para evitar sobrecostos y complejidades innecesarias. El uso de prototipos y el enfoque en la mitigación de riesgos lo convierten en una opción viable para proyectos donde la incertidumbre y la evolución constante son factores clave.