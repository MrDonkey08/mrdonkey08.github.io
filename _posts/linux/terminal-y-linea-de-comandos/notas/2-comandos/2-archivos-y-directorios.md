---
title: Manipulación de Archivos y Directorios
author: Alan Yahir Juárez Rubio
type: Nota

aliases: Comandos básicos, Coamndos esenciales
tags: Archivos, Directorios, Conversión, Compresión

creation date: 11-12-2023
last modification date: 13-12-2023
---

# Manipulación de Archivos y Directorios

## Desplazamiento

| Comando |         Nombre          | Descripción                             |  Flags   |       Argumento       | Ejemplo             |
| :-----: | :---------------------: | :-------------------------------------- | :------: | :-------------------: | ------------------- |
|  `cd`   |    Change Directory     | Cambia al directorio especificado       |    -     | `Ruta/del/directorio` | `cd documentos/pdf` |
|  `pwd`  | Print Working Directory | Muestra la `Ruta/del/directorio` actual | `L`, `P` |           -           | `pwd`               |

## Consulta

| Comando |     Nombre     | Descripción                                                                           |                   Flags                   | Argumento             | Ejemplo                                            |
| :-----: | :------------: | :------------------------------------------------------------------------------------ | :---------------------------------------: | :-------------------- | -------------------------------------------------- |
|  `ls`   |      List      | Lista los archivos y carpetas de un directorio                                        |  `a`, `A`, `h`, `l`, `r`, `s`, `S`, `t`   | `Ruta/del/directorio` | `ls -al`                                           |
| `tree`  | directory tree | Imprime los archivos y subdirectorios del directorio recursivamente a manera de árbol | `a`, `D`, `d`, `r`, `s`, `t`, `L <level>` | `Ruta/del/directorio` | `tree -dL 3`                                       |
| `file`  |       -        | Te muestra información acerca de los archivos especificados                           |               `b`, `c`, `z`               | `Archivo`             | `file archivo.txt act.pdf`, `file -z proyecto.zip` |

## Manipulación

| Comando |     Nombre     | Descripción                                                                                                    |     Flags      | Argumento        | Ejemplo                                                              |
| :-----: | :------------: | :------------------------------------------------------------------------------------------------------------- | :------------: | :--------------- | -------------------------------------------------------------------- |
| `touch` |       -        | Crea un archivo con el nombre especificado                                                                     | `c`, `d`, `m`  | `Archivo`        | `touch index.html styles.css`                                        |
| `mkdir` | Make directory | Crea una carpeta con el nombre especificado                                                                    | `m`, `p`, `v`  | `Nombre`         | `mkdir esp mate ingles`, `mkdir -p escuela/notas`                    |
|  `cp`   |      Copy      | Copia un archivo o carpeta en la ruta especificada                                                             | `f`, `i` , `r` | `Origen destino` | `cp foto1.png foto2.jpg galeria/`, `cp -r fondos/ galeria/`          |
|  `mv`   |      Move      | Mueve un archivo o carpeta en la ruta especificada. También puede modificar el nombre de un archivo/directorio |    `f`, `i`    | `Origen destino` | `mv programa.exe programa.msi programas/`, `mv file.txt archivo.txt` |
|  `rm`   |     Remove     | Elimina permenanetemente los archivos especificados                                                            | `f`, `i` , `r` | `Archivo`        | `rm borrador.md carta.docx` , `rm -ri musica/`                       |

## Conversión y compresión

|  Comando   |       Nombre       | Descripción                                                                                                                     |                      Flags                       | Argumento                                               | Ejemplo                                                        |
| :--------: | :----------------: | :------------------------------------------------------------------------------------------------------------------------------ | :----------------------------------------------: | :------------------------------------------------------ | -------------------------------------------------------------- |
| `compress` |     Comprimir      | Remplaza el archivo original con una versión comprimida con la extensión `.z`, manteniendo los mismos atributos que el original |             `c`, `f`, `i` , `r`, `v`             | Archivo de entrada                                      | `compress receta.txt`                                          |
| `convert`  | Convertir (magick) | Convierte el formato de una imagen a otro sin reemplzar la imagen original                                                      |        `-resize <n>%`, `-compress <type>`        | Imagen de entrada y salida                              | `convert rose.jpg -resize 50% rose.png`                        |
|   `tar`    |         -          | Comprime (`c`) o descomprime (`x`) un archivo/directorio con el formato `tar`                                                   | `a`, `c`, `f`, `j`, `r`, `v`, `t`, `u`, `x`, `z` | Archivo/carpeta de entrada y salida                     | `tar -cvf imagenes.tar fotos/`, `tar -xvf fotos/ imagenes.tar` |
|   `zip`    |         -          | Comprime un archivo/carpeta con el formato `zip`                                                                                |        `d`, `m`, `P`, `r`, `u`, `v`, `x`         | Archivo de salida (`.zip`) y archivo/carpeta de entrada | `consultas.zip doc1.txt doc2.txt`                              |
|  `unzip`   |         -          | Descomprime un archivo `zip`                                                                                                    |           `d`, `l`, `n`, `P`, `q`, `x`           | Archivo de entrada (`.zip`)                             | `unzip consultas.zip`                                          |

## Referencias

- https://platzi.com/new-home/clases/2292-terminal/37342-aprendiendo-a-caminar-en-la-terminal/
- https://platzi.com/new-home/clases/2292-terminal/37344-manipulando-archivos-y-directorios/
- https://static.platzi.com/media/public/uploads/command-line-cheat-sheet_93c5cbb9-8acf-423e-a92e-351a461f15ae.pdf
- https://www.hostinger.mx/tutoriales/linux-comandos#15_Comando_df
- https://www.geeksforgeeks.org/zip-command-in-linux-with-examples/
