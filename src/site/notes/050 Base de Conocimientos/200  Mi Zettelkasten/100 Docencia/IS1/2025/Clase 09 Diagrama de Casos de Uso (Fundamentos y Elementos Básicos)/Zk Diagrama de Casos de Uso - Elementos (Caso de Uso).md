---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Caso de Uso)/","tags":["digitalGarden","diagramaCasosDeUso","casosDeUso"]}
---

## Caso de Uso

Un **caso de uso** es una unidad funcional coherente que describe cómo un [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Sujeto)\|sujeto]] (sistema, subsistema o cualquier componente, en el amplio sentido de la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 05 Sistemas, Subsistemas, Suprasistemas/Zk Sistema - Definición\|TGS]]), modelado como una [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 08 Elementos de un Sistema (Proceso de Conversión, Corriente de Salida, Mecanismos de Retroalimentación)/Zk Caja Negra\|caja negra]], interactúa con uno o más [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Elementos (Actores)\|actores]] para lograr un objetivo específico. Incluye todas lassecuencias principales, variaciones y excepciones del comportamiento esperado, junto con las respuestas asociadas. Aunque los casos de uso son conceptualmente independientes entre sí, pueden surgir dependencias implícitas debido a objetos compartidos en la implementación ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, 246)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).

### Características

| Característica            | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Comportamiento Externo    | Representa el comportamiento visible del sistema desde la perspectiva del usuario [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Centrado en Objetivos     | Cada caso de uso persigue un resultado específico y medible para el actor [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Granularidad Adecuada     | Representa una funcionalidad completa, no fragmentada [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|(Booch et al., 2006, 246)]]                                                                                                                                                                                                                                                                                                                                                                                            |
| Independencia Tecnológica | Describe el "qué" (requisitos), no el "cómo" (implementación) ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, 244)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).                                                                                                                                                                                                                                                             |
| Ejecución Dinámica        | Especificada mediante diagramas de [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Secuencia)\|secuencia]], [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Estados)\|estados]], [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 07 Modelo Conceptual del UML - Diagramas/Zk Modelo Conceptual del UML (Diagrama de Comunicación)\|comunicación]] o descripciones textuales [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].                                                                                                                                                                                                                      |
| Colaboración entre Clases | Los casos de uso se implementan mediante colaboraciones entre clases que pueden desempeñar múltiples roles. Son esenciales para implementar casos de uso complejos sin introducir dependencias innecesarias. ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, 246)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]). |

### **Relación con la Implementación**

Un caso de uso es una **descripción lógica de funcionalidad**, no una construcción explícita de la implementación. Su comportamiento se materializa mediante:

1. **Correspondencia con clases**:

    - Cada caso de uso se asocia a clases que implementan sus operaciones y transiciones [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].

    - Una clase puede participar en múltiples casos de uso al desempeñar distintos roles (ejemplo: una clase Usuario gestiona tanto autenticación como preferencias.

2. **Diseño de colaboraciones**:

    - La implementación se modela mediante **colaboraciones** (conjuntos de clases que interactúan para realizar el caso de uso) [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).

    - El desafío de diseño radica en combinar roles de clases sin introducir complejidad innecesaria  [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].

#### Implementación Mediante Clases GUI y Colaboraciones
En sistemas con interfaz gráfica (GUI), los casos de uso suelen ser implementados por una clase GUI que actúa como intermediaria entre los actores y las clases internas del sistema. Estas clases GUI capturan las interacciones del usuario y colaboran con otras clases para cumplir los objetivos del caso de uso ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, capítulo 17, 18)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).

1. **Rol de las Clases GUI**:
    
    - Capturan entradas del usuario (actores).
    - Traducen las interacciones en llamadas a métodos internos.
    - Presentan los resultados al usuario.
        
2. **Colaboraciones entre Clases**:
    
    - Los casos de uso rara vez son implementados por una sola clase; requieren la interacción entre:
        - Clases GUI (interfaz).
        - Clases de dominio (lógica de negocio).
        - Clases de servicio (coordinación).

#### Ejemplo Práctico
A modo de ejemplo simplificado, caso de uso "Realizar Inscripción":

- `InscripciónGUI`: Captura los datos del usuario.
- `InscipciónService`: Valida los datos y coordina la operación.
- `Asignaturas`: Verifica disponibilidad en la base de datos.
- `Curso`: Lugar donde se registra la inscripción

#### Implementación en Sistemas sin GUI

En sistemas sin interfaz gráfica, como APIs o procesos batch, los casos de uso se implementan mediante servicios backend y componentes especializados:

- **Actor**: Sistemas externos o eventos programados.
    
- **Clases involucradas**: Servicios REST, manejadores de eventos y clases DAO.
    
- **Ejemplo**: Un caso como "Procesar Lote" podría involucrar un servicio que recibe datos y los distribuye entre clases encargadas del cálculo y almacenamiento.

### Estructura de un Caso de Uso

| Componente          | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Nombre**          | Verbo en infinitivo (ejemplo: "Realizar Inscripción") que refleja la acción del actor [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|(Booch et al., 2006, 247)]].                                                                                                                                                                                                                                                |
| **Precondiciones**  | Condiciones que deben cumplirse antes de iniciar el caso de uso (ejemplo: "Usuario autenticado") [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000, 70)]].                                                                                                                                                                                                                                                                                       |
| **Flujo principal** | Secuencia de pasos para alcanzar el objetivo sin desvíos ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, capítulos 17,18)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).                              |
| **Flujos alternos** | Variaciones del flujo principal por excepciones (ejemplo: "Solapamiento de Horarios") ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, capítulos 17,18)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]). |
| **Postcondiciones** | Estado del sistema tras ejecutar el caso de uso (ejemplo: "Inscripción confirmada") ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2000) Booch, G., Rumbaugh, J., y Jacobson, I. (2000). El lenguaje Unificado de Modelado (1a ed.). Addison-Wesley.\|Booch et al. (2006, capítulos 17,18)]]; [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk (OMG, 2017) About the Unified Modeling Language Specification Version 2.5.1\|OMG (2017, sección18.1)]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al. (2000, 70)]]).   |

#### Ejemplo Práctico: Inscribir a Curso

Un estudiante interactúa con el sistema académico para inscribirse en un curso:

- **Actor Principal**:
	- Estudiante.

- **Precondiciones**:
	- El estudiante debe estar autenticado.

- **Flujo Principal**:
    - Seleccionar curso.
    - Verificar disponibilidad.
    - Registrar inscripción.
    - Confirmar inscripción.
    
- **Flujos Alternos**:
    - Si no hay cupos disponibles, ofrecer alternativas.
    - Si hay conflictos horarios, solicitar nueva selección.

- **Postcondiciones**:
	- Inscripción registrada y visible en el perfil del estudiante.
