---
{"dg-publish":true,"permalink":"/050 Base de Conocimientos/200  Mi Zettelkasten/100 Docencia/IS1/2025/Clase 16 Diagrama de Estados/Zk Diagrama de Estados (Ejercicios y Ejemplos)/","tags":["digitalGarden"]}
---

## Diagrama de Estados (Ejemplos)

**Figura**
_Estados de una Factura en un CRM_
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 0.8

[*] -> Facturada
Facturada :exit/ Factura cargada en sistema
Facturada -> Anulada :Factura Anulada [error]
Facturada -> Impresa :Factura Registrada [Ok]
Impresa -> PreparandoEntrega : Impresión completada
PreparandoEntrega --> EnReparto :Mercaderías Listas
EnReparto -> Entregada :Entrega Total
Entregada -> PreparandoEntrega :Entrega Incompleta
Entregada --> Cobrada :Cliente Conforme
Cobrada --> [*] :Pago Recibido
Anulada --> [*]

@enduml
```
_Nota_: Cada sistema CRM puede tener estados de facturas específicos, es es solo en ejemplo ilustrativo.

Figura
_Estados de un Teléfono Celular para lLamadas Salientes_
![Zk Diagrama de Estados (Ejercicios y Ejemplos).png|400](/img/user/050%20Base%20de%20Conocimientos/200%20%20Mi%20Zettelkasten/100%20Docencia/IS1/2025/Clase%2016%20Diagrama%20de%20Estados/000%20Adjuntos/Zk%20Diagrama%20de%20Estados%20(Ejercicios%20y%20Ejemplos).png)

**Figura**
_Estados de un Pedido en un CRM_
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 1

[*] -> Esperando_pedido : Pedido recibido

Esperando_pedido --> Verificando_inventario : Inventario suficiente / Inventario insuficiente\n{evento = Pedido en espera,\nguarda = Verificar inventario}

Verificando_inventario --> Autenticando_pago : Pago válido / Pago inválido\n{evento = Inventario verificado,\nguarda = Verificar pago}

Autenticando_pago --> Procesando_pedido : Pago confirmado / Pago inválido\n{evento = Pago autenticado,\nguarda = Pedido en proceso,\nacciones = Actualizar pago}

Procesando_pedido --> Enviando_confirmacion : Pedido procesado y enviado\n{evento = Pedido en camino,\nacciones = Enviar confirmación}

Enviando_confirmacion --> [*] : Confirmación recibida\n{evento = Confirmación recibida}

Verificando_inventario --> Finalizando_pedido : Inventario insuficiente\n{guarda = Pedido cancelado,\nacciones = Cancelar pedido}
Finalizando_pedido --> [*] : Pedido finalizado\n{evento = Pedido finalizado}

Esperando_pedido --> Cancelando_pedido : Cancelar pedido\n{guarda = Pagado}
Cancelando_pedido --> [*] : Pedido cancelado\n{evento = Pedido cancelado}

@enduml
```
_Nota_: Cada sistema CRM puede tener estados de pedidos específicos, es es solo en ejemplo ilustrativo.

**Figura**
_Estados de un Ascensor_
```plantuml
!pragma layout smetana
skinparam style strictuml
skinparam BackgroundColor LightGray
skinparam conditionStyle InsideDiamond
scale 1

state Inactivo {
  [*] --> EsperandoLlamada
  EsperandoLlamada --> Movimiento : LlamadaRecibida\n{efecto = EncenderLuz,\nguarda = NoEstoyEnPisoDestino}
  EsperandoLlamada --> Detenido : LlamadaRecibida\n{efecto = EncenderLuz,\nguarda = EstoyEnPisoDestino}
  Movimiento --> Detenido : AlcanzadoDestino\n{efecto = ApagarMotor}
  Detenido --> EsperandoLlamada : NoHayLlamadas\n{efecto = ApagarLuz}
}

state Movimiento {
  [*] --> Subiendo
  Subiendo :entry/ MostrarPisoActual
  Subiendo :do/ ActualizarPisoActual
  Subiendo :exit/ OcultarPisoActual
  Subiendo --> Subiendo : EnMovimiento\n{guarda = NoEstoyEnPisoDestino}
  Subiendo --> DeteniendoSubida : EnMovimiento\n{guarda = EstoyEnPisoDestino}
  DeteniendoSubida :entry/ FrenarMotor
  DeteniendoSubida :do/ MostrarPisoActual
  DeteniendoSubida :exit/ ApagarMotor
}

state Detenido {
  [*] --> PuertasCerradas
  PuertasCerradas :entry/ IniciarTemporizador
  PuertasCerradas :do/ MostrarTiempoEspera
  PuertasCerradas :exit/ DetenerTemporizador
  PuertasCerradas --> AbriendoPuertas : AbrirPuertas\n{efecto = EncenderLucesInternas,\nguarda = HayPasajeros}
  AbriendoPuertas --> PuertasAbiertas : PuertasAbiertas\n{efecto = DetenerTimbre,\nguarda = PuertasTotalmenteAbiertas}
  PuertasAbiertas :entry/ AbrirPuertas
  PuertasAbiertas :do/ MostrarMensajePuertasAbiertas
  PuertasAbiertas :exit/ DetenerTimbre
  PuertasAbiertas --> CerrandoPuertas : CerrarPuertas\n{efecto = ApagarLucesInternas,\nguarda = NoHayPasajeros}
  CerrandoPuertas :entry/ CerrarPuertas
  CerrandoPuertas :do/ MostrarMensajeCerrandoPuertas
  CerrandoPuertas :exit/ IniciarTemporizador
}

Inactivo --> [*]
@enduml
```
_Nota_: Ejemplo meramente ilustrativo

