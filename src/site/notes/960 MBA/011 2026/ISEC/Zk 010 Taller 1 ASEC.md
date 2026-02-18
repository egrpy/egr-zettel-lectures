---
{"dg-publish":true,"permalink":"/960 MBA/011 2026/ISEC/Zk 010 Taller 1 ASEC/","tags":["definir"]}
---

## Taller

### 1. Configuración del Taller

Lo tratado en este taller es absolutamente confidencial para ambas partes.

#### Objetivos
- Validar el esquema “MBA ERP Cloud Edition” como base de solución.
- Elicitar requerimientos **no funcionales** (seguridad, performance, disponibilidad, soporte, cumplimiento)
- Identificar requerimientos de **integración** y **puntos de dolor** del sistema / infrastructura actual

#### Participantes
- MBA S.A
	- Facilitador
	- Gerente Técnico
	- Consultores
- ASEC
	- Socios
	- Referente de Sistemas
	- key users

---

### 2. Agenda propuesta (120 minutos)

#### Bloque 1 – Contexto y Esquema Propuesto (20 min)

- 5 min – Bienvenida y Objetivo
    - Presentación de MBA ( 34 años de experiencia, principales sectores atendidos, etc.)
    - No venimos a definir pantallas modulares, sino a acordar un modelo de servicio / plataforma y entender qué necesitan en NFR e integraciones.​

- 15 min – Presentación MBA ERP Cloud Edition
    
    - Cliente → ASEC → Capa de Administración → Aplicación multi‑tenant → BD por cliente → Gestión de Cambios → Roadmap Funcional.
        
    - Pregunta de chequeo al final:
        - ¿Esto refleja cómo les gustaría consumir el servicio en el futuro?

**Salida:** Acuerdo de que el esquema es una base razonable (o registrar objeciones mayores).

---

#### Bloque 2 – Puntos de Dolor del Sistema Actual (25 min)

Objetivo: Identificación de los PD

Recomendación: Abrir el tema desde el negocio, no desde la tecnología

- 5 min – Pregunta disparadora (plenario)
    
    - En una frase, ¿qué es lo que más les ‘duele’ hoy de su sistema e infraestructura actual?
        
- 15 min – Mapa rápido de dolores (pizarra / post‑its / transparencia)
    Clasificar en tres columnas (puede ser en una slide con notas):
    - Operativos (productividad, tiempos, errores).
    - Tecnológicos (caídas, performance, backups, seguridad).
    - Negocio (limitaciones para crecer, abrir nuevos servicios, cumplir normativas).
    
- 5 min – Priorización rápida
    - Cada participante marca 3 pains que considera críticos.


Salida: Lista priorizada de dolores para usar como criterios de NFR.

---

### Bloque 3 – NFR Claves (seguridad, disponibilidad, performance, soporte) (40 min)

En base a los dolores y los NFR como “drivers arquitectónicos”.

Dividir en 4 temas (10 min cada uno, formato conversación guiada):

1. **Disponibilidad y Continuidad**
    
    - Preguntas:
        - ¿Qué tiempo máximo de caída tolerarían en horario crítico?
        - ¿Qué épocas del año son más sensibles (cierres, fiscales, etc.)?
            
    - Intentar concretar: % disponibilidad deseada, ventanas de mantenimiento aceptables.
        
2. **Performance y Escalabilidad**
    
    - Preguntas:
        - ¿En qué momentos sienten lentitud hoy? (cierres, picos de facturación, acceso remoto).
        - Con 75 clientes, ¿qué les preocupa más: tiempos de respuesta, tiempos de proceso, etc.?

3. **Seguridad y Cumplimiento**
    
    - Preguntas:
        - ¿Qué requisitos concretos tienen hoy (normas locales, auditorías, segregación de funciones, logs)?
        - ¿Qué quieren mejorar respecto a hoy con respecto al acceso remoto?

4. **Soporte y Operación del Servicio**
    
    - Preguntas:
        - ¿Qué esperan de nosotros como proveedor: horarios de soporte, tiempos de respuesta, canales?
        - ¿Qué hoy hace perder más tiempo al equipo de ASEC cuando algo falla?

En cada bloque, tomar nota de los NFR de manera simple. Ejemplo:
- Disponibilidad: X horas/mes de downtime máximo, con ventanas de mantenimiento programadas.
- Performance: respuesta < N segundos para consulta típica de contabilidad con M registros.

---

## Bloque 4 – Integraciones y Datos (20 min)

Objetivo: entender el ecosistema alrededor del ERP

- 10 min – Mapa de sistemas actuales
    
    - Pregunta: ¿Con qué otros sistemas se tiene que hablar hoy su sistema contable?
    - Ejemplos: facturación electrónica, bancos, planillas, sistemas de sueldos, portales de clientes, Equifax, etc.
    - Dibujar un círculo con el ERP en medio y flechas a cada sistema nombrado.

- 10 min – Priorización y Tipo de Integración

    - Para cada sistema, preguntar:
        - ¿Necesitamos integración en tiempo real, diaria, mensual?
        - ¿Qué datos intercambiamos hoy y qué faltaría?

Salida: lista de integraciones + frecuencia + tipo de datos.

---

## Bloque 5 – Cierre y próximos pasos (15 min)

- 10 min – Síntesis por parte de MBA
    
    - Releer los NFR más importantes y los dolores críticos.
    - Pregunta: ¿Falta algo grande o estamos reflejando bien sus preocupaciones?​

- 5 min – Acordar siguientes pasos
