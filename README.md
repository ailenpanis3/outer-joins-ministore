¿Por qué usaste LEFT JOIN para la Consulta 1 y no INNER JOIN? ¿Qué se perdería si usaras INNER JOIN?
Útilice LEFT JOIN y no INNER JOIN para la Consulta 1 ya que me interesaba no perder la información de la tabla de la izquierda, en este caso, la de ventas. Si hubiera utilizado INNER JOIN
perdía la información de aquellos productos que no se vendieron aún.

¿Por qué usaste RIGHT JOIN para la Consulta 2? ¿Qué tabla está a la izquierda y cuál a la derecha en tu consulta?
En la Consulta 2, utilicé RIGHT JOIN ya que me interesaba saber qué ventas tuve que no estaban relacionadas a una venta_id, que podría ser por un error de carga de los datos.
La tabla de la izquierda es la de ventas, y la de la derecha es la de productos.

¿Qué representan los valores NULL en cada resultado? Explicá con un ejemplo concreto de los datos qué significa que venta_id sea NULL en la Consulta 1 y que producto_id de productos sea NULL en la Consulta 2.
¿Cuándo usarías FULL OUTER JOIN en un caso real de negocio?
Los valores NULL representan que no hay información, en el primer caso no hay información de ventas, es decir, son productos cargados en el sistema que aún no se vendieron.
Y en el segundo caso no hay información de los productos_id, es decir, son ventas que no tienen asociadas un producto_id. 
FULL OUTER JOIN lo podría utilizar para ver estos errores de NULL y poder corregirlos. En este caso sirve para analizar las posibles causas del error.
