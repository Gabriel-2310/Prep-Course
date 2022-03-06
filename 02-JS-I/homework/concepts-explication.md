 JAVASCRIPT

 El lenguaje de programacion javascript es muy flexible, es decir, no es tan estricto: te permitira abreviar en ciertos casos, y en otros encontraras varias formas de escritura con la misma accion; por esto javascrpit es una buena eleccion para iniciar con los lenguajes de programacion.

 CONCEPTOS

 * Variables

 las variables son formas de almacenar datos de acceso rapido, se utilizan las siguientes:
 - var
 - let 
 - const
la diferencia mas palpable entre var y const es que en var puedo sobreescribir, pisar o modificar su contenido o valor mientras que const conserva lo preserva impidiendonos cambiarlo; su estructura es la siguiente:
 
  var saludo = "hola, como estas"

  const PI = 3,1416

la parte "var" o "const" es una keywords o palabra clave, cuando la utilizamos el interprete asume que seguido de la misma declararemos una variable; "saludo" o "PI" es el nombre que le damos a la variable puede ser cualquiera excepto keywords o palabras claves y tiene que ser una sola palabra (no puede presentar espacios); "=" es asignacion (para igualdad se utiliza ==) despues colocaremos los datos.
Para invocar una variable se escribe su nombre, el interprete remplaza el nombre de la variable con los datos al resolver un codigo. ejemplo:

var numero = 5    

numero + 5
10

TIPOS DE DATOS

cuando le brindamos informacion al interprete, esta informacion se puede clasificar en 

 * Strings
 * numbers 
 * Valores booleanos (`true`, `false`)

- STRINGS

Es un hilo de caracteres, se identifican por estar entre comillas, las comillas pueden ser dobles o sencillas.

"Soy un strings," + " " +"estoy entre comillas"
"soy un strings, estoy entre comillas"

un strings puede ser palabras, numeros, letras o incluso pueden estar vacios: los string se pueden sumar esto se llama concadenar y es unir hilos de caracteres, ten presente que al concadenar se unen exactamente donde estan las comillas si necesitas un espacio para separar recuerda dejarlo antes de las comillas 

- NUMBERS 

Son datos numericos con los que se pueden realizar operaciones (+ - * / %); la operacion % nos brinda el resto de una division (21 % 5 : 1).

- VALORES BOOLEANOS (`true`, `false`)

Estos son datos evaluables donde el interprete despues de valorar el codigo  nos retornara una de dos opciones posibles, en el caso de JS 'true' o 'false'; se pueden utilizar strings o numbers para el codigo
 
 5 < 6
 true

 'a' == 'a'
 true

 4 > 6
 false

FUNCIONES 

Comunmente llamadas *callable objects*  objetos invocables, al igual que las varaibles nos almacena informacion para acceder rapidamente, pero no nos guarda datos las funciones nos guarda codigos. las funciones interactuan con las variables. su estructura 

function  nombre() {}

'funtion' es una keywords o palabra clave que hace alucion a funcion; 'nombre' es donde nombramos la funcion para poder invocarla mas adelante facilmente; () dentro de los parentesis van los argumentos; {} dentro de las llaves el codigo. las funciones tienen un alcance o un limite conocido como 'scope', al crearla colocamos un limite entre  la funcion  y archivo global, es decir que los cambios o codigos globales no me afectan dentra de la funcion y viceversa, (es de aclarar que como JS es tan flexible puede buscar globalmente si dentro de la funcion no encuentra los datos, variables..., para resolver el codigo) por esto mismo una funcion no nos retorna a menos que se lo expresemos.

- ARGUMENTOS 

Los argumentos son datos que procesara el codigo, en una funcion pueden haber uno o varios argumentos 

example

 function example(a, x) {
     var suma = a + x
 }

example(2, 3)
undefined

esta funcion nos retorna undefined por que una funcion no retorna como se explico anteriormente ('scope')

- RETURN 

Return es una keywords o palabra clave que le dice al interprete que retorne la informacion especificada, se utiliza en las funciones para extraer datos que por el scope no retornan. 

example

 function example(a, x) {
     var suma = a + x
     return = suma
 }

example(2, 3)
5

 DECLARACIONES

 Dentro de una funcion podemos dar declaraciones tales como return, if..., que nos condicionan el codigo como en el caso de return que es una declaracion de retorno que le expresa al interprete que datos pueden ser extraidos.

 - IF
Es un condicional, que nos permite evaluar un dato con unos criterios constituidos, retornando uno de los resultados establecidos .

function ejemplo (x) {
    if (x < 10) {
        return 'verdadero';
    } return 'falso';
}

ejemplo (2)
'verdadero'

ejemplo ('12)
'falso'