

* OBJETOS

Los objetos son parecidos a los arrays pero son mas organizados y se utilizan para guardar informacion sobre una cosa,  se crean con llaves({})  

var object = {
	clave1: valor1,// arrays
	clave2: valor2,// string
	clave3: valor3,// funtion ()
}

* PROPIEDADES 

Son la informacion dispuesta entre llaves; en los arrays se acceden a ellos por un indice, en los objetor  se utilizan pares de clave:valor donde clave es el nombre y valor es el valor de la propiedad; como se muestra en el anterior ejemplo laspropiedades se separan por comas(,) y su asignacion son con dos puntos(:); el valor de una propiedad puede ser un string, un int, un booleano, un arrays, una funcion.

* METODOS 

En el caso de las funciones contenidas en un objeto se le da el nombre de metodos, ya hemos trabajado con diferentes metodos como .push, .lenght, .pop, entre otros; mas adelante entenderemos por que reciben el mismo nombre.

* INVOCAR PROPIEDADES

Para acceder a una propiedad, modificarla o elminarla primero se hace alucion a el objeto y depues a la propiedad.Existen dos formas
 
 - notacion de puntos 

 se invoca el objeto y seguido de un punto su propiedad, esta forma no nos sirva cuando utilizamos variables

 object.clave1; //valor1 //arrays

- notacion de corchetes

se invoca el objeto y entre corchetes su propiedad, para invocar una propiedad de clave string o int se pone entre comillas y para variables se omiten las comillas; por comodidad es muy comun que esta notacion solo la usen con variables.

object['clave1']; //valor1 //arrays

* BUCLES FOR...IN

Como los objetos no tienen indice un bucle sencillo no nos servira, para los objetos se utilizan el bucle for...in loop, tiene un sintaxis diferente que nos permite analizar todas la propiedades del objeto y terminar la interacion al anlizar todas las propiedades del objeto

for (let bucle for object) {
	console.log(bucle);
    console.log(object[bucle])
}

// clave1
// valor1 // arrays
// clave2
// valor2 // string
// clave3
// valor3 // funtion ()

