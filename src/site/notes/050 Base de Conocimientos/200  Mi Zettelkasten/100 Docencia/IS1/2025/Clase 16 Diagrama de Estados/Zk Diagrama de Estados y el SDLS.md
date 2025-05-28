---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados y el SDLS/","tags":["digitalGarden","diagramaDeEstados"]}
---

## Diagrama de Estados y el SDLS

### **Definición y Propósito**  
El **Diagrama de Estados** es una herramienta UML para modelar el comportamiento dinámico de sistemas, objetos o colaboraciones mediante **estados**, **transiciones**, **eventos** y **acciones**. En el **Ciclo de Vida de Desarrollo de Software (SDLC)**, se utiliza para:

- Capturar requisitos de comportamiento en fase de **análisis**. 
- Especificar lógica de estados durante el **diseño de sistemas**
- Validar transiciones críticas en **pruebas**

---

### **Relación con Fases del SDLC**  
| **Fase SDLC**  | **Uso del Diagrama de Estados**                                                    |     |
| -------------- | ---------------------------------------------------------------------------------- | --- |
| Análisis       | Modelar escenarios complejos (ejemplo: flujos de autenticación)                    |     |
| Diseño         | Definir jerarquías de estados y regiones concurrentes (ejemplo: sistemas de pagos) |     |
| Implementación | Guiar la codificación de máquinas de estado finito.                                |     |
| Pruebas        | Generar casos de prueba para cubrir todas las transiciones.                        |     |

---

### **Mejores Prácticas**  
- **Evitar estados huérfanos**: Toda transición debe tener destino.
- **Usar jerarquías**: Agrupar estados relacionados (ejemplo: `Errores → Timeout, ConexiónFallida`).  
- **Documentar eventos críticos**: Especificar guardias y acciones en transiciones complejas.  

---

### **Conexiones con Otros Modelos**  
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 13 Diagrama de Clases (Fundamentos, Elementos, Relaciones, etc.)/Zk Diagrama de Clases (Introducción, Definición, Características y sus Usos)\|Diagrama de Clases]]: Los estados se definen para instancias de clases.  
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 09 Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)/Zk !MOC Diagrama de Casos de Uso (Fundamentos, Elementos, Relaciones)\|Diagrama de Casos de Uso]]: Los estados reflejan flujos alternativos de interacción.  
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 04 Modelos de Proceso de Software/Zk Modelos de Proceso de Software\|Modelos de Procesos]]: Integración en metodologías ágiles o en cascada.  

---

**Referencias**:  
- [[Zk Lit (Booch et al., 2006)\|Zk Lit (Booch et al., 2006)]]  
- [[Zk Lit (OMG, 2017)\|Zk Lit (OMG, 2017)]]  
- [[Zk Lit (Pressman, 2013)\|Zk Lit (Pressman, 2013)]]  
- [[Zk Lit (Rumbaugh et al., 2000)\|Zk Lit (Rumbaugh et al., 2000)]]  
