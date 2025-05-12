---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 13 Diagrama de Clases (Fundamentos, Elementos, Relaciones, etc.)/Zk Diagrama de Clases (Técnicas Comunes de Modelado)/","tags":["digitalGarden"]}
---

## Diagrama de Clases (Técnicas Comunes de Modelado)

> [!info] **Resumen**  
> Las técnicas de modelado en diagramas de clases permiten capturar la estructura estática de sistemas mediante cuatro enfoques complementarios: definición del vocabulario del dominio, distribución equilibrada de responsabilidades, modelado de entidades no software y gestión de datos primitivos. Estas técnicas se alinean con los principios fundamentales del UML [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]].

### Vocabulario del Sistema

#### Objetivo
Identificar y formalizar las abstracciones clave del dominio.

| Componente                 | Acciones                                                                                                                         | Participantes Involucrados |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| **Abstracciones**          | Modelar conceptos relevantes del entorno analizado                                                                               | Usuarios y desarrolladores |
| **Captura de vocabulario** | - Identificar conceptos clave  <br>- Definir para cada abstracción:  <br>- Responsabilidades  <br>- Atributos  <br>- Operaciones | Equipo interdisciplinario  |

#### Ejemplo  
En un sistema bancario, las abstracciones incluyen `Cuenta`, `Transacción` y `Cliente`, cada una con atributos como `saldo` y operaciones como `realizarDepósito()`.

### Distribución de Responsabilidades

#### Principio Rector
Equilibrio entre cohesión y acoplamiento [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006) ]]

#### Técnicas

1. **Responsabilidad única:** Cada clase modela una entidad discreta.
2. **Colaboración:** Grupos de clases trabajan para objetivos comunes.
3. **Refinamiento iterativo:**
    - Dividir clases sobredimensionadas
    - Consolidar clases mínimas
    - Buscar equilibrio en la carga funcional

#### Checklist de Validación

- ¿Cada clase tiene 3-7 responsabilidades principales?
- ¿Las operaciones están alineadas con los atributos de la clase?
    

### Modelado de Elementos No Software

#### Alcance
Incluir entidades físicas o conceptuales del dominio.

| Tipo                     | Ejemplos                 | Representación UML                    |
| ------------------------ | ------------------------ | ------------------------------------- |
| **Entidades físicas**    | Dispositivos, documentos | Clases con estereotipo `<<Physical>>` |
| **Conceptos abstractos** | Políticas, regulaciones  | Clases con notas adjuntas             |

### Modelado de Datos Primitivos

#### Estrategia
Clases como tipo de dato
