---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos y Elementos Básicos)/Zk Diagrama de Casos de Uso - Relaciones (Entre Casos de Uso, Comparación Generalización vs Dependencias include y extend)/","tags":["digitalGarden","diagramaCasosDeUso","relaciones"]}
---

## Comparación Generalización vs Dependencias include y extend en Diagramas de Casos de Uso

| Comparación                                 | Explicación                                                                                                                                                                                                                                                           |
| ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Dependencia `<<include>>` vs Generalización | La generalización modela variantes especializadas, mientras que `<<include>>` representa dependencias obligatorias entre casos.<br>        <br>Ejemplo: `<<include>>` se podría usar para incluir "Validar Usuario" dentro de "Realizar Pago", de manera obligatoria. |
| Dependencia `<<extend>>` vs Generalización  | La generalización es jerárquica y estática, mientras que dependencia `<<extend>>` es dinámica y condicional.<br>        <br>Ejemplo: `<<extend>>` se podría usar para agregar "Aplicar Descuento" a "Realizar Pago", de manera opcional                               |
