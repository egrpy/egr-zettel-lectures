---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/990 Varios/Zk When2Meet - Registrar Disponibilidad/","tags":["when2meet","reunión","planificación"]}
---

## Registrar Disponibilidad
1. Abrir el enlace del evento [URL]().
2. En la página del evento:
    - Ingrese su nombre en el campo **Your Name**.
    - No se requiere contraseña.
![Zk When2Meet EventAccess.png](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/990%20Varios/000%20Adjuntos/Zk%20When2Meet%20EventAccess.png)
3. Haga clic en ==Sign In==.
4. Una vez que haya ingresado, en el panel izquierdo (cuadrícula rosa):
    - Haga clic y arrastre para marcar sus horarios disponibles.
    - Las áreas seleccionadas cambiarán de color.
    - Es posible registrar rangos no contiguos.
![Zk When2Meet RegisterUserAvailability.png](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/990%20Varios/000%20Adjuntos/Zk%20When2Meet%20RegisterUserAvailability.png)

5. Para desmarcar, haga clic nuevamente sobre las áreas seleccionadas.
6. Los cambios se guardan automáticamente.
## Versión Gráfica
```plantuml
@startuml
!pragma layout smetana
skinparam defaultTextAlignment center
Title Registrar Disponibilidad
start
:Acceder a Enlace del Evento;
:Ingresar su Nombre (Your Name)\n(No se requiere password);
:Pulsar Sign In;

:Marcar Horarios Disponibles\n(En el Panel Izquierdo);
:Salir\nLos datos se gran automáticamente;
stop
@enduml
```

