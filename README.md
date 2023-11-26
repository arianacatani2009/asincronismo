# asincronismo
Pero, ¿qué implica el asincronismo? Se refiere a tareas que, al ejecutarse, pueden completarse en el momento o en el futuro, y su comportamiento no es bloqueante.

Un ejemplo típico es cuando nuestra aplicación solicita el catálogo de productos; envía una orden a través de una API y es el servidor quien procesa la solicitud. Cuando esté listo, devolverá el listado de datos.

En este punto, nuestra aplicación desconoce cuánto tiempo tomará al servidor responder, por lo que, si usáramos una función síncrona , la aplicación esperaría todo ese tiempo, bloqueando el proceso de funciones subsecuentes.

En cambio, una función asíncrona enviará la petición a la API y permitirá que nuestra aplicación continúe con la ejecución de otras tareas. Cuando el servidor responda, se notificará que los datos están listos para ser procesados.
