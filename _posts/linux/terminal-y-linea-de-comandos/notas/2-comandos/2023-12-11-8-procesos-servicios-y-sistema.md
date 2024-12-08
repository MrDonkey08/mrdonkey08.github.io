---
layout: post
title: Gestión de Procesos, Servicios y el Sistema
author: Alan Yahir Juárez Rubio
description: |
  Variedad de comandos para la el monitoreo y la gestión de procesos, servicios
  y el sistema

categories:
  - linux
  - comandos
tags:
  - logs
  - procesos
  - servicios
  - sistema

date: 2023-12-11 18:30
last_updated: 2024-12-08

toc:
  beginning: true

pretty_table: true
---

## Administración de Procesos

### Monitoreo

| Comando | Descripción                                                | Ejemplo |
| :-----: | :--------------------------------------------------------- | ------- |
|  `top`  | Muestra una lista interactiva de los procesos en ejecución | `top`   |
|  `ps`   | Muestra los procesos ejecutándose en la sesión de terminal | `ps`    |

### Job Control

| Comando | Descripción                                                                                                                                                                                               | Ejemplo                                       |
| :-----: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
|  `bg`   | Reanuda los procesos suspendidos (se suspenden con `ctrl` + `z`) y los manda al _background_                                                                                                              |                                               |
|  `fg`   | Manda el o los procesos que se encuentran el _background_ hacia el _foreground_                                                                                                                           |                                               |
| `nohup` | Dado un comando como parámetro, permite que el comando siga ejecutándose incluso cuando la terminal ha sido cerrada                                                                                       | `nohup zathura book.pdf`<br>`nohup firefox &` |
| `nice`  | Dado un comando, permite ejecutarlo con una prioridad de agenda (niceness) modificada (i.e. prioridad de ejecución). El _niceness_ es un número entero entre -20 (mayor prioridad) y 19 (menor prioridad) |                                               |

### Comandos de Terminación de Procesos

|  Comando  | Descripción                                                                                                         |       Argumento        | Ejemplo           |
| :-------: | :------------------------------------------------------------------------------------------------------------------ | :--------------------: | ----------------- |
|  `kill`   | Termina el proceso indicado (si no se especifica una señal, se enviará una por defecto, que suele ser SIGTERM (15)) | `PID` (ID del Proceso) | `kill 2983`       |
| `killall` | Igual que `kill`, con la diferencia de que termina cierto proceso y sus respectivos procesos hijos                  |  `Nombre del proceso`  | `killall firefox` |
|  `pkill`  | Igual que `kill` con la diferencia de que pasas el nombre del proceso como argumento                                |  `Nombre del proceso`  | `pkill apache2`   |

## Servicios

|   Comando   | Descripción                                                                                                            |
| :---------: | :--------------------------------------------------------------------------------------------------------------------- |
| `systemctl` | Herramienta para controlar el sistema _systemd_ y el administrador de servicios                                        |
|  `crontab`  | Agenda tareas periódicas en una fecha y hora establecida                                                               |
|    `at`     | Permite agendar tareas en una hora específica para su única ejecución. Adicionalmente es posible especificar una fecha |

## Monitoreo del Sistema

|       Comando       | Descripción                                                                                   |
| :-----------------: | --------------------------------------------------------------------------------------------- |
|        `top`        | Muestra información en tiempo real sobre los procesos en ejecución                            |
|        `df`         | Imprime el uso de espacio del sistema de archivos (e.g. unidades, particiones)                |
|       `dmesg`       | Imprime o controla el _kernel ring buffer_, información del arranque y errores del sistema    |
|      `iostat`       | Imprime estadísticas del CPU y estadísticas de _input/output_ para dispositivos y particiones |
|      `netstat`      | Imprime conexiones de red, tablas de enrutamiento, estadísticas de interfaz, etc              |
|        `ip`         | Imprime y manipula enrutamiento, dispositivos de red, interfaces y túneles                    |
|        `ss`         | Herramienta para investigar _sockets_ y conexiones de red                                     |
|       `free`        | Muestra la cantidad de memoria libre y usada en el sistema                                    |
| `cat /proc/cpuinfo` | Muestra información técnica acerca de la CPU                                                  |
| `cat /proc/meminfo` | Muestra información técnica acerca de la memoria                                              |

---

## Monitoreo de _Logs_ (Registros)

Directorio de Logs: `/var/log/`

| Archivo    | Contenido                                                                           |
| ---------- | ----------------------------------------------------------------------------------- |
| `boot`     | Logs acerca del arranque del sistema                                                |
| `chrony`   | Logs acerca del servicio `chrony`                                                   |
| `cron`     | Logs acerca de las tareas agendadas mediante `crontab`                              |
| `mailog`   | Logs acerca de los correos entrantes y salientes del sistema                        |
| `secure`   | Logs acerca del inicio y cierre de sesión (autenticación)                           |
| `messages` | Logs acerca de la información sobre software, hardware, aplicaciones, procesos, etc |
| `httpd`    | Logs del servidor web Apache HTTP (si está instalado)                               |

<div style="page-break-after: always;"></div>

---

## Referencias

- [Linux Command](https://linuxcommand.org/).
  (s.f.).
  _Job Control_.
  Consultado el 08 de diciembre de 2024 de
- <https://linuxcommand.org/lc3_lts0100.php>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f)
  _108. System Logs Monitor (/var/log)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9656582>

- [Imran Afzal](https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/#instructor-1)
  (s.f)
  _System Monitoring Commands (df, dmesg, iostat 1, netstat, free, top)_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 08 de diciembre de 2024 de
- <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9165602/12445338>
