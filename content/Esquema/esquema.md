+++
pre = "<b>1. </b>"
title = "Proceso de carga de un recurso web"
weight = 1
+++

Partimos de la url: [https://www.reasonstudios.com/en/reason/instruments/kong](https://www.reasonstudios.com/en/reason/instruments/kong)

| Protocolo | Maquina | Recurso |
| ----------- | ----------- | --- |
| http:   | [www.reasonstudios.com](https://www.reasonstudios.com) |  en/reason/instruments/kong |

Esquema:

{{< mermaid align="left" >}}
graph LR;
    A[Navegador Máquina Cliente] -->|Petición URL| B[Sertvidor DNS]
    B --> C{<strong>Servidor principal</strong>}
    C --> |Se procesa el PHP| D[Módulo de PHP]
    D --> |Se devuelve el código en HTML|C
    C --> |Petición a la Base de Datos|E[Servidor Base de Datos]
    E --> |Respuesta de la Base de Datos|C
    C --> |La página final se muestra al cliente|A
{{< /mermaid >}}
---