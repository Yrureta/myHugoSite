+++
pre = "<b>4. </b>"
title = "Shortcode"
weight = 4
+++

### Ejercicio 4

##### Shortcode
--- 
Accede a la información de de shortcode de la plantilla de relearn e incluye en tu trabajo los elementos que a continuación se muestran.

###### 1. Botones.
{{% button href="https://www.audacityteam.org//" %}}Audacity{{% /button %}}
{{% button href="https://www.audacityteam.org/" icon="fas fa-download" %}}Audacity{{% /button %}}
{{% button href="https://www.audacityteam.org//" icon="fas fa-download" icon-position="right" %}}Audacity{{% /button %}}

--- 
###### 2. Páginas de descargas.
{{%attachments style="blue" title="Imágenes relacionadas" pattern=".*(png)"/%}}

--- 
###### 3. Acortar un texto con leer mas….
{{% expand "Haz click aquí!" "false" %}}
Hiciste click!
{{% /expand %}}

--- 
###### 4. Texto remarcado como una noticia.
{{% notice note %}}
**Descargo de responsabilidad**
Los anuncios sobre temas sociales, elecciones o política pueden requerir un descargo de responsabilidad, pero los requisitos varían en función del país. Este descargo aparecerá en los anuncios que pongas en circulación y puede incluir información sobre la organización o la persona responsable de ellos.
{{% /notice %}}

---
###### 5. Crear gráficos con mermaid.
{{< mermaid align="left" >}}
graph LR;
    A[Web site] --> B(Chapter 1)
    A[Web site] --> C(Chapter 2)
    A[Web site] --> D(Chapter 3)
    C --> F[Part 1]
    C --> E[Part 2]
{{< /mermaid >}}

--- 
###### 6. Tabs de diferentes elementos.
{{< tabs >}}
{{% tab name="Frutas" %}}
```Frutas
Manzana, pera, plátano
```
{{% /tab %}}
{{% tab name="Legumbres" %}}
```Legumbres
Garbanzo, lenteja, alubia
```
{{% /tab %}}
{{% tab name="Pescados" %}}
```Pescados
Atún, trucha, merluza
```
{{% /tab %}}
{{< /tabs >}}

--- 