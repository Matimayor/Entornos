## Análisis de codigo
Dadas las siguientes declaraciones:
```CSS

* { color:green; }
    a:link {color:gray }
    a:visited{color:blue }
    a:hover {color:fuchsia }
    a:active {color:red }

p { font-family: arial,helvetica;
    font-size: 10px;
    color:black; }

.contenido{font-size: 14px;
           font-weight: bold; }

```
Analizar los siguientes códigos y comparar sus efectos: 

### Código a
```HTML
<body>
    <p class="contenido" style="font-weight: normal;">Este es un texto ...............</p>
    <table>
        <tr>
            <td>Y esta es una tabla.......</td>
        </tr>
        <tr>
            <td>
                <a href="http://www.google.com.ar">con un
                enlace
                </a>
            </td>
        </tr>
    </table>
</body>
```

### Código b
```HTML
<body class="contenido">
    <p> Este es un texto................</p>
    <table>
        <tr>
            <td>Y esta es una tabla.......</td>
        </tr>
        <tr>
            <td><a href="http://www.google.com.ar">con un enlace</a></td>
        </tr>
    </table>
</body>
```

En el código 1, el párrafo tiene la clase "contenido" y se aplica un estilo en línea `(style="font-weight: normal;")` que establece el peso de la fuente en "normal", en donde: 
- El texto dentro del párrafo tiene un color verde debido a la declaración `* {color:green; }`. 
- El párrafo tiene un tamaño de fuente de 14px (definido por `.contenido`), pero el peso de la fuente se establece en "normal" debido al estilo en línea, lo que anula a la negrita definida en `.contenido`. 

En el código 2, el cuerpo `(body)` tiene la clase "contenido", y el párrafo no tiene una clase adicional, en donde: 
- El cuerpo `(body)` tiene un clor de texto verde debido a la declaración `*{color:green;}`.
- El párrafo tiene un tamaño de fuente de 14px y un peso de fuente en negrita debido a la clase "contenido" definida `contenido`. 

Puntualmente comparando los códigos tenemos que: 
-  Ambos códigos tienen un tamaño de fuente de 14px y un color de texto verde para el contenido dentro del cuerpo debido a la declaración `* {color:green; }`. 
-  Sin embargo, en el código 1, el párrafo tiene su peso de fuente anulado y se establece en "normal" debido al estilo en línea `style="font-weight: normal;"`, mientras que en el código 2, el párrafo manteiene su negrita debido a la clase "contenido" dentro del cuerpo.
