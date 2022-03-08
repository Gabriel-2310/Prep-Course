
* `prototype`

los objetos que pertenecen a la misma clase pueden compartir datos y metodos; si utlizaramos los metodos en cada objeto nuestro computador sufriria (refiriendonos a la capacidad de memoria, dado que las funciones gasta mucho recursos), por eso existe una forma de crear un solo metodo que afecte los objetos que necesitemos llamado prototype.

function Personal (nombre, edad) {
    this.nombre = nombre;
    this.edad  = edad;
}

Personal.prototype.presentar = function () {
    return 'Cordial saludo, mi nombre es ' + this.nombre + ' y tengo ' + this.edad + ' años.'
}

esta forma nos crea un metodo en la clase mas no en los objetos; para utilizar este metodo se hace lo siguiente

// como no hemos definido objetos en nuestra clase, creamos un objeto nuevo
var gabriel = new Personal (gabriel, 21);

// y este objeto lo podemos utilizar con el metodo creado anteriormente 
gabriel.presentar () 
'Cordial saludo, mi nombre es gabriel y tengo 21 años.'

* _Constructors_ (de Clases)

los constructors son metodos de crear clases; 

function Personal (nombre, edad) {
    this.nombre = nombre;
    this.edad  = edad;
}

esta forma es de ES6

class Personal {
    constructor (nombre, apellido) {
        this.nombre = nombre,
        this.apellido = apellido;
    }
    saludar () {
        console.log('Hola! ' + this.nombre);
    }
}

muchas vecez un objeto puede ser parte de varias clases. ejemplo un objeto gato puede ser parte de la clase animal, y de la clase mamifero, para esto pudemos crear una subclase a partir de clases personalizadas

class Empleado extends Personal {
    constructor (nombre, apellido, empleo, sueldo) {
        super (nombre, apellido);
        this.empleo = empleo;
        this.sueldo = sueldo;
    }
}

var luis = new Empleado ('luis', 'valencia', 'programador', 100);

para invocar una propiedad 

luis.saludar ()
// Hola! luis

el metodo saludar es de la clase Personal, es decir el interprete busca el metodo o propiedad de forma accendente: primero en el objeto, y seguido a la clase que pertenece y asi hasta encontrarla o llegar al final y retornar como error