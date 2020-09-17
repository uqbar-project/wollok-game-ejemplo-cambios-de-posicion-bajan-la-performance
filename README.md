# wollok-game-ejemplo-cambios-de-posicion-bajan-la-performance

## ¿Up, right, left y down hacen mas lento las cosas?

Pareciera que los mensajes up, right, left y down de alguna manera están teniendo un impacto en el juego, porque al usarlos luego de un rato se puede percibir que anda mas lento.

La forma en la que lo traté de reproducir en el ejemplo es la siguiente:
- Hay una acción que pasa cada 1 tick que mueve a un objeto 1 lugar hacia arriba y un lugar hacia la derecha.
- Hay otra acción que también pasa cada 1 tick que le suma uno a un contador y muestra el valor por consola

Al empezar el juego, que tiene width = 1 y height = 1 porque no me interesaba lo que se veía ahí, se puede ver en el output como empiezan a imprimirse números.
Al menos en mi caso me pasa que después de un rato los números empiezan a avanzar mucho más lento que al principio.

## ¿game.at arregla el problema?

Algo que también note es que si piso la posición usando game.at el problema desaparece, así que agregue que si se aprieta la barra de espacio pise la posicion del objeto con la misma posición en la que estaba pero usando game.at para lograr eso.
Y al menos en mi caso noto que cuando hago eso (apretar espacio) los números vuelven a subir muy rapido.

Acá se puede ver una demo: https://streamable.com/ue2d9w
