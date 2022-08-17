# El Algarrobo
 
## Planteo
La empresa El Algarrobo S.A. se dedica a la comercialización de muebles.
Realiza ventas al por mayor como así también al público en general. El proceso comienza con el ingreso de un cliente al local, el cual es atendido por un vendedor. Una vez que el cliente recorrió el salón, realiza el pedido al vendedor, quien se encarga de ver si el producto solicitado se encuentra en stock o en catálogo, si es así, obtiene su precio y confecciona la Factura por la venta y solicita al cliente que se dirija hacia la caja para efectuar el pago. En la caja, se gestiona la forma de pago en efectivo o con tarjeta de crédito y se le entrega la factura al cliente. Este se dirige con las mismas al salón de empaque donde el empaquetador controla el sello de pagado en la factura, y verifica lo que figura en la factura para organizar la entrega y traslado de los productos hacia la salida del local.
 
## A resolver
1. Objetivo del sistema de negocio.
2. Alcance del sistema de negocio.
3. Modelar un proceso del negocio.
4. Modelar el organigrama de la empresa (Extra) :bangbang:
 
## Solución
### 1 - Objetivo del Negocio
El objetivo de El Algarrobo S.A. es la comercialización de muebles al por mayor y menor.
 
### 2 - Alcance del Negocio
 - Seleccionar Proveedor
 - Realizar pedido a proveedor
 - Pagar a proveedor
 - Recibir mercadería del proveedor
 - Controlar mercadería recibida del proveedor
 - Atender consultas de clientes
 - Consultar stock disponible
 - Consultar precios de productos
 - Confeccionar factura del pedido del cliente
 - Consultar medios de pago disponibles
 - Informar medios de pago disponibles
 - Cobrar compra
 - Facturar compra
 - Entregar factura sellada
 - Recibir pedido de empaque
 - Controlar pago de factura
 - Organizar entrega del pedido
 - Despachar pedido
 
 
### 3 - Procesos
#### Compra
 
![alt text](./diagrams/compras-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Venta
 
![alt text](./diagrams/venta-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Facturación y Cobranza
 
![alt text](./diagrams/facturacionCobranza-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Empaque
 
![alt text](./diagrams/empaque-svg.svg ':class=diagramsCssClass :size=100%')
 
### 4 - Organigrama
 
```plantuml
@startuml
[[!include ./practica/el_algarrobo/diagrams/organigrama.puml]]
@enduml
```