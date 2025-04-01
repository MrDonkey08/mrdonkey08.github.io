---
layout: post
title: Introducción a Linux
author: Alan Yahir Juárez Rubio
description: |
  Qué es Linux, cuáles son sus orígenes, distribuciones de Linux y distintas
  maneras de instalar Linux

categories:
  - linux
tags:
  - gnu
  - linux
  - distro

date: 2025-03-29 16:24
last_updated: 2025-03-29 16:24

toc:
  sidebar: right

pretty_table: true
---

## Orígenes de Linux

### El Nacimiento del Kernel

El **kernel de Linux** fue creado por **Linus Torvalds** en 1991 como proyecto
universitario en Helsinki. Su objetivo inicial era desarrollar un kernel
**libre** y **gratuito** compatible con Unix.

### El Proyecto GNU

El proyecto **GNU (GNU's Not Unix)** fue iniciado por **Richard Stallman** en
1983 con el objetivo de desarrollar un SO completamente libre y de código
abierto denominado GNU.

El proyecto **GNU** desarrollo muchas de las herramientas esenciales que se
utilizan en los SO's modernos, tales como GCC (compilador de C/C++), Bash
(shell), bibliotecas del sistema, etc.

### GNU/Linux: La Unión Fundamental

**GNU/Linux** es la colaboración entre el proyecto **GNU** y el **kernel de
Linux** para desarrollar SO completo libre y de código abierto.

> - El término "Linux" coloquialmente se refiere a sistemas GNU/Linux, pero
>   técnicamente solo es el kernel.
>
> - Usaremos "Linux" para referirnos a los sistemas GNU/Linux de ahora en
>   adelante.
{: .block-note }

## Por Qué Usar Linux (Ventajas)

| Ventaja                                            | Detalle                                                                        |
| -------------------------------------------------- | ------------------------------------------------------------------------------ |
| **Gratuito**                                       | Sin costos de licencia (aunque algunas distros empresariales son pagadas)      |
| **Código abierto**                                 | Transparencia total: cualquiera puede auditar o modificar el código            |
| **Personalizable**                                 | Desde el kernel hasta el escritorio (ideal para desarrolladores y entusiastas) |
| **Eficiencia**                                     | Funciona en hardware antiguo (e.g., Pentium IV con 1GB RAM)                    |
| **Seguridad**                                      | Arquitectura de permisos robusta + menor objetivo de malware vs Windows        |
| **Dominio en servidores y computación en la nube** | ~96% de los top 1M sitios web usan Linux (ZDNet, 2024)                         |
| **Herramientas nativas**                           | Mejor soporte para desarrollo, redes y ciberseguridad (Python, Docker, etc.)   |

## Por Qué No Usar Linux (Desventajas)

| Desventaja               | Detalle                                                                                    |
| ------------------------ | ------------------------------------------------------------------------------------------ |
| **Compatibilidad**       | Algunas aplicaciones populares no están disponibles (e.g., Adobe Suite, muchos juegos AAA) |
| **Curva de aprendizaje** | Requiere aprender comandos básicos para tareas avanzadas                                   |
| **Drivers**              | Hardware muy nuevo o especializado puede no tener soporte inmediato                        |

## Distribuciones de Linux

Linux es una **familia de sistemas operativos** personalizables llamados
**distribuciones** (distros). Cada distro combina:

- Kernel Linux
- Herramientas GNU
- Entorno de escritorio
- Gestor de paquetes
- Software preinstalado

### Fáciles

| Distro     | Descripción                                          | Basada en |
| ---------- | ---------------------------------------------------- | --------- |
| Debian     | Estable, versátil y comunidad sólida                 | -         |
| Ubuntu     | Sistema operativo popular y fácil para principiantes | Debian    |
| Fedora     | Innovadora, ideal para desarrolladores               | Red Hat   |
| Linux Mint | Estable y elegante, basado en Ubuntu                 | Ubuntu    |
| MX Linux   | Ligera y estable con herramientas preinstaladas      | Debian    |
| Deepin     | Interfaz visual moderna y fluida                     | Ubuntu    |
| Zorin OS   | Diseñado para transición desde Windows/macOS         | Ubuntu    |

### Avanzadas

| Distro     | Descripción                                    | Basada en |
| ---------- | ---------------------------------------------- | --------- |
| Arch Linux | Rolling-release, altamente personalizable      | -         |
| Gentoo     | Compilada desde código para máximo control     | -         |
| Slackware  | Una de las distros más antiguas y minimalistas | -         |

### Super Ligeras (<500MB RAM)

| Distro      | Descripción                              | Basada en |
| ----------- | ---------------------------------------- | --------- |
| AntiX       | Minimalista para hardware antiguo        | Debian    |
| Puppy Linux | Ultracompacta, ejecutable desde RAM      | -         |
| Tiny Core   | Mínimo tamaño (~15MB), altamente modular | -         |

### Ligeras (1GB+ RAM)

| Distro        | Descripción                                   | Basada en |
| ------------- | --------------------------------------------- | --------- |
| Lubuntu       | Ubuntu con LXQt/LXDE para hardware modesto    | Ubuntu    |
| Xubuntu       | Ubuntu con Xfce, equilibrio entre rendimiento | Ubuntu    |
| Linux Lite    | Diseñada para usuarios de Windows             | Ubuntu    |
| Peppermint OS | Híbrida entre escritorio y nube               | Debian    |

### Ciberseguridad

| Distro     | Descripción                              | Basada en  |
| ---------- | ---------------------------------------- | ---------- |
| Kali Linux | Herramientas de pentesting preinstaladas | Debian     |
| Parrot OS  | Seguridad, privacidad y desarrollo       | Debian     |
| BlackArch  | Repositorio especializado en pentesting  | Arch Linux |

### Privacidad

| Distro   | Descripción                                       | Basada en |
| -------- | ------------------------------------------------- | --------- |
| Tails    | Enfoque en anonimato, ejecutable desde USB        | Debian    |
| Whonix   | Aislamiento de red a través de máquinas virtuales | Debian    |
| Qubes OS | Seguridad por aislamiento (múltiples máquinas)    | Fedora    |

### Gaming

| Distro   | Descripción                      | Basada en  |
| -------- | -------------------------------- | ---------- |
| SteamOS  | Optimizada para Steam y consolas | Arch Linux |
| Pop!\_OS | Drivers NVIDIA/AMD integrados    | Ubuntu     |

### Enterprise/Servidores

| Distro             | Descripción                                | Basada en |
| ------------------ | ------------------------------------------ | --------- |
| CentOS             | Estabilidad empresarial (heredado de RHEL) | RHEL      |
| Red Hat Enterprise | Estándar corporativo con soporte pago      | -         |
| Ubuntu Server      | Servidores y servicios en la nube          | Ubuntu    |
| openSUSE Leap      | Estabilidad para servidores y empresas     | SUSE      |

## Tipos de Instalación de Linux

### Instalación Nativa (Bare Metal)

Instalación directa en el disco duro del equipo, reemplazando o coexistiendo con
otros sistemas operativos.

- **Dual-Boot/Multi-Boot**: Permite tener varios sistemas operativos (e.g.,
  Windows, Linux, macOS) en la misma máquina. Se usa un gestor de arranque como
  **GRUB** para seleccionar el SO al iniciar.

- **Ventajas**: Máximo rendimiento (acceso completo a recursos del hardware),
  ideal para uso profesional o servidores.

- **Desventajas**: Requiere particionar el disco, lo que puede ser complejo para
  principiantes. Cambiar entre SO requiere reiniciar.

### Máquina Virtual (Virtualización)

Ejecutar Linux dentro de un entorno virtualizado usando software como
VirtualBox, VMware o Hyper-V.

- **Aislamiento**: El SO invitado (Linux) funciona independientemente del SO
  anfitrión (e.g., Windows, macOS).

- **Ventajas**: Seguridad (pruebas sin riesgo), compatibilidad con múltiples SO
  simultáneos, snapshots para guardar estados.

- **Desventajas**: Rendimiento reducido por la capa de virtualización
  (especialmente en gráficos o tareas intensivas).

### WSL (Windows Subsystem for Linux)

Integración nativa de Microsoft para ejecutar herramientas y entornos Linux
directamente en Windows 10/11.

- **Versiones**:

  - **WSL1**: Traduce llamadas de Linux a Windows (sin kernel real).
  - **WSL2**: Usa un kernel Linux completo en una máquina virtual ligera
    (Hyper-V).

- **Ventajas**: Integración perfecta con Windows (acceso al sistema de archivos,
  herramientas CLI), ideal para desarrollo.

- **Desventajas**: Limitado para aplicaciones gráficas (requiere configuración
  adicional) y servicios de bajo nivel.

### Live USB/CD

Ejecutar Linux desde un medio externo (USB, DVD) sin instalar nada en el disco
duro.

- **Ventajas**: Ideal para pruebas, recuperación de sistemas, o uso temporal. No
  altera el sistema anfitrión.

- **Desventajas**: Rendimiento más lento (depende de la velocidad del USB) y
  cambios no guardados por defecto.

<div style="page-break-after: always;"></div>

## Referencias

- Imran Afzal
  (s.f.).
  _What is Linux?_.
  Complete Linux Training Course to Get Your Dream IT Job 2024.
  Consultado el 30 de marzo de 2025 de
  <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9176134>

- MaheshShukla1
  (mayo 16, 2024).
  Introduction to Linux Operating System\_.
  Consultado el 30 de marzo de 2025 de
  <https://github.com/MaheshShukla1/Linux-Basic-to-Advanced-Notes/wiki/Introduction-to-Linux-Operating-System>

- Contando Bits
  (abril 08, 2024).
  _✅ Curso de LINUX Ubuntu Básico Desde Cero Gratis en Español \[Completo\] 2024_.
  Consultado el 30 de marzo de 2025 de
  <https://www.youtube.com/watch?v=woLS7yc95j0&list=PLG1hKOHdoXktPkbN_sxqr1fLqDle8wnOh>

- Stallman, R.
  (s.f.).
  _The GNU Project_.
  Consultado el 30 de marzo de 2025 de
  <https://www.gnu.org/gnu/thegnuproject.html>

- Linux.com
  (s.f.).
  _What is Linux?_.
  Consultado el 30 de marzo de 2025 de
  <https://www.linux.com/what-is-linux/>

- Branka
  (febrero 17, 2024).
  _Linux Statistics - 2024_.
  Consultado el 30 de marzo de 2025 de
  <https://truelist.co/blog/linux-statistics/>
