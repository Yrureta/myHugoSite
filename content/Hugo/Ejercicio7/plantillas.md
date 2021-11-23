+++
layout = "footer_fijo"
pre = "<b>7. </b>"
title = "Plantillas"
weight = 7
+++

### Ejercicio 7

##### Plantillas

###### 1. Prueba a crear una plantilla personal y muéstrala.

Vamos a realizar una plantilla que coloca un **footer** fijo al final de la página.

Creamos un fichero html que llamaremos **footer_fijo.html** y lo almacenamos en la carpeta  **layouts/_default/**.

Escribimos el código siguiente:
```html
{{- partial "header.html" . }}
{{ partial "content.html" . }}
          <footer class="footline">
          {{- with .Params.LastModifierDisplayName }}
            <i class='fas fa-user'></i> <a href="mailto:{{ $.Params.LastModifierEmail }}">{{ . }}</a> {{ with $.Date }} <i class='fas fa-calendar'></i> {{ .Format "02/01/2006" }}{{ end }}
          {{- end }}
          </footer>
{{- partial "footer.html" . }}
<style>
    #footer {
        color: black;
        font-weight: bold;
        position: fixed;
        padding: 10px 10px 0px 10px;
        bottom: 0;
        width: 100%;
        height: 40px;
        background: grey;
    }
</style>
<div id="footer">DWES - Práctica 1 - Miguel Yrureta</div>
```
Ahora solo nos queda indicar en el **frontmatter** de nuestro archivo **plantillas.md** que utilice la plantilla que acabamos de hacer.
```
+++
layout = "footer_fijo"
pre = "<b>7. </b>"
title = "Plantillas"
weight = 7
+++
```
Podemos ver el footer nuevo al final de la página.

--- 