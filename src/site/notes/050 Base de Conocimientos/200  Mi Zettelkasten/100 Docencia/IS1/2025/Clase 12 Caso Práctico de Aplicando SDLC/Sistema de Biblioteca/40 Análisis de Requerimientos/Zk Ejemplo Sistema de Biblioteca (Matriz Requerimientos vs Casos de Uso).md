---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Matriz Requerimientos vs Casos de Uso)/","tags":["digitalGarden","ejemplos","diagramaCasosDeUso"]}
---

## Matriz Requerimientos vs Casos de Uso

La matriz **Requerimientos vs Casos de Uso** es una herramienta para garantizar la trazabilidad entre los requerimientos del sistema y los casos de uso definidos durante el análisis. Su principal objetivo es asegurar que cada requerimiento esté debidamente cubierto por al menos un caso de uso, permitiendo así una verificación clara de su implementación dentro del diseño del sistema.

En esta matriz se cruzan los casos de uso identificados con los requerimientos del sistema, evidenciando la relación directa entre lo que el sistema debe hacer y cómo se espera que lo haga. Además, se incluyen dos elementos de diseño representados como **RD001** y **RD0022**, que aluden a decisiones técnicas o funcionalidades auxiliares vinculadas a más de un caso de uso.

Este tipo de matriz resulta especialmente útil en etapas posteriores del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 03 Costos y Complejidad del Software/Zk Ciclo de Vida del Desarrollo del Software\|Ciclo de Vida del Desarrollo del Software]], como la validación, la verificación, y la gestión del cambio, ya que permite responder de forma sistemática a preguntas como:

- ¿Está cada requerimiento cubierto por algún caso de uso?
- ¿Hay casos de uso que no aportan directamente al cumplimiento de requerimientos?
- ¿Qué impacto tendría modificar un requerimiento en los casos de uso existentes?

La claridad y estructuración que ofrece esta matriz favorecen una comunicación efectiva entre los distintos actores del proyecto (analistas, desarrolladores, testers y stakeholders), y promueven una mejor toma de decisiones en el proceso de construcción del sistema.
  
**Tabla**
_Matriz [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/30 Captura de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Lista de Requerimientos del Sistema)\|Requerimientos]] vs [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Análisis de Requerimientos del Sistema)\|Casos de Uso]]_

| Caso de Uso                                                                                                      | RF001 | RF002 | RF003 | RF004 | RF005 | RF006 | RF007 | RF008 | RNF001 | RNF002 | RNF003 | RNF004 | RD001 | RD002 |
| ---------------------------------------------------------------------------------------------------------------- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :----: | :----: | :----: | :----: | :---: | :---: |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Buscar Libros)\|Buscar Libro]]                |   X   |       |       |       |       |       |       |       |   X    |   X    |   X    |   X    |   X   |   X   |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Realizar Préstamo)\|Realizar Préstamo]]       |       |   X   |       |       |   X   |       |       |       |   X    |   X    |   X    |        |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Renovar Préstamo)\|Renovar Préstamo]]         |       |       |       |       |       |       |       |   X   |   X    |   X    |   X    |        |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Devolver Libro)\|Devolver Libro]]             |       |       |   X   |       |   X   |       |       |       |   X    |   X    |   X    |        |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Consultar Historial)\|Consultar Historial]]   |       |       |       |       |       |   X   |       |       |   X    |   X    |   X    |   X    |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Administrar Catálogo)\|Administrar Catálogo]] |       |       |       |   X   |       |       |       |       |   X    |   X    |   X    |   X    |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Gestionar Usuario)\|Gestionar Usuario]]       |       |       |       |       |       |       |   X   |       |   X    |   X    |   X    |   X    |   X   |       |
| [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Caso Práctico de Aplicando SDLC/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Generar Recibo)\|Generar Recibos]]            |       |       |       |       |   X   |       |       |       |   X    |   X    |   X    |        |   X   |       |

_Notas:_
- **RNF001 (Interfaz intuitiva):** Aplica a todos los casos de uso.
- **RNF003 (MySQL):** Todos los CU que interactúan con la base de datos.
- **RD002 (Tiempo ≤3s):** Aplica específicamente a "Buscar Libros".