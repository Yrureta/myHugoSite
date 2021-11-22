+++
pre = "<b>3. </b>"
title = "Contenido"
weight = 3
+++

### Ejercicio 3

##### Contenido
--- 
###### 1. Instala el tema relearn.

Para instalar el tema en Hugo escribimos en la consola:

    git init
    git submodule add https://github.com/McShelby/hugo-theme-relearn.git ./themes/relearn

Una vez instalado tenemos que escribir en el archivo de configuración config.toml:

    theme =['relearn']
    
---
###### 2. Ejecuta el comando de hugo para abrir un puerto en local.

Para abrir un puerto en local escribimos en la consola:

    hugo server &
---
###### 3. Visualiza tu proyecto en el servidor.

![image2](https://i.ibb.co/Z6sKwDX/DWEC-002.png)

---

Ahora practica tú
😀

Establece un contenido para tu sitio web. Para ello debes de tener clara las secciones y en cada sección los ficheros contenidos Por ejemplo podría ser parte del contenido de este curso visto anteriormente
practica2.md
practica1.md
_index.md
contenido.md
temas.md
instalacion.md
_index.md
OOP.md
Arrays_formularios.md
Sintaxis.md
_index.md
Práctica
teoría.md
_index.md
instalación.md
arquitectura_web.md
conceptos_generales.md
_index.md
PHP
Static
Introducción
content_ (directorio raíz base)
Con esto nos aparecerá la siguiente estructura:

contenido ejemplo

Ahora completa los ficheros con contenido (no hace falta que haya muchos, mejor que tenga sentido, que vayas realizando tu portfolio, que sea tu forma de presentarte y mostrar a los demás en qué estás trabajando, puede ser un blog, …

Recuerda cómo se crean las secciones, ficheros _index y ficheros de contenido en este template

También podrías usar la estructura anterior e ir completándola con esquemas, resúmenes de los aspectos que vayas aprendiendo en el curso.

Ahora reordena todo usando el frontmatter, recuerda la propiedad weight, modifica los títulos según consideres y puedes poner una descripción.

Ve revisando como queda todo al visualizarlo en la web

Comprueba en el servidor como se ha actualizado tu sitio web