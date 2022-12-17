# Plan de ataque.
A continuacion se muestra la lista de los inconvenientes detectados y corregidos  en el testeo realizado sobre el proyecto SOLUCION-TEST-QA-BANRURAL.

1. # Error. 
no se realizar ninguna accion al realizar click en el boton "Ingrese el  numero aleatorio".
   # Solucion.
Se corrigio la llamada del metodo addEventListener.
 
2. # Error.
el input permitia entrada de caracteres alfanumericos.
   # Solucion.
se cambio el atributo del input de tipo "text" a "number".

3. # Error.
El numero aleatorio generado era decimal dentro del rango de 1 a 10.
   # Solucion.
Se implemento el metodo Math.floor() para redondear como entero, ademas se incremento el rango aleatoriedad asta 100.

4. # Error.
el juego solo permitia 5 intentos unicamente por partida.
   # Solucion.
se incremento el valor de la constante ATTEMPS a 10.

5. # Error.
No se reconocia el elemento "lowOrHi".
   # Solucion.
se corrigio el argumento enviado al document.querySelector() de 'lowOrHi' a '.lowOrHi'.

6. # Error.
En el escenario en el cual se ingresa el numero aleatorio correcto, no se muestra el respectivo mensaje 'Felicitaciones! adivinaste el número!'. 
   # Solucion.
se utilizo el metodo parseFloat(guessField.value) para asignarle el valor numerico a la variable userGuess, esto con la finalidad de poder realizar correctamente la comparacion en el if que valida si el numero ingresado coinside con el generado aleatoriamente, ya que se compara tanto el valor como el tipo de datos de los mismos.

7. # Error.
En el escenario en el cual se ingresa el numero aleatorio correcto, se muestra el mensaje '¡¡¡Perdistes!!!', con un backgroundColor en color negro.
   # Solucion.
correccion del color a verde en el backgroundColor, y se cambio el mensaje de respuesta a 'Felicitaciones! adivinaste el número!'.

8. # Error.
Error al modificar el elemento "lowOrHi"
   # Solucion.
Se cambio el ambito de la variable a global (de 'let' a 'var').

9. # Error.
En el escenario en el cual se ingresa un numero incorrecto, el backgroundColor se muestra como verde.
   # Solucion.
se corrigio el backgroundColor de verde a negro.

10. # Error.
Al ingresar un numero de incorrecto, los mensajes 'El número es mayor!' y 'El número es menor!' se muestran de manera inversa.
   # Solucion.
Se invirtieron los operadores '<' y '>' en sus respectivos If.

11. # Error.
Inconveniente en la funcion setGameOver().
   # Solucion.
Se corrigio la llamada del metodo addEventListener.

12. # Error.
Inconvenientes en la funcion resetGame().
   # Solucion.
se agrego el rango de aleatoridad en el mentodo Math.random.

13. # Error.
El Input permite el ingreso de numero decimales, mayores a 100, menores a 1, y el no ingresar ningun valor.
   # Solucion.
Se realizo un if que validara que el campo no este vacion, el digito sea un entero, que sea mayor o igual a 1 y menor o igual a 100. de no cumplirse estas condiciones, se muestra un alert con el mensaje "Por fabor ingrese un numero entero dentro del rango del 1 a 100".
