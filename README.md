# Olivanders

Ollivanders es una tienda de objetos mágicos que actualizan su calidad de distintas maneras. Con este proyecto haremos que esa actualización sea de manera automática.

La clase Item no se puede modificar!

Existen dos tipos de objetos, los normalItem y los conjuredItem.

Los normalItem generaliza todos los objetos menos los conjuredItem, pero existen normalItem que no se actualizan de la misma forma y para ello hemos creado una interfaz, llamada updateable (ya que lo que buscamos es que todos los objetos se actualizen). Con esta interfaz podremos decir de que manera queremos que se actulice cada item de la tienda.

Cada item de la tienda tiene una fecha de "caducidad", una calidad y un nombre.

La calidad de un item nunca será negativa, una vez llegue la calidad a 0, será siempre 0. Y cómo máximo tendrá una calidad de 50.

## NormalItem

Los items degradarán en 1 su calidad cuando el item no haya llegado a su fecha de "caducidad" y al llegar ese momento, se degradarán en 2.

Estos items son todos los que no estén mencionados a continuación

## AgedBrie

Estos items van al revés de los demás, según pasen los días aumentarán su calidad en 1

## Sulfuras

Es un tipo de normalItem y son artículos legendarios, eso significa que su calidad nunca cambia y nunca tiene que venderse.

## BackStage

Aumentan su calidad según se acercan a la fecha de "caducidad". Cuando queden 10 días o menos, la calidadd aumentará en 2 y en 3 cuando queden 5 días o menos.
Una vez llega la fecha de "caducidad", la calidad cae a 0.

## ConjuredItem

Los items conjurados se degradan dos veces más rápido que los normalItem.
