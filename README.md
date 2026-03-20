# Laboratorio

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

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
R//

Describa en qué situación utilizó v-if y qué problema resuelve dentro de su
interfaz.
R//

Explique cómo se realiza la validación de datos en su aplicación y por qué es
importante validar la información ingresada por el usuario.
R//
