+++
pre = "<b>3. </b>"
title = "Contenido"
weight = 3
+++

### Ejercicio 3

##### Contenido
--- 
###### 1. Crea la estructura de tu sitio web.

![image2](https://i.ibb.co/p4Cj0qB/dwesc-003.png)
--- 
###### 2. Completa los ficheros con contenido.

Para crear las secciones y ficheros **_index.md** utilizamos por ejemplo:

    hugo new --kind chapter Hugo/_index.md
    hugo new --kind chapter Hugo/Ejercicio1/instalacion.md

Seguidamente utilizamos **markdown** para añadir el contenido:

    ###### 1. Crea un sitio nuevo con el nombre que quieras.

    Para crear un nuevo sitio con Hugo escribimos en la consola:

        hugo new site myHugoSite

    ---
    ###### 2. Entra en el directorio creado y observa las diferentes carpetas que tienes.

    ![image1](https://i.ibb.co/93XZjgH/dwesc-001.png)

Y luego se visualizará de esta manera en el navegador:

  ![image4](https://i.ibb.co/zb9pqVw/dwes-004.png)

---
###### 3. Ahora reordena todo usando el frontmatter.

Los ficheros generados tienen en su cabecera una serie de valores por defecto, para que queden ordenados cambiamos el valor numérico de la propiedad **weight**. 

---
###### 3. Comprueba en el servidor como se ha actualizado tu sitio web.

![image2](https://i.ibb.co/Z6sKwDX/DWEC-002.png)

---