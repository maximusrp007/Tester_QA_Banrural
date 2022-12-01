

# Prueba de tester, errores encontrados y modificaciones.
# Max Adolfo Rodríguez Pimentel


## --> Uncaught TypeError: guessSubmit.addeventListener is not a function: 
 Existencia de un error en linea 87 - > guesssubmit.addeventlistener('click', checkguess);
 Función addeventlistener no se reconoce, mala sintaxis.
# --> guessSubmit.addEventListener('click', checkGuess);

##  Uncaught TypeError: Cannot set properties of null (setting 'textContent')
Valores nulos reconocidos por el interprete.
Error en sintaxis, se agrega ** . ** en ('.lowOrHi');
# --> const lowOrHi = document.querySelector('.lowOrHi');,

## Uncaught TypeError: resetButton.addeventListener is not a function at setGameOver: 
No se reconoce addeventlistener, es un error por sintaxis. 
# --> resetButton.addEventListener('click', resetGame);

## La logica no es la adecuada:
else if(guessCount === ATTEMPS) El Programa solo se ejecuta 5 veces y se detiene ya que se pasa una variable constante. 
# ----> else if(userGuess == randomNumber), 
Cambio de variable que evalua la entrada y cambio en el operador.

## Error en iteracion 
# ----> if(userGuess === randomNumber) No existe iteracion entre 1 y 10.
# ----> if(guessCount > 9) Se realiza cambio en variable y en iteracion

## Error en numero random :
let randomNumber = Math.random() * 10; Se hace una conversion de numeros decimales a numeros enteros, y crea una condicion.
# ----> let randomNumber = Math.round(Math.random()*100);

## Cambio de color de las àreas y cambio de funcion  : 
Se cambia de color las áreas de texto donde se produce la impresión del mensaje por el color brindado en el requerimiento. 
# ----> lastResult.style.backgroundColor = 'green';
# ----> lastResult.style.backgroundColor = 'red';

