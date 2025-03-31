---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Tipos de Elementos)/","tags":["digitalGarden"]}
---

## Modelo Conceptual del UML (Tipos de Elementos)

El UML se compone de varios tipos de elementos que se clasifican en cuatro categorías principales: **estructurales**, **comportamiento**, **agrupación** y **anotación**. Cada categoría incluye elementos específicos que contribuyen a modelar diferentes aspectos de un sistema.

Se utilizan para modelar la organización y composición del sistema.

----
### Estructurales

| Definición                                                                                                                   | Usos                                                                |
| ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| Elementos que describen la estructura estática de un sistema, incluyendo clases, objetos, componentes, nodos y casos de uso. | Se utilizan para modelar la organización y composición del sistema. |

**Elementos Incluidos**

- Clases: Representan conceptos abstractos con atributos y métodos.
- Objetos: Instancias de clases con valores específicos.
- Componentes: Representan partes del sistema que pueden ser reutilizadas.
- Nodos: Dispositivos físicos en un sistema.

----
### Comportamiento

| Definición                                                                                                                    | Usos                                                             |
| ----------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Elementos que describen cómo se comporta un sistema en el tiempo, incluyendo actividades, estados, transiciones y secuencias. | Se utilizan para modelar el comportamiento dinámico del sistema. |

**Elementos Incluidos**

- Actividades: Representan flujos de trabajo.
- Estados: Indican estados específicos de un objeto.
- Transiciones: Conectan estados.
- Secuencias: Muestran la secuencia temporal de mensajes entre objetos.
- Casos de Uso: Describen interacciones entre actores y el sistema. Si bien el Caso de Uso es un clasificador desde el punto de vista del UML, en este contexto, se incluyen en la categoría de comportamiento porque describen cómo el sistema interactúa con sus usuarios para alcanzar objetivos específicos.

----
### Agrupación

| Definición                                                                                     | Usos                                                                  |
| ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Elementos que agrupan otros elementos para facilitar su gestión y organización, como paquetes. | Se utilizan para organizar grandes modelos y facilitar la navegación. |

**Elementos Incluidos**

- Paquetes: Contienen clases u otros paquetes.

----
### Anotación

| Definición                                                                                  | Usos                                              |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| Elementos que proporcionan información adicional sobre el modelo, como notas o comentarios. | Se utilizan para documentar y explicar el modelo. |

**Elementos Incluidos**
- Notas: Cajas con texto que se conectan a otros elementos.
- Comentarios: Texto que se coloca cerca de los elementos del modelo.

----
### Cuadro Comparativo

|Tipo de Elemento|Definición|Elementos Incluidos|Uso|
|---|---|---|---|
|**Estructurales**|Describe la estructura estática|Clases, objetos, componentes, nodos, casos de uso|Modelar organización y composición|
|**Comportamiento**|Describe el comportamiento dinámico|Actividades, estados, transiciones, secuencias|Modelar comportamiento en el tiempo|
|**Agrupación**|Agrupa elementos para facilitar la gestión|Paquetes|Organizar modelos y facilitar la navegación|
|**Anotación**|Proporciona información adicional|Notas, comentarios|Documentar y explicar el modelo|

