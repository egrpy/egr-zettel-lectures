---
{"dg-publish":true,"permalink":"/000 Bandeja de Entrada/Prueba MultiColum Plugin/"}
---

#pruebaConcepto

````col

```col-md

**Figura**
_Ejemplo Básico_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
skinparam linetype ortho
scale 1

' Elementos
actor Usuario

note over Usuario: Actor

participant ":Sistema" as Sistema
note over Sistema: Participante / Objeto

participant ":BaseDeDatos" as BaseDeDatos
note over BaseDeDatos: Participante / Objeto


' Mensaje directo
Usuario -> Sistema: Solicita datos()
note right: Mensaje

' Activación del sistema
activate Sistema
note right: Activación

' Consulta a base de datos
Sistema -> BaseDeDatos: Consulta datos()
activate BaseDeDatos

create Participant ":Objeto" as Objeto
BaseDeDatos -> Objeto :Calular()
Activate Objeto
Objeto --> BaseDeDatos
note right: Retorno
Deactivate Objeto
destroy Objeto
note right: Destrucción

deactivate BaseDeDatos

' Muestra datos al usuario
Sistema --> Usuario: Muestra datos()
deactivate Sistema
note right: Retorno

@enduml

```
Nota: Elaboración Propia, usando la herramienta [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Plantuml) Herramienta Para Crear Diagramas a Partir de Texto\|Plantuml]].

```

```col-md
line 1
line 2
```

````


--- start-multi-column: ExampleRegion1  
```column-settings  
number of columns: 2  
```

**Figura**
_Ejemplo Básico_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
skinparam linetype ortho
scale 1

' Elementos
actor Usuario

note over Usuario: Actor

participant ":Sistema" as Sistema
note over Sistema: Participante / Objeto

participant ":BaseDeDatos" as BaseDeDatos
note over BaseDeDatos: Participante / Objeto


' Mensaje directo
Usuario -> Sistema: Solicita datos()
note right: Mensaje

' Activación del sistema
activate Sistema
note right: Activación

' Consulta a base de datos
Sistema -> BaseDeDatos: Consulta datos()
activate BaseDeDatos

create Participant ":Objeto" as Objeto
BaseDeDatos -> Objeto :Calular()
Activate Objeto
Objeto --> BaseDeDatos
note right: Retorno
Deactivate Objeto
destroy Objeto
note right: Destrucción

deactivate BaseDeDatos

' Muestra datos al usuario
Sistema --> Usuario: Muestra datos()
deactivate Sistema
note right: Retorno

@enduml

```
Nota: Elaboración Propia, usando la herramienta [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Plantuml) Herramienta Para Crear Diagramas a Partir de Texto\|Plantuml]].

--- end-column ---

**Figura**
_Ejemplo Complejo_
```plantuml
@startuml
!pragma layout smetana
skinparam style strictuml
skinparam classAttributeIconSize 0
skinparam BackgroundColor LightGray
'left to right direction
'top to bottom direction
skinparam linetype ortho
scale 1

@startuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam linetype ortho

actor Usuario
actor Bibliotecario

rectangle ":GUIBuscarLibro" as GUIBuscarLibro
rectangle ":GUIRegistrarPréstamo" as GUIRegistrarPrestamo
rectangle ":libro" as Libro
rectangle ":prestamos" as Prestamos

' Disposición espacial para evitar cruces:
' Usuario y Bibliotecario arriba
' GUIBuscarLibro y GUIRegistrarPréstamo en el centro
' Libro y Prestamos abajo

Usuario --r-- Bibliotecario : 1: solicitar libro <&arrow-right>
Bibliotecario --d-- GUIBuscarLibro : 2: buscarLibro() <&arrow-bottom>
GUIBuscarLibro --r-- Libro : 3: verLibros() <&arrow-right>
Libro --l-- GUIBuscarLibro : 4: listaLibros <&arrow-left>
GUIBuscarLibro -u-- Bibliotecario : 5: mostrar listaLibros <&arrow-top>

' Alternativa: libro disponible
Bibliotecario --d-- GUIRegistrarPrestamo : 6: registrarPréstamo() <&arrow-bottom>
GUIRegistrarPrestamo -r- Prestamos : 7: registrarPréstamo() <&arrow-right>
Prestamos -l- GUIRegistrarPrestamo : 8: confirmarPréstamo() <&arrow-left>
GUIRegistrarPrestamo -u- Bibliotecario : 9: mostrar confirmación <&arrow-top>
Bibliotecario --l-- Usuario : 10: entregar libro físico <&arrow-left>

' Alternativa: libro no disponible
GUIBuscarLibro -u- Bibliotecario : 11: mostrar no disponible <&arrow-top>
Bibliotecario --l-- Usuario : 12: notificar no disponible <&arrow-left>

@enduml

```
Nota: Elaboración Propia, usando la herramienta [[050 Base de Conocimientos/900 Biblioteca/Zk Lit (Plantuml) Herramienta Para Crear Diagramas a Partir de Texto\|Plantuml]].

--- end-multi-column

