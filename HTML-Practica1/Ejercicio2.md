# Ejercitación 2

HTML está compuesto por un conjunto de elementos que son la base de su estructura. Los elementos 
están compuestos por dos tags (el de apertura y el de cierre) y el contenido en el medio (con excepción de los elementos vacíos ). Cada tag puede tener atributos (proporcionan ciertas características como altura, ancho, color, etc.) y eventos (asocian un script que se ejecuta cuando el evento ocurre).
Analizar los siguientes segmentos de código indicando en qué sección del documento HTML se colocan, cuál es el efecto que producen y señalar cada uno de los elementos, etiquetas, y atributos 
(nombre y valor), aclarando si es obligatorio.

### Inciso a
```html
<!-- Código controlado el día 12/08/2009 --&gt;-->
```
En este caso, nos encontramos frente a un comentario. Los comentarios pueden ser insertados en cualquier parte del código HTML, y son utilizados para que los programadores puedan dejar anotaciones que ayuden a otros a entender lo que está ocurriendo en esa porción de código. También se emplean para señalar dónde comienza una función específica o para explicar el propósito de una función en particular. En resumen, los comentarios son una buena práctica, especialmente cuando se trabaja en equipo con otros programadores, o simplemente para mantener una organización personal y dejar registros de diversas situaciones relacionadas con el código.

Para utilizar un comentario, debemos encapsular el texto que queremos comentar entre `<!-- Esto es un comentario -->`. De esta forma, el editor de código entenderá que no es una línea de código funcional, sino más bien una explicación o nota que no afectará el comportamiento del programa.


### Inciso b
```html
<div id="bloque1">Contenido del bloque1</div>
```
El fragmento de código que se presenta es un elemento contenedor, generalmente utilizado dentro del elemento *body* de la estructura de una página HTML. No obstante, también es común utilizarlo en otras secciones como el *header* o *footer*.

Este elemento tiene diversas funciones. Una de ellas es la capacidad de **agrupar contenido**. Esto nos permite reunir imágenes, texto, enlaces y otros elementos para aplicarles un mismo estilo o comportamiento. Otra función es la de **estructurar la página**, dividiéndola en secciones que faciliten el mantenimiento y la aplicación de estilos. Asimismo, se utiliza para **aplicar estilos** uniformes. Al agrupar elementos, podemos aplicar un estilo común a todos ellos, controlando aspectos como el tamaño, color y estilo.

Para utilizar este elemento, debemos referenciarlo utilizando la etiqueta `<div>` y luego cerrarla con `</div>`. Es posible agregar atributos antes del cierre de la etiqueta, como en el ejemplo proporcionado, donde encontramos el atributo `id="bloque1"`. Estos atributos no son obligatorios en el código, pero pueden proporcionar información adicional o configurar características específicas de los elementos HTML.


### Inciso c
```html
<img src="" alt="lugar imagen" id="im1" name="im1" width="32" height="32" longdesc="detalles.htm" />
```
El siguiente fragmento es una etiqueta de imagen con varios atributos que explicaremos a continuación. Esta etiqueta puede ser utilizada en cualquier parte del código, ya sea en el *body*, *header* o *footer*.

El atributo obligatorio es ***src***, donde se proporciona la ruta o URL de la imagen que se desea mostrar. Sin este atributo, la imagen no se visualizará.

Los demás atributos son opcionales, y a continuación explicaremos la función de cada uno:
- ***alt***: Este atributo se utiliza para ofrecer una descripción alternativa de la imagen. Es útil cuando la imagen no puede cargarse, para usuarios que utilizan lectores de pantalla o cuando la carga de imágenes está desactivada en el navegador.
- ***id***: Proporciona a la imagen un identificador único, que permite referirse específicamente a ese elemento en el documento o desde hojas de estilos o scripts. Cada id debe ser único en el documento.
- ***name***: En este caso, no tiene ningún significado ni funcionalidad. El atributo name se utiliza en otros elementos HTML como `<input>`, `<select>` o `<textarea>` para especificar nombres para esos elementos.
- ***width***: Este atributo se usa para definir el ancho de la imagen en píxeles. Proporciona al navegador información sobre el tamaño real de la imagen antes de cargarla, lo que permite reservar el espacio adecuado.
- ***height***: Similar al atributo width, este atributo se utiliza para establecer la altura de la imagen en píxeles, permitiendo controlar su tamaño en la presentación visual de la página.
- ***longdesc***: Este atributo proporciona una descripción detallada y extensa de la imagen. Su objetivo principal es ofrecer información adicional que no puede ser adecuadamente expresada en el atributo `alt` o para complementar la información que ya contiene.

### Inciso d
```html
<meta name="keywords" lang="es" content="casa, compra, venta, alquiler " />
```
Esta línea de código utiliza dos metaetiquetas para proporcionar información adicional sobre la página web de manera específica:
- `name="keywords"`: Esta metaetiqueta se emplea para especificar una lista de palabras clave que están relacionadas con el contenido de la página. Esta lista ayuda a los motores de búsqueda a entender de qué trata la página, lo que puede mejorar la indexación y el posicionamiento de los resultados en las búsquedas.
- `lang="es"`: Esta metaetiqueta se usa para indicar el idioma principal de la página, en este caso, español.
- `content="casa, compra, venta, alquiler"`: El atributo `content` contiene una lista de palabras clave separadas por comas. Esta información se incorpora dentro del documento y complementa la metaetiqueta `keywords`.


```html
<meta http-equiv="expires" content="16-Sep-2019 7:49 PM" />
```
Esta línea de código utiliza la metaetiqueta `http-equiv` para proporcionar información de cabecera HTTP adicional en la página. Se emplean los siguientes atributos:
- `http-equiv="expires"`: Al utilizar `"expires"`, se instruye al navegador a considerar cuándo la página ha caducado o expirado.
- `content="16-Sep-2019 7:49 PM"`: Este atributo especifica el valor para la cabecera HTTP simulada. En este caso, establece la fecha y hora de expiración en la fecha indicada, indicando que después de esa fecha y hora, el navegador debe considerar que la página ha caducado y podría mostrar una versión más actualizada.

### Inciso e
```html
<a href="http://www.e-style.com.ar/resumen.html" type="text/html" hreflang="es" charset="utf-8" rel="help">Resumen HTML </a>
```
Esta parte del código crea un enlace que dirige al usuario a la página indicada en español. Veamos lo que hace cada atributo:
- `href="http://www.e-style.com.ar/resumen.html"`: Este atributo se emplea para especificar la URL o dirección a la que llevará el enlace.
- `type="text/html"`: Indica el tipo de contenido presente en la URL del enlace. En este caso, denota que el contenido de la página es HTML.
- `hreflang="es"`: Se utiliza para definir el idioma del recurso al que apunta el enlace, que en este caso es español.
- `charset="utf-8"`: Este atributo se emplea para especificar la codificación de caracteres del recurso al que apunta el enlace. Al ser `"utf-8"`, se trata de una codificación ampliamente utilizada y compatible con la mayoría de los idiomas y caracteres.
- `rel="help"`: Indica la relación del enlace con la página actual. Al establecerse como `"help"`, se señala que el enlace proporciona ayuda o información complementaria al contenido de la página actual.
- `Resumen HTML`: Este texto será visible para el usuario y representa la parte en la que se debe hacer clic para ser redirigido a la URL indicada en el atributo `href`.

### Inciso f
```html
<table width="200" summary="Datos correspondientes al ejercicio vencido">
<caption align="top"> Título </caption>
<tr>
<th scope="col">&nbsp;</th>
<th scope="col">A</th>
<th scope="col">B</th>
<th scope="col">C</th>
</tr>
<tr>
<th scope="row">1º</th>
<td>&nbsp;</td>
<td>&nbsp;</td>
<td>&nbsp;</td>
</tr>
<tr>
<th scope="row">2º</th>
<td>&nbsp;</td>
<td>&nbsp;</td>
<td>&nbsp;</td>
</tr>
</table>
```
Este código representa una tabla en HTML. Explicaremos el propósito de cada parte del código de manera específica:
- `<table width="200" summary="Datos correspondientes al ejercicio vencido">`: Aquí se abre la etiqueta `<table>` con dos atributos:
    - `width="200"`: Define el ancho de la tabla en 200 píxeles, lo que indica un ancho fijo de 200 píxeles.
    - `summary="Datos correspondientes al ejercicio vencido"`: El atributo `summary` brinda una descripción resumida de la tabla, que puede ser utilizada por lectores de pantalla y otros dispositivos de asistencia para entender la estructura y el propósito de la tabla.
- `<caption align="top"> Título </caption>`: Aquí se emplea la etiqueta `<caption>` para ofrecer un título o descripción a la tabla. El texto "Título" se presenta como título de la tabla. El atributo `align="top"` alinea el título en la parte superior de la tabla.
- `<tr>`: Esta etiqueta representa una fila de la tabla. Cada fila contiene celdas que pueden ser encabezados `<th>` o datos `<td>`.
- `<th scope="col">&nbsp;</th>`: Aquí se crea una celda de encabezado `<th>` para la columna. El atributo `scope="col"` indica que esta celda es un encabezado de columna. El contenido de la celda es un espacio en blanco `&nbsp;`, lo que resulta en una celda vacía en la primera columna del encabezado.
- `<th scope="row">1º</th>`: En esta línea, se crea una celda de encabezado para la primera fila `<th scope="row">`. El atributo `scope="row"` indica que esta celda es un encabezado de fila. El contenido de la celda es "1º", que representa el encabezado de la primera fila.
- `<td>&nbsp;</td>`: Aquí se generan celdas de datos `<td>` en la tabla. Cada celda de datos contiene un espacio en blanco `&nbsp;`, lo que crea celdas vacías en la tabla.






