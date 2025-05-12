# Propuesta TP DSW

## Grupo
### Integrantes
* 44004 - Ruiz, Juan Pablo
* 51408 - Sanchez Machado,Tomás
* legajo - Apellido(s), Facundo

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
Sistema de gestión para un local de comida rápida que permitirá a los clientes consultar productos, realizar pedidos, efectuar pagos y dejar reseñas. A su vez, el sistema brindará herramientas al personal administrativo para gestionar productos, ingredientes, promociones, proveedores y pedidos en tiempo real. El objetivo es optimizar la experiencia del cliente y facilitar la operación interna del local.

### Modelo
!https://drive.google.com/file/d/1IKAVBwg-HUcDQRirVyASKb3dZpRd-MN6/view?usp=sharing

## Alcance Funcional 

|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Proveedor<br>3. CRUD Ingrediente<br>4. CRUD Producto<br>5. CRUD Promocion|
|CRUD dependiente|1. CRUD Pedido {depende de} CRUD Usuario<br>2. CRUD Pago {depende de} CRUD Pedido<br>3. CRUD Linea_Pedido {depende de} CRUD Pedido y CRUD Poducto<br>4. CRUD Producto_Ingrediente {depende de} CRUD Producto y CRUD Ingrediente => detalle CRUD PRODUCTO
|Listado<br>+<br>detalle| 1. Listado de productos, muestra Nombre, descripción, precio y promociones aplicables? => detalle CRUD Habitacion<br> 2. Listado de promociones mostrando descripción, productos incluidos, fecha de validez, precio con descuento => detalle muestra datos completos de la PROMOCION<br> 3. Listado de reseñas filtrado por producto mostrando nombre del producto, calificación, comentario => detalle muestra datos completos de la entidad RESEÑA|
|CUU/Epic|1. Registrar reseña del USUARIO respecto a un producto<br>2. Registrar pago de un PEDIDO<br>3. Registrar un nuevo USUARIO<br>4. Validar un USUARIO<br>5. Notificar por mail un PEDIDO|
