---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)/","tags":["digitalGarden","diagramaDeEstados"]}
---

## Diagrama de Estados (Elementos y Relaciones)

Los diagramas de estados permiten modelar el comportamiento dinámico de un sistema, objeto, clase o colaboración, representando los diferentes estados que puede adoptar y las transiciones entre ellos. Son especialmente útiles para describir ciclos de vida, respuestas a eventos y situaciones donde el comportamiento depende del historial o contexto interno del sistema ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]).

- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Estado\|Estado]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Transición\|Transición]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Evento\|Evento]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Acción\|Acción]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Jerarquía de Estados\|Jerarquía de Estados]]
- [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Elementos)#Región Concurrente\|Región Concurrente]]

---
### Estado  
Un estado representa una situación o condición en la que puede encontrarse un objeto durante su existencia. Puede caracterizarse como un conjunto de valores cualitativamente similares, un periodo de espera a eventos, o un periodo de ejecución de actividades. Los estados pueden ser simples o compuestos, y pueden definir actividades de entrada (`entry`) y salida (`exit`) ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Ejemplo**: `Soltero`, `Casado`, `EnEjecución`.  
- **Características** [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]] :  
  - Tiene actividades de entrada (`entry/`) y salida (`exit/`) [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000)]].  

#### Tipos de Estado

##### Inicial
Indica el inicio y final de la transición de estados.

**Figura**
_Estado Inicial y Final
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

[*] --> [*]
@enduml
```
Ver [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Relación con Otros Diagramas)\|Ejemplo]]

##### Simple
Su característica principal es que no posee subestados.

**Figura**
_Estado Simple y Transición_
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8
[*] --> Estado

Estado --> [*]
@enduml
```
Ver [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Relación con Otros Diagramas)\|Ejemplo]]

##### Compuesto
Es un estado que está compuesto por varios subestados.

**Figura**
_Estado Compuesto y Subestados_
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

[*] --> EstadoCompuesto: transición()
state EstadoCompuesto {
	[*] --> SubEstado1
	SubEstado1 --> SubEstado2 : transición2()
}
EstadoCompuesto --> [*]

@enduml
```

Ver [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Relación con Otros Diagramas)\|Ejemplo]]

---
### Transición  
Una transición es el vínculo que conecta dos estados y representa el cambio de un estado a otro como respuesta a un evento. Puede estar condicionada por una guarda (expresión booleana) y asociada a un efecto o acción. Las transiciones pueden ser externas (cambian el estado activo) o internas (no cambian el estado activo, pero ejecutan un efecto) ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Estructura**: `Evento [Guardia] / Acción`. 

| Estructura | Explicación                                                                                                                                                                        |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Evento     | Son las condiciones que desencadenan la transición entre dos estados. Puede ser:<br>- Interno (sin cambio de estado, ejecuta una acción).<br>- Externo (cambio de estado).         |
| Guarda     | Condiciones que deben satisfacerse antes de que se pueda realizar una transición.<br>Evalúa una expresión lógica y determina si se cumple la condición para realizar la transición |
| Acción     | Son tareas que se realizan automáticamente o manualmente después de que se haya realizado una transición                                                                           |
| Efecto     | **Son las acciones que se realizan después de que se haya realizado la transición, y pueden incluir la actualización de variables, cambios en el estado del sistema, entre otros** |

- **Ejemplo**: `presionarBotón() [nivelBatería > 5%] / activarPantalla`.  

---
#### Evento  
Un evento es una ocurrencia significativa que puede disparar una transición. Se clasifican en eventos de señal (comunicación asincrónica), llamada (invocación de operación), cambio (modificación de una condición) y tiempo (paso de tiempo). Los eventos pueden tener parámetros y su ocurrencia puede tener consecuencias en el modelo ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Ejemplos**: `matrimonio`, `divorcio`, `timeout`.  
- **Clasificación**:  
  - Señal (comunicación asincrónica).  
  - Llamada (invocación de operación).  
  - Temporal (paso de tiempo) ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

---
#### Acción  
Una acción es una operación atómica y no interrumpible que se ejecuta como efecto de una transición o como actividad de entrada/salida de un estado. Ejemplos incluyen la actualización de atributos, el envío de señales o la invocación de operaciones ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Ubicación**:  
  - En transiciones (`/activarAlarma`).  
  - En entrada/salida de estados (`entry/inicializar`).  
- **Ejemplo**: `exit/liberarRecursos` 

---
### Jerarquía de Estados  
Los estados pueden organizarse jerárquicamente mediante estados compuestos y subestados. Esto permite modelar comportamientos complejos, reutilizar transiciones y definir excepciones o condiciones de error de manera más eficiente ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Estado compuesto**: Agrupa subestados (ejemplo: `EnLlamada` con subestados `Activa` y `EnEspera`).  
- **Reutilización**: Permite definir comportamientos comunes en superestados [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]].  

---
### Región Concurrente  
Una región concurrente es una subdivisión de un estado compuesto donde pueden coexistir varios subestados activos en paralelo. Permiten modelar situaciones en las que un objeto puede estar simultáneamente en varios estados independientes, facilitando la representación de concurrencia dentro del sistema ([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

- **Ejemplo**: En un sistema de seguridad, `DetecciónMovimiento` y `MonitoreoTemperatura` operan simultáneamente.  
- **Sincronización**: Las regiones pueden coordinarse mediante eventos compartidos([[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|Booch et al., 2006]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|OMG, 2017]]; [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2007) Lenguaje Unificado de Modelado. Manual de Referencia\|Rumbaugh et al., 2007]]). 

**Figura**
_Estados Concurrentes_
![Zk Diagrama de Estados (Elementos).png](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/IS1/2025/Clase%2016%20Diagrama%20de%20Estados/000%20Adjuntos/Zk%20Diagrama%20de%20Estados%20(Elementos).png)

```
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

[*] --> EstadoCompuesto
state EstadoCompuesto {
	[*] --> Estado1
	Estado1 --> Estado2 : e12()
	Estado2 --> Estado1 : e21()
	||
	[*] --> Estado3
	Estado3 --> Estado4 : e34()
	Estado4 --> Estado3 : e43()
}
@enduml
```

---

### Referencias
- [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Booch et al., 2006) Booch, G., Rumbaugh, J., y Jacobson, I. (2006). El lenguaje Unificado de Modelado - Guía del Usuario (2a ed). Addison-Wesley.\|(Booch et al., 2006)]]  
- [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (OMG, 2017) UML Specifications\|(OMG, 2017)]]  
- [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Pressman, 2013) Ingeniería del Software - Un Enfoque Práctico (Séptima edición). McGraw-Hill Education\|(Pressman, 2013)]]  
- [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Rumbaugh et al., 2000) Lenguaje Unificado de Modelado. Manual de Referencia\|(Rumbaugh et al., 2000)]]  
