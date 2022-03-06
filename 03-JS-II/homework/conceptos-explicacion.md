BUCLES 

Los bucles son repeticiones que se generan hasta resolver una condicion, hasta que se exprese la terminacion del proceso y en otros casos se generan bucles infinitos por falta de alguno de las anteriores puntos.

- FOR

 Una de las formas de expresar un bucle es por "for"; su estructura es:

for (let i = 0; i < 10; i++) {
    console.log(i);
}

En el siguiente caso se monstrara un bucle infinito

for (let i = 0; i >= 0; i++) {
    console.log(i);
}

OPERADORES LOGICOS

Se puede valorar varias condiciones en una misma expresion, y saber cual es verdadera o si ninguna es verdadera etcetera, estos son los operadores logicos:

&& and (y)
|| or (o)
!  not (no)
 
- &&

este operador nos dice, para que el codigo se ejecute todas las condiciones deben ser correctas

if (10 > 9 && 10 === 10) {
    console.log (estas exprecciones son correctas)
}

- ||

este operador nos expresa, para que el codigo se ejecute alguna de las condiciones debe ser correcta

if (1 > 3 || 6 === 7 || 5 < 10) { 
    console.log( Una de estas condiciones es correcta)
}

- !

este operador nos cambia el resultado booleano esperado

if (!( 'b' === 'a')) {
    console.log ( la condicion es correcta, se ejecuta el codigo)
}


