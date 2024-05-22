> Antes de comenzar se debe advertir que mucho del contenido si lo usas para estudiar debe ser leido en la pagina oficial de NextJS ya que este contenido es solo un resumen de lo que se encuentra en la pagina oficial y además de mi interpretación del mismo, vas a poder ver los cambios realizados entre los commit que realize mientras este estudiando el contenido. Me encargo de colocarlo al español para poder acercar esta documentación a quienes no lideran el ingles. Desde ya muchas gracias si lees este comentario.

# Instalación previa

Antes de comenzar se debe instalar NodeJs

Luego de tener NodeJs instalado se debe instalar NextJs y su respositorio de ejemplo el cual se trata de una plantilla que se puede usar para comenzar a trabajar

Para instalar NextJs se debe correr el siguiente comando

```bash

npx create-next-app@latest nextjs-dashboard --use-npm --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example"

```

Este comando usa `npx` para correr el comando `create-next-app` y crear una nueva aplicacion de NextJs llamada `nextjs-dashboard` y usa el repositorio de ejemplo `

> npx es un paquete que viene con npm 5.2+ y superior. Su función es ejecutar paquetes de npm que no estan instalados en tu maquina local.

## Explorando el proyecto

Dentro del repositorio extradido desde el comando anterior se encontraran los siguientes archivos y carpetas

- /app: Contiene todas las rutas, componentes y logica de tu aplicacion, aqui es donde vas a trabajar mayormente
- /app/lib: Contiene funciones usadas en tu aplicacion, como funciones de utilidad reutilizables y funciones de obtencion de datos
- /app/ui: Contiene todos los componentes de UI para tu aplicacion, como tarjetas, tablas y formularios. Para ahorrar tiempo, se ha creado una serie de componentes de UI reutilizables para el estudiante.
- /public: Contiene todos los activos estaticos para tu aplicacion, como imagenes
- /scripts: Contiene un script de siembra que se usara para poblar tu base de datos en un capitulo posterior
- Archivos de configuracion: Tambien notaras archivos de configuracion como next.config.js en la raiz de tu aplicacion. La mayoria de estos archivos son creados y preconfigurados cuando inicias un nuevo proyecto usando create-next-app. No necesitaras modificarlos en este curso.

> El curso te invita a revisar las carpetas y archivos para que te familiarices con la estructura de la aplicacion y los archivos que contiene. Posiblemente adjunte archivo README.md dentro de cada carpeta que explore y las deje en las notas de este curso. Para que sirva de guía para futuras referencias de quienes encuentren este repositorio.

---

# Notas de las partes de Next Js

## Lanzar el servidor de desarrollo

Para lanzar el servidor de desarrollo, se debe correr el siguiente comando

```bash

npm run dev

```

Este comando inicia el servidor de desarrollo de Next.js en http://localhost:3000. La pagina se recargara automaticamente si se realiza algun cambio en el codigo.


## tsconfig.json

Este archivo es el archivo de configuracion de TypeScript. TypeScript es un superconjunto de JavaScript que agrega tipos a JavaScript. TypeScript es un lenguaje de programacion de codigo abierto desarrollado y mantenido por Microsoft. TypeScript es JavaScript con tipos. TypeScript es un lenguaje de programacion de codigo abierto desarrollado y mantenido por Microsoft. TypeScript es JavaScript con tipos.

## tailwind.config.ts

Este archivo es el archivo de configuracion de Tailwind CSS para tu aplicacion. Tailwind CSS es un marco de diseño de CSS utilitario de bajo nivel que te permite construir rapidamente disenos personalizados.

## postcss.config.js

Este archivo es el archivo de configuracion de PostCSS para tu aplicacion. PostCSS es una herramienta de posprocesamiento de CSS que te permite transformar estilos con JavaScript que utiliza tailwindcss para agregar prefijos de vendedor, minificar y optimizar tu CSS.

## package-lock.json

Este archivo es un archivo de bloqueo de versiones de npm. npm crea este archivo para asegurarse de que las versiones de los paquetes que se instalan en tu aplicacion sean las mismas que las versiones que se instalaron en tu maquina local.

## next.config.js

Este archivo es el archivo de configuracion de Next.js para tu aplicacion. Next.js es un marco de trabajo de React de codigo abierto que te permite construir aplicaciones web y aplicaciones web progresivas (PWA) con React.

## .gitignore

Este archivo es un archivo de exclusion de git. Git usa este archivo para determinar que archivos y carpetas no se deben incluir en el control de versiones.

## .eslintrc.json

Este archivo es el archivo de configuracion de ESLint para tu aplicacion. ESLint es una herramienta de analisis de codigo estatico para identificar problemas en el codigo JavaScript.

## package.json

Este archivo es el archivo de manifiesto de tu aplicacion. npm usa este archivo para almacenar metadatos sobre tu aplicacion, como el nombre de la aplicacion, la version de la aplicacion y las dependencias de la aplicacion.

# .nvmrc

Este archivo es un archivo de version de Node. nvm usa este archivo para determinar que version de Node.js se debe usar para tu aplicacion.

# ./scripts/seed.js

Este archivo es un script de siembra que se usara para poblar tu base de datos en un capitulo posterior.

# ./public

Esta carpeta contiene todos los activos estaticos para tu aplicacion, como imagenes.

# ./app

Esta carpeta contiene todas las rutas, componentes y logica de tu aplicacion. Aqui es donde vas a trabajar mayormente. Dentro de esta carpeta, encontraras las siguientes carpetas:

- ./app/lib: Contiene funciones usadas en tu aplicacion, como funciones de utilidad reutilizables y funciones de obtencion de datos.
- ./app/ui: Contiene todos los componentes de UI para tu aplicacion, como tarjetas, tablas y formularios. Para ahorrar tiempo, se ha creado una serie de componentes de UI reutilizables para el estudiante.

## page.tsx

Este archivo es un archivo de pagina de React. Next.js usa este archivo para renderizar paginas de React en tu aplicacion. 

## layout.tsx

Este archivo es un archivo de diseño de React. Next.js usa este archivo para envolver paginas de React en un diseno comun.

### ejemplo de layout.tsx con un borde sobre el contenido


```javascript

import React from 'react'; // importa la libreria de React

const Layout = ({ children }) => { // se crea un componente de React llamado Layout
    return ( // retorna el contenido de la pagina
        <div className="border border-gray-200"> // borde sobre el contenido
            {children} // children es un prop especial que representa el contenido de la pagina
        </div>
    );
};

export default Layout; // exporta el componente Layout

```


---

# Datos de marcador de posición

Cuando creas una interfaz de usuario, es útil tener algunos datos de marcador de posición. Si la base de datos o API no esta disponible, puedes:

- Crear un marcador de posición en formato JSON o en objetos de JavaScript
- Usa servicios de terceros como [mockAPI](https://mockapi.io/) o [JSONPlaceholder](https://jsonplaceholder.typicode.com/)

Para este proyecto, hemos proporcionado algunos datos de marcador de posición en app/lib/placeholder-data.js. Cada objeto JavaScript en el archivo representa una tabla en tu base de datos. Por ejemplo, para la tabla de facturas:
    
    ```javascript

    cont invoices = [ // array de objetos de facturas de clientes
        {
            customer_id: customers[0].id, // id del cliente 0
            amount: 15795, // cantidad
            status: 'pending', // estado
            date: '2022-21-06', // fecha
        },
        {
            customer_id: customers[1].id, // id del cliente 1
            amount: 20348, // cantidad
            status: 'pending', // estado
            date: '2022-11-14', // fecha
        },
        // lo que vemos dentro del Json es un ejemplo de como se veria un marcador de posición lo que muestra acerca de las facturas de los clientes
    ];
    ```
> Nota explicando lo que ocurre hasta el momento en el curso, se ha creado un proyecto de NextJS con un repositorio de ejemplo, se ha explorado la estructura de la aplicacion y se ha hablado de los datos de marcador de posición que se pueden usar para simular una base de datos en caso de que no se tenga una base de datos real. Se ha mostrado un ejemplo de como se veria un marcador de posición en formato JSON.

En el capítulo sobre la [configuración de tu base de datos(./06 - CAPITULO 6)], utilizarás estos datos para sembrar tu base de datos (poblarla con algunos datos iniciales).

# TypeScript

