---
title: Archivos y Permisos
author: Alan Yahir Juárez Rubio
type: Nota

aliases:
tags:

creation date: 11-12-2023
last modification date: 14-12-2023
---

# Archivos

## Tipos de Archivos

| Atributos |      Tipo de Archivo       | Descripción                                                               |
| :-------: | :------------------------: | ------------------------------------------------------------------------- |
|     d     |       Archivo normal       |                                                                           |
|     l     |       Link simbólico       |                                                                           |
|     b     | Archivo de bloque especial | Archivo que manejea la información de los _bloques de datos_ como una USB |

## Permisos de Usuarios

| Comando  | Nombre | Descripción                                                     |               Flags               | Argumento | Ejemplo |
| :------: | :----: | :-------------------------------------------------------------- | :-------------------------------: | :-------: | ------- |
| `chmod`  |        | Cambia los permisos del archivo                                 |                                   |           |         |
|   `id`   |        |                                                                 | `a`, `G`, `g`, `n`, `r`, `u`, `z` |           |         |
| `whoami` |        | Muestra el nombre de usuario                                    |                                   |           |         |
|   `su`   |        | Cambias al usuario root                                         |                                   |           |         |
|  `sudo`  |        | Da privilegios de root para ejecutar comandos por cierto tiempo |                                   |           |         |
| `chown`  |        | Cambia el propietario y grupo del archivo                       |      `c`, `f`, `v`, `h`, `r`      |           |         |
| `chgrp`  |        |                                                                 |                                   |           |         |
| `passwd` |        |                                                                 |                                   |           |         |
| `groups` |        |                                                                 |                                   |           |         |
| `umask`  |        |                                                                 |                                   |           |         |

<div style="page-break-after: always;"></div>

## Referencias
