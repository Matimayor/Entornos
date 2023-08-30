## Analize el siguiente código señalando declaraciones y aplicaciones de reglas, y su efecto. 

```CSS
p#normal {
        font-family: arial,helvetica;
        font-size: 11px;
        font-weight: bold;
        }

*#destacado {
            border-style: solid;
            border-color: blue;
            border-width: 2px;
            }

#distinto {
            background-color: #9EC7EB;
            color: red;
          }
```
```HTML
<p id="normal">Este es un párrafo</p>

<p id="destacado">Este es otro párrafo</p>

<table id="destacado"><tr><td>Esta es una tabla</ td></tr></table>
<p id="distinto">Este es el último párrafo</p>
```

### Del código de CSS
En primer lugar las reglas para `p#normal`, donde este mismo es un selector que apunta a elementos `<p>` con un atributo `id` de "normal", y dentro tenemos:
- `font-family: arial, helvetica;`: establece que la fuente del texto en arial o Helvetica si estan disponibles en el sistema. 
- `font-size: 11px;`: Establece el tamaño de la fuente en 11 píxeles. 
- `font-weight: bold;`: Establece el peso de la fuente en negrita. 

Luego tenemos las reglas de `#destacado`,el cual es un selector que apunta a todos los elementos `*` con un atributo `id` de "destacado", y dentro de este podemos ver: 
- `border-style: solid;`: Establece el estilo de borde como sólido.
- `border-color: blue;`: Establece el color del borde en azul.
- `border-width: 2px;`: Establece el ancho del borde en 2 píxeles.

Y por último tenemos las reglas para `#distinto`, el mismo se trata de un selector que apunta a elemenbtos con un atributo `id` de "distinto", y podemos ver:
- `background-color: #9EC7EB;`: Establece el color de fondo en un tono de azul claro.
- `color: red;`: Establece el color del texto en rojo.

### Del código de HTML
De la aplicación de esta regla en html del código podemos decir que: 
```HTML
<p id="normal">Este es un párrafo</p>
```
Este párrafo tiene la fuente Arial o Helvetica, el tamaño de fuente de 11px y el texto en negrita por las reglas de `p#normal`. 

```HTML
<p id="normal">Este es un párrafo</p>
```
Este párrafo tiene un borde sólido azul de 2 píxeles debido a las reglas `*#destacado`

```HTML
<p id="normal">Este es un párrafo</p>
```
La tabla tiene un borde sólido azul de 2 píxeles debido a las reglas `*#destacado`
 
```HTML
<p id="normal">Este es un párrafo</p>
```
Este párrafo tiene un fondo azul claro y el texto en rojo debido a las reglas `#distinto`. 