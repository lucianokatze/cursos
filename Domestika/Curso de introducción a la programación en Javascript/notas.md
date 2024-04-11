# ¿Qué es JavaScript?

- **JavaScript** es un lenguaje de programación que se utiliza principalmente para crear páginas web interactivas. es un lenguaje de programación de alto nivel, interpretado, débilmente tipado y dinámico. Es un lenguaje de programación que se utiliza principalmente para crear páginas web interactivas del lado del cliente.

Javascript no tiene relación con Java (a pesar de que su nombre pueda llevar a confusión), es un lenguaje de programación independiente.

## ECMA Script

- **ECMAScript** es la especificación de un lenguaje de programación estándar, que se creó para estandarizar JavaScript. ECMAScript es el estándar en el que se basa JavaScript, y es el que se sigue para implementar JavaScript en los navegadores.

## ¿Qué se puede hacer con JavaScript?

- **JavaScript** se utiliza para crear páginas web interactivas, aplicaciones web, juegos, aplicaciones móviles, etc. Se puede utilizar para realizar diferentes tareas, como validar formularios, crear animaciones, manipular el DOM, enviar y recibir datos del servidor, etc.
    - **Validar formularios**: Se puede utilizar JavaScript para validar los datos que se introducen en un formulario antes de enviarlos al servidor.
    - **Crear animaciones**: Se puede utilizar JavaScript para crear animaciones en una página web, como animaciones de desplazamiento, animaciones de cambio de color, etc.
    - **Manipular el DOM**: Se puede utilizar JavaScript para manipular el DOM (Document Object Model) de una página web, es decir, para modificar los elementos de la página web, añadir nuevos elementos, eliminar elementos, etc.
    - **Enviar y recibir datos del servidor**: Se puede utilizar JavaScript para enviar y recibir datos del servidor, por ejemplo, para enviar datos de un formulario a un servidor y recibir una respuesta del servidor.
    - **Crear aplicaciones web**: Se puede utilizar JavaScript para crear aplicaciones web, es decir, aplicaciones que se ejecutan en un navegador web.
    - **Crear juegos**: Se puede utilizar JavaScript para crear juegos en línea, como juegos de plataformas, juegos de puzles, juegos de acción, etc.
    - **Crear aplicaciones móviles**: Se puede utilizar JavaScript para crear aplicaciones móviles, es decir, aplicaciones que se ejecutan en dispositivos móviles como smartphones y tabletas.


## Uso de Frameworks y Librerías

- **JavaScript** es un lenguaje de programación muy versátil y se puede utilizar para realizar una amplia variedad de tareas. Sin embargo, para algunas tareas específicas, puede ser útil utilizar un framework o una librería de JavaScript.
    - **Frameworks**: Un framework es un conjunto de herramientas y librerías que facilitan el desarrollo de aplicaciones web. Algunos ejemplos de frameworks de JavaScript son Angular, React y Vue.
        - **Angular**: Angular es un framework de JavaScript desarrollado por Google que se utiliza para crear aplicaciones web de una sola página (SPA).
        - **React**: React es una biblioteca de JavaScript desarrollada por Facebook que se utiliza para crear interfaces de usuario interactivas.
        - **Vue**: Vue es un framework de JavaScript que se utiliza para crear aplicaciones web interactivas y reactivas.
        - **Node.js**: Node.js es un entorno de ejecución de JavaScript que se utiliza para ejecutar código JavaScript en el servidor.
    - **Librerías**: Una librería es un conjunto de funciones y métodos que se pueden utilizar para realizar tareas específicas. Algunos ejemplos de librerías de JavaScript son jQuery, Lodash y Moment.js.
        - **jQuery**: jQuery es una librería de JavaScript que se utiliza para simplificar la manipulación del DOM, el manejo de eventos, las animaciones y las peticiones AJAX.
        - **Lodash**: Lodash es una librería de JavaScript que se utiliza para realizar operaciones de manipulación de datos de forma sencilla y eficiente.
        - **Moment.js**: Moment.js es una librería de JavaScript que se utiliza para manipular y formatear fechas y horas de forma sencilla y eficiente.

# Tipos de carga de javascript en Html

Los tipos de carga son para indicarle al navegador cómo debe cargar y ejecutar el script de JavaScript. Hay dos tipos de carga de JavaScript: carga sincrónica y carga asincrónica.

## Carga Sincrónica

- La carga sincrónica de JavaScript se produce cuando el navegador encuentra una etiqueta `<script>` en el HTML y detiene la carga de la página hasta que se haya descargado y ejecutado el script. Esto significa que el navegador no mostrará el contenido de la página hasta que se haya cargado y ejecutado el script.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Carga Sincrónica</title>
</head>
<body>
    <h1>Carga Sincrónica</h1>
    <script src="script.js"></script>
    <p>Este es un párrafo de ejemplo.</p>
</body>
</html>
```
# Carga Asincrónica

- La carga asincrónica de JavaScript se produce cuando el navegador encuentra una etiqueta `<script>` en el HTML con el atributo `async` o `defer`. Esto permite que el navegador continúe cargando la página mientras se descarga y ejecuta el script. El atributo `async` indica que el script se descargará y ejecutará de forma asíncrona, es decir, en paralelo con la carga de la página. El atributo `defer` indica que el script se descargará de forma asíncrona, pero se ejecutará después de que se haya cargado la página.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Carga Asincrónica</title>
</head>
<body>
    <h1>Carga Asincrónica</h1>
    <script src="script.js" async></script>
    <p>Este es un párrafo de ejemplo.</p>
</body>
</html>
```

# Uso de consola en JavaScript

- La consola de JavaScript es una herramienta que se utiliza para depurar y probar el código JavaScript en un navegador web. La consola permite mostrar mensajes de depuración, errores y advertencias, así como ejecutar comandos de JavaScript en tiempo real.

## Métodos de la consola

- **console.log()**: Muestra un mensaje en la consola.
- **console.error()**: Muestra un mensaje de error en la consola.
- **console.warn()**: Muestra un mensaje de advertencia en la consola.
- **console.info()**: Muestra un mensaje informativo en la consola.
- **console.clear()**: Limpia la consola.
- **console.table()**: Muestra una tabla en la consola.
- **console.time()**: Inicia un temporizador en la consola.
- **console.timeEnd()**: Detiene un temporizador en la consola y muestra el tiempo transcurrido.
- **console.group()**: Crea un grupo en la consola.
- **console.groupEnd()**: Cierra un grupo en la consola.

### Ejemplo de uso de la consola

```javascript
console.log('Mensaje de depuración'); // Se usa cuando se quiere mostrar un mensaje de depuración en la consola.
console.error('Mensaje de error'); // Se usa cuando se quiere mostrar un mensaje de error en la consola.
console.warn('Mensaje de advertencia'); // Se usa cuando se quiere mostrar un mensaje de advertencia en la consola.
console.info('Mensaje informativo'); // Se usa cuando se quiere mostrar un mensaje informativo en la consola.
console.clear (); // Se usa para limpiar la consola.
console.table(['Manzana', 'Banana', 'Naranja']); // Se usa para mostrar una tabla en la consola.
console.time('Tiempo transcurrido'); // Se usa para iniciar un temporizador en la consola.
console.timeEnd('Tiempo transcurrido'); // Se usa para detener un temporizador en la consola y mostrar el tiempo transcurrido.
console.group('Grupo de mensajes'); // Se usa para crear un grupo de mensajes en la consola.
console.log('Mensaje 1'); // Se usa para mostrar un mensaje en el grupo de mensajes.
console.log('Mensaje 2'); // Se usa para mostrar un mensaje en el grupo de mensajes.
console.groupEnd(); // Se usa para cerrar el grupo de mensajes en la consola.
```

### Ejemplos de uso de los console.log() y console.error()

```javascript
console.log('Hola, mundo!'); // Muestra el mensaje 'Hola, mundo!' en la consola.
console.error('Error: No se puede dividir por cero.'); // Muestra el mensaje de error 'Error: No se puede dividir por cero.' en la consola.
```

# Comentarios en JavaScript

- Los comentarios en JavaScript se utilizan para explicar el código y hacerlo más legible. Los comentarios son líneas de texto que se ignoran cuando se ejecuta el código. Los comentarios en JavaScript se pueden escribir de dos formas: con `//` para comentarios de una sola línea y con `/* */` para comentarios de varias líneas.

# Elementos de JavaScript y su sintaxis

## Variables

- Una variable es un contenedor que se utiliza para almacenar datos en un programa. En JavaScript, las variables se declaran con la palabra clave `var`, `let` o `const`, seguida de un nombre de variable y, opcionalmente, un valor inicial.

```javascript
var nombre = 'Luciano';
let edad = 30;
const PI = 3.1416;
```

### Diferencias entre tipos de variables 'var', 'let' y 'const'

- **var**: La palabra clave `var` se utilizaba para declarar variables en JavaScript antes de la introducción de `let` y `const`. Las variables declaradas con `var` tienen un ámbito de función, lo que significa que están disponibles en toda la función en la que se declaran.
- **let**: La palabra clave `let` se utiliza para declarar variables en JavaScript. Las variables declaradas con `let` tienen un ámbito de bloque, lo que significa que están disponibles solo dentro del bloque en el que se declaran.
- **const**: La palabra clave `const` se utiliza para declarar constantes en JavaScript. Las constantes declaradas con `const` tienen un ámbito de bloque y no se pueden reasignar.

### Ejemplos de uso de cada tipo de variable en casos avanzados

```javascript
// Ejemplo de uso de var en un bloque de código anidado
function ejemploVar() {
    if (true) {
        var mensaje = 'Hola, mundo!';
    }
    console.log(mensaje); // Salida: Hola, mundo!
}
ejemploVar();

// Ejemplo de uso de let en un bloque de código anidado con error de alcance de variable

function ejemploLet() {
    if (true) {
        let mensaje = 'Hola, mundo!';
    }
    console.log(mensaje); // Error: mensaje is not defined significa que la variable mensaje no está definida.
}
ejemploLet();

// Ejemplo de uso de const

const PI = 3.1416;
PI = 3.14; // Error: Assignment to constant variable. significa que no se puede reasignar una constante.
```


## Tipos de datos

- En JavaScript, los tipos de datos se dividen en dos categorías: tipos de datos primitivos y tipos de datos compuestos.

### Tipos de datos primitivos

- Los tipos de datos primitivos son los tipos de datos más básicos en JavaScript. Los tipos de datos primitivos son inmutables, lo que significa que una vez que se han creado, no se pueden modificar.

    - **String**: Cadena de texto.
    - **Number**: Número.
    - **Boolean**: Valor booleano (verdadero o falso).
    - **Null**: Valor nulo.
    - **Undefined**: Valor indefinido.
    - **Symbol**: Valor único e inmutable.
    - **BigInt**: Número entero de precisión arbitraria.
- Ejemplos de tipos de datos primitivos:

```javascript
let nombre = 'Luciano'; // String
let edad = 30; // Number
let esMayor = true; // Boolean
let nulo = null; // Null
let indefinido = undefined; // Undefined
let simbolo = Symbol('simbolo'); // Symbol
let numeroGrande = 1234567890123456789012345678901234567890n; // BigInt
```

### Tipos de datos compuestos

- Los tipos de datos compuestos son tipos de datos que pueden contener múltiples valores. Los tipos de datos compuestos son mutables, lo que significa que se pueden modificar después de haber sido creados.

    - **Array**: Colección ordenada de elementos.
    - **Object**: Colección de pares clave-valor.
    - **Function**: Bloque de código reutilizable.
- Ejemplos de tipos de datos compuestos:

```javascript
let colores = ['rojo', 'verde', 'azul']; // Array
let persona = {nombre: 'Luciano', edad: 30}; // Object
function saludar() {
    console.log('Hola, mundo!');
} // Function
```
## Funciones

- Una función es un bloque de código reutilizable que se utiliza para realizar una tarea específica. En JavaScript, las funciones se declaran con la palabra clave `function`, seguida de un nombre de función y, opcionalmente, una lista de parámetros.

```javascript
function saludar(nombre) {
    console.log('Hola, ' + nombre + '!');
}
saludar('Luciano'); // Salida: Hola, Luciano!
```

### Funciones de flecha

- Las funciones de flecha son una forma más concisa de escribir funciones en JavaScript. Las funciones de flecha se declaran con una flecha `=>` en lugar de la palabra clave `function`.
Los momentos en los cuales puedes usar funciones de flecha son:
    - Cuando la función no tiene parámetros.
    - Cuando la función tiene un solo parámetro.
    - Cuando la función tiene más de un parámetro.
    - Cuando la función tiene una sola línea de código.
    - Cuando la función tiene más de una línea de código.

```javascript
const saludar = (nombre) => {
    console.log('Hola, ' + nombre + '!');
}
saludar('Luciano'); // Salida: Hola, Luciano!
```

Ejemplo de una funcion de flecha usada en un `forEach`:

```javascript
let colores = ['rojo', 'verde', 'azul'];
colores.forEach(color => {
    console.log(color);
});
```

> **Nota**: Las funciones de flecha no tienen su propio `this`, `arguments`, `super` o `new.target`. Estas funciones son ideales para funciones que no necesitan acceder a estos valores.

## Condicionales

- Los condicionales se utilizan para tomar decisiones en un programa. En JavaScript, los condicionales se declaran con la palabra clave `if`, seguida de una condición y un bloque de código que se ejecutará si la condición es verdadera.

```javascript
let edad = 30;
if (edad >= 18) { // Si la condición es verdadera, se ejecuta el bloque de código dentro del if.
    console.log('Eres mayor de edad.');
} else { // Si la condición es falsa, se ejecuta el bloque de código dentro del else.
    console.log('Eres menor de edad.');
}
```

## Objetos y metodos de los objetos

- Un objeto es una colección de pares clave-valor. En JavaScript, los objetos se declaran con llaves `{}`, seguidas de una lista de propiedades y métodos separados por comas. 

```javascript
let persona = { // Declaración de un objeto persona.
    nombre: 'Luciano', // Propiedad del objeto persona.
    edad: 30, // Propiedades del objeto persona.
    saludar: function() { // Método del objeto persona.
        console.log('Hola, soy ' + this.nombre + ' y tengo ' + this.edad + ' años.'); // this se refiere al objeto persona.
    }
};
persona.saludar(); // Salida: Hola, soy Luciano y tengo 30 años.
```

## Acceso al DOM

- El DOM (Document Object Model) es una representación en forma de árbol de la estructura de un documento HTML. En JavaScript, se puede acceder al DOM y manipularlo utilizando métodos y propiedades del objeto `document`.

### Métodos de acceso al DOM

- **getElementById()**: Devuelve un elemento del DOM por su ID.
- **getElementsByClassName()**: Devuelve una colección de elementos del DOM por su clase.
- **getElementsByTagName()**: Devuelve una colección de elementos del DOM por su etiqueta.
- **querySelector()**: Devuelve el primer elemento del DOM que coincide con un selector CSS.
- **querySelectorAll()**: Devuelve una colección de elementos del DOM que coinciden con un selector CSS.

### Ejemplos de acceso al DOM

```html
<!DOCTYPE html>
<html>
<head>
    <title>Acceso al DOM</title>
</head>
<body>
    <h1 id="titulo">Título de la página</h1>
    <p class="parrafo">Este es un párrafo de ejemplo.</p>
    <ul>
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
    </ul>
    <script>
        // Acceso al DOM
        let titulo = document.getElementById('titulo');
        let parrafos = document.getElementsByClassName('parrafo');
        let elementos = document.getElementsByTagName('li');
        let primerParrafo = document.querySelector('.parrafo');
        let listaElementos = document.querySelectorAll('li');
        console.log(titulo.textContent); // Salida: Título de la página
        console.log(parrafos[0].textContent); // Salida: Este es un párrafo de ejemplo.
        console.log(elementos[0].textContent); // Salida: Elemento 1
        console.log(primerParrafo.textContent); // Salida: Este es un párrafo de ejemplo.
        listaElementos.forEach(elemento => {
            console.log(elemento.textContent);
        });
    </script>
</body>
</html>
```

## Eventos

- Los eventos son acciones que se producen en un documento HTML, como hacer clic en un botón, mover el ratón sobre un elemento, etc. En JavaScript, se pueden manejar los eventos utilizando métodos y propiedades del objeto `document`.

### Métodos de manejo de eventos

- **addEventListener()**: Agrega un evento a un elemento del DOM.
- **removeEventListener()**: Elimina un evento de un elemento del DOM.

### Ejemplos de manejo de eventos

```html
<!DOCTYPE html>
<html>
<head>
    <title>Eventos</title>
</head>
<body>
    <button id="boton">Haz clic aquí</button>
    <script>
        // Manejo de eventos
        let boton = document.getElementById('boton');
        boton.addEventListener('click', function() {
            alert('Haz hecho clic en el botón.');
        });
    </script>
</body>
</html>
```

## Ciclos

- Los ciclos se utilizan para repetir una serie de instrucciones en un programa. En JavaScript, se pueden utilizar ciclos `for`, `while` y `do...while` para repetir una serie de instrucciones.

### Ciclo for

- El ciclo `for` se utiliza para repetir una serie de instrucciones un número determinado de veces. El ciclo `for` consta de tres partes: una inicialización, una condición y una expresión de incremento.

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i); // Salida: 0, 1, 2, 3, 4
}
```

### Ciclo while

- El ciclo `while` se utiliza para repetir una serie de instrucciones mientras una condición sea verdadera.

```javascript
let i = 0;
while (i < 5) {
    console.log(i); // Salida: 0, 1, 2, 3, 4
    i++;
}
```

### Ciclo do...while

- El ciclo `do...while` se utiliza para repetir una serie de instrucciones al menos una vez y luego mientras una condición sea verdadera.

```javascript
let i = 0;
do {
    console.log(i); // Salida: 0
    i++;
} while (i < 0);
```

## Arrays

- Un array es una colección ordenada de elementos que se almacenan en una variable. En JavaScript, los arrays se declaran con corchetes `[]`, seguidos de una lista de elementos separados por comas.

```javascript
let colores = ['rojo', 'verde', 'azul'];
console.log(colores[0]); // Salida: rojo
console.log(colores[1]); // Salida: verde
console.log(colores[2]); // Salida: azul
```

### Métodos de los arrays

- **push()**: Agrega un elemento al final del array.
- **pop()**: Elimina el último elemento del array.
- **shift()**: Elimina el primer elemento del array.
- **unshift()**: Agrega un elemento al principio del array.
- **splice()**: Agrega o elimina elementos de un array en una posición específica.
- **slice()**: Devuelve una parte de un array como un nuevo array.
- **concat()**: Combina dos o más arrays en un nuevo array.
- **join()**: Convierte un array en una cadena de texto.
- **reverse()**: Invierte el orden de los elementos de un array.
- **sort()**: Ordena los elementos de un array.

### Ejemplos de uso de los métodos de los arrays

```javascript
let colores = ['rojo', 'verde', 'azul'];
colores.push('amarillo'); // Agrega 'amarillo' al final del array.
colores.pop(); // Elimina 'amarillo' del final del array.
colores.shift(); // Elimina 'rojo' del principio del array.
colores.unshift('naranja'); // Agrega 'naranja' al principio del array.
colores.splice(1, 0, 'blanco'); // Agrega 'blanco' en la posición 1 del array.
colores.splice(2, 1); // Elimina el elemento en la posición 2 del array.
let colores2 = colores.slice(1, 3); // Devuelve ['verde', 'azul'].
let colores3 = colores.concat(colores2); // Combina colores y colores2 en un nuevo array.
let colores4 = colores.join(', '); // Convierte colores en 'verde, azul'.
colores.reverse(); // Invierte el orden de los elementos de colores.
colores.sort(); // Ordena los elementos de colores alfabéticamente.
```

## Métodos de los strings

- Los strings son cadenas de texto que se utilizan para almacenar y manipular texto en un programa. En JavaScript, los strings se declaran con comillas simples `' '` o dobles `" "`. Los strings tienen una serie de métodos que se pueden utilizar para manipularlos.

### Métodos de los strings

- **length**: Devuelve la longitud de un string.
- **toUpperCase()**: Convierte un string a mayúsculas.
- **toLowerCase()**: Convierte un string a minúsculas.
- **charAt()**: Devuelve el carácter en una posición específica de un string.
- **indexOf()**: Devuelve la posición de la primera ocurrencia de un carácter en un string.
- **lastIndexOf()**: Devuelve la posición de la última ocurrencia de un carácter en un string.
- **includes()**: Devuelve `true` si un string contiene un carácter específico, de lo contrario, devuelve `false`.
- **startsWith()**: Devuelve `true` si un string comienza con un carácter específico, de lo contrario, devuelve `false`.
- **endsWith()**: Devuelve `true` si un string termina con un carácter específico, de lo contrario, devuelve `false`.

### Ejemplos de uso de los métodos de los strings

```javascript
let nombre = 'Luciano';
console.log(nombre.length); // Salida: 7
console.log(nombre.toUpperCase()); // Salida: LUCIANO
console.log(nombre.toLowerCase()); // Salida: luciano
console.log(nombre.charAt(0)); // Salida: L
console.log(nombre.indexOf('c')); // Salida: 2
console.log(nombre.lastIndexOf('c')); // Salida: 3
console.log(nombre.includes('a')); // Salida: true
console.log(nombre.startsWith('L')); // Salida: true
console.log(nombre.endsWith('o')); // Salida: true
```

## Operadores

- Los operadores se utilizan para realizar operaciones en un programa. En JavaScript, se pueden utilizar operadores aritméticos, de asignación, de comparación, lógicos y de concatenación.

### Operadores aritméticos

- **+**: Suma dos valores.
- **-**: Resta dos valores.
- **\***: Multiplica dos valores.
- **/**: Divide dos valores.
- **%**: Devuelve el resto de una división.

### Operadores de asignación

- **=**: Asigna un valor a una variable.
- **+=**: Suma un valor a una variable.
- **-=**: Resta un valor a una variable.
- **\*=**: Multiplica un valor a una variable.
- **/=**: Divide un valor a una variable.
- **%=**: Asigna el resto de una división a una variable.

### Operadores de comparación

- **==**: Compara dos valores y devuelve `true` si son iguales.
- **!=**: Compara dos valores y devuelve `true` si son diferentes.
- **===**: Compara dos valores y devuelve `true` si son iguales en valor y tipo.
- **!==**: Compara dos valores y devuelve `true` si son diferentes en valor o tipo.
- **>**: Devuelve `true` si el primer valor es mayor que el segundo.
- **<**: Devuelve `true` si el primer valor es menor que el segundo.
- **>=**: Devuelve `true` si el primer valor es mayor o igual que el segundo.
- **<=**: Devuelve `true` si el primer valor es menor o igual que el segundo.

### Operadores lógicos

- **&&**: Devuelve `true` si ambos valores son `true`.
- **||**: Devuelve `true` si al menos uno de los valores es `true`.
- **!**: Devuelve `true` si el valor es `false`.

### Operadores de concatenación

- **+**: Concatena dos strings.

### Ejemplos de uso de los operadores

```javascript
let a = 5;
let b = 3;
console.log(a + b); // Salida: 8
console.log(a - b); // Salida: 2
console.log(a * b); // Salida: 15
console.log(a / b); // Salida: 1.6666666666666667
console.log(a % b); // Salida: 2
let c = 10;
c += 5; // c = c + 5
c -= 5; // c = c - 5
c *= 5; // c = c * 5
c /= 5; // c = c / 5
c %= 5; // c = c % 5
let d = 5;
let e = '5';
console.log(d == e); // Salida: true
console.log(d === e); // Salida: false
console.log(d > b); // Salida: true
console.log(d < b); // Salida: false
console.log(d >= b); // Salida: true
console.log(d <= b); // Salida: false
let f = true;
let g = false;
console.log(f && g); // Salida: false
console.log(f || g); // Salida: true
console.log(!f); // Salida: false
let h = 'Hola, ';
let i = 'mundo!';
console.log(h + i); // Salida: Hola, mundo!
```

## Clases

- Una clase es una plantilla para crear objetos en un programa. En JavaScript, las clases se declaran con la palabra clave `class`, seguida de un nombre de clase y un bloque de código que define las propiedades y métodos de la clase.

```javascript
class Persona { // Declaración de una clase Persona.
    constructor(nombre, edad) { // Constructor de la clase Persona.
        this.nombre = nombre; // Propiedad nombre de la clase Persona.
        this.edad = edad; // Propiedad edad de la clase Persona.
    }
    saludar() { // Método saludar de la clase Persona.
        console.log('Hola, soy ' + this.nombre + ' y tengo ' + this.edad + ' años.'); // this se refiere a la clase Persona.
    }
}
let persona = new Persona('Luciano', 30); // Creación de un objeto persona.
persona.saludar(); // Salida: Hola, soy Luciano y tengo 30 años.
```

### Herencia

- La herencia es un mecanismo que permite a una clase heredar propiedades y métodos de otra clase. En JavaScript, se puede utilizar la palabra clave `extends` para heredar una clase.

```javascript
class Empleado extends Persona {
    constructor(nombre, edad, cargo) {
        super(nombre, edad);
        this.cargo = cargo;
    }
    presentarse() {
        console.log('Hola, soy ' + this.nombre + ' y trabajo como ' + this.cargo + '.');
    }
}
let empleado = new Empleado('Luciano', 30, 'Desarrollador');
empleado.saludar(); // Salida: Hola, soy Luciano y tengo 30 años.
empleado.presentarse(); // Salida: Hola, soy Luciano y trabajo como Desarrollador.
```

