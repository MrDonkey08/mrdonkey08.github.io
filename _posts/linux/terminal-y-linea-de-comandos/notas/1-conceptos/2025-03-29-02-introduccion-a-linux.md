---
layout: post
title: Introducción a Linux
author: Alan Yahir Juárez Rubio
description: |
  Qué es Linux, Unix y GNU, cuáles son sus orígenes, distribuciones de Linux y
  distintas maneras de instalar Linux

categories:
  - linux
tags:
  - gnu
  - linux
  - unix
  - distro

date: 2025-03-29 16:24
last_updated: 2025-04-28 21:52

toc:
  sidebar: right

pretty_table: true
---

## Orígenes de Linux

### El Proyecto Unix

**Unix** fue un proyecto iniciado por **Ken Thompson** en 1961 el cual planteaba
crear un sistema que permitiese ejecutar tareas de forma paralela en las
computadoras.

Para las primeras versiones de Unix, era necesario portearlo para
las diferentes arquitecturas. Sin embargo, con la llegada del lenguaje de
programación C y con el pasar del tiempo, **Ken Thompson** y **Dennis Richard**
fueron capaz de desarrollar un Unix portable.

### Innovaciones de Unix

El SO **Unix** trajo una serie de características que fueron un pilar
fundamental para el desarrollo de SO's, entre ellas se encuentran:

- **Usuario root**:

  - uid: 0
  - gid: 0

- **Fork**: Función que permitió la gestión de procesos _multitasking_.
  Implementó un sistema de procesos jerárquico

- **Sistema de archivos jerárquico**: Dónde el sistema parte de la raíz y tiene
  una serie de carpetas con un propósito específico.

- **La forma de interactuar con la terminal**

  - Gestión de procesos en la terminal
  - Capacidad de utilizar la salida de un comando como la entrada de otro
    comando.

- **Filosofía de diseño**:

  - Todo es un archivo
  - Haz una cosa y hazla bien

> Los SO's basadas en Unix, utilizan todas estas características mencionadas
> previamente. A estos SO's se les denomina SO's Unix-like.
{: .block-note }

### El Proyecto GNU

El proyecto **GNU (GNU's Not Unix)** fue iniciado por **Richard Stallman** en
1983 con el objetivo de desarrollar un SO basado en Unix, completamente libre y
de código abierto denominado GNU.

El proyecto **GNU** desarrollo muchas de las herramientas esenciales que se
utilizan en los SO's modernos, tales como GCC (compilador de C/C++), Bash
(shell), GDB (debugger), glibc (bibliotecas del sistema), etc.

Richard Stallman, tenía todos los componentes del SO's, a excepción del kernel.
Como parte del desarrollo del proyecto GNU, Richard Stallman en 1990 comenzó a
desarrollar el proyecto GNU Hurd, el cual planteaba desarrollar el kernel del
proyecto **GNU**.

### El Proyecto Linux

**Linus Torvalds** en 1991, comenzó a desarrollar un sistema operativo gratuito
y libre basado en Minix (clon de Unix con fines educativos). Desarrolló su
propio kernel y porteó herramientas del proyecto GNU para consolidar su propio
SO.

> Este proyecto desarrolló la pieza clave que le hacia falta al proyecto GNU, el
> kernel. Este kernel se terminó llamando **linux**
{: .block-important }

### GNU/Linux: La Unión Fundamental

El proyecto de **Linux Torvalds** se terminó convirtiendo en **GNU/Linux**, el
cual es una colaboración entre el proyecto **GNU** y el **kernel de Linux** para
desarrollar SO completo libre y de código abierto.

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
| **Eficiencia**                                     | Funciona en hardware antiguo (e.g., Pentium IV con 1 GB RAM)                   |
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

| Distro     | Descripción                                                | Basada en  |
| ---------- | ---------------------------------------------------------- | ---------- |
| Kali Linux | Herramientas de pentesting y forense digital preinstaladas | Debian     |
| Parrot OS  | Herramientas de pentesting y forense digital preinstaladas | Debian     |
| BlackArch  | Repositorio especializado en pentesting                    | Arch Linux |

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

| Distro             | Descripción                                  | Basada en |
| ------------------ | -------------------------------------------- | --------- |
| Red Hat Enterprise | Estándar corporativo basada en suscripciones | -         |
| CentOS             | Estabilidad empresarial (heredado de RHEL)   | RHEL      |
| AlmaLinux          | Reemplazo comunitario estable de CentOS 8    | CentOS    |
| Ubuntu Server      | Servidores y servicios en la nube            | Ubuntu    |
| openSUSE Leap      | Estabilidad para servidores y empresas       | SUSE      |

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

- Google
  (s.f.).
  _More Linux distributions_
  Consultado el 28 de abril de 2024 de
  <https://www.coursera.org/learn/linux-and-sql/supplement/wJh3U/more-linux-distributions>

- eimnwux
  (abril 18, 2025).
  _Cómo UNIX Sentó las Bases de GNU/Linux_.
  Consultado el 28 de abril de 2024 de
  <https://www.youtube.com/watch?v=R4znx49SLxA&t=2s>

- eimnwux
  (abril 18, 2025).
  _Cómo Nació GNU/Linux: Software Libre y una Chispa Explosiva_.
  Consultado el 28 de abril de 2024 de
- <https://www.youtube.com/watch?v=Rch039H0SL4>
