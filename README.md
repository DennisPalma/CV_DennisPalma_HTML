"# CV_DennisPalma_HTML" 
// .push agrega un elemento a un arreglo y lo coloca al fnal como ultimo elemnto aniadido//
//.unshift agrega un elemento a un arreglo y lo coloca al principio como primer elemento // 
//.pop elimina el ultimo elemnto de un arreglo y puede ser almacenado en una nueva variable// 

//.shift elimina el primer elemnto de un arreglo y puede ser almacenado en una nueva variable //

//la siguiente linea de codigo es un ejemplo de un arreglo miltidimencional o sea arreglos dentro de un arreglo//

var myArreglo=[["elemnto1",10],["elemnto2",20],["elemento3",30],"etc"]

function test (myCondition) {
  if (myCondition) {
    return "It was true";
  }
  return "It was false";
}

test(true);
test(false);

// este codigo tiene una funcion que requiere un parametro de valor boolean y para que funcione se le deve indicar por ley ese valor que seria o true o false, a continuacion otro ejemplo para codificar una funcion con condicion if y parametros de valor boolen//

function trueOrFalse(wasThatTrue) {

if (wasThatTrue){
  return "Yes, that was true";
}
return "No, that was false";


}
trueOrFalse(true);

/*el siguiente ejempo de una funcion con condicion toma en cuenta un operador de igualdad == este verifica si una variable o un resultado externo tiene un valor especifico que se indica despues del operador de igualdad si el valor de la variable o resultado externo depositado en dicha variable es igual a lo indicado despues del operador de igualdad, el resultado de la condicion se determina verdadero (true) de lo contrario se determina falso(false)*/

Comparación con el operador de estricta igualdad
La estricta igualdad (===) es la contraparte del operador de igualdad (==). Sin embargo, a diferencia del operador de igualdad, el cual intenta convertir ambos valores comparados a un tipo común, el operador de estricta igualdad no realiza una conversión de tipo.

Si los valores que se comparan tienen diferentes tipos, se consideran desiguales, y el operador de estricta igualdad devolverá falso.

Ejemplos

3 ===  3
3 === '3'
Estas condiciones devuelven true y false respectivamente.

En el segundo ejemplo, 3 es de tipo Number (número) y '3' es de tipo String (cadena).

          operador de estricta igualdad ===

En los dos últimos desafíos, aprendimos sobre el operador de igualdad (==) y el operador de estricta igualdad (===). Vamos a hacer una rápida revisión y práctica utilizando estos operadores un poco más.

Si los valores que se comparan no son del mismo tipo, el operador de igualdad realizará una conversión de tipo y luego evaluará los valores. Sin embargo, el operador de estricta igualdad comparará tanto el tipo de datos como el valor tal como es, sin convertir un tipo a otro.

Ejemplos

3 == '3' devuelve true porque JavaScript realiza la conversión de tipo de cadena a número. 3 === '3' devuelve false porque los tipos son diferentes y la conversión de tipo no se realiza.

Nota: En JavaScript, puedes determinar el tipo de una variable o un valor con el operador typeof, de la siguiente manera:

typeof 3
typeof '3'
typeof 3 devuelve la cadena number y typeof '3' devuelve la cadena string.
La función compareEquality en el editor compara dos valores usando el operador de igualdad. Modifica la función para que devuelva la cadena Equal sólo cuando los valores son estrictamente iguales.

        Comparación con el operador de desigualdad
El operador de desigualdad (!=) es lo opuesto al operador de igualdad. Esto quiere decir que no es igual, y devuelve false cuando la comparación de igualdad devuelva true y vice versa. Al igual que el operador de igualdad, el operador de desigualdad convertirá los tipos de datos mientras los compara.

Ejemplos

1 !=  2
1 != "1"
1 != '1'
1 != true
0 != false
En orden, estas expresiones se evaluarían como true, false, false, false y false.


       Comparación con el operador de estricta desigualdad
El operador de estricta desigualdad !== es el opuesto lógico del operador de estricta igualdad. Esto significa "Estrictamente Desigual", y devuelve false cuando la comparación de estricta igualdad devolvería true y vice versa. El operador de estricta desigualdad no convertirá los tipos de datos.

Ejemplos

3 !==  3
3 !== '3'
4 !==  3
En orden, estas expresiones se evaluarían como false, true y true.


      Comparación con el operador "mayor que"
El operador mayor que (>) compara los valores de dos números. Si el número a la izquierda es mayor que el número a la derecha, devuelve true. De lo contrario, devuelve false.

Al igual que el operador de igualdad, el operador mayor que convertirá los tipos de datos de valores mientras los compara.

Ejemplos

5   >  3
7   > '3'
2   >  3
'1' >  9
En orden, estas expresiones se evaluarían como true, true, false y false.


             Comparación con el operador "mayor o igual que"
El operador mayor o igual que (>=) compara el valor de dos números. Si el número de la izquierda es mayor o igual que el número de la derecha, devuelve true. De lo contrario, devuelve false.

Al igual que el operador de igualdad, el operador mayor o igual que convertirá los tipos de datos mientras los compara.

Ejemplos

6   >=  6
7   >= '3'
2   >=  3
'7' >=  9
En orden, estas expresiones se evaluarían como true, true, false y false.



               Comparación con el operador "menor que"
El operador menor que (<) compara los valores de dos números. Si el número a la izquierda es menor que el número a la derecha, devuelve true. De lo contrario, devuelve false. Al igual que el operador de igualdad, el operador menor que convertirá los tipos de datos mientras los compara.

Ejemplos

2   < 5
'3' < 7
5   < 5
3   < 2
'8' < 4
En orden, estas expresiones se evaluarían como true, true, false, false y false.



             Comparación con el operador "menor o igual que"
El operador menor o igual que (<=) compara el valor de dos números. Si el número de la izquierda es menor o igual que el número de la derecha, devuelve true. Si el número a la izquierda es mayor que el número a la derecha, devuelve false. Al igual que el operador de igualdad, el operador menor o igual que convertirá los tipos de datos mientras los compara.

Ejemplos

4   <= 5
'7' <= 7
5   <= 5
3   <= 2
'8' <= 4
En orden, estas expresiones se evaluarían como true, true, true, false y false.


             Comparaciones con el operador lógico "and"
A veces tendrás que probar más de una cosa a la vez. El operador lógico and (&&) devuelve true si y solo si los operandos a la izquierda y a la derecha son verdaderos.

El mismo efecto se podría lograr anidando una sentencia if dentro de otra sentencia if:

if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";
solo devolverá Yes si num es mayor que 5 y menor que 10. La misma lógica se puede escribir como:

if (num > 5 && num < 10) {
  return "Yes";
}
return "No";



            Comparaciones con el operador lógico "or"
El operador lógico or (||) devuelve true si cualquiera de los operandos es true. De lo contrario, devuelve false.

El operador lógico or se compone de dos símbolos de barra vertical: (||). Este se puede encontrar normalmente entre las teclas de tabulación y escape.

El patrón de abajo debería parecer familiar desde los puntos de referencia anteriores:

if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
devolverá Yes sólo si num está entre 5 y 10 (5 y 10 incluidos). La misma lógica se puede escribir como:

if (num > 10 || num < 5) {
  return "No";
}
return "Yes";



    Introducción a las sentencias "Else If"
Si tienes múltiples condiciones que necesitan ser resueltas, puedes encadenar sentencias if junto con sentencias else if.

if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}



Orden lógico de las sentencias "if else"
El orden es importante en las sentencias if, else if.

La función se ejecuta de arriba a abajo, por lo que habrá que tener cuidado con qué sentencia va primero.

Tomemos como ejemplo estas dos funciones.

Aquí está la primera:

function foo(x) {
  if (x < 1) {
    return "Less than one";
  } else if (x < 2) {
    return "Less than two";
  } else {
    return "Greater than or equal to two";
  }
}
Y la segunda, simplemente cambia el orden de las sentencias:

function bar(x) {
  if (x < 2) {
    return "Less than two";
  } else if (x < 1) {
    return "Less than one";
  } else {
    return "Greater than or equal to two";
  }
}
Mientras que estas dos funciones parecen casi idénticas, si pasamos un número a ambas, obtenemos diferentes salidas.

foo(0)
bar(0)
foo(0) devolverá la cadena Less than one, y bar(0) devolverá la cadena Less than two.


         Agrega una opción predeterminada en las declaraciones switch
En una declaración switch puede que no seas capaz de especificar todos los valores posibles como declaraciones de case (caso). En su lugar, se puede añadir la declaración default, la cual se ejecutará si no se encuentran declaraciones case. Piensa en ella como la última sentencia else en una cadena if/else.

Una declaración default debe ser el último caso.

switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}



Múltiples opciones idénticas en las declaraciones "switch"
Si la sentencia break es omitida en un caso (case) de una sentencia switch, las siguientes sentencias case serán ejecutadas hasta encontrar un break. Si tienes múltiples entradas con la misma salida, puedes representarlas en una sentencia switch como esta:

let result = "";
switch(val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}
Los casos 1, 2 y 3 producirán el mismo resultado.


se puede reemplazar la cadena de sentencias if/else por sentencias switch


             Devuelve valores booleanos desde funciones
Podrás recordar que en Comparación con el operador de igualdad todos los operadores de comparación devuelven un valor booleano true, o false.

A veces la gente usa una sentencia if/else para hacer una comparación, como esta:

function isEqual(a, b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
Pero hay una mejor manera de hacer esto. Puesto que === devuelve true o false, podemos devolver el resultado de la comparación:

function isEqual(a, b) {
  return a === b;
}

            CONTEO DE CARTAS EJMP CODIG

var count=0;
function cc(card) {
  // Only change code below this line
  
  if (card == 2 || card == 3 || card == 4 || card ==5 || card ==6) {
  	//alert("2 3 4 5 6");
    count += 1;
  }
  else if (card == 7 || card == 8 || card == 9) {
      count += 0;
  }
  else if (card == 10 || card == "J" || card == "Q" || card == "K" || card == "A") {
      count -= 1;
  }
  if (count <= 0) {
  	return String(count) + " Hold";
  }
  else {
  	return String(count) + " Bet";
  }
  
  // Only change code above this line
}


cc(2); cc(3); cc(4); cc(5); cc(6);
cc(7); cc(8); cc(9);
cc(10); cc("J"); cc("Q"); cc('K'); cc('A');
cc(3); cc(7); cc("Q"); cc(8); cc("A");
cc(2); cc("J"); cc(9); cc(2); cc(7);
cc(2); cc(2); cc(10);
cc(3); cc(2); cc("A"); cc(10); cc('K');

         



         CREACION DE OBJETOS EN JavaScript

Crea un objeto que represente a un perro llamado myDog que contenga las propiedades name (una cadena), legs, tails y friends.

Puedes establecer estas propiedades del objeto a los valores que quieras, siempre y cuando name sea una cadena, legs y tails sean números, y friends sea un arreglo.            

const myDog = {
name: "cosita",
legs: 4,
tails: 1,
friends: ["human","food"]
};




             ACCEDE A LAS PROPIEDADES de objetos con NOTACIO DE PUNTOS 
Hay dos maneras de acceder a las propiedades de un objeto: notación de puntos (.) y notación de corchetes ([]), similar a un arreglo.

La notación de puntos es lo que se usa cuando conoces el nombre de la propiedad a la que intentas acceder con antelación.

Aquí hay un ejemplo de cómo usar la notación de puntos (.) para leer la propiedad de un objeto:

const myObj = {
  prop1: "val1",
  prop2: "val2"
};

const prop1val = myObj.prop1;
const prop2val = myObj.prop2;
prop1val tendrá una cadena con valor val1 y prop2val tendrá una cadena con valor val2.



ACCEDE A LAS PROPIEDADES de pbjetos con NOTACIO DE CORCHETE [] 
La segunda manera de acceder a las propiedades de un objeto es con la notación de corchetes ([]). Si la propiedad del objeto al que intentas acceder tiene un espacio en el nombre, necesitarás usar notación de corchetes.

Sin embargo, también puedes utilizar la notación de corchetes en las propiedades de objeto sin espacios.

Aquí hay un ejemplo de cómo usar la notación de corchetes para leer la propiedad de un objeto:

const myObj = {
  "Space Name": "Kirk",
  "More Space": "Spock",
  "NoSpace": "USS Enterprise"
};

myObj["Space Name"];
myObj['More Space'];
myObj["NoSpace"];
myObj["Space Name"] sería la cadena Kirk, myObj['More Space'] sería la cadena Spock, y myObj["NoSpace"] sería la cadena USS Enterprise.

Ten en cuenta que los nombres de las propiedades con espacios deben estar entre comillas (simples o dobles).
Accede a propiedades de objetos con variables
Otro uso de la notación de corchetes en objetos es acceder a una propiedad que está almacenada como el valor de una variable. Esto puede ser muy útil para iterar a través de las propiedades de un objeto o para acceder a una tabla de búsqueda.

Aquí hay un ejemplo del uso de una variable para acceder a una propiedad:

const dogs = {
  Fido: "Mutt",
  Hunter: "Doberman",
  Snoopie: "Beagle"
};

const myDog = "Hunter";
const myBreed = dogs[myDog];
console.log(myBreed);
La cadena Doberman se mostrará en la consola.

Otra forma de usar este concepto es cuando el nombre de la propiedad se recoge dinámicamente durante la ejecución del programa, de la siguiente manera:

const someObj = {
  propName: "John"
};

function propPrefix(str) {
  const s = "prop";
  return s + str;
}

const someProp = propPrefix("Name");
console.log(someObj[someProp]);
someProp tendrá una cadena con un valor propName y la cadena John se mostrará en la consola.

Ten en cuenta que no usamos comillas alrededor del nombre de la variable cuando la usamos para acceder a la propiedad porque utilizamos el valor de la variable, no el nombre.



      PODEMOS AGREGAR UNA NUEVA PROPIDAD AUN OBJETO DE IGUAL MANERA SE PUEDE MODIFICAR 
      const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.bark="Woof";


      PODEMOS ELIMINAR UNA PROPIEDAD O ELEMTO DE UN OBJETO UTILIZANDO EK CODIGO: DELETE

      const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};
delete myDog.tails;



    EJEMPLO DE BUSQUEDA UTILIZANDO OBJETOS
    function phoneticLookup(val) {
  let result = "";

  // Cambia solo el código debajo de esta línea
  const lookup = {
"alpha": "Adams",
"bravo": "Boston",
"charlie" : "Chicago",
"delta" : "Denver",
 "echo" : "Easy",
"foxtrot": "Frank"
  };
  const value = val;
  result=lookup[value];
  // Cambia solo el código encima de esta línea
  return result;
}
phoneticLookup("alpha");
phoneticLookup("bravo");
phoneticLookup("charlie");
phoneticLookup("delta");
phoneticLookup("echo");
phoneticLookup("foxtrot");
phoneticLookup("");


               Verifica las propiedades de un objeto CON EL METODO .hasOwnProperty()
A veces es útil comprobar si existe o no la propiedad de un objeto dado. Podemos utilizar el método .hasOwnProperty(propname) para determinar si un objeto tiene una propiedad con ese nombre. .hasOwnProperty() devuelve true o false si se encuentra la propiedad o no.

Por ejemplo

const myObj = {
  top: "hat",
  bottom: "pants"
};

myObj.hasOwnProperty("top");
myObj.hasOwnProperty("middle");
El primer hasOwnProperty devuelve true, mientras que el segundo devuelve false.


   VERIFICACION DE LAS PROPIEDADES DE UN OBJETO

   
function checkObj(obj, checkProp) {
  // Cambia solo el código debajo de esta línea
  if (obj.hasOwnProperty(checkProp)){
    return obj[checkProp];
  }
else {
  return "Not Found";
  // Cambia solo el código encima de esta línea
}
}
checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "gift");
checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "pet");
checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "house");
checkObj({city: "Seattle"}, "city"); 
checkObj({city: "Seattle"}, "district");
checkObj({pet: "kitten", bed: "sleigh"}, "gift"); 

 UN EJEMPLO DE MANIPULACION DE OBJETOS COMPLETOS 

 const myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },
  {
     "artist": "Daft rock",
    "title": "Homework",
    "release_year": 1997,
    "formats": [ 
      "CD", 
      "Cassette", 
      "LP"
    ],
    "gold": true
  }
];

        UN EJEPLO DE COMO ACCEDER A LA MANIPULACION DE  UN OBJETO COMPLETO


const myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

const gloveBoxContents = myStorage.car.inside["glove box"]



        UN EJEMPLO DE COMO ACCEDER A ARREGLOS ANINADOS

const myPlants = [
  {
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }
];

const secondTree = myPlants[1].list[1];
        
