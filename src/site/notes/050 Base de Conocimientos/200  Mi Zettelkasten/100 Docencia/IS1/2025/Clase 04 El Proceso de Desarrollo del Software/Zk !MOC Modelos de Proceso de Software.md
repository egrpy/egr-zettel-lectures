---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk !MOC Modelos de Proceso de Software/","tags":["digitalGarden","moc","software","proceso"]}
---

## Contenido

### Introducción
Los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos de Proceso de Software\|modelos de proceso de software]] forman parte del concepto más amplio del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 03 Costos y Complejidad del Software/Zk Ciclo de Vida del Desarrollo del Software\|Ciclo de Vida del Desarrollo del Software (SDLC)]], el cual define las fases generales que atraviesa un producto de software, desde su concepción hasta su mantenimiento. Dentro de este marco, los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos de Proceso de Software\|modelos de proceso]] estructuran estas fases en distintos esquemas, proporcionando estrategias específicas para gestionar el desarrollo de software.

Como [[050 Base de Conocimientos/200  Mi Zettelkasten/010 Informática/Zk Framework o Marco de Trabajo\|marcos de trabajo]], los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos de Proceso de Software\|modelos de proceso de software]] establecen la secuencia de actividades, tareas y productos entregables necesarios para desarrollar software de alta calidad. Funcionan como una **hoja de ruta** para los equipos de desarrollo, permitiéndoles organizar el proceso, gestionar riesgos, planificar proyectos y asignar recursos de manera eficiente.

Además, estos modelos no son estáticos; evolucionan y se adaptan a las necesidades específicas de cada proyecto. Su desarrollo ha dado lugar a enfoques más flexibles y contemporáneos, como los modelos ágiles y DevOps, que buscan optimizar la entrega de software y mejorar la colaboración en los equipos.

```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray

class "Ciclo de Vida del Desarrollo del Software (SDLC)" {
    + Fases [Identificación del Problema, Planificación, Requerimientos, ...]
    + Define las fases generales del desarrollo()
}

class "Modelos de Proceso de Software" {
    + Ejemplos [Cascada, Espiral, Incremental, Ágiles]
    + Organizan las fases del SDLC()
    + Proveen estrategias de desarrollo()
}

class "Frameworks" {
    + Estructuran la gestión del desarrollo()
    + Adaptables a proyectos específicos()
    + Ejemplos [Scrum, Kanban, Extreme Programming]
}

class "Actividades" {
    + Diseño()
    + Implementación()
    + Pruebas()
    + Despliegue()
    + Mantenimiento()
    + ...
}

class "Tareas" {
    + Requisitos()
    + Codificación()
    + Validación()
    + Integración()
    + ...
}

class "Productos Entregables" {
    + Documentación()
    + Código Fuente()
    + Manuales()
    + Informes de Pruebas()
    + ...
}

"Ciclo de Vida del Desarrollo del Software (SDLC)" --* "Modelos de Proceso de Software"
"Modelos de Proceso de Software" --* "Frameworks"
"Modelos de Proceso de Software" --* "Actividades"
"Actividades" --* "Tareas"
"Actividades" --* "Productos Entregables"
@enduml

```

## Desarrollo
[[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos de Proceso de Software\|Modelos de Proceso de Software]]

Distinguimos dos tipos de Modelo de Procesos de Software:
1. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos Clásicos de Proceso de Software\|Modelos Clásicos]]
	1.1 [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelo en Cascada (Waterfall Model)\|Modelo en Cascada]]
	1.2 [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelo Incremental\|Modelo Incremental]]
	1.3 [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelo Evolutivo (Prototipos y Espiral)\|Modelo Evolutivo (Prototipos y Espiral)]]

2. [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos Contemporáneos (Enfoques) de Proceso de Software\|Modelos Contemporáneos]]
	2.1  [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos Ágiles\|Modelos Ágiles]]
	2.2 [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk DevOps (Development and Operation)\|DevOps]]

[[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Adaptación de Modelos Clásicos en Entornos Modernos\|Adaptación de Modelos Clásicos en Entornos Modernos]]

## Conclusión
Los [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 El Proceso de Desarrollo del Software/Zk Modelos de Proceso de Software\|modelos de proceso de software]] han evolucionado desde enfoques tradicionales como el Modelo en Cascada, Incremental y Evolutivo, hasta enfoques contemporáneos como los modelos ágiles y DevOps. La adaptación de modelos clásicos a tecnologías emergentes como AI es crucial para mantener su relevancia.

**Ventajas y Desafíos**, la integración de tecnologías emergentes mejora la flexibilidad y eficiencia, pero también plantea desafíos culturales y técnicos.

**Futuro del Desarrollo de Software**, el futuro del desarrollo de software dependerá de la capacidad de los modelos de proceso para adaptarse a nuevas tecnologías y necesidades cambiantes del mercado.
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray

class "Ciclo de Vida del Desarrollo del Software (SDLC)" {
    + Fases [Identificación del Problema, Planificación, Requerimientos, ...]
    + Define las fases generales del desarrollo()
}

class "Modelos de Proceso de Software" {
    + Ejemplos [Cascada, Espiral, Incremental, Ágiles]
    + Organizan las fases del SDLC()
    + Proveen estrategias de desarrollo()
}

class "Modelos Clásicos" {
    + Modelo en Cascada
    + Modelo Incremental
    + Modelo Evolutivo
...
}

class "Modelos Contemporáneos" {
    + Modelos Ágiles
    + DevOps
...
}

class "Tecnologías Emergentes" {
    + Inteligencia Artificial
    + Blockchain
...
}

class "Ventajas de la Adaptación" {
    + Flexibilidad Aumentada()
    + Eficiencia Mejorada()
    + Innovación Incrementada()
}

class "Desafíos de la Adaptación" {
    + Cambios Culturales()
    + Complejidad Técnica()
}

"Ciclo de Vida del Desarrollo del Software (SDLC)" --* "Modelos de Proceso de Software"
"Modelos de Proceso de Software" --* "Modelos Clásicos"
"Modelos de Proceso de Software" --* "Modelos Contemporáneos"
"Modelos Clásicos" --* "Modelos Contemporáneos"
"Modelos Contemporáneos" --* "Tecnologías Emergentes"
"Tecnologías Emergentes" --* "Ventajas de la Adaptación"
"Tecnologías Emergentes" --* "Desafíos de la Adaptación"
@enduml

```
