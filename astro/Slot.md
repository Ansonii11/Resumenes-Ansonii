

`<slot />` actúa como un marcador de posición dentro de la plantilla de un componente para la inserción de html externo con elementos hijo. esto permite crear componentes reutilizables cuya estructura general se mantiene pero cuyo contenido especifico puede variar dependiendo de el contexto en que se usen . Los Slot pueden ser nombrados con la propiedad `name`, facilitando la inserción de contenido en ubicaciones precisas.

Es posible definir contenido de FallBack dentro de una etiqueta slot que se renderizara por defecto en caso de que no se proporcione ningún elemento hijo para ese slot en particular