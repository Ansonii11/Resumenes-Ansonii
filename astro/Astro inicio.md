## Básico
1. [[Astro inicio]]
2. [[Componentes]]
3. [[Lazy Loading]]

## Propiedades

1. [[Astro Island]]
2. [[Tabla Componente.Etiquetas]]

Astro es un framework para la construcción de sitios webs estáticos centrado en el rendimiento y en la experiencia de desarrollo. 

### Astro Island

Se distinge por su arquitectura de [[Astro Island]] que priorisa la entrega de HTML estatico con la minima cantidad de js posible 

### Zero Js by default

El principal principio de astro es renderizar por omisión HTML estático durante el proceso de construcción eliminando cualquier Js que no sea estrictamente necesario para la funcionalidad interactiva

La funcionalidad interactiva se introduce estratégicamente con las [[Astro Island]] que permiten la hidratación selectiva del componentes específicos.
 
*La ausencia de Js por defecto no implica una limitación en la capacidad de astro de generar sitios web dinámicos*

### Componentes

En el nucleo de la arquitectura de Astro se encuentran los [[Componentes]], que actuan como los bloques de construccion escenciales de cada proyecto.

### Enrutado

Astro emplea un sistema de enrutamiento basado en la estructura de archivos dentro del directorio `src/pages/`, lo que simplifica la definicion de rutas en tu sitio web. 


