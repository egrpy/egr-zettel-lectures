---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk Diagrama de Casos de Uso - Relaciones (Entre Casos de Uso, Comparación de Dependencias include y extend)/","tags":["digitalGarden","diagramaCasosDeUso","relaciones"]}
---

## Comparación de Dependencias include vs extend

| Característica | `<<include>>`                                            | `<<extend>>`                                                 |
| -------------- | -------------------------------------------------------- | ------------------------------------------------------------ |
| Obligatoriedad | El caso incluido es obligatorio.                         | El caso extendido es opcional/condicional.                   |
| Dirección      | El caso base depende del incluido (base apunta incluído) | El caso extendido depende del base (extendido apunta a base) |
| Ejemplo        | `Realizar Reserva .> Validar Usuario :<<include>>`       | `Aplicar Descuento .> Realizar :<<extend>>`                  |
| **Ejemplo**    | `Aplicar Descuento .> Realizar Compra`                   | `Realizar Reserva .> Validar Usuario`                        |
