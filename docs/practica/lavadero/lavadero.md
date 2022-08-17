# Lavadero

## Planteo
Un servicio de lavado rápido realiza distintos tipos de servicio (referidos a distintas formas de lavado: lavado a seco, con máquina lavadora, etc.) a las prendas que habitualmente traen sus clientes.
Cuando un cliente llega, se le toman sus datos personales: apellido y nombre del cliente, domicilio (calle, nro, dpto y piso), barrio y teléfono. A continuación, se le informa los precios y fecha posible de entrega de acuerdo con el tipo de servicio requerido y la/s prenda/s que va a dejar.
Una vez que el cliente, está de acuerdo con el servicio se genera un número de pedido, y se registra la fecha de pedido, el tipo de prenda, tipo de servicio para esa prenda, la cantidad de prendas que deja por cada tipo de servicio, y se le informa al cliente el precio unitario, y el precio total de lo pedido. Un cliente puede requerir en un mismo pedido distintos servicios para cada prenda, por lo cual, al momento de la programación de lavado se controla el servicio solicitado y actualiza el estado del pedido. En general un tipo de servicio puede aplicarse a cualquier tipo de prenda.
Todos los días se emite un listado de los pedidos atendidos para llevar un control de caja y se emite un listado de insumos faltantes para poder cumplir con la demanda de los clientes respetando las fechas de entrega acordadas.

## A resolver
1. Definir Objetivo del Sistema de información.
2. Definir el límite del Sistema de información.
3. Definir el alcance del Sistema de información y organizarlo mediante subsistemas (Req. Globales.)

## Solución
### 1 - Objectivo del Sistema de Información
Brindar información para gestionar clientes, gestionar pedidos, gestionar servicios y gestionar insumos con el fin de facilitar la toma de decisiones sobre la gestión de insumos y el control de caja.

### 2 - Límite del Sistema de información
**Desde** que se registra un cliente
**Hasta** que se emiten los listados de pedidos e insumos faltantes

### 3 - Alcance del Sistema de información

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

