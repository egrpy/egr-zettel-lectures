---
{"dg-publish":true,"permalink":"/060 Desarrollos/UI-UML Specification Framework (UUSF)/01 Overview/Zk SDLC - Ciclo de Vida del Desarrollo del Software (Detallado)/","tags":["digitalGarden","sdlc"]}
---

## SDLC - Ciclo de Vida del Desarrollo del Software (Detallado)
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam conditionStyle InsideDiamond

'|Analista|
start
:Inicio del Proyecto;
partition "Captura de\nRequerimientos" {
  fork
      :Identificar y Analizar\nRequierimientos;
      floating note right: Reuniones, Entrevistas,\nObservación, Manuales,\nCuestionarios, Focus Group, etc.
      :Redactar Requerimientos;
      :Definir Indicadores\de Evaluación;
  fork again
    :Identificar Candidatos\na Actores;
    :Describir Actores;
  end fork
}
partition Análisis {
  fork
    :Identificar Casos de Uso\nCantidatos;
    :Desarrollar Modelo\nde Casos de Uso;
    fork
      :Desarrollar Modelo de\nClases x Caso de Uso;
    fork again
      ::Desarrollar Modelo de\nInteracción x Caso de Uso;
    fork again
      :Desarrollar Modelo de Estados\npara las Clases/Colaboraciones\nque lo requieran;
    end fork
  fork again
    :Analizar Requerimientos\nno Funcionales;
  end fork
}

'|Diseñador|
partition Diseño {
  fork
    :Definir y Diseñar\nla Arquitectura;
    floating note right: Puede haber dependencia\nentre ambas actividades
  fork again
    :Configurar Infraestructura;
  end fork
  fork
    :Refinar Modelo de Clases;
  fork again
    :Identificar Clases Persistentes;
    :Diseño de Base de Datos;
  end fork
  :Agrupar Funcionalidades;
  :Especificar Opciones\nMenú del Software;
  #pink :Especificar GUI;
  floating note right: Aplicar UUSF
  :Diseñar GUI;
}

'|Programador|
partition Desarrollo {
  :Configurar Entorno\nDesarrollo;
  :Crear Base de Datos;
  :Desarrollar Programas;
  :Pruebas Unitarias;
  :Prueba Subconjuntos;
  :Prueba Total;
  :Test de Aceptación;
}

partition "Puesta en\nProducción" {
  :Instalación;
  :Pruebas Finales;
  :Pruesta en Producción;
}

partition Mantenimiento {
  :Inicio del Mantenimiento;
}
stop
@enduml
```

