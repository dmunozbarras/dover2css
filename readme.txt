# Primer diseño Web en HTML
Para realizar este diseño he usado como tema un grupo de música español de rock.

La estructura básica de un HTML es la siguiente:

    <!DOCTYPE html>
    <html>

    <head>

    </head>

    <body>

    </body>
    </html>


  * Hay que comenzar con la linea `<!DOCTYPE html>` para que el editor reconozca que
  el lenguaje empleado es <b>html</b>.
  * Dentro de  `<html>`: Colocamos la cabecera `<head>` y el cuerpo `<body>` una vez acabada cada parte hay que cerrarlas con "/" ejemplo:`</head>`.

  * En`<head>`colocamos `<title>`que sera lo que mostraremos en la barra superior del navegador, para que de una forma simple saber el contenido de nuestra web. Ejemplo: Dover el grupo de música rock Español.
```
<html>
  <head>
    <title>Grupo de música rock Español Dover</title>
  </head>
```

   En `<body>` añadimos los parámetros `<body style ="background-color:PAPAYAWHIP">`para cambiar el color de fondo de nuestra web.
  * Creamos la cabecera <b>h1</b> que mostrara el título de la web, poniéndole otro color y alineación centro.

   `<h1 style="background-color:DodgerBlue" & Align=center>Dover el grupo de música rock Español</h1>`.
  * Ponemos un salto de linea con el parámetro <b>`<br>`</b> para que la imagen del centro

  * Creamos una sección con alineación central, el parámetro <b>img</b> donde se especifica donde esta la imagen y con el alt la comentamos.`<div align=center><img src="dover2.jpg"alt="foto del grupo completo Dover"></img></div>`.

   Donde irán las dos imágenes y en el medio el texto, para las imágenes he usado el parámetro `<img style="float:left; margin:10px, src y alt">`
  `<img style="float:left;  margin:10px;" src="dover1.jpg" alt="Portada disco Devil come to ME de Dover"/>` y `<img style="float:right; margin:10px;" src="dover3.jpg"alt="Portada disco Follow the citi lights de Dover"/>`
  El texto esta ordenado por párrafos con el parámetro `<p>`y a su vez las fechas están en negrita, los nombres de los discos en cursiva y los nombres propios tienen un hipervínculo hacia su página en <b>Wikipedia</b>.
  * Usamos varios saltos de línea `<br>`y nos vamos a crear una nueva sección con alineación central en la que colocaremos la tabla.
* Usamos un estilo de tabla para que contenga el año y nombre del disco del grupo:

`````
<div align=center>
  <style>

  table, th, td {
      border: 1px solid black;
  }

  </style>

<table style="width:50%"; "height:50%" border=1>

<tr align="center" bottom="middle">

<tr>
  <th><strong>Año</strong></th>
  <th><strong>Album</strong></th>
</tr>

<tr>
  <td>1995</td>
  <td> <a href="https://es.wikipedia.org/wiki/Sister_(%C3%A1lbum_de_Dover)"> Sister </a> </td>
</tr>
````
  * Definimos que la tabla ocupe el 50% y tenga el borde 1, y que los nombres de año y álbum estén mas definidos con el parámetro `<strong>`
  Cada título de cada álbum tiene un hipervínculo para poner obtener mas información en la Wikipedia.

  * Creamos una sección nueva con  una lista desordenada desde la cual podemos visitar sitios webs de interés.
  ```
  <div>
      <UL TYPE=circle>
      <LI> <a href="https://es.wikipedia.org/wiki/Dover_(banda)#Discograf.C3.ADa">Dover en Wikipedia</a>
      <LI> <a href="https://twitter.com/dover_oficial?lang=es">Dover en Twitter </a>
      <LI> <a href="https://www.facebook.com/pg/Dover-47690923459/about/">Dover en Facebook</a>
      </UL>
  </div>
````
* Creamos otra sección para el Copyright con el parámetro <small> para que el texto sea mas pequeño.
````
  <div align=center>
    <small>Copyright 2017-2018 by David Muñoz Barras.</small>
    <A href="javascript:closer();">[ Salir ]</A>
  </div>
````
* Por último e buscado un <b>Script</b> que cuando le de a cerrar se cierre la web.

```
  <script language=javascript>
  function closer() {
  var ventana = window.self;
  ventana.opener = window.self;
  ventana.close();
  }
  </script>
```
  Para realizar el trabajo e visitado las siguientes páginas Web:
  * https://es.wikipedia.org/wiki/Dover
  * http://www.europafm.com/artistas/dover_20151006561374826584a8ebfab2b5e0.html
  * https://markdown.es/sintaxis-markdown/#codigo
  * https://www.w3schools.com/html/default.asp
  * https://github.com
  * https://rawgit.com/

  La url del repositorio es:
  * https://github.com/dmunozbarras/Dover

  La url del rawgit es:
  * https://rawgit.com/dmunozbarras/Dover/master/index.html
  
