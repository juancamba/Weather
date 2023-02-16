# Wheather

Creación de un proyecto de tipo API en .net core 6.

Esta API tendrá un solo controlador.

El controlador tendrá dos endpoints.
* Un endpoint para el registro de pedidos (un pedido estará compuesto por una cabecera y un detalle de pedido, los campos te los puedes inventar). Este endpoint registra un pedido en una base de datos MongoDB y en una base de datos Mysql al mismo tiempo. Además este endpoint tendrá un parámetro llamado "sandbox" que si es igual a true almacenará los datos en unas bases de datos diferentes a las de producción.
* Un segundo endpoint que al pasarle como parámetro una localización/ciudad nos devuelve el tiempo (temperatura y humedad) del mismo. Para lo cual enlazaremos con el servicio https://weatherstack.com/

Además, en el endpoint de registro de pedidos adjuntaremos al pedido el clima asociado al mismo, es decir, la temperatura ambiente y humedad en el momento de registro del pedido. (NOTA: como un pedido está asociado a un local/restaurante sabemos la ubicación de ese pedido).

Crea un proyecto con las pruebas unitarias.
