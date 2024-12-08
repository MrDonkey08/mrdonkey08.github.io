---
layout: post
title: Tipos de Archivos y Permisos de Archivos
author: Alan Yahir Juárez Rubio
description: |
  Cuáles son los diferentes tipos de archivos y en qué se diferencian. Además
  como gestionar los permisos de archivos y como gestionar a los usuarios

categories:
  - linux
  - comandos
tags:
  - archivos
  - directorios
  - grupos
  - permisos
  - usuarios

date: 2023-12-11 15:22
last_updated: 2024-12-08

toc:
  beginning: true

pretty_table: true
---

## Tipos de Archivos

| Atributos | Tipo de Archivo                           | Descripción                                                                                                            |
| :-------: | ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
|     -     | Archivo normal                            | Archivo de texto, binario u otro formato estándar                                                                      |
|     d     | Directorio                                | Carpeta que contiene archivos y otros directorios                                                                      |
|     l     | Link (simbólico o fuerte)                 | Referencia a otro archivo o directorio. Un enlace simbólico es flexible, pero un enlace fuerte comparte el mismo inode |
|     c     | Archivo especial o archivo de dispositivo | Representa dispositivos como terminales, impresoras u otros periféricos                                                |
|     s     | Socket                                    | Archivos usados para la comunicación de redes entre procesos                                                           |
|     p     | Tubería nombrada                          | Representa archivos FIFO, usados para la comunicación entre procesos                                                   |
|     b     | Archivo de bloque especial                | Archivos que manejan información en bloques, como discos duros o unidades USB                                          |

## Permisos de Usuarios

| Comando  | Descripción                                                            | Argumento                                                                | Ejemplo                                                                     |
| -------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------ | --------------------------------------------------------------------------- |
| `su`     | Permite cambiar de usuario. Si no se especifica usuario, cambia a root | Usuario a iniciar sesión                                                 | `su`<br>`su administrador`                                                  |
| `sudo`   | Ejecuta un comando con privilegios de root por cierto tiempo           | Comando a ejecutar                                                       | `sudo updatedb`                                                             |
| `chmod`  | Cambia los permisos del archivo                                        | tipo de usuario(s) +/- permiso<br>permiso de usuarios en dígitos octales | `chmod u+x programa`<br>`chmod 644 archivo.txt`                             |
| `chown`  | Cambia el propietario y grupo del archivo                              | Usuario y grupo                                                          | `chown tecnico:tecnicos archivo.log`<br>`chown -R contador:contadores sat/` |
| `chgrp`  | Cambia el grupo propietario del archivo                                | Grupo                                                                    | `chgrp administradores archivo.txt`                                         |
| `passwd` | Cambia la contraseña de un usuario                                     | Usuario (si no se especifica, cambia la contraseña del usuario actual)   | `passwd usuario1`                                                           |
| `groups` | Muestra los grupos a los que pertenece el usuario actual               | Ninguno                                                                  | `groups`                                                                    |
| `umask`  | Configura los permisos por defecto para archivos nuevos                | Máscara de permisos en formato octal                                     | `umask 022`                                                                 |

## Gestión de Usuarios

| Comando    | Descripción                                                       | Argumento          | Ejemplo                     |
| ---------- | ----------------------------------------------------------------- | ------------------ | --------------------------- |
| `useradd`  | Crea un nuevo usuario                                             | Nombre de usuario  | `useradd usuario1`          |
| `groupadd` | Crea un nuevo grupo                                               | Nombre de grupo    | `groupadd contadores`       |
| `usermod`  | Modifica la configuración de un usuario                           | Opciones y usuario | `usermod -aG sudo usuario1` |
| `userdel`  | Elimina un usuario (opción `-r` para eliminar su directorio home) | Nombre de usuario  | `userdel -r usuario1`       |
| `groupdel` | Elimina un grupo                                                  | Nombre de grupo    | `groupdel contadores`       |

<div style="page-break-after: always;"></div>

---

## Referencias

- Platzi
  (s.f.).
  _Command Line Cheat Sheet_.
  Consultado el 04 de diciembre de 2023 de
- <https://static.platzi.com/media/public/uploads/command-line-cheat-sheet_93c5cbb9-8acf-423e-a92e-351a461f15ae.pdf>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f)
  _Linux File Types_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/10173348>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f)
  _User Account Management (useradd, groupadd, usermod, userdel, groupdel)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9165636>
