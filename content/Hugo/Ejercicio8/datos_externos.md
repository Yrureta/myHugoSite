+++
pre = "<b>8. </b>"
title = "Datos externos"
weight = 8
layout = "datos_tv"
+++

### Ejercicio 8

##### Datos externos

Ubicamos el fichero **tv.json** en la carpeta **data**. El fichero lo obtenemos de https://github.com/MAlejandroR/staticSite/blob/main/data/tv.json.

Creamos una plantilla html **datos_tv.html** y la ubicamos en **themes/relearn/layouts/_default**.

Código de la plantilla:

    <ul>
      {{ range  .Site.Data.tv }}
      <h1><li>  {{ .name }}</li></h1>
      {{ range .channels }}
          <a href="{{ .web}}" >
          <img src="{{.logo}}" alt="{{ .name }}">
          </a>
       {{ end }}
      {{ end }}
    </ul>

Una vez que creada la plantilla, vamos a consumirla desde un fichero de markdown. Buscamos la plantilla base para incluir los elementos en esta plantilla en la nuestra. **datos_tv.html** quedaría así:

    {{- partial "header.html" . }}
    {{ partial "content.html" . }}
       <ul>
        {{ range  .Site.Data.tv }}
        <h2><li>  {{ .name }}</li></h2>
        {{ range .channels }}
        <a href="{{ .web}}" >
            <img src="{{.logo}}" alt="{{ .name }}">
        </a>
    
        {{ end }}
        {{ end }}
        </ul>
        <footer class="footline">
        {{- with .Params.LastModifierDisplayName }}
        <i class='fas fa-user'></i> <a href="mailto:{{ $.Params.LastModifierEmail }}">{{ . }}</a> {{ with $.Date }} <i class='fas fa-calendar'></i> {{ .Format "02/01/2006" }}{{ end }}
        {{- end }}
        </footer>
    {{- partial "footer.html" . }}

Ahora le indicamos a nuestra página **datos_externos.md** que use esta plantilla:

    +++
    pre = "<b>8. </b>"
    title = "Datos externos"
    weight = 8
    layout = "datos_tv"
    +++
    
---
# Listado de canales de tv