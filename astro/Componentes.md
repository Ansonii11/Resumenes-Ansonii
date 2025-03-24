Los componentes en astro se dividen en 2 "Component Script" y "Component Template"

tambien se pueden declarar componentes espesificos en archivos separados como en react pero cada uno de esos archivos igualmente tendra dentro estos dos componentes

## Component Script

Este componente se delimita entre la sintaxis especifica `---`, alberga la lógica Js necesaria para la representación del componente, incluyendo *importaciones de otros componentes de astro o de frameworks externos como react, datos, llamadas a APIs y la importación de datos desde un Json* 
Además es en este componente donde se definen las variables que posteriormente se utilizaran para inyectar datos dinámicos a la plantilla

Este componente se escribe usando TypeScript

Este código Typescript se ejecuta en el servidor

**Ejemplo:** 
archivo: ejemplo.astro
```JavaScript
---
const mensaje = 'Hola, Astro!';
---

<h1>{mensaje}</h1>
```


## Component Template

Este componente se ubica justo después de el componente script y es la encargada de definir la salida HTML del componente. Esta plantilla soporta toda la sintaxis HTML, puede integrar expresiones de css y Js como mismo en el html o sea con la etiqueta `<style>` y `<script>`  pero tambien soporta elementos Js entre llaves `{}`. Esto permite la facil incorporacion de los elementos definidos en el componente script , también se añade en esta parte otros componentes importados y directivas del propio astro



La distinción entre la lógica del servidor y la presentación en la arquitectura de componentes en Astro facilita la creación de sitios web estaticos con la capacidad de incorporar interactividad de manera eficiente 