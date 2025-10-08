---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Ejemplo de Especificación de Requerimiento de Software (SRS) - Sistema de Registros de Asistencia Clases/","tags":["#digitalGarden"]}
---

## Ejemplo de Especificación de Requerimiento de Software (SRS) - Sistema de Registros de Asistencia Clases

### Especificación de Requerimiento de Software (SRS) - Sistema de Registros de Asistencia Clases

Formato [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Norma IEEE 830 - 1998\|IEEE 830-1998]], ver también la actualización de este en [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk Norma IEEE 29148 - 2018\|Zk Norma IEEE 29148 - 2018]] y su [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS2/2025/Clase 11 Captura de Requerimientos/Zk IEEE 830 - 1998 vs ISO IEC IEEE 29148 - 2011 (Comparativo)\|comparativo]].

## 1. Introducción

### 1.1 Propósito

Este documento especifica los requerimientos para el Sistema de Registro de Asistencias (SRA), cuyo propósito es permitir a los docentes registrar la asistencia de los estudiantes a sus clases de manera confiable y eficiente, a través de aplicaciones móviles y web, integrándose como un sistema satélite del Sistema de Gestión Académica (SGA).

### 1.2 Alcance

El SRA permitirá:

- Registro de asistencias por parte de los docentes.
- Consultas de asistencias por estudiantes y directivos.
- Generación de reportes de asistencia.
- Integración con el SGA para mantener sincronizada la información académica (asignaturas, estudiantes, horarios).

El sistema estará disponible en versión web y móvil, asegurando facilidad de uso y accesibilidad.

### 1.3 Definiciones, acrónimos y abreviaturas

- **SRA**: Sistema de Registro de Asistencias.
- **SGA**: Sistema de Gestión Académica.
- **API**: Interfaz de Programación de Aplicaciones.
- **QR**: Código de respuesta rápida.

### 1.4 Referencias

IEEE Std 830-1998.

---

## 2. Descripción General

### 2.1 Perspectiva del producto

El SRA será un sistema satélite conectado mediante APIs al SGA. Su principal función es optimizar el registro de asistencias, reduciendo errores manuales y mejorando la trazabilidad.

### 2.2 Funciones principales

- Registro de asistencias por docentes (manual o con código QR).
- Consulta de asistencias por estudiante, docente y Directivos/funcionarios.
- Reportes de asistencia por semestre, materia o estudiante.
- Sincronización automática con el SGA.
- Notificaciones a estudiantes sobre su porcentaje de asistencia.

### 2.3 Características de los usuarios

- **Docentes**: registran la asistencia.
- **Estudiantes**: consultan su historial de asistencia.
- **Directivos / Funcionarios**: obtienen reportes globales.

### 2.4 Restricciones

- Depende de la integración con el SGA.
- Requiere conectividad a internet para sincronización.

---

## 3. Requerimientos Específicos

### 3.1 Requerimientos Funcionales

- **RF1**: El sistema debe permitir a los docentes registrar la asistencia de estudiantes desde aplicación web y móvil.

- **RF2**: El sistema debe permitir registrar la asistencia manualmente.
    
- **RF3**: El sistema debe sincronizar automáticamente la información de materias, docentes y estudiantes desde el SGA.
    
- **RF4**: El sistema debe permitir la consulta del historial de asistencias por parte de estudiantes y docentes.
    
- **RF5**: El sistema debe generar reportes de asistencia por estudiante, curso o periodo académico en formatos PDF/Excel.
    
- **RF6**: El sistema debe enviar notificaciones automáticas a los estudiantes cuando su porcentaje de asistencia esté por debajo del mínimo requerido.
    
- **RF7**: El sistema debe permitir a los directivos / funcinarios visualizar dashboards con estadísticas de asistencia global e individual.


---

### 3.2 Requerimientos No Funcionales

- **RNF1**: El sistema debe implementar **autenticación segura** (usuario, contraseña, tokens).
    
- **RNF2**: El sistema debe garantizar **disponibilidad del 99%** durante el calendario académico.
    
- **RNF3**: El sistema debe ser **escalable**, soportando al menos 5000 usuarios concurrentes.
    
- **RNF4**: El sistema debe ser **multi-plataforma** (Android, iOS, navegadores web).
    
- **RNF5**: El sistema debe asegurar **usabilidad y accesibilidad** (cumplir normas WCAG).
    
- **RNF6**: El sistema debe garantizar la **integridad y trazabilidad** de los registros de asistencia.
    
- **RNF7**: El sistema debe permitir integración mediante **APIs seguras** con el SGA.
    

---

### 3.3 Pseudorequerimientos (Condiciones externas/no controlables)

- **PR1**: Disponibilidad y estabilidad del **SGA** para la sincronización de datos.
    
- **PR2**: Acceso a internet en las aulas y dispositivos móviles de los docentes.
    
- **PR3**: Regulaciones académicas que definan criterios de aprobación en base a asistencia.
    
- **PR4**: Disponibilidad de servicios externos para notificaciones (correo, push).
    
- **PR5**: Capacitación de docentes y estudiantes en el uso de la aplicación.
    

---

## 4. Matriz de Trazabilidad de Requerimientos

|**RF**|**RNF asociados**|**PR asociados**|**Comentarios**|
|---|---|---|---|
|RF1: Registro de asistencia (web/móvil)|RNF1, RNF2, RNF4, RNF5|PR2, PR5|Registro central de todas las clases.|
|RF2: Registro con QR|RNF1, RNF2, RNF4|PR2, PR5|Requiere conectividad y capacitación mínima.|
|RF3: Sincronización con SGA|RNF6, RNF7, RNF2|PR1|Depende totalmente de APIs del SGA.|
|RF4: Consulta de historial|RNF2, RNF5, RNF6|PR2|Estudiantes deben poder consultar en cualquier momento.|
|RF5: Reportes PDF/Excel|RNF6, RNF4, RNF7|PR1, PR3|Útil para procesos administrativos.|
|RF6: Notificaciones a estudiantes|RNF2, RNF4, RNF5|PR4, PR2|Depende de proveedores externos (correo, push).|
|RF7: Dashboards para directivos|RNF2, RNF3, RNF5|PR1, PR3|Información consolidada, útil en toma de decisiones.|
