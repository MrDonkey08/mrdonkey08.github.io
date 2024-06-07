---
layout: post
title: Árbol AVL
author: Alan Yahir Juárez Rubio
description: Qué son los árboles AVL, para qué sirven y cómo funcionan

categories:
  - matematicas
  - matematicas-discretas
  - arboles
tags:
  - arbol
  - arbol-binario
  - arbol-de-busqueda
  - arbol-avl

date: 2023-11-26 23:00:00
last_updated: 2024-06-06 10:52:16
---

## Árbol AVL

Un **árbol AVL** es un _arbol binario de búsqueda_ en el que, para todos los
nodos, la diferencia entre _altura de la **rama izq**_ y la _altura de la
**rama der**_ es menor o igual a uno.

### Conversión a Árbol AVL

Cuando en un **árbol AVL** se le inserta un **nodo**, este puede _perder el
equilibrio_, es decir, dejar de ser un **AVL**.

Para convertir un **arbol binario** a uno **árbol AVL** se tienen que aplicar
rotaciones en sus _subárboles_ que no cumplen la _condición AVL_.

> ###### NOTA
>
> - **Nodo conflictivo:** Aquel que no cumple la _condición AVL_
> - **Nodo responsable:** Nodo que provoca al _nodo conflictivo_
{: .block-note }

- **Rotación simple:** El **nodo conflictivo** rota sobre el **hijo
  responsable** del conflicto
  - **Con hijo:** El _nodo hijo del nodo responsable_ pasa a ser _hijo_ del
    **nodo conflictivo**
    - **Izq - Izq:** Pasa a ser _hijo izquiedo_
    - **Der - der:** Pasa a ser _hijo derecho_

<div align="center">
  <figure>
    <img
      src="https://upload.wikimedia.org/wikipedia/commons/f/fd/AVL_Tree_Example.gif"
      alt="Ejemplo de Árbol AVL"
    >
    <figcaption>Fig. 1: Ejemplo de Árbol AVL</figcaption>
  </figure>
</div>

La **rotación doble** se utiliza cuando el camino hacia el _nodo conflictivo_
hace zigzag, es decir, el _hijo_ va hacia una dirección mientras el _nieto_
(nodo conflictivo) va hacia otra dirección (izq-der o der-izq).

- **Rotación doble:** El _hijo_ rota sobre el _nieto_ (rotación simple)
  - El _nodo conflictivo_ rota sobre el _nuevo hijo_.

<div style="page-break-after: always;"></div>

---

## Referencias

- Departamento de Informática - Universidad de Valladolid.
  (septiembre 10, 2011).
  _Tema 4: Árboles_.
  Recuperado el 26 de noviembre de 2023 de
  <https://www.infor.uva.es/~cvaca/asigs/doceda/tema4.pdf>

- Wikipedia (s.f.).
  _Árbol AVU_.
  Recuperado el 26 de noviembre de 2023 de
  <https://es.wikipedia.org/wiki/%C3%81rbol_AVL#>

- Estrategias de Programación y Estructuras de Datos
  (marzo 28, 2020).
  _Tema 7 (1/1): Árboles Binarios de Búsqueda y Árboles AVL_.
  Recuperado el 26 de noviembre de 2023 de
  <https://www.youtube.com/watch?v=RXIpsIa_SCY>
