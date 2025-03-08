---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/040 Teoría General de Sistemas (TGS)/Zk Diagrama de Bucle Causal - Relación Positiva/","tags":["definir"]}
---

## Relación Positiva

Un signo (+) significa que un **cambio** en la variable de **origen** provoca un **cambio** en el **mismo sentido** en la variable **destino**.

## Ejemplos
### Un Ejemplo Genérico
- Un **incremento** de A, produce un **incremento** de B
- Una **disminución** de A provoca una **disminución** de B
```plantuml
!pragma layout smetana
left to right direction
(A) --> (B) :+
```

### Un Ejemplo Práctico
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

## Para Tener en Cuenta
El signo (+) positivo no implica un efecto "bueno", simplemente describen el tipo de influencia entre las variables.
