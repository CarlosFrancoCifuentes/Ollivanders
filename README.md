# Olivanders

Ollivanders es una tienda de objetos mágicos que actualizan su calidad de distintas maneras. Con este proyecto haremos que esa actualización sea de manera automática.

La clase Item no se puede modificar!

Existen dos tipos de objetos, los normalItem y los conjuredItem.

Los normalItem generaliza todos los objetos menos los conjuredItem, pero existen normalItem que no se actualizan de la misma forma y para ello hemos creado una interfaz, llamada updateable (ya que lo que buscamos es que todos los objetos se actualizen). Con esta interfaz podremos decir de que manera queremos que se actulice cada item de la tienda.

## AgedBrie

Si los item AgedBrie no están caducados, por cada día que pase la calidad augmentará en 1.
