## Analize el siguiente código señalando declaraciones y aplicaciones de reglas, y su efecto. 

```CSS
p.quitar {
            color: red;
         }

*.desarrollo {
                font-size: 8px;
             }

.importante {
                font-size: 20px;
            }
```
``` HTML
<p class="desarrollo"> 
En este primer párrafo trataremos lo siguiente:
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</p>

<p class="quitar">
Este párrafo debe ser quitado de la obra…
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</p>

<p >
En este otro párrafo trataremos otro tema:<br />
xxxxxxxxxxxxxxxxxxxxxxxxx
</p>

<p class="importante">
Y este es el párrafo más importante de la obra…
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</ p>

<h1 class="quitar">Este encabezado también debe ser quitado de la obra</h1>

<p class="quitar importante">Se pueden aplicar varias clases a la vez</p>
```

### Del código de CSS
En primer lugar vemos el selector `p.quitar` que apunta a elementos `<p>` con la clase "quitar", donde solamente se establece el color de texto en rojo para los párrafos con esta clase. 

Luego aparece la regla para `*.desrrollo` la cual se trata de un selector que apunta a todos los elementos `*` con la clase "desarrollo", en donde solamente se establece el tamaño de fuente en 8 píxeles.

Por último, el selector que apunta a elementos con la clase "importante", en donde solo se establece el tamaño de fuente en 2o píxeles para los elementos con esta clse.

### Del código de HTML
``` HTML
<p class="desarrollo"> 
En este primer párrafo trataremos lo siguiente:
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</p>
```
Este párrafo tiene un tamaño de fuente de 8px debido a las reglas de `*.desarrollo`. 

``` HTML
<p class="quitar">
Este párrafo debe ser quitado de la obra…
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</p>
```
Este párrafo tiene un color de texto en rojo por la etiqueta `p.quitar`. 

``` HTML
En este otro párrafo trataremos otro tema:<br />
xxxxxxxxxxxxxxxxxxxxxxxxx
```
Este párrafo no tiene ninuna clase asociada por lo que no se aplican reglas definidas.

``` HTML
<p class="importante">
Y este es el párrafo más importante de la obra…
<br />xxxxxxxxxxxxxxxxxxxxxxxxx
</ p>
```
Este párrafo tiene un tamaño de fuente de 20px debido a la regla `importante`. 

``` HTML
<h1 class="quitar">Este encabezado también debe ser quitado de la obra</h1>
```
Este encabezado tiene el color de texto en rojo debido a las reglas `p.quitar`. 

``` HTML
<p class="quitar importante">Se pueden aplicar varias clases a la vez</p>
``` 
Este párrafo tiene el color de texto en rojo debido a las reglas `p.quitar`, pero también tiene un tamaño de fuente de 20px debido a las reglas `.importante`.  
