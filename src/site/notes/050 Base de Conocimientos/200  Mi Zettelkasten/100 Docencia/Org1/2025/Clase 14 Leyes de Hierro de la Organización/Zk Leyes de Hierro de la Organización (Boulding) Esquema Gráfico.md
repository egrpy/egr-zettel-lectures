---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) Esquema Gráfico/","tags":["digitalGarden"]}
---

## Leyes de Hierro de la Organización (Boulding) Esquema Gráfico

Este diagrama sintetiza las **interacciones dinámicas** entre las seis Leyes de Hierro de la Organización propuestas por Boulding y mencionadas en [[(Johansen Bertoglio, 1982) Anatomía de la Empresa - Una Teoría General de las Organizaciones Sociales. Limusa  Noriega.pdf|Johansen Bertoglio (1982)]]. Su estructura refleja la visión sistémica de las organizaciones como redes de retroalimentación interdependientes.

**Figura**
_Esquema Gráfico de las Leyes de Hierro de la Organización_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
skinparam linestyle ortho
scale 1

' Diagrama de Clases: Leyes de Hierro de la Organización (Boulding/Johansen Bertoglio)

package "Leyes de Hierro" {
  class "Ley del Crecimiento" as LeyCrecimiento
  class "Ley de la Cultura" as LeyCultura
  class "Ley del Tamaño Óptimo" as LeyTamanoOptimo
  class "Ley de la Jerarquía" as LeyJerarquia
  class "Ley de la Inestabilidad" as LeyInestabilidad
  class "Ley de la Persistencia del Rol" as LeyPersistenciaRol
}

class "Sistema Organizacional" as SistemaOrganizacional
class "Sinergia"
class "Recursividad"
class "Entropía"
class "Neguentropía"
class "Entorno"

' Relaciones entre leyes
LeyCrecimiento -- LeyTamanoOptimo : "supera límites →\nfragmentación"
LeyCultura -- LeyJerarquia : "rigidez →\nconflictos"
LeyTamanoOptimo -- LeyInestabilidad : "fragmentación →\nvulnerabilidad"
LeyPersistenciaRol -- LeyInestabilidad : "roles obsoletos →\ninercia"
LeyCultura -- LeyPersistenciaRol : "valores →\nperpetuación roles"

' Conexión sistema-organización con leyes
SistemaOrganizacional <--- "Leyes de Hierro" : está regido por

' Conexión con conceptos sistémicos
SistemaOrganizacional <-u- Sinergia
SistemaOrganizacional <-u- Recursividad
SistemaOrganizacional <-u- Entropía
SistemaOrganizacional <-u- Neguentropía
SistemaOrganizacional <-u- Entorno

@enduml
```
Nota: Elaboración Propia, basado en [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Johansen Bertoglio, 1982) Anatomía de la Empresa - Una Teoría General de las Organizaciones Sociales. Limusa  Noriega\|Johansen (1982)]].

### Interpretación del Esquema Gráfico

| Elemento                           | Explicación                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Paquete de Leyes de Hierro         | Agrupa los seis principios fundamentales:<br><br>1a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley del Crecimiento)\|Ley del Crecimiento]]: Dinámica exponencial vs. límites logísticos.<br><br>2a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Cultura)\|Ley de la Cultura]]: Resistencia a cambios en patrones internalizados.<br><br>3a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley del Tamaño Óptimo)\|Ley del Tamaño Óptimo]]: Umbral crítico de eficiencia organizacional.<br><br>4a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Jerarquía)\|Ley de la Jerarquía]]: Distorsiones en estructuras de poder.<br><br>5a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Inestabilidad)\|Ley de la Inestabilidad]]: Fragilidad por factores internos/externos.<br><br>6a. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Persistencia del Rol)\|Ley de la Persistencia del Rol]]: Rigidez en funciones institucionalizadas.                                                    |
| Relación entre las Leyes           | Las flechas indican **efectos sinérgicos**:<br>    <br>- El crecimiento descontrolado ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley del Crecimiento)\|1a. Ley]]) acelera la pérdida de tamaño óptimo ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley del Tamaño Óptimo)\|3a. Ley]]).<br>        <br>- La rigidez cultural ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Cultura)\|2a. Ley]]) potencia conflictos jerárquicos ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Jerarquía)\|4a. Ley]]).<br>        <br>- La fragmentación estructural ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley del Tamaño Óptimo)\|3a. Ley]]) incrementa vulnerabilidad ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Inestabilidad)\|5a. Ley]]).<br>        <br>- Roles obsoletos ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Persistencia del Rol)\|6a. Ley]]) agravan la inestabilidad ([[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding) (Ley de la Inestabilidad)\|5a. Ley]]). |
| Conexión con Principios Sistémicos | - **Sinergia**: Emergencia de propiedades no predecibles desde partes aisladas.<br>	<br>- **Recursividad**: Jerarquía de sistemas dentro de sistemas .<br>	<br>- **Entropía/Neguentropía**: Tensión entre desorden y autoorganización .<br>	<br>- **Entorno**: Limitaciones y presiones contextuales sobre la organización.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
_Nota_: Los sistemas organizacionales, operan en permanente puja entre las fuerzas [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 06 Sistemas, Fundamentos, Propiedades, Principios Básicos/Zk Entropía\|entrópicas]] y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 12 Entropía y Neguentropía/Zk Neguentropía (Entropía Negativa)\|neguentrópicas]]. La [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 12 Entropía y Neguentropía/Zk Entropía y Neguentropía (Sistemas Viables)\|viabilidad organizacional]] depende del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 13 Principio de Organicidad/Zk Principio de Organicidad (Equilibrio Dinámico de Sistemas)\|equilibrio dinámico]] entre estos [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 06 Sistemas, Fundamentos, Propiedades, Principios Básicos/Zk Entropía\|entropía]] y [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 12 Entropía y Neguentropía/Zk Neguentropía (Entropía Negativa)\|neguentropía]], donde las [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 14 Leyes de Hierro de la Organización/Zk Leyes de Hierro de la Organización (Boulding)\|Leyes de Hierro]] actúan como marcos reguladores que condicionan su trayectoria evolutiva.
