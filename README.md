# connect-four (Funcionalidad)
Es un juego que consiste en que tenemos dos jugadores, de los cuales uno de estos debe completar una fila de 4 círculos.
Cada jugador tiene un color asignado para los círculos. Jugador 1 (Rojo) y jugador 2 (Azul). Esta fila no puede ser interrumpida
por el otro jugador. Y puede ser vertical, horizontal o diagonal. Estos círculos no pueden ir en cualquier lado. Algunas posiciones son incorrectas por lo tanto si seleccionamos 5 veces posiciones incorrectas perderemos el juego y este se reiniciará.

Las posiciones correctas son: Al inicio del cuadrado, o sea por la parte de abajo, o si ya hay un círculo podemos poner otro encima de ese. Por lo tanto las posiciones serán siempre encima de otro circulo o en el principio del recuadro, de lo contrario nos descontara una vida de los 5 que tenemos.


## Funciones que utilice para los requerimientos del taller:
* La primera función que implemente es mostrarInstrucciones(){
Esta función lo que hace es que cuando le damos click en el botón de instrucciones que tenemos en el html nos va a amostrar las instrucciones del juego, Con un swal.fire.
}

* La otra función que utilice es NombreInicio(){
Esta función es para que cuando iniciemos la página esta nos solicite el nombre de los dos jugadores con un par de condiciones que lo que hacen es tomar el valor de lo que ingresamos para tomarlo y luego enviarlo mediante un document.getElementById  a un div  que tenemos en el html el cual nos mostrara los nombres que ingresamos, y para este caso le puse una condición de que si no ingresamos nada nos va a recargar el recuadro de los nombres.
}

* La otra función que utilice para que me recargara la página cuando SE PIERDA EL JUEGO o cuando NO ingresan el nombre fue recargar(){
En esta función lo que hago es llamar otra función que me recarga toda la página, la utilice para las condiciones que le di a los swal.fire de los nombres, dado que si no se ingresa el nombre, el juego no se iniciara. Y de cuando se pierde el juego, para que los jugadores no puedan seguir jugando se bloquea la pantalla con un swal.fire y se espera un determinado tiempo mientras los jugadores leen la advertencia y se reinicia el juego
}




