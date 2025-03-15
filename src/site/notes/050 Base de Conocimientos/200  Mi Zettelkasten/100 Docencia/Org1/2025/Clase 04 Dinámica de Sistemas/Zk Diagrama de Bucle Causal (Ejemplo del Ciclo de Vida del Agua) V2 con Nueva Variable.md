---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 04 Dinámica de Sistemas/Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable/","tags":["definir"]}
---

## Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) con una Nueva Variable

En el modelado, análisis y simulación del comportamiento de sistemas complejos, a menudo es necesario agregar o eliminar variables para evaluar su impacto en un contexto específico.En este caso, incorporaremos una nueva variable para analizar su efecto particular.

En el ejemplo sobre el el [[050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/Org1/2025/Clase 04 Dinámica de Sistemas/Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V1\|Ciclo de Vida del Agua]], consideraremos que no toda el agua de lluvia regresa directamente a las Superficies de Agua. En la realidad, una parte se infiltra en el suelo y queda almacenada en él. Introduciremos al modelo la variable **Almacenamiento de Agua en el Suelo**.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/050-base-de-conocimientos/200-mi-zettelkasten/100-docencia/org1/2025/clase-03-sinergia-y-recursividad/zk-sinergia-en-accion-ciclo-de-vida-del-agua/#variables" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Variables
- Aguas Superficiales (lagos, estanques, océanos, etc.)
- Evaporación (evaporación de las aguas)
- Lluvia (agua evaporada que vuelve a caer)
- Corrientes de Agua (rios, arroyos, etc.)


</div></div>

- Almacenamiento de Agua en el Suelo

----
### Diagrama de Flujo Causal
**Figura**
_Diagrama de Bucle Causal con Nueva Variable sin Identificar Relación Causal_
![Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable.png](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/Org1/2025/Clase%2004%20Din%C3%A1mica%20de%20Sistemas/000%20Adjuntos/Zk%20Diagrama%20de%20Bucle%20Causal%20(Ejemplo%20del%20Ciclo%20de%20Vida%20del%20Agua)%20V2%20con%20Nueva%20Variable.png)
Fuente: Elaboración propia.

----
### Análisis de Variables
Solo analizaremos la nueva variable introducida, las demás permanecen como en el ejemplo original.

| Variables                                        | Relaciones                                                                                                                                                                                                                                                 |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aguas Superficiales y Evaporación                | La cantidad de agua en las aguas superficiales influye positivamente en la evaporación. Cuanto más agua en las aguas superficiales, más evaporación ocurre.<br>Tipo de Relación Causal: **Positiva (+)**                                                   |
| Evaporación y Lluvias                            | La evaporación influye positivamente en la lluvia. Más evaporación significa más vapor de agua disponible para condensarse y caer como lluvia.<br>Tipo de Relación Causal: **Positiva (+)**                                                                |
| Lluvia y Corrientes de Agua                      | La lluvia influye positivamente en las corrientes de agua. Más lluvia significa más agua disponible para las corrientes.<br>Tipo de Relación Causal: **Positiva (+)**                                                                                      |
| Corrientes de Agua y Evaporación                 | La cantidad de agua en las corrientes de agua influye positivamente en la evaporación, aunque en menor medida que las Aguas Superficiales. Cuanto más agua en las corrientes de agua, más evaporación ocurre.<br>Tipo de Relación Causal: **Positiva (+)** |
| Corrientes de Agua y Aguas Superficiales         | Las corrientes de agua influyen positivamente en las aguas superficiales. Las corrientes finalmente desembocan en las aguas superficiales, aumentando su volumen.<br>Tipo de Relación Causal: **Positiva (+)**                                             |
| Lluvia y Almacenamiento de Agua en el Suelo      | La lluvia favorece que los suelos permeables absorban parte del agua<br>Tipo de Relación Causal: **Positiva (+)**                                                                                                                                          |
| Almacenamiento de Agua en el Suelo y Evaporación | El agua absorbida por el suelo, hace que la cantidad de agua evaporada disminuya<br>Tipo de Relación Causal: **Negativa (-)**                                                                                                                              |
### Diagrama de Flujo Causal
**Figura**
_Diagrama de Bucle Causal con Nueva Variable con Relaciones Causales Identificadas_
![Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable-1.png](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/Org1/2025/Clase%2004%20Din%C3%A1mica%20de%20Sistemas/000%20Adjuntos/Zk%20Diagrama%20de%20Bucle%20Causal%20(Ejemplo%20del%20Ciclo%20de%20Vida%20del%20Agua)%20V2%20con%20Nueva%20Variable-1.png)
Fuente: Elaboración propia.

----
### Identificación de Bucles
#### Bucle 1
**Relaciones**: Aguas Superficiales →+ Evaporación →+ Lluvia →+ Corrientes de Agua →+ Aguas Superficiales
**Tipo**: **Refuerzo (+)**, porque el número de relaciones negativas es cero (par).

**Figura**
_Bucle 1_
![Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable-2.png|200](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/Org1/2025/Clase%2004%20Din%C3%A1mica%20de%20Sistemas/000%20Adjuntos/Zk%20Diagrama%20de%20Bucle%20Causal%20(Ejemplo%20del%20Ciclo%20de%20Vida%20del%20Agua)%20V2%20con%20Nueva%20Variable-2.png)
Fuente: Elaboración Propia

----
#### Bucle 2
**Relaciones**: Aguas Superficiales →+ Evaporación →+ Lluvia →+ Corrientes de Agua →+ Evaporación
**Tipo**: **Refuerzo (+)**, porque el número de relaciones negativas es cero (par).

**Figura**
_Bucle 2_
![Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable-3.png|200](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/Org1/2025/Clase%2004%20Din%C3%A1mica%20de%20Sistemas/000%20Adjuntos/Zk%20Diagrama%20de%20Bucle%20Causal%20(Ejemplo%20del%20Ciclo%20de%20Vida%20del%20Agua)%20V2%20con%20Nueva%20Variable-3.png)
Fuente: Elaboración Propia

----
#### Bucle 3
**Relaciones**: Evaporación →+ Lluvia →+ Almacenamiento de Agua en el Suelo →- Evaporación
**Tipo**: **Refuerzo (-)**, porque el número de relaciones negativas es uno (impar).

**Figura**
_Bucle 3_
![Zk Diagrama de Bucle Causal (Ejemplo del Ciclo de Vida del Agua) V2 con Nueva Variable-4.png|200](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/Org1/2025/Clase%2004%20Din%C3%A1mica%20de%20Sistemas/000%20Adjuntos/Zk%20Diagrama%20de%20Bucle%20Causal%20(Ejemplo%20del%20Ciclo%20de%20Vida%20del%20Agua)%20V2%20con%20Nueva%20Variable-4.png)
Fuente: Elaboración Propia



### Análisis de la Estabilidad del Modelo
Para determinar si un modelo es estable o inestable en el contexto de un Diagrama de Bucle Causal, se analiza el comportamiento de los bucles presentes en el sistema. Un sistema es estable si tiende a regresar a un estado de equilibrio después de una perturbación, mientras que un sistema inestable se aleja del equilibrio.

La estabilidad del sistema depende de cómo interactúan los bucles entre sí.

En este caso, el bucle de equilibrio (Evaporación >+ Lluvia >+ Almacenamiento de Agua en el Suelo >- Evaporación) actúa como un mecanismo de retroalimentación negativa que ayuda a estabilizar el sistema. 

Cuando la evaporación aumenta, más agua se evapora, lo que eventualmente conduce a más lluvia, que a su vez aumenta el almacenamiento de agua en el suelo. A medida que el suelo se satura, la evaporación disminuye debido a la relación negativa entre el almacenamiento de agua en el suelo y la evaporación.

Por lo tanto, el modelo puede considerarse **estable** porque incluye un bucle de equilibrio que ayuda a mantener el sistema en un estado estable a pesar de las perturbaciones. Sin embargo, la estabilidad real dependerá de los parámetros específicos del sistema, como la intensidad de las relaciones y las condiciones iniciales.