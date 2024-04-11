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
console.log('Mensaje de depuración');
console.error('Mensaje de error');
console.warn('Mensaje de advertencia');
console.info('Mensaje informativo');
console.clear
console.table(['Manzana', 'Banana', 'Naranja']);
console.time('Tiempo transcurrido');
console.timeEnd('Tiempo transcurrido');
console.group('Grupo de mensajes');
console.log('Mensaje 1');
console.log('Mensaje 2');
console.groupEnd();
```

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


