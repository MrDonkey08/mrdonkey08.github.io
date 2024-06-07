---
title: Linea de Comandos
author: Alan Yahir Juárez Rubio
type: Nota

aliases:
tags: Manual, Ayuda

creation date:: 11-12-2023
last modification date: 13-12-2023
---

# Línea de Comandos

## Utilidad de la Línea de Comandos

|  Comando   |     Nombre      | Descripción                                                                                                        |                         Flags                          |           Argumento            | Ejemplo                                                                     |
| :--------: | :-------------: | :----------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------: | :----------------------------: | --------------------------------------------------------------------------- |
|  `clear`   |     limpiar     | Limpia la pantalla de la terminal                                                                                  |                          `x`                           |               -                | `clear`                                                                     |
|   `echo`   |        -        | Imprime texto en la terminal                                                                                       |    `e` (habilita interpretación de backslash `\`),     |           `"Texto"`            | `echo "Mensaje"`, `echo - e "Mensaje \nSalto de línea"`                     |
|  `printf`  | print formatted | Imprime texto operando como `printf` de C/C++                                                                      |                           -                            | `"Texto" valores-a-concatenar` | `printf "Hola, %s, tú número es: %i\n\n" Alberto 123`                       |
|   `date`   |      fecha      | Imprime o establece la fecha y hora del sistema                                                                    |                   `d`, `s`, `f`, `r`                   |        `Opción formato`        | `date`, `date "+%m/%d/%y"`                                                  |
|   `cal`    |    calendar     | Imprime un calendario (mes actual si no se indican parámetros)                                                     |            `3`, `A <n>`, `B <n>`, `j`, `y`             |       `Año` o `mes año`        | `cal`, `cal 2020`, `cal 8 2022`, `cal -y`, `cal -j`, `cal -A 2`, `cal -B 2` |
| `hostname` | nombre del host | Imprime el nombre del host                                                                                         |             `b <nuevo hostname>`, `i`, `I`             |               -                | `hostname`                                                                  |
|   `who`    |      quién      | Imprime información sobre el usuario actual                                                                        |                           -                            |               -                | `who`                                                                       |
|    `w`     |        -        | Igual que `who`, pero imprime mucha más información                                                                |                           -                            |               -                | `w`                                                                         |
|    `ps`    |        -        | Muestra los procesos ejecutándose en la sesión de Terminal                                                         |                           -                            |               -                | `ps`                                                                        |
|   `kill`   | matar/terminar  | Temina el proceso indicado (Si no se especifica una señal, se enviará una por defecto, que suele ser SIGTERM (15)) | `s <nombre de señal>`, `n <número de señal>`, `l`, `L` |     `PID` (ID del Proceso)     | `kill 2983`                                                                 |

## Ayuda

| Comando  | Nombre | Descripción                                         | Argumento  | Ejemplo        |
| :------: | :----: | :-------------------------------------------------- | :--------: | -------------- |
|  `man`   | manual | Muestra el manual de un comando específico          |  Comando   | `man ls`       |
|  `help`  | ayuda  | Muestra información de ayuda para comandos de shell | Comando(s) | `help cd`      |
| `which`  |  cuál  | Muestra la ruta del ejecutable de un comando        |  Comando   | `which python` |
| `whatis` | qué es | Muestra una breve descripción del comando           |  Comando   | `whatis ls`    |

## Referencias

- https://www.geeksforgeeks.org/clear-command-in-linux-with-examples/
- https://linuxopsys.com/topics/cal-command-in-linux
