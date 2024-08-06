---
layout: post
title: "GitHub: Configuración de llaves SSH"
author: Alan Yahir Juárez Rubio
description: Guía para configurar las llaves SSH en GitHub para Windows, Linux y Mac

categories:
  - informatica
  - github
tags:
  - config
  - ssh

date: 2023-08-15 15:00:00
last_updated: 2024-06-05 19:16:54
---

## Generar Llaves

- Ejecuta el siguiente comando sustituyendo `"tu@email.com"` por tu email:

```shell
ssh-keygen -t ed25519 -C "tu@email.com"
```

> ##### NOTA
>
> Si estás usando un sistema legacy que no soporta Iel algoritmo Ed25519,
> utiliza:
>
> ```shell
>  ssh-keygen -t rsa -b 4096 -C "tu@email.com"
> ```
>
{: .block-note }

```shell
Introduce la ruta en donde se guardará la llave (/home/YOU/.ssh/ALGORITHM): [Press enter]
```

## Agregar tu Llave al ssh-agent

- Inicia el ssh-agent en segundo plano

```shell
eval "$(ssh-agent -s)"
```

- Agrega tu llave SSH privada

```shell
ssh-add ~/.ssh/id_ed25519
```

### macOS Sierra 10.12.2 o Superior

- Crea un archivo config en la ruta ~/.ssh
  - Insértale el siguiente contenido

```shell
Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa
```

- Agrega tu llave SSH privada; en caso de error ejecuta sin el argumento `-K`

```shell
ssh-add -K ~/.ssh/id_rsa
```

  <div style="page-break-after: always;"></div>

---

## Referencias

- [Vega, F.](https://platzi.com/profes/freddier) & Rojas, L.
  (mayo 20, 2019)
  _Configura tus llaves SSH en local_.
  [Platzi](https://platzi.com/).
  [Curso Profesional de Git y GitHub](https://platzi.com/cursos/git-github/).
  Consultado el 15 de agosto de 2023 de
  <https://platzi.com/clases/1557-git-github/19950-configurar-llaves-ssh-en-github/>

- [GitHub Docs](https://docs.github.com/en).
  (s.f).
  _Generating a new SSH key and adding it to the ssh-agent_.
  Consultado el 15 de agosto de 2023 de
  <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>
