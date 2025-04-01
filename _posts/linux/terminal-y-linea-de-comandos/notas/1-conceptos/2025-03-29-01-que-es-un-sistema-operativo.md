---
layout: post
title: Introducción a los Sistemas Operativos
author: Alan Yahir Juárez Rubio
description: |
  Qué es un sistema operativo, cuáles son sus componentes y los diferentes tipos

categories:
  - linux
tags:
  - sistema-operativo
  - kernel

date: 2025-03-29 12:56
last_updated: 2025-03-29 12:56

toc:
  sidebar: right

pretty_table: true
---

## Qué es un Sistema Operativo

Un **sistema operativo (SO)** es un conjunto de programas que actúa como
intermediario entre el **hardware** (componentes físicos) y los
**programas/usuarios**. Sus funciones principales incluyen:

- Gestionar recursos del sistema (CPU, memoria RAM, almacenamiento, dispositivos
  de E/S).
- Proporcionar un entorno para ejecutar aplicaciones.
- Ofrecer interfaces de usuario para interactuar con el dispositivo.

El SO provee **interfaces de usuario**, que son programas que permiten a los
usuarios interactuar con los servicios del sistema:

## Tipos de Sistemas Operativos

- **Desktop/Escritorio:** Enfocados en interactividad y usabilidad para usuarios
  finales.

> - Windows
> - macOS
> - Ubuntu
> - Fedora
{: .block-example }

- **Mobile:** Optimizados para pantallas táctiles y recursos limitados.

> Android (basado en Linux)
> - iOS (basado en Unix)
> - HarmonyOS.
{: .block-example }

- **Server/Servidor:** Diseñados para alta estabilidad, seguridad y manejo de
  múltiples solicitudes.

> - Red Hat Enterprise Linux
> - Windows Server
> - Ubuntu Server.
{: .block-example }

- **Embebidos:** Altamente especializados para hardware específico.

> - Sistemas en routers
> - Smart TVs (Tizen, webOS)
> - Automóviles (QNX),
> - IoT (Raspberry Pi OS).
{: .block-example }

## Qué es un Kernel

El **kernel** es el **núcleo central del sistema operativo**. Opera en el nivel
más bajo, interactuando directamente con el hardware y gestionando recursos
críticos:

- **Gestión de procesos**: Crea, detiene y prioriza programas en ejecución
  (multitarea).

- **Gestión de memoria**: Asigna RAM a procesos y maneja memoria virtual (swap).

- **Controladores**: Comunica el SO con dispositivos físicos (ej. tarjetas de
  red, discos duros).

- **Llamadas al sistema**: API para que los programas soliciten servicios del SO
  (ej. abrir un archivo).

## Tipos de Kernel

### Monolítico

- Todo el kernel (gestión de memoria, drivers, sistema de archivos) se ejecuta
    en un único espacio de memoria.

- Alto rendimiento pero mayor riesgo de fallos (un error puede colapsar todo
    el sistema).

> - Linux
> - FreeBSD
> - MS-DOS.
{: .block-example }

### Microkernel

- Funcionalidad mínima en el kernel (solo gestión básica de procesos y
    memoria).

- Servicios como drivers o protocolos de red se ejecutan en modo usuario,
    mejorando estabilidad.

- Menor rendimiento debido a la comunicación constante entre componentes.

> -  QNX (usado en sistemas médicos y automóviles)
> - MINIX.
{: .block-example }

### Kernel Híbrido

- Combina aspectos de núcleos monolíticos y microkernels.

- Parte del código se ejecuta en modo usuario para mayor estabilidad, pero
    conserva componentes críticos en el kernel para eficiencia.

> - Windows NT (Windows 10/11, Windows Server).
> - MacOS (XNU kernel, basado en Mach y BSD).
{: .block-example }

<div style="page-break-after: always;"></div>

## Referencias

- <https://www.udemy.com/course/complete-linux-training-course-to-get-your-dream-it-job/learn/lecture/9176134#overview>
- <https://www.uow.edu.au/student/support-services/academic-skills/online-resources/technology-and-software/operating-systems/>
- <https://github.com/MaheshShukla1/Linux-Basic-to-Advanced-Notes/wiki/Introduction-to-Linux-Operating-System>
