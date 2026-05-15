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
| CRUD simple | 1. CRUD Empleado<br>2. CRUD Mesa<br>3. CRUD Producto |
| CRUD dependiente | 1. CRUD Pedido (depende de Empleado y Mesa)<br>2. CRUD Mesa-Producto (depende de Mesa y Producto) |
| Listado + detalle | 1. Listado de empleados con datos básicos (nombre, rol, estado) + vista de detalle individual<br>2. Listado de mesas con estado (libre/ocupada) + detalle de pedidos asociados |
| CUU/Epic | 1. Gestión de mesas<br>2. Gestión de empleados|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Admin {depende de} Empleado<br>2. CRUD Mesa<br>3. CRUD Producto<br>4. CRUD Mesa-Producto {depende de} Mesa y Producto<br>5. CRUD Insumos<br>6. CRUD Receta {depende de} Producto e Insumos<br>7. CRUD Pago<br>8. CRUD Tarjeta {depende de} Pago<br>9. CRUD Efectivo {depende de} Pago<br>10. CRUD Pedido_Pago {depende de} Pedido y Pago|



### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
