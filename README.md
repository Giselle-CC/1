Clase 10: Repaso general

En esta clase vamos a repasar los conceptos aprendidos durante las clases anteriores, construyendo un template de aplicación desde cero. Este template será nuestro punto de partida para realizar el primer entregable de la materia (Clase 11).
Si bien nos va a acompañar el profe en el paso a paso, dejamos acá el flujo completo de trabajo.

Paso 1 - Inicializamos una aplicación con CRA

El primer paso consiste en iniciar un proyecto en React desde cero. Para ello, vamos a utilizar create-react-app, ejecutando el siguiente comando:

npx create-react-app template-react

(se puede cambiar el nombre del proyecto utilizando otro en vez de template-react)
Esperamos que se ejecute el script, el cual inicializa el proyecto e instalará las dependencias necesarias.
Una vez finalizado, vamos a levantar el proyecto:

cd template-react
npm start o yarn start

Con eso, mostramos a los estudiantes el proyecto corriendo localmente. Aprovechamos para recorrer la estructura de carpeta y archivos y podemos hacer algún cambio menor para mostrar cómo el mismo se ve reflejado inmediatamente en el navegador (hot reload).

Paso 2 - Construimos un componente <Card/>
En primer lugar, vamos a crear un archivo Card.jsx en donde crearemos nuestro primer componente, con un breve mensaje que nos permita visualizarlo en la aplicación:
import React from "react";




const Card = () => {
  return <div>Hola, soy una tarjeta</div>;
};


export default Card;



Se pueden agregar estilos y más información; lo esencial acá es poder repasar el concepto de componente y JSX.
Luego, vamos a importar el componente en nuestro componente <App/> para poder ver como él mismo aparece en la pantalla:
import Card from "./Card";


function App() {
  return (
    <div className="App">
      <Card />
    </div>
  );
}


export default App;



En este punto, la idea es repasar el concepto de componente padre e hijo y como se maneja este tipo de arquitectura en una aplicación hecha con React.
También podemos agregar alguna prop al componente Card y pasarla cuando lo utilizamos en el componente App, para repasar el concepto y utilización de props.

Paso 3 - Agregamos un formulario
Finalmente, lo que vamos a hacer es agregar un componente form dentro de <App/>:

import Card from "./Card";


function App() {
  return (
    <div className="App">
      <h1>Carga de estudiantes</h1>
      <form></form>
      <Card />
    </div>
  );
}


export default App;



Los alumnos van a trabajar sobre ese formulario en el entregable de la clase siguiente, por lo que idealmente no vamos a agregar código en esa parte. No obstante, es viable hacer algún repaso oral sobre los temas vistos en clase sobre el uso de formularios.

Paso 4 - Hacemos un commit y push en Github
Dado que los alumnos van a tener que subir el entregable a un repositorio para que pueda ser corregido, se pueden dedicar unos minutos a mostrar de qué manera subir el proyecto con los cambios realizados a Github y evacuar dudas sobre este proceso.
