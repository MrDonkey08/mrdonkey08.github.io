---
layout: post
title: Redes
author: Alan Yahir Juárez Rubio
description: |
  Variedad de utilidades de red

categories:
  - linux
  - comandos
tags:
  - redes
  - ssh
  - utilidades

date: 2023-12-11
last_updated: 2024-12-08

toc:
  sidbar: right
---

## Utilidades de Red

| Comando                | Descripción                                                                                      | Argumento           | Ejemplo                                         |
| ---------------------- | ------------------------------------------------------------------------------------------------ | ------------------- | ----------------------------------------------- |
| `ping`                 | Envía paquetes ICMP a una dirección IP o dominio para comprobar la conectividad y medir latencia | Dirección o dominio | `ping google.com`                               |
| `ifup`                 | Activa una interfaz de red especificada en la configuración del sistema                          | Interfaz            | `ifup eth0`                                     |
| `ifdown`               | Desactiva una interfaz de red especificada en la configuración del sistema                       | Interfaz            | `ifdown wlan0`                                  |
| `nmcli`                | Herramienta de línea de comandos para gestionar conexiones de red mediante NetworkManager        | Comandos y opciones | `nmcli dev status`, `nmcli con up "Wi-Fi"`      |
| `nm-connection-editor` | Abre una interfaz gráfica para editar las conexiones gestionadas por NetworkManager              | -                   | `nm-connection-editor`                          |
| `ethtool`              | Muestra o modifica los parámetros de una interfaz de red                                         | Interfaz            | `ethtool eth0`                                  |
| `netstat`              | Muestra estadísticas de red, conexiones activas, puertos abiertos y más. (Obsoleto, usar `ss`)   | Opciones            | `netstat -an`, `netstat -tuln`                  |
| `tcpdump`              | Captura y analiza paquetes de red en tiempo real                                                 | Interfaz y filtros  | `tcpdump -i eth0`, `tcpdump port 80`            |
| `ifconfig`             | Configura y muestra información sobre interfaces de red. (Obsoleto, usar `ip`)                   | Interfaz y opciones | `ifconfig eth0`, `ifconfig eth0 up`             |
| `curl`                 | Herramienta para transferir datos desde o hacia un servidor utilizando múltiples protocolos      | URL y opciones      | `curl https://example.com`                      |
| `wget`                 | Descarga archivos desde la web a través de HTTP, HTTPS o FTP                                     | URL                 | `wget https://example.com/archivo.zip`          |
| `traceroute`           | Muestra la ruta que toman los paquetes para llegar a un destino                                  | Dirección o dominio | `traceroute google.com`                         |
| `ssh`                  | Inicia una conexión segura a un servidor remoto a través del protocolo SSH                       | Usuario@host        | `ssh user@192.168.1.1`, `ssh -p 2222 user@host` |
| `telnet`               | Conecta a un puerto de un host remoto para pruebas de red                                        | Dirección y puerto  | `telnet 192.168.1.1 80`                         |
| `ss`                   | Muestra estadísticas y conexiones de red activas. Reemplaza a `netstat`                          | Opciones            | `ss -tuln`, `ss -p`                             |

<div style="page-break-after: always;"></div>

---

## Referencias
