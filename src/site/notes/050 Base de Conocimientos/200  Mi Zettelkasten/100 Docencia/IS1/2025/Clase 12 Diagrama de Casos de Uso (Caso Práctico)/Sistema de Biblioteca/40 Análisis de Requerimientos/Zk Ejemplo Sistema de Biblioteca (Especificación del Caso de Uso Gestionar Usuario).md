---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 12 Diagrama de Casos de Uso (Caso Práctico)/Sistema de Biblioteca/40 Análisis de Requerimientos/Zk Ejemplo Sistema de Biblioteca (Especificación del Caso de Uso Gestionar Usuario)/","tags":["digitalGarden","ejemplos","diagramaCasosDeUso"]}
---

## Caso de Uso: Gestionar Usuario

**Actores**
- Bibliotecario (primario)
- Usuario

**Escenario**
- Registrar, modificar o eliminar usuarios.

**Precondiciones**


**Flujo Principal**
1. Bibliotecario solicita datos del usuario.
2. Agregar/modificar/eliminar usuario.
3. Confirmar cambios en BD.

**Flujo Alternativo**
- **A1:** Si los datos ingresados son inválidos, el sistema muestra un mensaje de error y solicita la corrección de los mismos.

**Excepciones**
- **E1:** Si el usuario ya existe al intentar agregarlo, el sistema muestra un mensaje de error por duplicidad.

**Poscondiciones**
- El registro de usuarios queda actualizado en la base de datos.