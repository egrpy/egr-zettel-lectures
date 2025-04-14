---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema Biblioteca (Explicación del Diagrama de Casos de Uso)/","tags":["digitalGarden","diagramaCasosDeUso"]}
---

## Explicación del Diagrama de Casos de Uso

El diagrama de casos de uso presentado representa una **visión general del sistema**, mostrando cómo los diferentes actores interactúan con las funcionalidades principales del "Sistema de Gestión de Biblioteca". Este diagrama es una herramienta fundamental en la fase de **Análisis**dentro del [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 03 Costos y Complejidad del Software/Zk Ciclo de Vida del Desarrollo del Software\|Ciclo de Vida del Desarrollo del Software (SDLC)]], ya que permite capturar las necesidades funcionales desde la perspectiva de los usuarios.

### Objetivo del Diagrama

El diagrama tiene como objetivo principal proporcionar una representación clara y concisa de las **interacciones entre los actores y las funcionalidades del sistema**. Esto permite:

- Identificar y documentar los requerimientos funcionales asociados a cada caso de uso.
- Visualizar las dependencias entre casos, asegurando que las funcionalidades estén correctamente integradas.
- Facilitar la comunicación entre los interesados (clientes, desarrolladores y analistas) durante las fases posteriores del SDLC.

### Elementos Principales del Diagrama

1. **Actores**:
    
    - **"Usuario"**: Representa un actor general que agrupa a los roles específicos de "Estudiante" e "Investigador". Ambos roles heredan las capacidades básicas definidas para el "Usuario", como buscar libros, realizar préstamos y consultar su historial.
        
    - **"Estudiante"** y **"Investigador"**: Subactores especializados que comparten funcionalidades comunes, pero pueden tener restricciones o permisos específicos según el contexto.
        
    - **"Bibliotecario"**: Representa al administrador del sistema, responsable de gestionar el catálogo y los usuarios.
        
2. **Casos de Uso**:
    
    - Los casos de uso están representados como óvalos dentro del límite del sistema ("Sistema de Biblioteca"). Cada caso describe una funcionalidad específica que satisface un requerimiento funcional:
        
        - **"Buscar Libros"**: Permite a los usuarios buscar libros por título, autor o categoría.
            
        - **"Realizar Préstamo"**: Gestiona la solicitud de préstamo para libros disponibles.
            
        - **"Renovar Préstamo"**: Extiende la funcionalidad de "Realizar Préstamo", permitiendo renovar préstamos existentes bajo ciertas condiciones.
            
        - **"Devolver Libro"**: Permite registrar la devolución de libros prestados.
            
        - **"Consultar Historial"**: Muestra a los usuarios un registro detallado de sus préstamos y devoluciones.
            
        - **"Administrar Catálogo"**: Permite al bibliotecario gestionar el inventario bibliográfico (agregar, modificar o eliminar libros).
            
        - **"Gestionar Usuarios"**: Funcionalidad exclusiva para bibliotecarios, enfocada en la administración de perfiles de usuarios.
            
        - **"Generar Recibo"**: Caso incluido (`<<include>>`) en "Realizar Préstamo" y "Devolver Libro", encargado de generar un comprobante digital para cada transacción.
            
3. **Relaciones entre Elementos**:
    
    - **Generalización entre Actores**:
        
        - "Estudiante" e "Investigador" heredan las capacidades básicas del actor general "Usuario".
            
    - **Asociación entre Actores y Casos de Uso**:
        
        - Los actores están conectados a los casos que pueden ejecutar. Por ejemplo, "Estudiante" puede interactuar con "Buscar Libros", mientras que "Bibliotecario" está asociado a "Administrar Catálogo".
            
    - **Relaciones `<<include>>` y `<<extend>>` entre Casos de Uso**:
        
        - La relación `<<include>>` asegura que "Generar Recibo" sea ejecutado siempre como parte integral de los casos "Realizar Préstamo" y "Devolver Libro".

        - La relación `<<extend>>` permite que "Renovar Préstamo" amplíe la funcionalidad base definida en "Realizar Préstamo", dependiendo de condiciones específicas (por ejemplo, si el préstamo es renovable).

### Relación con los Requerimientos

Cada caso de uso está alineado con uno o más requerimientos funcionales definidos en la [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/30 Captura de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Lista de Requerimientos del Sistema)\|Lista de Requerimientos]]. Por ejemplo:

- El caso "Buscar Libros" satisface el requerimiento funcional RF001.
- El caso "Generar Recibo", incluido en otros casos, responde al RF005.

Además, se han considerado los requerimientos no funcionales (RNF) para garantizar que las interacciones sean intuitivas (RNF001), soporten múltiples usuarios concurrentes (RNF002), y utilicen una base de datos robusta para persistencia (RNF003).

### Conclusión

Este diagrama es una herramienta esencial para garantizar que el diseño e implementación del sistema cumplan con las expectativas definidas durante la fase inicial del proyecto. Al capturar todas las interacciones principales y sus relaciones, establece una base sólida para avanzar hacia etapas más detalladas como el diseño técnico y la programación.

Para más detalles sobre cada caso, consultar las [[Zk Ejemplo Sistema de Biblioteca (Especificaciones Textuales)\|Especificaciones de Casos de Uso]] correspondientes.
