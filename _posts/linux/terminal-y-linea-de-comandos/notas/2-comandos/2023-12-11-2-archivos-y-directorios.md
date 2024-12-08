---
layout: post
title: Manejo de Archivos y Directorios
author: Alan Yahir Juárez Rubio
description: |
  Comandos básicoas para la nevegación entre archivos y directorios y variedad
  de comandos para su respectiva manipulación

categories:
  - linux
  - comandos
tags:
  - archivado
  - archivos
  - directorios
  - conversión
  - compresión

date: 2023-12-11 10:55
last_updated: 2024-12-08

toc:
  beginning: true

pretty_table: true
---

## Navegación Entre Archivos

### Desplazamiento

| Comando | Descripción                                    | Argumento           | Ejemplo                       |
| ------- | ---------------------------------------------- | ------------------- | ----------------------------- |
| `cd`    | Cambia al directorio especificado              | Ruta del directorio | `cd documentos/pdf`<br>`cd ~` |
| `pwd`   | Muestra la ruta completa del directorio actual | -                   | `pwd`                         |

### Consulta

| Comando | Descripción                                                                           | Argumento           | Ejemplo                                              |
| ------- | ------------------------------------------------------------------------------------- | ------------------- | ---------------------------------------------------- |
| `ls`    | Lista los archivos y carpetas de un directorio. Con opciones muestra más detalles     | Ruta del directorio | `ls`<br>`ls -al`                                     |
| `tree`  | Imprime los archivos y subdirectorios del directorio recursivamente en forma de árbol | Ruta del directorio | `tree`<br>`tree -dL 3`                               |
| `file`  | Muestra información acerca de los archivos especificados                              | Archivo(s)          | `file archivo.txt act.pdf`<br>`file -z proyecto.zip` |
| `stat`  | Muestra detalles de un archivo (fecha de modificación, tamaño, etc.)                  | Archivo             | `stat archivo.txt`                                   |
| `du`    | Muestra el uso de espacio de archivos y carpetas                                      | Archivo o carpeta   | `du -sh carpeta/`<br>`du -a archivos/`               |

## Manipulación de Archivos

| Comando | Descripción                                                                                        | Argumento         | Ejemplo                                                       |
| ------- | -------------------------------------------------------------------------------------------------- | ----------------- | ------------------------------------------------------------- |
| `touch` | Crea un archivo vacío con el nombre especificado o actualiza la fecha de modificación              | Archivo           | `touch index.html styles.css`                                 |
| `mkdir` | Crea una carpeta con el nombre especificado. Usa `-p` para crear subdirectorios en cascada         | Nombre            | `mkdir esp mate ingles`<br>`mkdir -p escuela/notas`           |
| `cp`    | Copia un archivo o carpeta en la ruta especificada. Usa `-r` para copiar recursivamente carpetas   | Origen destino    | `cp foto1.png foto2.jpg galeria/`<br>`cp -r fondos/ galeria/` |
| `mv`    | Mueve un archivo o carpeta en la ruta especificada. También puede renombrar archivos o carpetas    | Origen destino    | `mv programa.exe programas/`<br>`mv file.txt archivo.txt`     |
| `rm`    | Elimina permanentemente los archivos especificados. Usa `-r` para eliminar carpetas recursivamente | Archivo o carpeta | `rm borrador.md`<br>`rm -ri musica/`                          |
| `ln`    | Crea un enlace simbólico o físico a un archivo                                                     | Enlace destino    | `ln -s archivo.txt enlace.txt`                                |

### Conversión

| Comando   | Descripción                                                                                      | Argumento                   | Ejemplo                                |
| --------- | ------------------------------------------------------------------------------------------------ | --------------------------- | -------------------------------------- |
| `convert` | Convierte el formato de una imagen a otro (si está instalado ImageMagick)                        | Imagen de entrada y salida  | `magick rose.jpg -resize 50% rose.png` |
| `ffmpeg`  | Convertidor de _media_ universal (audio, video, etc.). Convierte, corta o combina archivos       | Entrada y salida            | `ffmpeg -i entrada.mp4 salida.mp3`     |
| `ffplay`  | Reproductor de _media_ universal (audio, video, etc.)                                            | Archivo                     | `ffplay video.mp4`                     |
| `pandoc`  | Convertidor de _markup_ universal. Convierte entre formatos de texto como Markdown, HTML y LaTeX | Archivo de entrada y salida | `pandoc archivo.md -o archivo.pdf`     |

### Archivado

| Comando | Descripción                                                                     | Argumento                                            | Ejemplo                                                   |
| ------- | ------------------------------------------------------------------------------- | ---------------------------------------------------- | --------------------------------------------------------- |
| `tar`   | Comprime (`-c`) o descomprime (`-x`) un archivo/directorio con el formato `tar` | Archivo de salida y archivo(s)/carpeta(s) de entrada | `tar -cvf imagenes.tar fotos/`<br>`tar -xvf imagenes.tar` |

### Compresión

| Comando               | Descripción                                                                    | Argumento                                               | Ejemplo                               |
| --------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------- | ------------------------------------- |
| `compress`            | Reemplaza el archivo original con una versión comprimida con la extensión `.Z` | Archivo de entrada                                      | `compress receta.txt`                 |
| `gzip`                | Comprime un archivo con formato `gzip`. No funciona con carpetas sin `tar`     | Archivo(s) a comprimir                                  | `gzip todo.txt imagenes.tar`          |
| `gzip -d`<br>`gunzip` | Descomprime un archivo con formato `gzip`                                      | Archivo(s) a descomprimir                               | `gzip -d todo.txt.gz imagenes.tar.gz` |
| `zip`                 | Comprime un archivo/carpeta con el formato `zip`                               | Archivo de salida (`.zip`) y archivo/carpeta de entrada | `zip consultas.zip doc1.txt doc2.txt` |
| `unzip`               | Descomprime un archivo `zip`                                                   | Archivo de entrada (`.zip`)                             | `unzip consultas.zip`                 |
| `xz`                  | Comprime archivos usando el formato `xz`                                       | Archivo(s)                                              | `xz archivo.txt`                      |
| `unxz`                | Descomprime archivos comprimidos con `xz`                                      | Archivo(s)                                              | `unxz archivo.txt.xz`                 |

<div style="page-break-after: always;"></div>

---

### Referencias

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f.).
  _File System Navigation Commands (cd, ls and pwd)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9540520>

- Devars E
  (s.f.).
  _¿Aprendiendo a camninar en la terminal?_.
  Consultado el 04 de diciembre de 2023 de
  <https://platzi.com/home/clases/2292-terminal/37342-aprendiendo-a-caminar-en-la-terminal/>

- Devars E
  (s.f.).
  _Manipulando archivos y directorios_.
  Consultado el 04 de diciembre de 2023 de
- <https://platzi.com/home/clases/2292-terminal/37344-manipulando-archivos-y-directorios/>

- Platzi
  (s.f.).
  _Command Line Cheat Sheet_.
  Consultado el 04 de diciembre de 2023 de
- <https://static.platzi.com/media/public/uploads/command-line-cheat-sheet_93c5cbb9-8acf-423e-a92e-351a461f15ae.pdf>

- Deyimar A.
  (noviembre 21, 2024).
  _Los 40 comandos de Linux más populares e imprescindibles_.
  Consultado el 04 de diciembre de 2023 de
  <https://www.hostinger.mx/tutoriales/linux-comandos>

- Geeksforgeeks
  (julio 12, 2024).
  _ZIP command in Linux with examples_.
  Consultado el 08 de diciembre de 2024 de
  <https://www.geeksforgeeks.org/zip-command-in-linux-with-examples/>
