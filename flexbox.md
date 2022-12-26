# Qué es FLEXBOX 

Es un modulo de CSS creado para diseñar layouts de una manera mas sencilla. esto es gracias a su flexibilidad.

Si quieres usar flexbox debes tener un contenedor y dentro elementos. La mayoría de acciones se ejecutan en el contenedor padre.

Propiedades en contenedores padre 
**display: flex;**

 # El más importante al querer utilizar flexbox ya que sin esta propiedad display nada funciona.

Una vez aplicado este comando, los elementos dentro del contenedor cambiaran ocupando el alto total de todo el contenedor. Claro que esto se puede modificar a voluntad con ayuda de las demás propiedades de flexbox.

__flex-direction: row | column | row-reverse | column-reverse;__


Esos son los valores que recibe flex-direction.

__row:__ valor por defecto. Posicionamiento de izquierda a derecha.
__column:__ coloca los elementos en columna de arriba hacia abajo.
row-reverse opuesto a row
column-reverse opuesto a reverse.

__flex-wrap: no-wrap | wrap | wrap-reverse;__

no-wrap Hará que absolutamente todos los elementos queden en una sola línea horizontal. Sin importar las especificaciones en proporción que le hubiésemos asignado. Por más que sean los elementos nunca se posicionaron debajo del otro.
wrap Ayuda a que si un elemento del contenedor es más grande lo coloca debajo automaticamente.
wrap-reverse Misma idea que wrap con la diferencia que el orden de los elementos se invierte.

__flex-flow: flex-direction | flex-wrap;__

 *Esta propiedad es un atajo que ahorra líneas de código ya que en su primer valor colocas flex-direction y luego flex-wrap, te recomiendo utilizarlo siempre. Hará nuestro código más optimo.*

 __justify-content: flex-start | flex-end | center | space-around | space-between;__

 Está propiedad se puede considerar como la magia de flexbox en cierto modo. Nos ayuda a decidir la posición de nuestros elementos y la distribución que tendrán.

__flex-start__ valor por defecto. Posición izquierda, de mayor a menor.
__flex-end__ posición derecha. Del menor al mayor, sin alterar el orden de los elementos.
__center__ sencillamente lo centra horizontalmente, sin tener que usar nada más que esto para centrar.
__space-around__ Distribuye todos los elementos por todo el contenedor padre y deja espacios entre cada uno de ellos. El espacio tanto al inicio como al final y entre cada uno de ellos será proporional.
__space-between__ Es básicamente lo mismo que space-around pero sin esos margenes al principio y final.

__align-items: flex-start | flex-end | center | stretch | baseline;__

__flex-start__ valor por defecto. Posiciona los elementos arriba del contenedor.
__flex-end__ posiciona los elementos abajo del contenedor.
__center__ nos permite centrar los elementos de manera vertical. Junto a __justify-content: center;__ nos genera un centrado tanto vertical como horizontal. Todo depende de lo que necesitemos.
__stretch__ para utilizar este valor debes tener un height: auto; Lo que hace este valor es que los elementos ocupen el 100% del contenedor en lo que altura se refiere.
__baseline__ Se utiliza para orientar la base de la fuente del elemento en una misma altura no importando que su tamaño fuente sea distinto entre cada elemento.

__align-contenet: flex-start | flex-end | center | stretch | space-around | space-between;__

 Está propiedad solo se utiliza cuando tenemos varias filas de elementos, pero si es una sola línea de elementos se usa align-items.

__flex-start__ valor por defecto. Posiciona los elementos arriba del contenedor.
__flex-end__ posiciona los elementos abajo del contenedor.
center nos permite centrar los elementos de manera vertical. Junto a __justify-content: center;__ nos genera un centrado tanto vertical como horizontal. Todo depende de lo que necesitemos.
__stretch__
 para utilizar este valor debes tener un height: auto; Lo que hace este valor es que los elementos ocupen el 100% del contenedor en lo que altura se refiere.
space-around Distribuye todos los elementos por todo el contenedor padre y deja espacios entre cada uno de ellos. El espacio tanto al inicio como al final y entre cada uno de ellos será proporional.
space-between Es básicamente lo mismo que space-around pero sin esos margenes al principio y final.

Propiedades en elementos hijo
__flex-basis: 100px;__

Es una propiedad que nos permite sustituir el weight de un elemento, la diferencia es que flex-basis es dinámico porque podemos indicar la dirección tanto del ancho como del alto dependiendo claro del flex-direction que le asignemos.

__flex-grow: #__;

A esta propiedad se coloca el valor que nosotros queramos normalmente es un 1.
Es un valor con el que le indicamos el crecimiento que va a tener el elemento en comparación de los demás elementos hermanos proporcionalmente. Todos van a tener la misma proporción para que abarquen el 100%. Esto nos puede servir para decirle a un elemento que crezca en proporción a los demás.

__flex-shrink: #;__

 Lo opuesto a flex.grow, es el nivel de decremento.

__flex: flex-grow | flex-shrink | flex-basis;__

Esta propiedad es un atajo que nos permite utilizar tres propiedades diferentes en una sola línea de código.

__order: #;__

Con esta propiedad podemos cambiar el orden de nuestros elementos.
Es importante que cada elemento dentro del contenedor tenga declarado un order para que funcione.
Esta modificación se aplica visualmente, la estructura HTML se mantiene igual.

__align-self: flex-start | flex-end | center | stretch | baseline;__


 Muy importante, si en el contenedor padre tenemos declarado un flex.direction: row; esta propiedad nos ordenara los elementos verticalmente. Pero si flex-direction: column; entonces lo ordenara horizontalmente.

__flex-start row__ hasta arriba | column hasta izquierda
__flex-end row__ hasta abajo | column hasta derecha
__stretch row__ colocar height auto | __column__ colocar weight auto
__baseline__ Se utiliza para orientar la base de la fuente del elemento en una misma altura no importando que su tamaño fuente sea distinto entre cada elemento.
















