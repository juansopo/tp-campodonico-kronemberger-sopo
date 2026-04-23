# Propuesta TP DSW

## Grupo
### Integrantes
* legajo - Apellido(s), Nombre(s)

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
*2 a 6 líneas describiendo el negocio (menos es más)*

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Empleado<br>2. CRUD Mesa<br>3. CRUD Producto<br>4. CRUD Categoría<br>5. CRUD Insumos
|CRUD dependiente|1. CRUD Mozo {depende de} Empleado<br>2. CRUD Admin {depende de} Empleado<br>3. CRUD Pedido {depende de} Mozo y Mesa<br>4. CRUD Pedidos-Producto {depende de} Pedido y Producto<br>5. CRUD Receta {depende de} Producto e Insumos|
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Empleado<br>2. CRUD Mozo {depende de} Empleado<br>3. CRUD Admin {depende de} Empleado<br>4. CRUD Mesa<br>5. CRUD Pedido<br>6. CRUD Producto<br>7. CRUD Categoría<br>8. CRUD Pedidos-Producto {depende de} Pedido y Producto<br>9. CRUD Insumos<br>10. CRUD Receta {depende de} Producto e Insumos<br>11. CRUD Pago<br>12. CRUD Tarjeta {depende de} Pago<br>13. CRUD Efectivo {depende de} Pago<br>14. CRUD Pedido_Pago {depende de} Pedido y Pago|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

