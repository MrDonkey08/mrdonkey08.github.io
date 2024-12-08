---
layout: post
title: Búsqueda de Archivos y Procesamiento de Texto
author: Alan Yahir Juárez Rubio
description: |
  Variedad de comandos útiles para encontrar archivos, mostrar su contenido
  y filtrarlo, procesar dicho contenido

categories:
  - linux
  - comandos
tags:
  - archivos
  - busqueda
  - filtros
  - impresion

date: 2023-12-11 13:02
last_updated: 2024-12-08

toc:
  beginning: true

pretty_table: true
---

## Búsqueda de Archivos

| Comando   | Descripción                                                                                                                     | Argumento                          | Ejemplo                                                   |
| --------- | ------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- | --------------------------------------------------------- |
| `find`    | Busca archivos en una jerarquía de directorios, filtrando por nombre, tamaño, tipo, etc                                         | Ruta del directorio y criterio     | `find ./ -name "main.cpp"`<br>`find ~/Documents/ -type d` |
| `locate`  | Busca archivos rápidamente a partir de una base de datos que puede ser actualizada con `updatedb`. No incluye cambios recientes | Nombre del archivo (o parte de él) | `locate bash`<br>`locate '*.txt'`                         |
| `whereis` | Encuentra la ubicación de binarios, fuentes y manuales de un comando                                                            | Comando                            | `whereis ls`                                              |
| `which`   | Muestra la ruta completa del binario ejecutable asociado a un comando                                                           | Comando                            | `which python`                                            |

## Muestreo de Texto

| Comando | Descripción                                                                                               | Argumento  | Ejemplo                                    |
| ------- | --------------------------------------------------------------------------------------------------------- | ---------- | ------------------------------------------ |
| `head`  | Imprime las primeras 10 líneas de un archivo. Usa `-n` para especificar el número de líneas               | Archivo    | `head nota.md`<br>`head -n 5 archivo.txt`  |
| `tail`  | Imprime las últimas 10 líneas de un archivo. Usa `-n` para especificar el número de líneas                | Archivo    | `tail log.txt`<br>`tail -n 20 archivo.log` |
| `more`  | Imprime el contenido de un archivo página por página                                                      | Archivo    | `more log`                                 |
| `less`  | Similar a `more`, pero con funcionalidad extra (e.g., búsqueda interactiva). Se puede navegar hacia atrás | Archivo    | `less main.c`                              |
| `cat`   | Concatena el contenido de archivos y lo imprime en la salida estándar                                     | Archivo(s) | `cat archivo1.txt archivo2.txt`            |
| `tac`   | Similar a `cat`, pero imprime el contenido en orden inverso                                               | Archivo    | `tac archivo.txt`                          |

## Filtros o Procesamiento de Texto

| Comando   | Descripción                                                                                          | Argumento             | Ejemplo                                           |
| --------- | ---------------------------------------------------------------------------------------------------- | --------------------- | ------------------------------------------------- |
| `grep`    | Busca patrones en un archivo e imprime las líneas donde se encuentran los patrones                   | Archivo y expresión   | `grep "todo" tasks.txt`                           |
| `grep -E` | Versión extendida de `grep`. Similar a `egrep` pero preferida actualmente                            | Archivo y expresión   | `grep -E "(Error\|Warning)" archivo.log`          |
| `grep -i` | Realiza una búsqueda insensible a mayúsculas                                                         | Archivo y expresión   | `grep -i "Linux" texto.txt`                       |
| `cut`     | Extrae secciones específicas de las líneas de un archivo basado en campos o caracteres delimitadores | Archivo y delimitador | `cut -d':' -f1 archivo.csv`                       |
| `awk`     | Herramienta de procesamiento de texto avanzada; selecciona y manipula columnas de texto              | Archivo y script      | `awk '{print $1}' archivo.txt`                    |
| `sort`    | Ordena las líneas de un archivo                                                                      | Archivo y opciones    | `sort archivo.txt`<br>`sort -r archivo.txt`       |
| `uniq`    | Elimina líneas duplicadas consecutivas (requiere que la entrada esté ordenada)                       | Archivo               | `uniq archivo.txt`                                |
| `wc`      | Cuenta palabras, líneas y caracteres de un archivo                                                   | Archivo               | `wc archivo.txt`<br>`wc -l archivo.txt`           |
| `fmt`     | Reformatea texto para ajustarlo a un ancho de línea específico                                       | Archivo               | `fmt -w 50 texto.txt`                             |
| `pr`      | Divide un archivo en páginas para su impresión                                                       | Archivo y opciones    | `pr -h "Título" archivo.txt`                      |
| `tr`      | Traduce o elimina caracteres específicos                                                             | Entrada y salida      | `tr 'a-z' 'A-Z' < archivo.txt`<br>`tr -d 'aeiou'` |
| `sed`     | Procesa y transforma texto mediante expresiones regulares. Permite editar archivos en línea          | Archivo y script      | `sed 's/Linux/Unix/' archivo.txt`                 |

<div style="page-break-after: always;"></div>

---

## Referencias

- Platzi
  (s.f.).
  _Explorando el contenido de nuestros archivos_.
  Consultado el 04 de diciembre de 2023 de
  <https://platzi.com/home/clases/2292-terminal/37345-explorando-el-contenido-de-nuestros-archivos/>

- Platzi
  (s.f.).
  _Command Line Cheat Sheet_.
  Consultado el 04 de diciembre de 2023 de
- <https://static.platzi.com/media/public/uploads/command-line-cheat-sheet_93c5cbb9-8acf-423e-a92e-351a461f15ae.pdf>

- Pankaj & Singh A.
  (Agosto 3, 2022).
  _Grep Command in Linux/UNIX_.
  Consultado el 04 de diciembre de 2023 de
  <https://www.digitalocean.com/community/tutorials/grep-command-in-linux-unix>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f)
  _Filters / Text Processing Commands_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/16199784>
