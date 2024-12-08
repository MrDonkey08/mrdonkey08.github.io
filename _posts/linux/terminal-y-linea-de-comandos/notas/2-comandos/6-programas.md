---
layout: post
title: Programas
author: Alan Yahir Juárez Rubio
description: |
  Programas para abrir archivos

categories:
  - linux
  - comandos
tags:
  - editores
  - vi
  - vim
  - neovim

date: 2023-12-11
last_updated: 2024-12-08

toc:
  sidbar: right
---

## Abrir Archivos con Programas

### Abrir con Programas Predeterminados

| Comando    | Descripción                                                                                          | Argumento            | Ejemplo                                            |
| ---------- | ---------------------------------------------------------------------------------------------------- | -------------------- | -------------------------------------------------- |
| `open`     | Abre un archivo con su aplicación predeterminada (solo en macOS)                                     | Archivo o ruta       | `open documento.pdf`                               |
| `xdg-open` | Abre un archivo con su aplicación predeterminada (compatible con la mayoría de distribuciones Linux) | Archivo o ruta       | `xdg-open imagen.png`                              |
| `xdg-mime` | Establece la aplicación predeterminada para abrir un tipo de archivo específico                      | Tipo MIME y programa | `xdg-mime default zathura.desktop application/pdf` |

### Editores de Texto en Terminal

| Nombre | Descripción                                                                                                 |
| ------ | ----------------------------------------------------------------------------------------------------------- |
| nano   | Editor de texto sencillo y fácil de usar, ideal para principiantes                                          |
| vi     | Editor de texto tradicional, liviano pero básico; parte del estándar POSIX                                  |
| vim    | "Vi IMproved", un editor más avanzado basado en **vi**, con soporte para sintaxis y funcionalidad extendida |
| neovim | "Neovim", una versión modernizada de **vim** con mejor extensibilidad y soporte para plugins                |
| emacs  | Editor de texto avanzado con funcionalidades integradas como IDE, navegador y cliente de correo             |
| e      | Editor de texto en línea básica; útil para automatización o uso en sistemas sin editores avanzados          |
| ex     | Extensión de **ed**, precursor de **vi**, que permite trabajar en modo de comandos en un entorno visual     |
| pico   | Editor de texto liviano y sencillo, precursor de **nano**                                                   |

### Editores de Texto Gráficos

| Nombre | Descripción                                                                                        |
| ------ | -------------------------------------------------------------------------------------------------- |
| gedit  | Editor proporcionado por GNOME. Fácil de usar y con suficientes funcionaledades para principiantes |
| kwrite | Editor avanzado proprocionado por KDE. Cuenta con \_syntax highlighting, útil para programadores   |

<div style="page-break-after: always;"></div>

---

## Referencias

- [Linux Command](https://linuxcommand.org/).
  (s.f.).
  _Writing Our First Script and Getting It to Work_
  Recuperado el 08 de diciembre de 2024 de
  <https://linuxcommand.org/lc3_wss0010.php>

- [Prakash A.](https://itsfoss.com/author/abhishek/)
  (julio 29, 2024).
  _9 Best Text Editors for the Linux Command Line_
  Recuperado el 08 de diciembre de 2024 de
  <https://itsfoss.com/command-line-text-editors-linux/>
