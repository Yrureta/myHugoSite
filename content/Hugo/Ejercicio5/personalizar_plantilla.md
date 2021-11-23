+++
pre = "<b>5. </b>"
title = "Personalizar la plantilla"
weight = 5
+++

### Ejercicio 5

##### Personalizar la plantilla

Modifica la plantilla según se ha visto en este tema.

###### 1. Cambia el logo.

Para cambiar el logo u otras características de la plantilla modificamos el contenido del archivo correspendiente de la carpeta **layouts/partials** de nuestra plantilla. En este caso modificamos **logo.html**.
```html
<a id="logo"
    href="{{ .Site.Params.landingPageURL | default "/" | relLangURL }}"
    style="
        color: #3d414d;
        font-family: 'Novacento Sans Wide', 'Helvetica', 'Tahoma', 'Geneva', 'Arial', sans-serif;
        font-size: 30px;
        font-weight: bold;
        margin-top: -2px;">
    <img src="https://i.ibb.co/H7GYpgm/hugo-logo.png" alt="Logo de HUGO">Hugo
</a>
```
--- 
###### 2. Establece otros colores según consideres.

Esta plantilla tiene hasta tres estilos de colores diferentes preparados. Para utilizarlos basta con establecer el valor correspondiente de la variable themeVariant en el fichero de configuración **config.toml**. Los valores permitidos son red, green y blue.

    [params]
       themeVariant = "green"

--- 
###### 3. Añade un menú principal.
1. Que tenga 4 opciones al menos.
2. Establece icono de fan awesome.
3. Establece un título para ese menú.

Añadimos en el fichero de configuración **config.toml** el código siguiente:

    [[menu.shortcuts]]
    name="<i class='fas fa-circle'></i>   American Music Club"
    identified=""
    url="https://open.spotify.com/album/7ADzHyUaZJvF930EffNDHU?si=VTjqhD-0TdufMC_OuZE00Q" 
    weight=1

    [[menu.shortcuts]]
    name="<i class='fas fa-circle'></i>   Deerhunter"
    identified=""
    url="https://open.spotify.com/album/3a3Yp0PRguSTH3dBOeWRyZ?si=Mk4kQa8cRSGLHNmEkvdAxA" 
    weight=2

    [[menu.shortcuts]]
    name="<i class='fas fa-circle'></i>   Beach House"
    identified=""
    url="https://open.spotify.com/album/7ejB3MHdDNcY3GzRsQRAHs?si=re-UeiyYS2a6ml7hMG9sJQ" 
    weight=3

    [[menu.shortcuts]]
    name="<i class='fas fa-circle'></i>   Vetiver"
    identified=""
    url="https://open.spotify.com/album/6kbbOgKxIWVt49DGihtm8Q?si=apqDEQgmSqKsYN1RbwuadQ" 
    weight=4

Para establecer un título para el menú tenemos que editar los ficheros de idioma. Par editar el fichero de español editaremos **es.toml**.

    [Shortcuts-Title]
    other = "Música"

--- 
###### 4. Modifica el footer de la página.

Modificamos el fichero **footer.html**.

    {{- if .Params.chapter }}
    </div> 
    <!-- end chapter-->
    {{- end }}
    </main>
    DWES - Práctica 1 - Miguel Yrureta
    <!-- #body-inner -->

--- 







