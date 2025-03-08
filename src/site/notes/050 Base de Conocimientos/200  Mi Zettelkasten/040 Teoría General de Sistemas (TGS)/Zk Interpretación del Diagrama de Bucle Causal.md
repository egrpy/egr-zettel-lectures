---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Interpretación del Diagrama de Bucle Causal/","tags":["definir"]}
---

## Interpretación del Diagrama de Bucle Causal
Según [[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Dinámica de Sistemas#Referencia\|García (2020)]], en el diagrama causal, las flechas entre variables llevan un signo más "+" ó un signo menos "-" para indicar cómo una variable influye en otra.

----
### Relación Positiva{ #6ea4b5}


Un signo (+) significa que un **cambio** en la variable de **origen** provoca un **cambio** en el **mismo sentido** en la variable **destino**.
#### Ejemplo Genérico
- Un **incremento** de A, produce un **incremento** de B
- Una **disminución** de A provoca una **disminución** de B
```plantuml
!pragma layout smetana
left to right direction
(A) --> (B) :+
```

#### Ejemplos Prácticos
Cuando **aumenta la lluvia**, más agua cae en ríos, arroyos y lagos, esto provoca la **Acumulación de Agua**.
```plantuml
!pragma layout smetana
left to right direction
(Mucha Lluvia) --> (Mayor Acumulación de Agua) :+
```

Una **disminución de la Lluvia** provoca una **disminución** de la **Acumulación de Agua**.
```plantuml
!pragma layout smetana
left to right direction
(Poca Lluvia) --> (Disminuye la Acumulación de Agua) :+
```

----
### Relación Negativa{ #7acdee}


Un signo (-) indica que el **cambio** en la variable de **origen** causa un **cambio** en **sentido opuesto** en la variable **destino**.

#### Ejemplo Genérico
- Un **incremento** de A, produce una **disminución** de B
- Una **disminución** de A provoca un **aumento** de B
```plantuml
!pragma layout smetana
left to right direction
(A) --> (B) :-
```

#### Ejemplos Prácticos
Cuando **mejora** la **Alimentación** de una persona, **disminuye** la **Probabilidad de Enfermedades**.
```plantuml
!pragma layout smetana
left to right direction
(Mejor Alimentación) --> (Menor Probabilidad de Enfermedades) :-
```

Cuando **peor** es la **Alimentación** de una persona, **aumenta** la **Probabilidad de Enfermedades**.
```plantuml
!pragma layout smetana
left to right direction
(Peor Alimentación) --> (Mayor Probabilidad de Enfermedades) :-
```

Es importante resaltar que:
- El signo (+) positivo no implica un efecto "bueno" y que,
- El signo (-) negativo no implica un efecto "malo"
Simplemente describen el tipo de influencia entre las variables.

## Enlaces
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Dinámica de Sistemas\|Zk Dinámica de Sistemas]]
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Diagrama de Bucle Causal\|Zk Diagrama de Bucle Causal]]
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Bucles de Retroalimentación en Diagrama Causal\|Zk Bucles de Retroalimentación en Diagrama Causal]]