# Propuesta TP DSW

## Grupo
### Integrantes
* 54913 Facundo, Campodonico
* 54284 Agustin, Kronemberger
* 54812 Sopo, Juan Esteban

### Repositorios
* [frontend app]([http://hyperlinkToGihubOrGitlab](https://github.com/FacuCampodonico/FrontEnd-Lution))
* [backend app]([http://hyperlinkToGihubOrGitlab](https://github.com/FacuCampodonico/BackEnd-Lution))


## Tema
### Descripción
Sistema de gestión para restaurante que permite administrar pedidos, mesas, empleados (mozos y administradores), productos con sus categorías e insumos, y pagos (efectivo o tarjeta). Incluye seguimiento de recetas y stock de insumos.

### Modelo
https://drive.google.com/file/d/1FjrYlUkRbaD9eWgYDLq-ql1AdkbXdvil/view?usp=sharing

## Alcance Funcional 

### Alcance Mínimo


Regularidad:
| Req | Detalle |
|-----|---------|
| CRUD simple | 1. CRUD Empleado<br>2. CRUD Mesa<br>3. CRUD Producto<br>4. CRUD Categoría<br>5. CRUD Insumos |
| CRUD dependiente | 1. CRUD Pedido (depende de Mozo y Mesa)<br>2. CRUD Pedidos-Producto (depende de Pedido y Producto)<br>3. CRUD Receta (depende de Producto e Insumos) |
| Listado + detalle | 1. Listado de empleados con datos básicos (nombre, rol, estado) + vista de detalle individual<br>2. Listado de mesas con estado (libre/ocupada) + detalle de pedidos asociados<br>3. Listado de productos con categoría y precio + detalle con insumos asociados<br>4. Listado de pedidos con estado + detalle completo (productos, cantidades, total, mesa, mozo)<br>5. Listado de insumos con stock + detalle de consumo por recetas |
| CUU/Epic | 1. Gestión de empleados<br>2. Gestión de mesas<br>3. Gestión de productos<br>4. Gestión de pedidos<br>5. Gestión de insumos |


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Admin {depende de} Empleado<br>2. CRUD Mesa<br>3. CRUD Pedido<br>4. CRUD Producto<br>5. CRUD Categoría<br>6. CRUD Pedidos-Producto {depende de} Pedido y Producto<br>7. CRUD Insumos<br>8. CRUD Receta {depende de} Producto e Insumos<br>9. CRUD Pago<br>10. CRUD Tarjeta {depende de} Pago<br>11. CRUD Efectivo {depende de} Pago<br>12. CRUD Pedido_Pago {depende de} Pedido y Pago|



### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
