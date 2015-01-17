Es hora de un verdadero reto.

Permíteme recordarte una función que ya hemos usado, pero no explicado a detalle... de hecho, son 2.   

Serial.begin(9600); que se ubica en el void Setup (solo lo necesitamos 1 vez)  
Serial.read(); lee un dato y lo almacena en una variable.  (va en el void loop)  
Ejemplo:   
char dato;  
dato = Serial.read();  

El reto de esta semana es....
Usando un RGB, variar el color usando solo UN potenciómetro.

Esto se hace de la siguiente manera.   
1) Leo un valor analógico por el pin A0  
2) Cuando envío una letra 'r' por el monitor serial, almacena ese valor, y lo escribe (analogWrite() )en un pin que maneja el color rojo en el led RGB
3) Si escribo la letra 'g' lo imprime en el 2do pin que maneja el color verde
4) Si escribo la letra 'b' lo imprime en el 3er pin que maneja el color azul

Recuerden poner una resistencia por cada pin del led, y que un RGB funciona como 3 leds en uno. Al variar la intensidad en cada uno, se pueden obtener combinaciones de colores. Este ejercicio no es particularmente complicado, pero es un reto que les enseñará a trabajar con el puerto serial :D

¡Mucha suerte! (bueno, no creo que la necesiten ;) ) Envíanos tu comentario y un par de fotos del circuito funcionando.