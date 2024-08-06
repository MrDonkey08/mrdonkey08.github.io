---
layout: post
title: Vim CheatSet
author: Alan Yahir Juárez Rubio
description: "Guía Completa de Uso de Vim: Modos, Acciones, Comandos..."

categories:
  - software
  - linux
tags:
  - linux
  - windows
  - mac
  - vi
  - vim
  - nvim
  - neovim
  - cheatsheet

date: 2024-06-10 13:16

toc:
  sidebar: right

pretty_table: true
---

**Vi** es un editor de texto de terminal.

**Vim** es el sucesor de _vi_.

**Nvim** es un versión de **vim** escrito por la comunidad en la que se
reescribe _vim_ y se añaden funciones, mejoras.

## Modos

**Vim** tiene varios modos de uso

### Normal

El **modo normal** es aquel que nos permite navegar a través del archivo.
Adicionalmente, este modo nos permite cambiar a los demás modos.

Para regresar al modo normal basta con presionar `<esc>`

#### Navegación

Para navegar a través de vim es necesario estar en _modo normal_. Existen
varios atajos para navegar a través de vim:

##### Desplazamiento

Te puedes desplazar con las flechas, sin embargo, se recomiendan los siguientes comandos:

###### Carácteres

|  Acción   | Atajo |
| :-------: | :---: |
| Izquierda |  `h`  |
|   Abajo   |  `j`  |
|  Arriba   |  `k`  |
|  Derecha  |  `l`  |

###### Lineas

|           Acción           | Atajo |
| :------------------------: | :---: |
|      Inicio de línea       |  `0`  |
|     Final de la línea      |  `$`  |
| Primer carácter imprimible |  `^`  |

###### Palabras

|                   Acción                   | Atajo | Nombre |
| :----------------------------------------: | :---: | :----: |
|         Palabra siguiente (Incio)          |  `w`  |  word  |
| Palabra anterior tomando espacios (Inicio) |  `W`  |  Word  |
|          Palabra anterior (Incio)          |  `b`  |  back  |
| Palabra anterior tomando espacios (Inicio) |  `B`  |  Back  |
|         Palabra siguiente (Final)          |  `e`  |  end   |
| Palabra anterior tomando espacios (Final)  |  `E`  |  End   |

###### Signos de Agrupación

|                 Acción                  | Atajo |
| :-------------------------------------: | :---: |
| Alternar entre los signos de agrupación |  `%`  |

##### Scroll

|       Acción       |    Atajo     |  Nombre  |
| :----------------: | :----------: | :------: |
|       Bajar        | `<ctrl> + y` |          |
|       Subir        | `<ctrl> + e` |          |
| Bajar media página | `<ctrl + u`  |    up    |
| Subir media página | `<ctrl> + d` |   down   |
|    Subir página    | `<ctrl> + f` |  foward  |
|    Bajar página    | `<ctrl> + b` | backward |

##### Sección

|      Acción      |    Atajo     | Nombre |
| :--------------: | :----------: | :----: |
|  Primera línea   |     `G`      |        |
|   Última línea   |     `gg`     |        |
| Línea especifica | `«num» + gg` |        |

#### Copiar, Pegar y Cortar

> ##### TIP
>
> Puedes utilizar `i` de _inner word_ para copiar, pegar, cortar... la palabra,
> {: block-tip }

##### Copiar (yank)

|                   Acción                   |   Atajo    |   Nombre   |
| :----------------------------------------: | :--------: | :--------: |
|               Copiar palabra               |    `yw`    | yank word  |
|                Copiar línea                |    `yy`    | yank line  |
|          Copiar múltiples líneas           | `«num» yy` | yank lines |
|     Copiar hasta el inicio de la línea     |    `y0`    |            |
|     Copiar hasta el final de la línea      |    `y$`    |            |
| Copiar hasta el primer carácter imprimible |    `y^`    |            |

##### Pegar (paste)

|     Acción     | Atajo | Nombre |
| :------------: | :---: | :----: |
| Pegar adelante |  `p`  | paste  |
|  Pegar atrás   |  `P`  | Paste  |

##### Cortar (delete)

|                    Acción                    |     Atajo     |   Nombre    |
| :------------------------------------------: | :-----------: | :---------: |
|               Eliminar palabra               |     `dw`      | delete word |
|              Eliminar carácter               | `d + <space>` |   delete    |
|     Eliminar hasta el inicio de la línea     |     `d0`      |             |
|     Eliminar hasta el final de la línea      |     `d$`      |             |
| Eliminar hasta el primer carácter imprimible |     `d^`      |             |

##### Cortar y reemplazar (change)

|                    Acción                    | Atajo |   Nombre    |
| :------------------------------------------: | :---: | :---------: |
|         Cortar y reemplazar palabra          | `cw`  | change word |
| Cortar hasta el final de la línea e insertar |  `C`  |   Change    |
|       Cortar y reemplazar línea entera       | `cc`  |             |

### Edition

#### Inserción

El **modo edition** o **edicion** es aquel que se utiliza en todos los editores
de texto; es aquel que nos permite editar el archivo.

|     Acción      | Atajo | Nombre |
| :-------------: | :---: | :----: |
|    Insertar     |  `i`  | insert |
|     Añadir      |  `a`  | append |
| Inicio de línea |  `I`  | Insert |
| Final de línea  |  `A`  | Append |

#### Revertir y Rehacer

|  Acción  |    Atajo     | Nombre |
| :------: | :----------: | :----: |
| Revertir |     `u`      |  undo  |
| Rehacer  | `<ctrl> + r` |  redo  |

### Visual

### Replace

El **modo replace** o **reemplazo** es el modo que nos permite reemplazar uno o
varios carácteres de un texto.

|              Acción               | Atajo | Nombre  |
| :-------------------------------: | :---: | :-----: |
|        Reemplazar carácter        |  `r`  | replace |
|         Reemplazar texto          |  `R`  | Replace |
| Sustituir carácter y añadir texto |  `s`  |         |
|     Sustituir línea con texto     |  `S`  |         |

### Comandos

Las funciones de vim se ejecutan a traves de comandos. Para ejecutar un comando
se ejecutan los siguientes pasos:

- Se entra al modo normal presionando `<esc>`
- Se presiona `:`
- Se escribe el comando
- Se presiona `<enter>` para ejecutar el comando

#### Básicos

|           Acción           |    Comando    |     Nombre     |
| :------------------------: | :-----------: | :------------: |
|          Guardar           |      `w`      |     Write      |
|           Salir            |      `q`      |      Quit      |
|      Guardar y salir       |   `wq`, `x`   | Write and Quit |
| Guardar todos los archivos |     `wa`      |    Write ll    |
|           Abrir            | `o «archivo»` |      open      |
