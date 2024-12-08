---
layout: post
title: Otros
author: Alan Yahir Juárez Rubio
description: null

categories:
  - linux
  - comandos
tags:
  - redirecciones
  - operadores-de-control
  - variables-de-entorno

date: 2023-12-11
last_updated: 2024-12-08

toc:
  sidbar: right
---

## Redirecciones I/O

| Comando | Descripción                                                                                 | Argumento          | Ejemplo                              |
| :-----: | :------------------------------------------------------------------------------------------ | ------------------ | ------------------------------------ |
|   `<`   | Redirige la entrada de un comando desde un archivo                                          | Archivo de entrada | `sort < lista.txt`                   |
|   `>`   | Redirige la salida estándar de un comando hacia un archivo, sobrescribiéndolo               | Archivo de salida  | `echo "Hola Mundo" > saludo.txt`     |
|  `>>`   | Redirige la salida estándar de un comando hacia un archivo, añadiendo el contenido al final | Archivo de salida  | `echo "Nuevo mensaje" >> saludo.txt` |
|  `2>`   | Redirige los errores estándar (stderr) de un comando hacia un archivo                       | Archivo de salida  | `ls /nonexistent 2> error.log`       |
|  `\|`   | Redirige la salida de un comando hacia otro comando como entrada (pipe)                     | Comando(s)         | `cat archivo.txt \| grep "texto"`    |
|  `tee`  | Redirige la salida estándar a un archivo y también la muestra en la terminal                | Archivo de salida  | `echo "Texto" \| tee archivo.txt`    |

## Operadores de Control

| Comando | Descripción                                                                            | Argumento  | Ejemplo                                  |
| :-----: | :------------------------------------------------------------------------------------- | ---------- | ---------------------------------------- |
|   `;`   | Ejecuta varios comandos secuencialmente, sin importar si los anteriores tuvieron éxito | Comando(s) | `echo "Hola"; ls`                        |
|   `&`   | Ejecuta un comando en segundo plano                                                    | Comando    | `sleep 10 &`                             |
|  `&&`   | Ejecuta el segundo comando solo si el primero tuvo éxito (exit code 0)                 | Comando(s) | `mkdir carpeta && cd carpeta`            |
| `\|\|`  | Ejecuta o el primer comando o el segundo comando                                       | Comando(s) | `locate "name" \|\| find / -name "name"` |

## Variables de Entorno

|       Comando       | Descripción                                                        | Ejemplo                            |
| :-----------------: | :----------------------------------------------------------------- | ---------------------------------- |
| `env`<br>`printenv` | Imprime todas las variables de entorno                             | `printenv`                         |
|  `export $VAR=val`  | Crea e inicializa una variable de entorno válida durante la sesión | `export PATH=$PATH:/usr/local/bin` |

### Variables Comunes de Entorno

| Variable de Entorno | Descripción                                                                                                                               |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `PATH`              | Define los directorios donde se buscan los ejecutables. Cuando se escribe un comando, el sistema busca el ejecutable en estos directorios |
| `HOME`              | Especifica el directorio personal del usuario                                                                                             |
| `SHELL`             | Define el tipo de shell que se está utilizando (por ejemplo, `/bin/bash`)                                                                 |
| `USER`              | Contiene el nombre del usuario que está actualmente conectado                                                                             |
| `GROUPS`            | Lista los grupos a los que pertenece el usuario                                                                                           |
| `LANG`              | Especifica la configuración de idioma y la localización del sistema                                                                       |
| `TZ`                | Define la zona horaria del sistema                                                                                                        |
| `XDG_DATA_DIRS`     | Lista los directorios en los que se buscan los archivos de datos de las aplicaciones de escritorio                                        |
| `EDITOR`            | Especifica el editor de texto predeterminado                                                                                              |
| `VISUAL`            | Especifica el editor de texto visual preferido para las aplicaciones que requieren un editor interactivo                                  |

### Otras Variables Comunes

| Variable de Entorno | Descripción                                                                        |
| ------------------- | ---------------------------------------------------------------------------------- |
| `PS1`               | Define la cadena de prompt principal (por ejemplo, `usuario@hostname:/directorio`) |
| `LD_LIBRARY_PATH`   | Especifica las rutas donde se buscan bibliotecas compartidas                       |
| `TERM`              | Define el tipo de terminal (por ejemplo, `xterm` o `linux`)                        |
| `HISTFILE`          | Ubicación del archivo donde se guarda el historial de comandos                     |
| `SHLVL`             | Indica el nivel de profundidad de los shells anidados                              |
| `MAIL`              | Indica la ubicación del buzón de correo del usuario                                |

## Comunicación Entre Usuarios

| Comando |                                 Nombre                                  | Descripción                 |
| :-----: | :---------------------------------------------------------------------: | --------------------------- |
| `users` |       Muestra todos los usuarios que están logeados en el sistema       | `users`                     |
| `wall`  |      Envía un mensaje a todos los usuarios logeados en el sistema       | `wall "Mensaje para todos"` |
| `write` | Envía un mensaje a un usuario específico que está logeado en el sistema | `write usuario`             |

<div style="page-break-after: always;"></div>

---

## Referencias

- Gite V.
  (noviembre 01, 2024).
  _Linux List All Environment Variables Command_
  Recuperado el 08 de diciembre de 2024 de
  <https://www.cyberciti.biz/faq/linux-list-all-environment-variables-env-command/>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f.).
  _Talkin to Users (users, wall, write)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Recuperado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9846908>
