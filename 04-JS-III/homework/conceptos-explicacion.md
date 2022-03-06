
ARRAYS (ARREGLOS)

Los arrays son listas de elemtos, pueden contener strings, numeros, booleanos, funciones, incluso arrays; para crearlo primero cramos una variable dandole su respectivo nombre y le asignamos entre corchetes y separados por comas los elemtos a guardar en la lista.

var lista = ['hola', 23, null, undefined, true, function () {console.log('sor un arrays')}, [1, 2, 3, 4, 5]]
               0     1    3        4       5                    6                                   7

lista
 ['hola', 23, null, undefined, true, ƒ, Array(5)]

podemos acceder a sus elementos y modificarlos por medio de un indice que se le da a cada elemto de forma creciente desde el 0 

lista [0]
'hola'

lista [0] [0]
'h'

tambien podemos acceder a lo que hay dentro de los elementos, un strings es considero una lista de caracteres por eso podemos acceder a ella

podemos cambiar, adiccionar o pisar los elementos

lista [0] = 'me modifican'

lista [0]
'me modifican'

lista [7] = 'soy nuevo'

lista
['me modifican', 23, null, undefined, true, ƒ, Array(5), 'soy nuevo']


PROPIEDADES

Length

Al igual que con los strings esta propiedad nos cuenta los elementos presentes en la arrays

lista.length
8

Push & Pop

estas propiedades nos modifica los ultimos elementos del arrays; push nos agrega y pop los extrae

lista.push('me agregaron')
9

lista
(9) ['me modifican', 23, null, undefined, true, ƒ, Array(5), 'soy nuevo', 'me agregaron']

lista.pop()
'me agregaron'
lista
(8) ['me modifican', 23, null, undefined, true, ƒ, Array(5), 'soy nuevo']

Unshift $ Shift

Al igual que push y pop, agregan y extraen pero al inicio de la lista

lista.unshift(12)
9

lista
(9) [12, 'me modifican', 23, null, undefined, true, ƒ, Array(5), 'soy nuevo']

lista.shift()
12

lista
(8) ['me modifican', 23, null, undefined, true, ƒ, Array(5), 'soy nuevo']



BUCLES Y ARRAYS

Se pueden utilizar arrays en bucles para acceder, modificar, extraer etcetera,  su lista

for (var i = 0; i < lista.length -1; ++i) {
    console.log(lista[i])}
me modifican
23
null
undefined
true
ƒ () {console.log('sor un arrays')}
(5) [1, 2, 3, 4, 5]
undefined

