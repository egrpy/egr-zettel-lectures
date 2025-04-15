---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk Herramienta CASE (Computer Aided Software Engineering)/","tags":["digitalGarden","herramientaCase"]}
---

## Herramienta CASE (Computer Aided Software Engineering)

Las herramientas CASE (Computer-Aided Software Engineering) son aplicaciones informáticas diseñadas para asistir en las diversas fases del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 03 Costos y Complejidad del Software/Zk Ciclo de Vida del Desarrollo del Software\|Ciclo de Vida del Desarrollo de Software (SDLC)]], desde la planificación hasta el mantenimiento. Estas herramientas automatizan tareas como el modelado, generación de código, pruebas y documentación, mejorando la eficiencia y calidad del software desarrollado ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Case, 1985) Computer-aided software engineering (CASE) - Technology for improving software development productivity.\|Case, 1985]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Chen et al., 1989) Computer-aided software engineering - Present status and future directions\|Chen et al., 1989]]).

### Usos

Las herramientas CASE se emplean para​ ([Bhuyan, 2023)](https://faun.pub/comprehensive-overview-of-case-tools-streamlining-software-development-e367b156cb18); [Cabot, 2024](https://modeling-languages.com/text-uml-tools-complete-list/); [(Chervany y Lending, 1998)](https://dl.acm.org/doi/pdf/10.1145/292349.292353#:~:text=In%20a%20follow%2Dup%20survey,measurable%20returns%2C%20and%20unrealistic%20expectations.); [Jones, 2002](https://www.umsl.edu/~sauterv/analysis/488_f02_papers/CASE.html)):

- Modelar sistemas mediante diagramas UML y otros lenguajes de modelado.
- Generar código fuente a partir de modelos.
- Gestionar requisitos y trazabilidad.
- Realizar pruebas y validaciones automáticas.
- Mantener la documentación actualizada del sistema.

### Beneficios

Entre los beneficios de utilizar herramientas CASE se incluyen ([Burkhard y Jenster, 1989](https://dl.acm.org/doi/10.1145/86227.86238); 
[(Chervany y Lending, 1998a)](http://portal.acm.org/citation.cfm?doid=279179.279187.)).

- **Reducción de tiempo y costos**: al automatizar tareas repetitivas y propensas a errores .
- **Mejora en la calidad del software**: mediante la estandarización de procesos y documentación .
- **Facilitación de la colaboración**: al proporcionar un entorno común para desarrolladores, analistas y otros stakeholders.​

----
### Ejemplo de Herramientas CASE de Pago

| Nombre               | Fabricante      | Diagramas UML Soportados | Etapas del SDLC Soportadas         | Curva de Aprendizaje | Tipo de Licencia |
| -------------------- | --------------- | :----------------------: | ---------------------------------- | :------------------: | :--------------: |
| PowerDesigner        | SAP             |          Todos           | Análisis, Diseño, Implementación   |         Alta         |    Comercial     |
| Enterprise Architect | Sparx Systems   |          Todos           | Requisitos, Diseño, Implementación |        Media         |    Comercial     |
| Visual Paradigm      | Visual Paradigm |          Todos           | Requisitos, Diseño, Implementación |        Media         |    Comercial     |
| IBM Rational Rose    | IBM             |          Todos           | Análisis, Diseño, Implementación   |         Alta         |    Comercial     |
| MagicDraw            | No Magic        |          Todos           | Requisitos, Diseño, Implementación |         Alta         |    Comercial     |

----
### Ejemplo de Herramientas CASE de Código Abierto

| Nombre   | Fabricante         | Diagramas UML Soportados | Etapas del SDLC Soportadas         | Curva de Aprendizaje | Tipo de Licencia |
| -------- | ------------------ | :----------------------: | ---------------------------------- | :------------------: | :--------------: |
| Modelio  | Modeliosoft        |       UML 2, BPMN        | Requisitos, Diseño, Implementación |        Media         |       GPL        |
| ArgoUML  | Tigris             |         UML 1.4          | Diseño                             |        Media         |       BSD        |
| StarUML  | MKLab              |          UML 2           | Diseño, Implementación             |        Media         |       GPL        |
| Umbrello | KDE                |          UML 2           | Diseño                             |         Baja         |       GPL        |
| Papyrus  | Eclipse Foundation |          UML 2           | Requisitos, Diseño                 |         Alta         |       EPL        |

----
### Herramientas No CASE con Soporte UML y Otros Modelos

Existen herramientas que, aunque no se consideran CASE en sentido estricto, permiten la creación de diagramas UML y otros modelos utilizados en la ingeniería del software. Estas se dividen en:​

- **Graficadores Visuales**: permiten crear diagramas mediante interfaces gráficas.
- **Graficadores Basados en Texto**: utilizan lenguajes descriptivos para generar diagramas.​

Estas herramientas son útiles para la documentación y comunicación de diseños, pero no ofrecen funcionalidades completas de ingeniería de software como las herramientas CASE.​

----
## Top 5 Herramientas No CASE (Graficadores)

| Nombre                                         | Fabricante      | Diagramas UML Soportados                        | Curva de Aprendizaje | Tipo de Graficador | Tipo de Licencia |
| ---------------------------------------------- | --------------- | ----------------------------------------------- | :------------------: | :----------------: | :--------------: |
| [PlantUML](https://plantuml.com/es/)           | PlantUML        | Casos de Uso, Clase, Secuencia, Actividad, etc. |        Media         |  Basado en Texto   |      Libre       |
| [draw.io](https://app.diagrams.net)            | JGraph          | Clase, Secuencia, Actividad, etc.               |         Baja         |       Visual       |      Libre       |
| [Lucidchart](https://www.lucidchart.com/pages) | Lucid Software  | Clase, Secuencia, Actividad, etc.               |         Baja         |       Visual       |     Freemium     |
| [Mermaid](https://mermaid.js.org)              | Knut Sveidqvist | Clase, Secuencia, etc.                          |        Media         |  Basado en Texto   |       MIT        |
| [yEd](https://www.yworks.com/products/yed)     | yWorks          | Clase, Actividad                                |         Baja         |       Visual       |      Libre       |

----
### Cuadro Comparativo: Herramientas CASE vs. Graficadores

| Característica            | Herramientas CASE | Graficadores  |
| ------------------------- | :---------------: | :-----------: |
| Automatización del SDLC   |        Sí         |      No       |
| Generación de Código      |        Sí         |      No       |
| Gestión de Requisitos     |        Sí         |   Limitada    |
| Validación y Verificación |        Sí         |      No       |
| Colaboración Integrada    |        Sí         |   Limitada    |
| Curva de Aprendizaje      |       Alta        |     Baja      |
| Costo                     |       Alto        | Bajo o Gratis |

_Nota:_ La implementación de estas características pueden variar de un producto a otro.