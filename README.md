# Primeros pasos en Git

   ## Instalar Git
  
  https://git-scm.com
  
  `git --version` verifica la versión de git
  
   ## Establecer valores de configuración

   Esta información se utiliza para tener registro en los cambios que se van a desarrollar
   
   El comando `git config --global user.name "your_username` añadirá el nombre de usuario dentro del ordenador.
   
   También deberemos añadir nuestro correo electrónico con el comando 
   
   `git config --global user.email "your_email_adress@example.com`
   
   Por último, para estar seguros de que hemos hecho todo lo correcto para registrarnos, utilizaremos este comando
   
   `git config --global --list`
   
Las páginas estáticas no necesitan de un servidor web para que funcionen.

Para probar el contenido utilizaremos un navegador.

   ## Elegir un repositorio y clonarlo

  Para esto, deberemos entrar en GitHub y copiar el enlace del repositorio para posteriormente clonarlo en Visual Studio.
  
Para clonar un repositorio tendremos que hacer esto:

- Git add

   con el comando **git add .** añadiremos el index.html y el README en los ficheros que hemos generado en un directorio.
   
- Git commit

   con el comando **git commit -m "mensaje"** cambiaremos el nombre del repositorio en lo que escribamos en "mensaje".
   
- Git push

   con el comando **git push origin main** subiremos los cambios a main de GitHub. Si actualizamos GitHub éste aparecerá y lo subiremos a GitHub desde local.
   
# index.html
   
   Ahora nos centraremos sobretodo en algunos comandos clave de index.html, que nos servirán para nuestra página web.
   
   El primer comando que deberemos escribir es el <html:5>, este html nos permitirá empezar nuestra página web, y nos pondrá un comando parecido a esto:
   
   ![alt text](https://www.lluiscodina.com/wp-content/uploads/2019/05/html-5-ejemplo-de-marcado.png)

**Ahora que tenemos el html, estamos listos para poder escribir lo que queramos en nuestra página web.**

## Poner una imagen en nuestra página web

   Para esto, necesitaremos escribir el comando **<img src="" alt="">**, tendremos que tener una carpeta llamada "img" en nuestro repositorio para guardar la imagen que            queramos y que cuando escribamos ./img dentro de las comillas del comando src="", es decir, <img src=**"./img"** nos aparezca la imagen justo como vemos en ésta:

![alt_text](https://aws1.discourse-cdn.com/netlify/original/2X/2/287e2276b7ace367624908fc72d1c1741f8660e4.png)

   Como vemos en la imagen, el cuadradito rojo nos indica que lo que hay escrito dentro de las "" de src (source) es el archivo donde se ubica esta misma imagen, que está          dentro de la carpeta que creamos (img).

   Hay que tener en cuenta que todo lo que escribamos debe estar dentro de **head** o **body**, debemos saber que todo lo que escribamos en **head**    se mantendrá en toda la página web, son como normas que asignamos a nuestra página que se deberán cumplir, como que todo se escriba en negrita. En **body** nuestra    orden sólo se cumplirá dentro de donde la hemos asignado, sólo 1 vez, esto también nos permitirá dar variedad a la página web.

   Dicho esto, podemos continuar con la sintaxis del html.

## Las etiquetas ol, li y ul
  
  La etiqueta **ol** sirve para hacer una lista ordenada en nuestro HTML, en otras palabras, la típica lista de la compra, como por ejemplo:
  
   1. Fresas
   2. Cebollas
   3. Patatas
  
  Para hacer esta lista en index.html se vería algo así:
  
  ```
   ol
   
     li
     
        Fresas
        
     /li
     
     li
        
        Cebollas
        
     /li
     
     li
     
        Patatas
     
     /li
     
  /ol
  ```
  
  La etiqueta **li** sirve para identificar un ítem dentro de la lista ordenada, es decir, para especificar el nombre o lo que querramos poner, igual que como se ve en la gráfica     anterior.
  
  La etiqueta **ul** hace exactamente lo mismo que **ol**, sólo que la lista que generará será una lista no ordenada, sin números que la organicen, sólo con · 
  
## Otras etiquetas importantes

 La etiqueta **p** identifica que lo que escribes es un párrafo, es la más utilizada para páginas web, pues es la que convierte todas las letras en texto.
 
 La etiqueta **a** abre un link para acceder desde una misma palabra con el HTML, es decir, convierte la palabra en un link para el HTML que tú hayas decidido, algo como [esto](https://www.google.com/).
 
 La etiqueta **p style="color: blue"** cambi}a el color de la letra que hemos escrito dentro de la etiqueta **p**, pero si este comando lo ponemos en **head** hará que todas las etiquetas **p** que pongamos deban ser de color azul. También podemos elegir el color que queramos, nos saldrá una opción despues de escribir `color:`.
 
 La opción **style**, por lo tanto, agrega estilos en línea.
 
 La opción **src** define la ruta de la imagen, como hemos explicado anteriormente para colocar una imagen en nuestro HTML.
 
 La opción **alt** es una imagen de descripción de la foto.


 El selector p{
         
         /*....*/
         
              }
              
 Aplica a todas las p lo que introduzcamos dentro de las llaves.
 
 **div p{...** sirve para agrupar lo que deseemos en el mismo bloque a todos los descendientes (en este caso **NO** es descenciente directo)
 
 **div>p{** sólo agrupará el descendiente directo de div, es decir, p{.
 
 Un ejemplo práctico para entender esto sería la siguiente gráfica:
 ```
 div
    div
       p.../p
    div
   p.../p
 div
```

Como podemos observar, si hubiésemos utilizado div<p{ el único que habría funcionado es el segundo div, ya que es el que tiene conexión directa con p, el primero.

div+p{ en este caso la diferencia que tenemos con los anteriores es que el + es el elemento adyacente, es decir, el primer objeto.

Ejemplo:

```
div class="a"
  p class="a" ... /p
/div
```
p·a{ significaría que el párrafo que tiene el clase "a" aplicaría los cambios que nosotros dijésemos. Con esto, nos ahorramos tener que repetir éstos cambios una y otra vez, si es que son muy largos. Gracias al gran número de combinaciones, podemos ahorrar tiempo y trabajar de manera muy específica.

 
 
 
 "
 Tema de los cuadritos
 "


Existen etiquetas que hacen lo mismo que div, como **"header"**, la diferencia es que si se leen en voz alta en vez de decir DIV dice encabezado, cosa que facilita a cualquier persona con alguna deficiencia a leer este mismo.

El **vh** es la altura de la pantalla del navegador, y si asignamos 100vh al header significa que el header ocupará toda la pantalla.

- Media query
```
@media only screen and (max-width: 400px) {
    body {
        background-color: white;
    }
}
```
Los **px** son los píxeles por pantalla, entonces hacemos que cuando la pantalla de la página web sea menor a
400 píxeles el fondo de esta misma cambie a color blanco.
El **vh** es la altura del navegador y el vw es la anchura de este, en ambos casos el número 100 es el 100% de este.

El **rem** sirve para multiplicar el tamaño que pongamos en el HTML, por ejemplo, ´html font-size: ***32px***´, si ponemos
**2rem** en p, la p pasará a tener ***64px***.

Además de esto, también hay etiquetas que hacen exactamente lo mismo que div como **"footer"** o **"header"**, básicamente nos ayuda a no perdernos y poder leer el código organizándonos, o también para que otras personas puedan leer el código de la web con mayor facilidad.

- href="#gallery">Item1 -> Sirve para asignar esta id a una palabra, y nos llevara allí donde pongamos la id=gallery, ya sea un div o una p, un footer, etc.

- scroll-behavior:smooth -> Nos servirá para que la página deslice la pantalla cuando cliquemos a un href en vez de "teletransportarse" directamente.


- form action="showview.html" -> Es un campo que te permite poner texto, el que quieras.
