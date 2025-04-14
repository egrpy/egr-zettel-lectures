---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso, Escenarios)/","tags":["digitalGarden","diagramaCasosDeUso","casosDeUso"]}
---

## Escenarios de un Casos de Uso

En el contexto de los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Casos de Uso)\|diagramas de casos de uso]], un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)\|caso de uso]] representa una unidad de funcionalidad que un sistema proporciona a sus [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]]. Sin embargo, cada caso de uso puede desarrollarse a través de diferentes situaciones específicas, conocidas como **escenarios**.

### Definición de Escenario

Un **escenario** es una instancia particular de un caso de uso, que describe un flujo específico de eventos en función de condiciones particulares. Es decir, un caso de uso puede comprender múltiples escenarios que representan distintas formas en las que se puede ejecutar la funcionalidad [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|(Booch et al., 2006, p. 249)]].

#### Ejemplo: Inscribirse a Asignatura

Un estudiante universitario que se inscribe para cursar una nueva asignatura puede enfrentar distintos escenarios, dependiendo de su situación académica y financiera:

| Escenario                                  | Explicación                                                                                                                                                |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| El estudiante no cuenta con beca           | Es el escenario más común, sigue el proceso estándar de inscripción y pago.                                                                                |
| El estudiante tiene una beca de Itaipú     | El sistema verifica automáticamente la cobertura de la beca antes de confirmar la inscripción, tiene un flujo "normal" pero distinto al escenario anterior |
| El estudiante cuento con otro tipo de beca | Pueden aplicarse reglas adicionales, como descuentos parciales o requisitos administrativos específicos.                                                   |

Cada uno de estos escenarios implica reglas de negocio particulares y puede representarse mediante una secuencia diferente de pasos dentro del caso de uso general.

### Importancia de los Escenarios en la Modelización

La identificación de escenarios dentro de un caso de uso puede ayudar para:

- Capturar variaciones en la ejecución de una funcionalidad.
- Identificar requisitos específicos para cada situación.
- Diseñar pruebas de software basadas en diferentes caminos de ejecución.
- Facilitar la comprensión del sistema por parte de los stakeholders.

Al modelar un caso de uso, es recomendable documentar los escenarios más relevantes, destacando los flujos normales y alternativos para garantizar una especificación clara y completa.

En sistemas de gestión, incluso aquellos de pequeña escala, es común que un solo caso de uso tenga múltiples escenarios posibles. A medida que el número de casos de uso y escenarios aumenta, la complejidad del sistema crece significativamente. Sin embargo, esta diversidad de escenarios es una característica inherente al desarrollo de software y debe abordarse mediante un modelado estructurado y preciso [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|(Booch et al., 2006, p. 249)]].