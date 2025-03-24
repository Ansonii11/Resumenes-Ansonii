
## Tabla de Contenido


| Componente/Etiquetas        | Descripcion                                                                                                                           | Propiedad clave                                                                                                   | Uso principal                                                                                                                                       |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<slot />` [[Slot]]         | Marcador de posición para contenido html externo, permitiendo la inyección de elementos hijo                                          | `name` para nombrar slots                                                                                         | Creación de componentes reutilizables y flexibles con contenido dinámico                                                                            |
| `<Fragment />` [[Fragment]] | Permite pasar varios elementos HTML en un mismo slot sin un div envolvente                                                            | `slot` para espesificar el slot al que pertenese                                                                  | Mantiene un html semánticamente limpio al evitar la introducción de `<div>` innecesarios al trabajar con slots                                      |
| `<Code />`                  | Proporciona resaltado de sintaxis para bloques de código en tiempo de build, sin JavaScript del lado del cliente                      | `code` codigo a resaltar.<br>`lang` Lenguaje.<br>`theme` tema del resaltado.<br>`wrap` habilitar ajustes de linea | Mostrar bloques de código en la documentación o en artículos técnicos de manera legible y profesional sin afectar el rendimiento del cliente        |
| `<Debug />`                 | Permite impeccionar valores de variable en el lado del cliente sin JavaScript                                                         |                                                                                                                   | Herramienta util para la depuracion                                                                                                                 |
| `<Image />`                 | Muestra verciones optimizadas de las imagenes y prebiene el **Cumulative Layout Shift (cls)**                                         | Las mismas que el img de html o sea `src`, `alt`, etc                                                             | Optimizacion del rendimiento de las imagenes, mejoras de la accesibilidad y prebencion de problemas de diseño relacionados con la carga de imagenes |
| `<Picture />`               | Crea imagenes responcivas con multiples formatos para una mejor compatibilidad y rendimiento en diferentes navegadores y dispocitivos | Las mismas que de `<Image />` añadiendo `formats` y propiedades avanzadas                                         | Entrega de imágenes optimizadas para diferentes contextos mejorando el rendimiento y la experiencia de usuario en varios dispositivos               |






