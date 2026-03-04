---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Ingeniería del Software 1/Clase 08 Modelo Conceptual del UML - Elementos, Relaciones, Reglas y Mecanismos Comunes/Zk Modelo Conceptual del UML (Elementos de Anotación)/","tags":["#digitalGarden"]}
---

## Elemento de Anotación del Modelo Conceptual del UML

Los elementos de anotación en UML son mecanismos para añadir **comentarios**, **restricciones** o **información adicional** a los modelos sin alterar su semántica estructural o comportamental. Su propósito es mejorar la claridad y el contexto del diseño ([[050 Base de Conocimientos/900 Biblioteca/boochLenguajeUnificadoModelado2006/Zk Ref boochLenguajeUnificadoModelado2006\|Booch et al. (2006)]]; [[050 Base de Conocimientos/900 Biblioteca/omgUnifiedModelingLanguage2017/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/rumbaughLenguajeUnificadoModelado2000/Zk Ref rumbaughLenguajeUnificadoModelado2000\|Rumbaugh et al., 2000]].

### Elemento

#### **Nota**

| Item       | Descripción                                                                                                                                                                                                                                                  |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Definición | Comentarios textuales libres, representados como rectángulos con esquina doblada [[050 Base de Conocimientos/900 Biblioteca/boochLenguajeUnificadoModelado2006/Zk Ref boochLenguajeUnificadoModelado2006\|(Booch et al., 2006)]]. |
| Uso        | - Explicar decisiones de diseño.<br>- Documentar supuestos o requisitos no formales.                                                                                                                                                                         |

**Figura**
_Representación Gráfica de la Nota _
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
top to bottom direction
skinparam linetype ortho

scale 2
note "Esta es una nota\naclaratoria de..." as N1

@enduml
```
_Nota:_ Estas notas pueden ir vinculadas a algún elemento o relación o flotantes.
