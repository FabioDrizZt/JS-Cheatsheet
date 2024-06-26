# 📓 JavaScript Cheatsheet

## Índice
1. [Variables](#variables)
2. [Tipos de Datos](#tipos-de-datos)
3. [Operadores](#operadores)
4. [Propiedades y Métodos Importantes](#propiedades-y-métodos-importantes)
5. [Estructuras Condicionales](#estructuras-condicionales)
6. [Estructuras Repetitivas](#estructuras-repetitivas)
7. [Parseo de Datos](#parseo-de-datos)

## Variables

```javascript
let variableLet = "Hola"; // Variable que puede cambiar
const variableConst = "Mundo"; // Variable constante
var variableVar = "JavaScript"; // Variable de alcance global o de función
```

## Tipos de Datos

```javascript
let numero = 42; // Number
let cadena = "Hola"; // String
let booleano = true; // Boolean
let arreglo = [1, 2, 3]; // Array
let objeto = { nombre: "Juan", edad: 30 }; // Object
let indefinido; // Undefined
let nulo = null; // Null
```

## Operadores

### Operadores Aritméticos

```javascript
let suma = 5 + 3;
let resta = 5 - 3;
let multiplicacion = 5 * 3;
let division = 5 / 3;
let modulo = 5 % 3;
let exponenciacion = 5 ** 3;
```

### Operadores de Asignación

```javascript
let x = 10;
x += 5; // x = x + 5
x -= 3; // x = x - 3
x *= 2; // x = x * 2
x /= 2; // x = x / 2
x %= 2; // x = x % 2
x **= 2; // x = x ** 2
```

### Operadores Lógicos

```javascript
let y = true && false; // AND lógico
let o = true || false; // OR lógico
let no = !true; // NOT lógico
```

## Propiedades y Métodos Importantes

### String

```javascript
let texto = "JavaScript";

texto.length; // Longitud de la cadena
texto.toUpperCase(); // Convierte a mayúsculas
texto.toLowerCase(); // Convierte a minúsculas
texto.includes("Java"); // Verifica si incluye "Java"
texto.indexOf("Script"); // Índice de la primera ocurrencia de "Script"
texto.replace("Java", "Type"); // Reemplaza "Java" por "Type"
texto.split(" "); // Divide la cadena en un arreglo
texto.substring(0, 4); // Subcadena del índice 0 al 4
```

### Number

```javascript
let numero = 123.456;

numero.toFixed(2); // Redondea a 2 decimales
numero.toString(); // Convierte a cadena
Number.isInteger(42); // Verifica si es un número entero
Number.parseFloat("123.456"); // Convierte cadena a número decimal
Number.parseInt("123.456"); // Convierte cadena a número entero
```

### Math

```javascript
Math.PI; // Propiedad PI
Math.round(4.7); // Redondea al número entero más cercano
Math.ceil(4.1); // Redondea hacia arriba
Math.floor(4.9); // Redondea hacia abajo
Math.sqrt(16); // Raíz cuadrada
Math.pow(2, 3); // Potencia de 2 elevado a 3
Math.random(); // Número aleatorio entre 0 y 1
Math.abs(-5); // Valor absoluto
```

## Estructuras Condicionales

### If-Else

```javascript
let a = 5;
if (a > 3) {
    console.log("a es mayor que 3");
} else {
    console.log("a no es mayor que 3");
}
```

### Operador Ternario

```javascript
let edad = 18;
let puedeVotar = (edad >= 18) ? "Sí" : "No"; // Si la edad es mayor o igual a 18, devuelve "Sí", de lo contrario, devuelve "No"
```

### Switch

```javascript
let x = 2;
switch (x) {
    case 1:
        console.log("x es 1");
        break;
    case 2:
        console.log("x es 2");
        break;
    default:
        console.log("x no es 1 ni 2");
}
```

## Estructuras Repetitivas

### For
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i); // Imprime los números del 0 al 4
}
```

### While
```javascript
let i = 0;
while (i < 5) {
    console.log(i); // Imprime los números del 0 al 4
    i++;
}
```

### Do-While
```javascript
let i = 0;
do {
    console.log(i); // Imprime los números del 0 al 4
    i++;
} while (i < 5);
```

### Break
```javascript
for (let i = 0; i < 10; i++) {
    if (i === 5) {
        break; // Sale del bucle cuando i es igual a 5
    }
    console.log(i);
}
```

### Continue
```javascript
for (let i = 0; i < 10; i++) {
    if (i === 5) {
        continue; // Salta a la siguiente iteración cuando i es igual a 5
    }
    console.log(i);
}
```

## Parseo de Datos
### Parseo de Cadenas a Números

```javascript
let cadenaNumerica = "123.45";
let numeroEntero = parseInt(cadenaNumerica); // 123
let numeroDecimal = parseFloat(cadenaNumerica); // 123.45
let numeroConNumber = Number(cadenaNumerica); // 123.45
```

### Parseo de Números a Cadenas

```javascript
let numero = 123;
let cadena = numero.toString(); // "123"
let cadenaConComillas = String(numero); // "123"
```
