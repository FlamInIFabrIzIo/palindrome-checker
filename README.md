# Palindrome Checker

Este proyecto es una aplicación web sencilla que permite verificar si un texto ingresado es un palíndromo. Fue desarrollado como parte de un ejercicio práctico para demostrar habilidades en desarrollo web y manipulación de DOM con JavaScript.

## Descripción

Un **palíndromo** es una palabra, frase, número u otra secuencia de caracteres que se lee igual de adelante hacia atrás que de atrás hacia adelante, ignorando espacios, puntuación y diferencias entre mayúsculas y minúsculas. Este proyecto toma un texto ingresado por el usuario, lo procesa para eliminar caracteres no alfanuméricos y verifica si es un palíndromo.

## Características

- **Interfaz amigable**: Una página web simple y limpia con un campo de entrada y un botón para realizar la verificación.
- **Validación de entrada**: Asegura que el usuario ingrese un texto válido antes de realizar la comprobación.
- **Resultados inmediatos**: Muestra un mensaje indicando si el texto ingresado es o no un palíndromo.

## Tecnologías utilizadas

- **HTML5**: Para la estructura de la página.
- **CSS3**: Para el diseño y estilo de la interfaz.
- **JavaScript**: Para la lógica de verificación y manipulación del DOM.

## Cómo usarlo

1. Abre el archivo `index.html` en tu navegador web.
2. Ingresa un texto en el campo de entrada.
3. Haz clic en el botón "Check".
4. Observa el resultado que se mostrará debajo del botón.

## Código principal

El núcleo de la funcionalidad está en la función `isPalindrome`, que realiza los siguientes pasos:

1. Limpia el texto ingresado eliminando caracteres no alfanuméricos y convirtiéndolo a minúsculas.
2. Invierte el texto limpio.
3. Compara el texto limpio con su versión invertida para determinar si es un palíndromo.

```javascript
function isPalindrome(str) {
  let cleaned = str.replace(/[^A-Za-z0-9]/g, "").toLowerCase();
  let reversed = cleaned.split("").reverse().join("");
  return cleaned === reversed;
}
```
