# Primeros pasos en Git

1. Instalar Git
  
  https://git-scm.com
  
  `git --version` verifica la versión de git
  
2. Establecer valores de configuración

   Esta información se utiliza para tener registro en los cambios que se van a desarrollar
   
   El comando `git config --global user.name "your_username` añadirá el nombre de usuario dentro del ordenador.
   
   También deberemos añadir nuestro correo electrónico con el comando 
   
   `git config --global user.email "your_email_adress@example.com`
   
   Por último, para estar seguros de que hemos hecho todo lo correcto para registrarnos, utilizaremos este comando
   
   `git config --global --list`
   
Las páginas estáticas no necesitan de un servidor web para que funcionen.

Para probar el contenido utilizaremos un navegador.

3. Elegir un repositorio y clonarlo

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
  
