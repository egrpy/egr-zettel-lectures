---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Realizar Préstamo)/","tags":["digitalGarden","ejemplos","diagramaCasosDeUso"]}
---

## Caso de Uso: Realizar Préstamo

**Actores**
- Usuario

**Escenario**
- Préstamo de libro físico

**Precondiciones**
- Libro disponible
- Usuario sin sanciones.

**Flujo Principal**
1. Seleccionar libro.
2. Si es una renovación ejecutar caso de uso [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Renovar Préstamo)\|Renovar Préstamo]]
3. Confirmar préstamo.
4. Ejecutar caso de uso  [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Generar Recibo)\|Generar Recibo]].

**Flujo Alternativo**
- Verificar...

**Excepciones**
1. Libro no disponible, notificación.

**Poscondiciones**
- Préstamo concretado ó
- Préstamos no concretado