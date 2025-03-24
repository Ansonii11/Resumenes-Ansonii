Esto representa un paradigma en la construcción de sitios web modernos, permitiendo que sitios web estáticos y de carga rápida añadan islas interactivas y dinámicas

Una *Astro Island* se define como un componente de interfaz de usuario interactivo que recide en una paguina HTML que, en su mayor parte , es estatica. en una misma paguina pueden coexistir multiples islas, cada una de ellas se renderiza y se hidrata de forma independiente del resto del contenido.

## Client Islands

Son componentes de interfaz de usuario interactivos que se construyen usando frameworks como React y cuya interactividad se habilita mediante un proceso llamado hidratacion, esto ocurre en el navegador del cliente

Para indicarle a Astro que una island es una client Island y por lo tanto deve de cargarse en el Js del cliente se usan las directivas `client:*` y se espesifica bajo que condiciones a de cargar ejemplo:

`client: load` Esto hace que se carge tan pronto como la web haya cargado completamente. Deben de usarse en componentes que han de ser interactivos de inmediato

`client: idle` Esto hace que se carge y se ejecute solo si el navegador esta en un estado de inactividad

`client: visible` Retrasa la carga del Js hasta que el componente sea visible en la ventana del navegador del usuario.

`client: media={QUERY}` permite indicar una media query de css y el js solo se cargara solo cuando la media query se cumpla

`client: only={framework}` Indica que solo debe de renderisarse del lado del cliente y no debe de incluirse en el HTML estatico inicial renderizado en el servidor. Requiere espesificar un framework ejemplo react

### Ejemplo con react

```JavaScript
---
import MyReactComponent from '../components/MyReactComponent.jsx'
---

<MyReactComponent client:load message="hola mundo" />
```

## Server Islands

Son componentes de interfaz de usuario que renderizan su contenido dinamico en el servidor, de forma independiente del resto de la paguina 

La directiva principal asociada es `server:defer` que hace que Astro renderize inmediatamente el resto de la pagina, incluyendo cualquier contenido de fallback que se haya proporcionado 