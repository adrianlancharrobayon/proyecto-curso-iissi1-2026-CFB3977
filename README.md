# Tienda de videojuegos digitales

## Miembros del grupo L6-XXX-X (sustituir)

1. Lancharro Bayón, Adrián
2. Ortega Moyano, Guillermo
3. Arroyo Sánchez, Jesús
4. Garrido Enríquez, Juan Luis

## 1. Introducción al problema

- Descripción del problema para poner en contexto el proyecto, incluyendo información sobre los clientes y usuarios, la situación actual, problemas, expectativas, etc. Se valorará la presencia de información multimedia (fotos, gráficos, documentos escaneados, etc.).

En una época en la que el formato físico está perdiendo fuerza frente al digital, hemos decidido crear una página en la cual la venta de videojuegos online sea lo más sencilla posible y así facilitar a nuestros usuarios la compra de videojuegos.

Vamos a crear una plataforma de venta de videojuegos digitales segura y de confianza que permita a los usuarios adquirir sus juegos en el momento, para diferentes plataformas y a unos precios competitivos. Tendremos un sistema de reseñas mediante el cual los usuarios de esta página que ya los hayan probado puedan valorarlos, y así, recomendarlos a otros usuarios. Además, aplicaremos descuentos en épocas de alta demanda (Navidad, Black Friday, ofertas de verano...). Nuestra plataforma permitirá al usuario realizar una compra segura, generando una factura de venta que justifique correctamente cualquier reembolso posterior. Queremos que a cada usuario se le recomienden los juegos según sus géneros preferidos en base a los datos que recojamos.

Esperamos que la plataforma crezca en usuarios y ofrecer a nuestro público no solo comprar sus juegos favoritos y deseados al momento, sino también conocer nuevos títulos relacionados que puedan satisfacer aún más horas de entretenimiento. Además, queremos ofrecer un servicio de suscripción anual, a un precio de 100€, donde los clientes obtendrán distintas ventajas.

## 2. Glosario de términos

- PVP: Precio de Venta al Público
- DLC: Contenido Descargable (Downloadable Content en inglés). Se trata de contenido adicional para un videojuego que se publica por internet después del lanzamiento del juego principal.
- PEGI: Información Paneuropea de Juegos (Pan European Game Information, en inglés). Es el sistema europeo de clasificación por edades y contenidos para videojuegos y software de entretenimiento

## 3. Visión general del sistema

### 3.1. Requisitos generales

#### R.G.01 Gestión de usuarios
Como administrador del sistema

quiero poder gestionar los usuarios

para tener un control de la plataforma

#### R.G.02 Gestión de devoluciones
Como administrador del sistema

quiero poder gestionar las devoluciones

para evitar posibles estafas

#### R.G.03 Gestión de pedidos
Como cliente

quiero poder gestionar mis pedidos

para revisar mis compras

#### R.G.04 Gestión de productos
Como administrador del sistema 

quiero gestionar los productos

para tener un catálogo actualizado.

#### R.G.05 Gestión de suscripciones
Como cliente

quiero poder gestionar mis suscripciones

para poder cancelarlas o activarlas cuando quiera

### 3.2. Usuarios del sistema
- Cliente
- Administrador del sistema

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01.1 Listado de usuarios
Como administrador del sistema 

quiero poder acceder a un listado de usuarios ordenados mensualmente

para saber las altas y las bajas de este mes.
 
**Prueba de aceptación**
- Al acceder como Administrador, en el menú lateral debe existir un botón llamado "Gestión de Usuarios". Al pulsarlo, debe cargar una pantalla con una tabla de datos que muestre las columnas: email y contraseña.
- Debe existir un menú desplegable (filtro) llamado "Filtrar por mes". Al seleccionar un mes (ej. Diciembre), la tabla debe actualizarse automáticamente para mostrar solo las altas y bajas de ese mes.

#### R.F.01.2 Creación de usuarios
Como administrador del sistema

quiero poder añadir y crear nuevos usuarios

para que queden registrados en el listado.

**Prueba de aceptación**
- Debe haber un botón llamado "Añadir Nuevo Usuario". Al pulsarlo, se debe abrir una ventana emergente pidiendo: email y contraseña. Al rellenar los datos y pulsar el botón "Guardar", debe aparecer una notificación verde indicando "Usuario creado con éxito". 

#### R.F.01.3 Edición de usuarios
Como administración del sistema 

quiero poder editar un usuario

para tener actualizados sus datos personales.

**Prueba de aceptación**
- En cada fila de la tabla del listado de usuarios, debe haber un botón(Editar). Al pulsarlo, se abrirá el mismo formulario de creación, pero con los datos actuales del usuario ya precargados.
- Al modificar cualquier campo (por ejemplo, cambiar el correo) y pulsar en el botón "Actualizar", la ventana se cerrará, la tabla se refrescará mostrando el nuevo dato y saldrá un aviso: "Usuario actualizado correctamente".

#### R.F.01.4 Borrado de usuarios
Como administración del sistema

quiero poder eliminar usuarios

para que desaparezcan del listado.

**Prueba de aceptación**
- En la tabla de usuarios, junto al botón de editar, debe haber un botón (Eliminar). Al pulsarlo, aparecerá una ventana emergente de confirmación con el texto: "¿Estás seguro de que deseas eliminar a este usuario permanentemente?" con dos botones: "Cancelar" y "Sí, eliminar".
- Al pulsar "Sí, eliminar", la ventana se cierra, el usuario desaparece de la tabla y se muestra un mensaje de confirmación "Usuario eliminado".

#### R.F.02.1 Listado de devoluciones
Como administrador del sistema 

quiero tener un listado de devoluciones mensuales

para poder gestionar las devoluciones del mes.

**Prueba de aceptación**
- El Administrador tendrá una pestaña en su panel de control llamada "Devoluciones". Al hacer clic, se mostrará una tabla con: cliente,pedido,motivo,validez y fecha. 

#### R.F.02.2 Creación de devoluciones
Como administrador del sistema

quiero añadir las nuevas devoluciones

para que queden registradas en el listado.

**Prueba de aceptación**
- En el panel del Cliente, dentro de sus pedidos, habrá un botón "Solicitar Devolución". Al pulsarlo, aparecerá un formulario donde el cliente debe escribir el motivo y adjuntar capturas si es necesario. Al pulsar "Enviar Solicitud", el estado del pedido pasará a "Devolución Pendiente".
- El Administrador, desde su panel de devoluciones, verá aparecer esta nueva solicitud automáticamente en el listado para poder gestionarla.

#### R.F.02.3 Edición de devoluciones
Como administrador del sistema

quiero poder gestionar las devoluciones

para tener actualizado el listado.

**Prueba de aceptación**
- El Administrador, al entrar en una devolución de la lista (botón "Gestionar"), verá la pantalla de detalles de la devolución. Aquí habrá un menú desplegable para cambiar el estado a "Aprobada" o "Rechazada".
- Al seleccionar "Aprobada" y hacer clic en el botón "Guardar cambios", el sistema debe generar automáticamente el reembolso al cliente y enviar un correo electrónico de confirmación de devolución.

#### R.F.02.4 Borrado de devoluciones
Como administrador del sistema

quiero borrar las devoluciones no efectuadas

para que no aparezca en el listado.

**Prueba de aceptación**
- Para las devoluciones marcadas como "Rechazadas" o canceladas por el cliente, el Administrador tendrá un botón de "Eliminar registro".
- Al pulsarlo, saltará una confirmación "¿Desea borrar este registro de devolución?". Al aceptar, la fila desaparecerá del listado principal para limpiar la vista.

#### R.F.03.1 Listado de pedidos
Como cliente

quiero poder acceder a mi lista de pedidos

para poder gestionar mis compras.
 

**Prueba de aceptación**
- El Cliente tendrá un icono de perfil en la cabecera de la web. Al desplegarlo y pulsar en "Mis Pedidos", se abrirá una pantalla con el historial de compras(pedidos) mostrando productos,importe,cantidad y fecha.
- Si el cliente nunca ha comprado nada, en lugar de la tabla debe aparecer un mensaje: "Aún no tienes pedidos" y un botón grande que diga "Ir a la tienda".


#### R.F.03.2 Creación de pedidos
Como cliente 

quiero poder crear un pedido

para hacer una compra.

**Prueba de aceptación**
- En el Carrito de compra, al pulsar el botón "Finalizar Compra", el usuario pasará a una pantalla de pasarela de pago. Tras introducir sus datos y pulsar "Pagar", si el pago es correcto, será redirigido a una pantalla de "¡Gracias por tu compra!" y se generará la factura.
- Se deben aplicar las reglas de negocio R.N.01. Si el carrito incluye un juego PEGI 18 y la fecha de nacimiento del cliente indica que es menor de edad, el botón "Pagar" se desactivará y saldrá un aviso: "No tienes edad suficiente para comprar uno de los artículos".

#### R.F.03.3 Edición de pedidos
Como cliente 

quiero poder editar mis pedidos

para gestionar mis compras.

**Prueba de aceptación**
- Si el pedido está en estado "Procesando" (antes de entregar la clave digital), el cliente puede entrar al detalle del pedido y pulsar un botón "Modificar método de pago" si el pago anterior falló.
- Si la clave del juego ya ha sido entregada, los botones de edición deben desaparecer de la pantalla del cliente, dejando solo la opción de solicitar devolución.

#### R.F.03.4 Borrado de pedidos
Como cliente

quiero poder borrar mis pedidos

para gestionar mis compras.

**Prueba de aceptación**
- Al borrar un pedido tras confirmar la acción, este desaparece de la lista del cliente.
- Si se cancela la confirmación, el pedido permanece en la lista sin cambios.
- Un cliente no puede borrar pedidos de otros clientes.

#### R.F.04.1 Listado de productos
Como administrador del sistema

quiero acceder al listado de productos disponibles

para ofrecerlos en la plataforma.

**Prueba de aceptación**
- El Administrador entra en la pestaña "Catálogo de Videojuegos". Verá una vista de cuadrícula/tabla con PEGI, tipo producto, nombre, precio,género y plataforma. 
- Debe haber una barra de búsqueda en la parte superior para encontrar juegos rápidamente escribiendo su título.

#### R.F.04.2 Creación de productos
Como administrador del sistema

quiero poder subir productos nuevos que ofrezcamos

para tener nuestra plataforma actualizada.

**Prueba de aceptación**
- Botón "Añadir Nuevo Juego". Abre una pantalla con un formulario detallado para subir nombre, precio, stock, etc. Al pulsar "Publicar", el juego aparece instantáneamente en la tienda del cliente.
- Se deben aplicar las reglas de negocio R.N.02.Si el administrador intenta poner un precio de venta menor  o igual a cero, el sistema bloqueará el guardado indicando: "El PVP no puede generar pérdidas".

#### R.F.04.3 Edición de productos
Como administrador del sistema

quiero poder asignarle un género y un tipo de producto a los productos

para que los usuarios los encuentren fácilmente.

**Prueba de aceptación**
- En el catálogo del administrador, al pulsar sobre un juego, se abrirá su ficha editable. Debe haber un desplegable para "Género" (Acción, RPG, Deportes) y otro para "Plataforma" (PC, PS5, Xbox).
- Al modificar el precio para hacer una rebaja y pulsar "Guardar", el cambio debe verse reflejado inmediatamente en la página principal (tienda) de los usuarios, mostrando el precio anterior tachado.

#### R.F.04.4 Borrado de productos
Como administrador del sistema

quiero poder eliminar productos que ya no ofrezcamos

para evitar confusiones en los usuarios.

**Prueba de aceptación**
- Botón de "Dar de baja producto" en la ficha del administrador. Al pulsarlo, pide confirmación. 
- Tras confirmar, el juego ya no debe aparecer en la barra de búsqueda ni en el catálogo de los clientes.

#### R.F.05.1 Listado de suscripciones
Como cliente

quiero acceder a mi listado de suscripciones activas y disponibles

para satisfacer mis necesidades.
 
**Prueba de aceptación**
- En el panel del Cliente habrá una sección "Mi Suscripción". Al entrar, debe mostrar una tarjeta con el estado actual ("Activa" / "Inactiva") y la fecha de la próxima renovación. 
- Si no está suscrito, se le mostrará una pantalla de ventas detallando los beneficios de ser suscriptor.

#### R.F.05.2 Creación de suscripciones
Como cliente

quiero poder suscribirme a la plataforma

para aprovechar sus ventajas.

**Prueba de aceptación**
- En la pantalla de beneficios, habrá un botón grande y llamativo que diga "Suscribirse ahora por 100€/año".
- Al pulsarlo, llevará a una pasarela de pago seguro. Una vez completado se le desbloquearán los descuentos disponibles de forma automática en la tienda.

#### R.F.05.3 Edición de suscripciones
Como cliente

quiero poder modificar mi plan de suscripción

para satisfacer mis necesidades.

**Prueba de aceptación**
- Dentro de "Mi Suscripción", debe existir un botón de "Gestionar Método de Pago". Al pulsarlo, debe permitir cambiar la tarjeta de crédito asociada a la suscripción. 
- Al guardar la nueva tarjeta, el sistema debe confirmar que los próximos cobros anuales se realizarán en ese nuevo método. 

#### R.F.05.4 Borrado de suscripciones
Como cliente

quiero poder cancelar mi plan de suscripción en cualquier momento

para dejar de tener acceso a los servicios que ofrece una vez ya no los considere necesarios.

**Prueba de aceptación**
- En la parte inferior de la pantalla "Mi Suscripción", debe haber un botón sutil que diga "Cancelar mi suscripción". Al pulsarlo, debe salir una pantalla intentando retener al usuario mostrando lo que se va a perder. 
- Si el usuario pulsa en "Sí, cancelar de todas formas", el estado pasará a "Cancelada", pero la pantalla debe indicarle claramente que podrá seguir disfrutando de sus beneficios hasta que termine el periodo anual que ya pagó.

#### 4.1.1. Requisitos de información

##### R.I.01. Información de usuario
Como administrador del sistema

quiero la siguiente información sobre usuarios:

Nombre y apellidos, ID, edad.

Un usuario está asociado a varios pedidos.
Un usuario puede estar asociado a una suscripción. 
Un usuario está asociado a varias devoluciones.

**Prueba de aceptación**
- Al consultar un usuario, el sistema muestra nombre y apellidos, ID y edad.
- El ID de cada usuario es único y no se repite entre usuarios.
- Un usuario puede tener varios pedidos asociados y varias devoluciones asociadas.
- Un usuario puede tener como máximo una suscripción asociada.
- La edad debe ser un número entero positivo. 

#### R.I.02. Información de devoluciones
Como administrador del sistema
		
quiero la siguiente información sobre devoluciones:

Motivo, fecha, validez.

Una devolución está asociada a un pedido.

**Prueba de aceptación**
- Al consultar una devolución, el sistema muestra motivo, fecha y validez.
- Toda devolución está asociada a un único pedido; no puede existir una devolución sin pedido.
- La validez de la devolución es coherente con la fecha de compra del pedido: no es válida si han pasado más de 7 días. Se aplica la regla de negocio R.N.03.

##### R.I.03. Información de pedidos
Como cliente

quiero la siguiente información sobre pedidos:

Importe total, cantidad, fecha.

N pedidos están asociados a m productos
**Prueba de aceptación**
- Al consultar un pedido, el sistema muestra importe total, cantidad y fecha.
- El importe total es siempre mayor que 0. Se aplica la regla de negocio R.N.02.
- Un pedido puede incluir varios productos, y un mismo producto puede aparecer en varios pedidos.
- El importe total coincide con la suma de los precios de los productos del pedido por su cantidad.

##### R.I.04. Información de productos
Como cliente

quiero la siguiente información sobre productos:

Precio, PEGI, tipo, género, nombre, plataforma.

**Prueba de aceptación**
- Al consultar un producto, el sistema muestra precio, PEGI, tipo, género, nombre y plataforma.
- El precio es un valor numérico mayor que 0 expresado en euros.
- El PEGI es uno de los valores admitidos (3, 7, 12, 16 o 18) y se usa para aplicar la restricción de edad. Se aplica la regla de negocio R.N.01.

##### R.I.05. Información de suscripciones
Como cliente

quiero la siguiente información sobre suscripciones:

Precio, fecha de inicio, fecha de fin.

**Prueba de aceptación**
- Al consultar una suscripción, el sistema muestra precio, fecha de inicio y fecha de fin.
- La fecha de fin no es anterior a la fecha de inicio. Se aplica la regla de negocio R.N.05.
- Una suscripción pertenece a un único usuario.

#### 4.1.2. Reglas de negocio
##### R.N.01. Restricción de edad
Los juegos PEGI 18 no podrán ser vendidos a menores de edad.

##### R.N.02. Restricción de importe
El importe de un pedido no puede ser menor o igual a 0.

##### R.N.03. Restricción de devolución
No se puede devolver un producto tras 7 días de su compra.

##### R.N.04. Restricción de contraseña
La contraseña de un usuario debe tener al menos 8 caracteres.

##### R.N.05. Restricción de suscripción
La fecha de fin de suscripción no puede ser anterior a la fecha de inicio.

### 4.2. Mapa de historias de usuario (opcional)

### 4.3. Requisitos no funcionales (opcional)

**R.N.F. 01. Título requisito no funcional**
Como [tipo de usuario]
quiero [servicio]
para [razón]

-- fin entregable 1 --

## 5. Modelo conceptual

### 5.1. Diagramas de clases UML

- con restricciones.

### 5.2. Escenarios de prueba

- con descripción textual y diagrama de objetos UML.

## 6. Matrices de trazabilidad

- Matriz de trazabilidad entre los elementos del modelo conceptual y los requisitos.

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:------|:-----------|:-----------|:-----------|:-----------|
| RI-1  | X          | X          | X          | X          |
| RI-2  |            | X          |            | X          |
| RF-1  |            | X          |            | X          |
| RF-2  | X          |            | X          | X          |
| RN-1  |            | X          |            |            |
| RN-2  | X          | X          | X          |            |
| ...   |            |            |            |            |

-- fin entregable 2 --

## 7. Modelo relacional en 3FN

- Relaciones obtenidas al aplicar la transformación del modelo conceptual.

### 7.1.  Justificación de la estrategia de transformación de jerarquías

- si se identificaron jerarquías en el MC.


### 8. Matriz de trazabilidad MC/SQL (opcional):

- Restricciones sobre el MC / Elementos del modelo tecnológico (SQL) (Triggers, checks, etc.)
- Incluir Reglas de negocio — Constraints/Triggers en las matrices de trazabilidad para el entregable 3

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:-------|:-------|:-------|:-------|:-------|
| TABLA-1 |        |        |        |        |
| TABLA-2 |        |        |        |        |
| TABLA-3 |        |        |        |        |
| TABLA-4 |        |        |        |        |
| TRIG-1 |        |        |        |        |
| TRIG-2 | X      | X      |        | X      |
| TRIG-3 |        | X      |        | X      |
| TRIG-4 |        |        | X      |        |
| CONST-1 |        |        |        |        |
| CONST-2 | X      | X      |        | X      |
| CONST-3 |        | X      |        | X      |
| CONST-4 |        |        | X      |        |

Se consideran todo tipo de constraints declarativas (aquellas definidas durante el CREATE TABLE).
-- fin entregable 3 --

## Referencias







