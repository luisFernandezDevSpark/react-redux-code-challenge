Utilizando el servicio de jsonplaceholder, la idea del ejercicio es crear una UI a 2 columnas. 
La columna izquierda muestra el listado de posts por título, cada item es clickeable.
La columna derecha muestra el detalle del item clickeado (title y body). El body tiene que poder ser editable. Para lograrlo, se debe renderear el contenido dentro de un textarea, y cuando el usuario da Enter, se dispara una acción de redux que realiza ésta llamada al servicio de jsonplaceholder: 'https://jsonplaceholder.typicode.com/posts/[POST_ID]', donde POST_ID es el id del post seleccionado, el método de la llamada debe ser 'PATCH' y el body del request debe ser un objecto { body: [TEXTAREA_VALUE] }, donde TEXTAREA_VALUE es el texto que el usuario escribió en el textarea.
Para la llamada al servicio se podría utilizar cualquier librería, como por ejemplo axios, pero recomiendo usar la función fetch() de javascript para evitarse instalar un paquete externo (los ejemplos de jsonplaceholde utilizan fetch())

Dentro de la carpeta src vas a encontrar principalmente 3 carpetas: actions, components y reducers.
Dentro de actions se encuentra el archivo posts.js, el cual tiene las funciones fetchPosts() y updatePost(postId), las cuales se deben completar para realizar las llamadas a la api de jsonplaceholder.
En la carpeta reducers, vas a encontrar posts.js, dentro del cual se debe crear la función que escuche las actions disparadas por fetchPosts y updatePost.
La carpeta components es donde se deben crear todos los componentes necesarios para la UI, que pueden ser la cantidad de quieras, mientras más mejor, pero mínimo 2 (uno para el listado de posteos, y otro para el detalle del posteo).

En cuanto a los estilos, la UI es bastante sencilla, tan sólo se debe respetar el layout (columna izquierda y derecha, separadas por una línea gris vertical), y cada item del listado separado por una línea gris horizontal. Cada item debe parecer clickeable al hacer hover sobre él. No hay una versión mobile del diseño, pero si podés hacerlo responsive (por ejemplo, implementando un hamburger menu para mostrar y esconder el listado de posts), es un gran plus.

Luego de clonar el repo, correr 'npm install' y luego 'npm run start' o 'yarn start' para levantar el proyecto.
Es importante no trabajar sobre la rama master, se debe crear una nueva rama con la siguiente nomenclatura [N]_[A]-dev, donde N es la inicial de tu nombre y A la de tu apellido (ej: Luis Fernández => L_F-dev)

UI
https://drive.google.com/file/d/16mCo5g3nirlOI2xjC2qVh4XJgGCq651V/view?usp=sharing

get all posts
https://jsonplaceholder.typicode.com/posts

more CRUDs
https://jsonplaceholder.typicode.com/guide.html