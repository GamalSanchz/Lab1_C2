Situación problemática
En muchas escuelas, el control de materiales como libros, útiles y equipos se realiza de manera manual en cuadernos o hojas sueltas. Esto provoca errores frecuentes, pérdidas de recursos y dificultad para saber qué materiales están disponibles. La falta de un sistema organizado afecta tanto a los docentes como al personal administrativo, generando retrasos y desorden.

Sectores beneficiados
Educación: Escuelas, colegios y centros de formación.

Administrativo: Personal encargado de bodegas y suministros.

Docentes y estudiantes: Acceso más rápido y confiable a los materiales necesarios.

Funciones de la solución web
La página web propuesta resolverá el problema mediante las siguientes funciones:

Registro de materiales

Ingreso de nuevos artículos con nombre, cantidad y categoría.

Actualización de existencias en tiempo real.

#############################################
#RESPUESTAS
Explique con sus propias palabras qué es Vue.js y cuál es su función dentro de la
página web desarrollada.
R// Vue.js es un framework de JavaScript que permite crear páginas dinámicas. En la aplicación controla la interacción entre los datos y la interfaz, actualizando la lista de materiales en tiempo real.

Describa qué variables reactivas utilizó en su aplicación y cuál es la función de
cada una dentro del sistema.
R//nuevoNombre guarda el nombre del material, nuevaCategoria almacena la categoría, nuevaCantidad registra la cantidad, inventario lista de materiales registrados, Errores envia mensajes de validación para campos vacíos o incorrectos.

Explique la diferencia entre las siguientes directivas utilizadas en su proyecto: v-
bind y v-model
R//v-bind enlaza atributos HTML con valores dinámicos y v-model conecta inputs con variables, permitiendo entrada y salida de datos en tiempo real.

Mencione al menos un ejemplo de evento utilizado dentro de su aplicación.
R//@submit.prevent="agregarMaterial"

Este evento se activa cuando el usuario hace clic en el botón Agregar dentro del formulario. Su función es evitar que la página se recargue y, en su lugar, ejecutar el método agregarMaterial, que valida los datos y añade el nuevo material al inventario.

Explique para qué utilizó la directiva v-for dentro de su aplicación.
R//La usamos para mostrar la lista de materiales del inventario, básicamente le digo a Vue: "por cada material que haya guardado, muéstrame una fila en la tabla con su nombre, categoría y cantidad". Sin v-for tendría que escribir cada fila a mano, lo cual no tiene sentido si los datos cambian dinámicamente

Describa en qué situación utilizó v-if y qué problema resuelve dentro de su
interfaz.
R//La usamos en dos momentos: primero para mostrar la tabla solo cuando hay materiales registrados, y segundo para mostrar los mensajes de error cuando el usuario deja un campo vacío o ingresa una cantidad inválida, el problema que resuelve es evitar mostrar una tabla vacía o confusa al usuario en cambio, aparece el mensaje "No hay materiales registrados" hasta que realmente haya algo que mostrar


Alumno: Brandom Gamaliel Sànchez Guevara
Alumno: Cristian Alexis Velasquez Hernàndez

Explique cómo se realiza la validación de datos en su aplicación y por qué es
importante validar la información ingresada por el usuario.
R//Cuando el usuario hace clic en "Agregar", primero se ejecuta una función que revisa que ningún campo esté vacío y que la cantidad sea mayor a cero, pero si algo está mal, se muestra un mensaje de error en rojo justo debajo del campo correspondiente y no se agrega nada al inventario, su importancia radica en que sin validación cualquier persona podría guardar datos incompletos o sin sentido, lo que arruinaría la información del sistema
