+++
pre = "<b>2. </b>"
title = "Themes o layout base"
weight = 2
+++

### Ejercicio 2

##### Themes o layout base
--- 
###### 1. Instala el tema relearn.

Para instalar el tema en Hugo escribimos en la consola:

    git init
    git submodule add https://github.com/McShelby/hugo-theme-relearn.git ./themes/relearn

Una vez instalado tenemos que añadir en el archivo de configuración **config.toml**:

    theme =['relearn']
    
---
###### 2. Ejecuta el comando de hugo para abrir un puerto en local.

Para abrir un puerto en local escribimos en la consola:

    hugo server &

Nos abre el puerto **35171**.

---
###### 3. Visualiza tu proyecto en el servidor.

Mediante el navegador accedemos a la dirección **http://localhost:1313/myHugoSite/**.

![image2](https://i.ibb.co/Z6sKwDX/DWEC-002.png)

---