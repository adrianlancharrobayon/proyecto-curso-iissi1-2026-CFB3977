# Tienda de videojuegos digitales

## Miembros del grupo L6-XXX-X (sustituir)

1. Lancharro Bayón, Adrián
2. Ortega Moyano, Guillermo
3. Arroyo Sánchez, Jesús
4. Garrido Enríquez, Juan Luis

## 1. Introducción al problema

- Descripción del problema para poner en contexto el proyecto, incluyendo información sobre los clientes y usuarios, la situación actual, problemas, expectativas, etc. Se valorará la presencia de información multimedia (fotos, gráficos, documentos escaneados, etc.).

En una época en la que el formato físico está perdiendo fuerza tras los anuncios de Sony del previsible abandono de este formato en los años venideros, hemos creado una página en la cual la venta de videojuegos online sea lo más sencilla posible y así facilitar a nuestros usuarios la compra de videojuegos.

![alt text](<Captura de pantalla 2026-10-06 123922.png>)

Vamos a crear una plataforma de venta de videojuegos digitales segura y de confianza que permita a los usuarios adquirir sus juegos en el momento, para diferentes plataformas y a unos precios competitivos. 
Tendremos un sistema de reseñas mediante el cual los usuarios de esta página que ya los hayan probado puedan valorarlos, y así, recomendarlos a nuestros usuarios o rebajarlos en épocas de alta demanda (Navidad, Black Friday, ofertas de verano...).
Nuestra plataforma permitirá al usuario la adquisicion del producto segura, actualizando en el momento la disponibilidad en stock y generando una factura de venta para un posible reembolso justificado correctamente a futuro.
Queremos que a cada usuario se le recomienden los juegos según sus géneros preferidos en base a los datos que recojamos. 

Nuestras expectativas son positivas a futuro, queriendo poder ofrecer a nuestro público no solo comprar sus juegos favoritos y deseados al momento, sino también conocer nuevos títulos relacionados los cuales puedan satisfacer aún más horas de entretenimiento.
Además, queremos ofrecer un servicio de suscripción anual, a un precio de 100€, donde los clientes obtendrán distintas ventajas.

## 2. Glosario de términos

- PVP: Precio de Venta al Público
- DLC: Contenido Descargable (Downloadable Content en inglés). Se trata de contenido adicional para un videojuego que se publica por internet después del lanzamiento del juego principal.


## 3. Visión general del sistema

### 3.1. Requisitos generales
- Como gestor del stock quiero poder visualizar a tiempo real el stock disponible.
- Como agente de atención al cliente/soporte quiero poder consultar y responder incidencias recibidas por usuarios, además de moderar las reseñas.
- Como proveedor de videojuegos quiero que se me garantice el pago antes de proporcionar el producto a la empresa.
- Como administrador del sistema quiero poder hacer una configuración global de la plataforma y poder gestionar los usuarios.
- Como cliente solicito poder comprar videojuegos de manera segura y que se me recomienden los videojuegos más adecuados según mis gustos.
- Como departamento financiero quiero registrar compras, generar facturas y liquidar pagos con proveedores de códigos, con posibilidad de consultar ingresos y márgenes de ganancia para estudiar la evolución de la empresa.

### 3.2. Usuarios del sistema
- Cliente
- Gestor de stock
- Proveedor de videojuegos
- Agente de atención al cliente/soporte
- Administración del sistema
- Departamento financiero

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01. Notificación de stock

Como cliente quiero que se me notifique por correo (si lo solicito) cuando se renueve el stock de un videojuego para poder comprarlo lo antes posible. 

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.02. Garantía de reembolso

Como cliente quiero que se me haga una factura y se me asegure una garantía de 7 días para un reembolso en caso de error en el videojuego para evitar malgastar mi dinero.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.03. Actualización del stock

Como gestor del stock quiero que la cantidad en stock de un producto se actualice cada 5 minutos para poder preveer los pedidos a nuestros proveedores.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.04. Gestión de Usuarios

Como administración del sistema quiero dar de alta, modificar o desactivar cuentas de usuarios, tanto clientes como gestores y agentes, para regular que cada uno tenga las funciones que le corresponden.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.05. Notificación cambios en la página

Como administración del sistema quiero un sistema que avise de todos los futuros cambios dentro de la plataforma que los demás departamentos indiquen que se deben hacer (subida/bajada de precios, próximos lanzamientos, promociones temporales…).

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.06. Verificación de incidencias

Como cliente quiero que se me haga una factura y se me asegure una garantía de 7 días para un reembolso en caso de error en el videojuego para evitar malgastar mi dinero.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

#### R.F.07. Garantía de compras

Como proveedor de videojuegos quiero una garantía de compras de videojuegos mínimas mensuales para que la venta de códigos me salga rentable.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.

#### R.F.08. Garantía de compras

Como proveedor de videojuegos quiero una garantía de compras de videojuegos mínimas mensuales para que la venta de códigos me salga rentable.

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.

#### 4.1.1. Requisitos de información

##### R.I.01. Información de stock al cliente

Como cliente, quiero la siguiente información sobre stock:
- Número de productos disponible
- Tratamiento de mi correo y propaganda
**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- ...

##### R.I.02. Información de garantías al cliente
Como cliente, quiero la siguiente información sobre garantías y facturación:
- Políticas de garantías
- Tiempo de garantía
- Método de facturación
**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- ...

##### R.I.03. Suscripciones

Como cliente, quiero la siguiente información sobre abonos y suscripciones.
- Precios de suscripciones
- Tipos de abonos
- Métodos de pago (mensual, anual)
- Catálogo de videojuegos asociado a cada tipo de suscripción

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- ...

#### 4.1.2. Reglas de negocio
##### R.N.01. Registro de usuario
Un usuario no puede registrarse con un correo electrónico o nombre de usuario que ya exista en la base de datos.
##### R.N.02. Publicación de videojuegos
Un juego no puede ser publicado sin tener asignado previamente una plataforma (Sony, Xbox…), un precio, una descripción y una clasificación por edad.
##### R.N.03. Restricción de edad
Los juegos de PEGI18 no podrán ser vendidos a usuarios menores de edad.
##### R.N.04. Precio de los productos
El precio de un producto no puede ser inferior al precio de adquisición pagado al proveedor de códigos.
##### R.N.05. Política de stock
Cuando un videojuego tenga un stock disponible igual a cero, debe estar catalogado como “Agotado”, impidiendo la compra de este.
##### R.N.06. Registro de usuario
##### R.N.07. Registro de usuario



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


