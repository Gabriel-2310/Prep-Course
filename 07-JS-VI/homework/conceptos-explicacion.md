
* Funciones Callback
 
Las funciones gastan muchos recursos en nuestra computadora (por esto debemos limitar la creacion de funciones para que nuestro programa no sea tan exigente en caracteristicas), lo mejor es crear funciones que podamos utilizar varias vecez y en diferentes casos; un caso muy particular es pasar funciones como argumentos de otras funciones, se le conocen como callback. Por convencion cuando utilizamos un callback lo representamos con 'cb' en el argumento.

// en el siguiente codigo queremos incrementar los elementos de un array, multiplicandolos por si mismo.

//creamos la funcion en la que pasaremos el array y  una funcion por argumento, es decir; un callback
function map(array, cb) {
  arr = array.map(cb);
  return arr;
}

undefined

// creamos el array
numers = [1, 2, 3, 4, 5]

(5) [1, 2, 3, 4, 5]

// creamos la funcion que pasaremos por callback 
function multi(num) {
return num * num;
}

undefined

// invocamos la funcion creada pasando por argumentos el array y el callback 
map(numers, multi)

(5) [1, 4, 9, 16, 25]

RECUERDA: Un callback es una funcion declarada que la ejecutamos dentro de una funcion; un metodo es una funcion declarado dentro de un objeto y la ejecutamos con sus propiedades, es decir, podemos crear una funcion y ejecutarlas cuando y donde las necesitemos pero teneiendo en cuenta la sintaxis.
 