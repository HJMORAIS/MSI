# Práctica MSI

# Sistemas de Negocio

## El Algarrobo
 
### Planteo
La empresa El Algarrobo S.A. se dedica a la comercialización de muebles.
Realiza ventas al por mayor como así también al público en general. El proceso comienza con el ingreso de un cliente al local, el cual es atendido por un vendedor. Una vez que el cliente recorrió el salón, realiza el pedido al vendedor, quien se encarga de ver si el producto solicitado se encuentra en stock o en catálogo, si es así, obtiene su precio y confecciona la Factura por la venta y solicita al cliente que se dirija hacia la caja para efectuar el pago. En la caja, se gestiona la forma de pago en efectivo o con tarjeta de crédito y se le entrega la factura al cliente. Este se dirige con las mismas al salón de empaque donde el empaquetador controla el sello de pagado en la factura, y verifica lo que figura en la factura para organizar la entrega y traslado de los productos hacia la salida del local.
 
### A resolver
1. Objetivo del sistema de negocio.
2. Alcance del sistema de negocio.
3. Modelar un proceso del negocio.
4. Modelar el organigrama de la empresa (Extra) :bangbang:
 
### Solución
#### 1 - Objetivo del Negocio
El objetivo de El Algarrobo S.A. es la comercialización de muebles al por mayor y menor.
 
#### 2 - Alcance del Negocio
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
 
 
#### 3 - Procesos
#### Compra
 
![alt text](./diagrams/compras-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Venta
 
![alt text](./diagrams/venta-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Facturación y Cobranza
 
![alt text](./diagrams/facturacionCobranza-svg.svg ':class=diagramsCssClass :size=100%')
 
#### Empaque
 
![alt text](./diagrams/empaque-svg.svg ':class=diagramsCssClass :size=100%')
 
#### 4 - Organigrama
 
```plantuml
@startuml
[[!include ./practica/diagrams/organigrama.puml]]
@enduml
```

# Sistemas de Información

## Lavadero

### Planteo
Un servicio de lavado rápido realiza distintos tipos de servicio (referidos a distintas formas de lavado: lavado a seco, con máquina lavadora, etc.) a las prendas que habitualmente traen sus clientes.
Cuando un cliente llega, se le toman sus datos personales: apellido y nombre del cliente, domicilio (calle, nro, dpto y piso), barrio y teléfono. A continuación, se le informa los precios y fecha posible de entrega de acuerdo con el tipo de servicio requerido y la/s prenda/s que va a dejar.
Una vez que el cliente, está de acuerdo con el servicio se genera un número de pedido, y se registra la fecha de pedido, el tipo de prenda, tipo de servicio para esa prenda, la cantidad de prendas que deja por cada tipo de servicio, y se le informa al cliente el precio unitario, y el precio total de lo pedido. Un cliente puede requerir en un mismo pedido distintos servicios para cada prenda, por lo cual, al momento de la programación de lavado se controla el servicio solicitado y actualiza el estado del pedido. En general un tipo de servicio puede aplicarse a cualquier tipo de prenda.
Todos los días se emite un listado de los pedidos atendidos para llevar un control de caja y se emite un listado de insumos faltantes para poder cumplir con la demanda de los clientes respetando las fechas de entrega acordadas.

### A resolver
1. Definir Objetivo del Sistema de información.
2. Definir el límite del Sistema de información.
3. Definir el alcance del Sistema de información y organizarlo mediante subsistemas (Req. Globales.)

### Solución
##### 1 - Objetivo del Sistema de Información
Brindar información para gestionar clientes, gestionar pedidos, gestionar servicios y gestionar insumos con el fin de facilitar la toma de decisiones sobre la gestión de insumos y el control de caja.

##### 2 - Límite del Sistema de información
**Desde** que se registra un cliente
**Hasta** que se emiten los listados de pedidos e insumos faltantes

##### 3 - Alcance del Sistema de información

**Gestión de Clientes**

- **Registrar** nuevo cliente
- **Eliminar** un cliente
- **Modificar** datos de un cliente
- **Consultar** información de clientes

**Gestión de Pedidos**

- **Registrar** nuevo pedido
- **Eliminar** un pedido
- **Modificar** datos de un pedido
- **Consultar** información de pedidos
- **Actualizar** estado de un pedido
- **Emitir** listado de pedidos

**Gestión de Servicios de Lavado**

- **Registrar** nuevo servicio
- **Eliminar** un servicio
- **Modificar** datos de un servicio
- **Consultar** información de servicios

**Gestión de Insumos**

- **Registrar** nuevo insumo
- **Eliminar** un insumo
- **Modificar** datos de un insumo
- **Consultar** información de insumos
- **Actualizar** stock de insumos
- **Emitir** listado de insumos faltantes

