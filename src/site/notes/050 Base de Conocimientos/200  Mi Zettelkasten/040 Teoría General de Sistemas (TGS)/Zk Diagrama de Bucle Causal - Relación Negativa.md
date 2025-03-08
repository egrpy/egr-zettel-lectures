---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Diagrama de Bucle Causal - Relación Negativa/","tags":["definir"]}
---

## Relación Negativa

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

## Para Tener en Cuenta
El signo (-) negativo no implica un efecto "malo", simplemente describen el tipo de influencia entre las variables.

## Enlaces
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Dinámica de Sistemas\|Zk Dinámica de Sistemas]]
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Diagrama de Bucle Causal\|Zk Diagrama de Bucle Causal]]
[[050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Bucles de Retroalimentación en Diagrama Causal\|Zk Bucles de Retroalimentación en Diagrama Causal]]