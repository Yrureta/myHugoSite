+++
pre = "<b>9. </b>"
title = "Links"
weight = 9
+++

### Ejercicio 9

##### Solucionando el problema de los links

Hugo por defecto abre los links en la misma página, pero nos interesa que los enlaces externos se abran en otra página.

Para solucionar esto creamos el archivo **render-link.html** en la carpeta **layouts/_default/_markup/**

Y añadimos el siguiente script:
```html
<a href="{{ .Destination | safeURL }}"{{ with .Title}} title="{{ . }}"{{ end }}{{ if strings.HasPrefix .Destination "http" }} target="_blank"{{ end }}>
{{ .Text }}
</a>
```
Para que funcione debemos de escribir los links de esta manera:

    [https://www.heroku.com/](https://www.heroku.com/)

[https://www.heroku.com/](https://www.heroku.com/)

Para que funcionen también de esta manera los links del menú **Música** no he podido encontrar una solución.

---