# Ejercitación 1 
## Responder el siguiente cuestionario

1.  ¿Qué es HTML, cuando fue creado, cuáles fueron las disntintas versiones y cuál es la última?

HTML, del inglés HyperText Markup Language, es un lenguaje de marcado para la creación de páginas web. Además de ser un estándar que sirve de referencia para el software relacionado con la creación de páginas web en sus diferentes versiones. Este lenguaje define una estructura básica y un conjunto de códigos para definir el contenido de una página web, que puede incluir texto, imágenes, videos, juegos, entre otros.

HTML tuvo sus inicios en la década de 1990 y ha pasado por una serie de revisiones y extensiones. Las primeras versiones y experimentos tuvieron lugar en el CERN (Organización Europea para la Investigación Nuclear). No obstante, el primer intento de HTML en 1995 resultó en HTML 3.0, que fue un esfuerzo frustrado. Sin embargo, esto llevó a un enfoque más pragmático conocido como HTML 3.2, que se completó en 1997. Pocos meses después de ese año, se introdujo HTML 4.01.

Posteriormente, se trabajaron en otros proyectos, lo que detuvo la actualización de nuevas versiones de HTML hasta 2006. En ese momento, comenzó a surgir el interés por desarrollar una nueva versión: HTML 5.0. Diversas empresas empezaron a trabajar en su desarrollo y, finalmente, en 2016, se presentó HTML5, convirtiéndose en el estándar para el lenguaje de la web. 

2. ¿Cuáles son los principios básicos que el W3C recomienda seguir para la creación de documentos
con HTML?



3. En las Especificaciones de HTML, ¿cuándo un elemento o atributo se considera desaprobado? ¿Y obsoleto?



4. ¿Qué es el DTD y cuáles son los posibles DTDs contemplados en la especificación de HTML 4.01?

DTD (Document Type Definition) es una declaración que se utilia para definir la estructura y la sintaxis válida de un documento HTML. Especifica qué elementos, atributos y reglas son permitidos y cómo debe ser organizados dentro del documento. 

En HTML 4.01, existian 3 tipos principales de DTDs que se pueden utilizar para definir la estructura de un documento HTML:

- **Strict DTD (DTD estricto):** Este DTD es el más restrictivo y cumple con las reglas estrictas de HTML. Define un conjunto de elementos y atributos que son considerados válidos en HTML, en donde no permite el uso de elementos y atributos obsoletos o que no cumplan con las normas estrictas de HTML. Para utilizar este tipo se declara en documento HTML de la siguiente manera: 
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

- **Transitional DTD (DTD de transición):** Este DTD es el más permisivo permitiendo el uso de elementos y atributos obsoletos, está destinado a ayudar en la transición de documentos HTML antiguos que se utilizaban anteriormente, para utilizar este tipo se declara en documento HTML de la siguiente manera: 
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

- **Frameset DTD (DTD de conjunto de marcos):** Este DTD se utiliza unicamente cuando se quiere utilizar marcos en el documento HTML, estos mismos permiten dividir una página web en varias áreas independientes y cada área puede mostrar un documento HTML diferente. Para utilizar este tipo se declara en documento HTML de la siguiente manera:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">
```

Es importante utilizar el DTD adecuado según los requerimientos del proyecto y asegurarse de que el documento cumpla con las normas estabelcidas para garantizar la compatibilidad y el correcto funcionamiento en diferentes navegadores y dispotivos. 

5. ¿Qué son los metadatos y cómo se especifican en HTML?

Los metadatos son información adicional sobre un documento que proporciona detalles acerca del contenido y características del mismo. Estos datos no son visibles directamente en la página web, pero son utilizados por navegadores, motores de búsqueda y otros sistemas para entender y procesar el documento de manera adecuada. 

En HTML, los metadatos se epecifican dentro del elemento `<head>` del documento, como se muestra a continuacion con algunos ejemplos de los metadatos más comunes. 

- **Meta etiqueta para el juego de caracteres**
Esta meta etiqueta especifica el juego de caracteres que se utiliza en el documento, lo que es importante para asegurar que los caracteres se vean correctamente en diferentes navegadores, en HTML se declara de la siguiente manera: 
```html
<head>
    <meta charset="UTF-8">
</head>
```
- **Meta etiqueta para la descripcion del documento**
Esta meta etiqueta proporciona una breve descripcion del contenido del documento, que a menudo se muestra en los resultados de búsqueda, en HTML se declara de la siguiente manera: 
```html
<head>
    <meta name="description" content="Esta es una página web de ejemplo">
</head>
```

- **Meta etiqueta para las palabras clave**
Esta meta etiqueta especifica una lista de palabras claves que describen el contenido del documento, en HTML se declara de la siguiente manera: 
```html
<head>
    <meta name="keywords" content="HTML, metadatos, descripción, palabras clave">
</head>
```

- **Meta etiqueta para el autor del documento**
Esta metaetiqueta se utiliza para identificar al creador del documento, para declararla en HTML se utiliza de la siguiente manera: 
```html
<head>
    <meta name="author" content="Nombre del Autor">
</head>
```

- **Meta etiqueta para el título del documento**
Esta metaetiqueta define el título del documento, que se muestra en la barra del título del navegador y en los resultados de búsqueda, para utilizarlo en HTML se declara de la siguiente manera: 
```html
<head>
    <meta name="title" content="Título de la página">
</head>
```

Estos son algunos ejemplos de los metadatos, existen muchas mas y además atributos que se pueden utilizar para proporcionar información adicional sobre el documento, como por ejemplo el idioma. El uso adecuado de los mismos ayuda a mejorar la accesibilidad, visibilidad y compresión de tus páginas web por parte de los usuarios y los motores de búsqueda. 