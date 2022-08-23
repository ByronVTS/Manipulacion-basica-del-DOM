 var  nombre = "Nombre";
var apellido = "Apellido";
 var NombredeusuarioenPlatzi = "Byron"
var edad = "Edad";
var Correoelectrónico = "ejemplo.com";
var Mayordeedad = true;
var Dineroahorrado = 23.00
var Deudas = 100.00;


//4 Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
console.log(nombre + apellido);
console.log(Dineroahorrado - Deudas);

Responde las siguientes preguntas en la sección de comentarios:
¿Qué es una función?
    Serie de pasos que podemos invocar cuando deseemos 
¿Cuándo me sirve usar una función en mi código?
    Cuando algo se vuelve repetitivo
¿Cuál es la diferencia entre parámetros y argumentos de una función?
    Parametros son los datos que establecemos cuando creamos una funcion
    Los argumentos son los datos que ingresamos  en la funcion


4 Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

const name1 = "Juan David";
const lastname = "Castro Gallego";
const completeName = name1 + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

function apodo (name1, lastname, nickname){
    console.log("Mi nombre es " + name1 + lastname + ", pero prefiero que me digas " + nickname + ".");
}

Condicionales

1 Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un condicional?
    Serie de instrucciones que se ejecutan dependiendo ciertas condiciones establecidas
¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    Condicion simple, solo ejecutar dependiende de un si  o no 
     Bicondicional, hay varias opciones de ejecuciones
¿Puedo combinar funciones y condicionales?
si 
2 Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:


const tipoDeSuscripcion = "Basic";


if(tipoDeSuscripcion === "Free"){
    console.log("Solo puedes tomar los cursos gratis");
   
}else if(tipoDeSuscripcion === "Basic"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
}else if(tipoDeSuscripcion === "Expert"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       
}else if(tipoDeSuscripcion ==="ExpertPlus"){
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
      
}else{
    console.log("No ha escogido ningun plan");
}

3 Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏

const tipoDeSuscripcion = "Basic";

if(tipoDeSuscripcion === "Free"){
    console.log("Solo puedes tomar los cursos gratis");
   
} if(tipoDeSuscripcion === "Basic"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} if(tipoDeSuscripcion === "Expert"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       
} if(tipoDeSuscripcion ==="ExpertPlus"){
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

Ciclos

1. Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un ciclo?
    Una secucencia de acciones que se repite hasta cumplir con las indicaciones determinadas
¿Qué tipos de ciclos existen en JavaScript?
    FormData, do while, while, for
¿Qué es un ciclo infinito y por qué es un problema?
    Un ciclo que no llega a terminarse nunca, no permitirar realizar nuevos procesos
¿Puedo mezclar ciclos y condicionales?
    si
    
2. Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

let i=0;

while( i < 5){
    console.log("El valor de i es "+ i);
    i++;
}

let  i = 10;

while(i>=2){
    console.log("El valor de i es " + i);
    i--;
}

3. Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.
💡 Pista: puedes usar la función prompt de JavaScript.


do {
    resultadoSuma = prompt("Cuanto es 2 + 2: ");
}while(resultadoSuma != 4);
console.log("Felicidades");

Listas
1. Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un array?
    Es un conjuntos de elementos
¿Qué es un objeto?
    es una entidad independiente con propiedades y tipos
¿Cuándo es mejor usar objetos o arrays?
    dependiendo el uso que se le va a dar
    Los objetos son utiles para dar elemtos que se le va  agregar caracteristicas
    Los arrays sirven para los elemtos que no van a cambiar
¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    si 

    2.  Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

    var compras = ["papas", "chocolates", "Yogurt", "Salsa"];
    var autos = ["toyota", "chevrolet", "mazda", "Saljacsa"];

    function primerElemento(grupo){
            console.log(grupo[0]);
    };
    
3.Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array c ompleto).

var compras = ["papas", "chocolates", "Yogurt", "Salsa"];
     let i=0;

while( i < compras.length){
    console.log(compras[i]);
    i++;
}

4. Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo)

var telefonos = {
    marca: "Samsung",
    modelo: "S22",
    annio: 2021
}

function mostrar(grupo){
for(var key in grupo){
    console.log(grupo[key]);
}
}
mostrar(telefonos);

