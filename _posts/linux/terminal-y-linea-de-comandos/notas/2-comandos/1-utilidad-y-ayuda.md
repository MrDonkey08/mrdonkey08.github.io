---
layout: post
title: Utilidad y Consulta
author: Alan Yahir Juárez Rubio
description: |
  Comandos útiles para el uso de la terminal y la consulta de información tal
  como soporte e información del usuario y el sistema

categories:
  - linux
  - comandos
tags:
  - ayuda
  - documentacion
  - utilidad

date: 2023-12-11
last_updated: 2024-12-08

toc:
  sidbar: right
---

## Utilidad

| Comando  | Descripción                                                                             | Argumento                | Ejemplo                                                                                 |
| -------- | --------------------------------------------------------------------------------------- | ------------------------ | --------------------------------------------------------------------------------------- |
| `clear`  | Limpia la pantalla de la terminal                                                       | -                        | `clear`                                                                                 |
| `exit`   | Abandona el _shell_, terminal o la sesión de usuario                                    | -                        | `exit`                                                                                  |
| `echo`   | Imprime texto en la terminal. Permite variables o salida de comandos con `$(comando)`   | "Texto"                  | `echo "Mensaje"`<br>`echo -e "Mensaje\nSalto de línea"`<br>`echo $(date)`               |
| `printf` | Imprime texto formateado similar a `printf` en C/C++                                    | "Formato" y valores      | `printf "Hola %s, tu número es: %i\n\n" Alberto 123`                                    |
| `date`   | Imprime o establece la fecha y hora del sistema. Es compatible con múltiples formatos   | Opción y formato         | `date`<br>`date "+%m/%d/%y"`<br>`date --set="2023-12-01 15:30"`                         |
| `cal`    | Imprime un calendario del mes actual o uno específico                                   | Año / Mes Año / Opciones | `cal`<br>`cal 2020`<br>`cal 8 2022`<br>`cal -y`<br>`cal -j`<br>`cal -A 2`<br>`cal -B 2` |
| `bc`     | Calculadora aritmética. Abre una sesión interactiva o ejecuta comandos desde un archivo | Archivo                  | `bc`<br>`echo "3+5"`<br>`bc archivo.txt`                                                |

## Ayuda

| Comando   | Descripción                                                                                              | Argumento | Ejemplo           |
| --------- | -------------------------------------------------------------------------------------------------------- | --------- | ----------------- |
| `man`     | Muestra el manual de un comando específico                                                               | Comando   | `man ls`          |
| `help`    | Muestra información de ayuda para comandos de shell                                                      | Comando   | `help cd`         |
| `info`    | Muestra la documentación en formato _info_                                                               | Comando   | `info mkdir`      |
| `which`   | Muestra la ruta completa del binario ejecutable asociado a un comando. Busca en todas las rutas del path | Comando   | `which python`    |
| `whatis`  | Muestra una breve descripción del comando                                                                | Comando   | `whatis grep`     |
| `type`    | Muestra información acerca del tipo de comando                                                           | Comando   | `type ls`         |
| `apropos` | Busca comandos relacionados con una palabra clave                                                        | Palabra   | `apropos network` |
| `whereis` | Encuentra la ubicación de binarios, fuentes y manuales de un comando                                     | Comando   | `whereis ls`      |

## Información del Usuario

| Comando  | Descripción                                                                            |
| -------- | -------------------------------------------------------------------------------------- |
| `whoami` | Imprime el nombre del usuario actual                                                   |
| `who`    | Imprime información sobre los usuarios conectados                                      |
| `w`      | Igual que `who`, pero incluye más información, como procesos y actividad               |
| `last`   | Imprime una lista de los últimos usuarios que se han conectado                         |
| `id`     | Imprime información sobre el ID del usuario y los ID de los grupos a los que pertenece |
| `groups` | Lista los grupos a los que pertenece el usuario actual                                 |

## Información del Sistema

| Comando       | Descripción                                                                                         |
| ------------- | --------------------------------------------------------------------------------------------------- |
| `hostname`    | Imprime el nombre del host                                                                          |
| `uptime`      | Imprime información acerca de cuánto tiempo ha estado corriendo el sistema                          |
| `uname`       | Imprime información básica del sistema operativo. Con `-a`, incluye más detalles                    |
| `lsb_release` | Imprime información de la distribución del sistema (solo en distribuciones basadas en Linux)        |
| `dmidecode`   | Describe componentes del sistema (_hardware_), números de serie, revisión de BIOS, etc              |
| `free`        | Muestra información de la memoria (RAM) disponible y usada                                          |
| `df`          | Reporta espacio disponible en discos y particiones. `-h` lo muestra en formato legible para humanos |

<div style="page-break-after: always;"></div>

---

## Referencias

- Geeksforgeeks
  (junio 09, 2023).
  _Clear Command in Linux with Examples_
  Recuperado el 08 de diciembre de 2024 de
  <https://www.geeksforgeeks.org/clear-command-in-linux-with-examples/>

- [Bobbin Zachariah](https://linuxopsys.com/author/bobbin)
  (noviembre 11, 2022).
  _Cal Command in Linux_
  [LinuxOPsys](https://linuxopsys.com/)
  Recuperado el 08 de diciembre de 2024 de
  <https://linuxopsys.com/topics/cal-command-in-linux>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f.).
  _93. Monitor Users (who, last, w, id)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Recuperado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9165640>

- [Linux Command](https://linuxcommand.org/).
  (s.f.).
  _Navigation_
  Recuperado el 08 de diciembre de 2024 de
  <https://linuxcommand.org/lc3_lts0020.php>
