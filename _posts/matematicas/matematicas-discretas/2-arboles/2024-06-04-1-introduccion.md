---
layout: post
title: Introducción a los Árboles
author: Alan Yahir Juárez Rubio
description: Explicación detallada y completa de qué son los árboles, cuáles son sus partes, cómo se categorizan, entre otras cosas.

categories:
  - matematicas
  - matematicas-discretas
  - arboles
tags:
  - arbol
  - nodo
  - recorridos-de-arboles
  - tipos-de-arboles

date: 2023-01-06 10:00:00
last_updated: 2024-06-04 17:58:52

toc:
  sidebar: right

featured: true
---

Un **árbol** consiste en una **agrupación de nodos**, el cuál parte de un
**nodo raíz** y se desgloza jerarquicamente en más nodos.

Los Árboles nos permiten organizar o estructurar información. Si tenemos un
nodo A y un nodo B, solo existirá una conexión entre ellos.

> ##### NOTA
>
> En los árboles solo puede haber una conexión entre dos nodos.
{: .block-note }

<div align="center">
  <figure>
    <img
      src="https://media.geeksforgeeks.org/wp-content/uploads/20221124153129/Treedatastructure.png"
      alt="Estructura de un Árbol"
      width="600px">
    <figcaption>Fig. 1: Estructura de un Árbol</figcaption>
  </figure>
</div>

Cuando el orden de los _nodos_ importa, entonces forman una lista y se le
denomina **árbol ordenado**.

En _informática_ los **arboles** son _estructuras de datos no lineales_. Cada
uno de sus _nodos_ guarda información de sí mismo y, a su vez, guarda la
_dirección_ de cada uno de los _nodos_ que le suceden (_nodos hijos_).

## Características de un Nodo

- **Brazo:** Conexión entre un nodo y otro.

- **Altura:** Longitud del camino más largo que comienza en el nodo y termina
  en una hoja. Se dice que la _altura_ del _nodo raíz_ es la _altura del árbol_.

- **Nivel o profundidad:** Longitud del camino (único) que comienza en la raíz
  (como nivel 0) y termina en dicho nodo.

## Partes de un árbol (tipos de nodos)

Un **árbol** es una _agrupación de nodos_ ordenados jerarquicamente. Estos
nodos se catalogan de la siguiente manera:

- **Raíz:** Nodo del cuál se desprenden todos los demás nodos.

- **Padre:** Nodo que engloba a dicho nodo.

- **Hijo:** Nodo que se desprende un _nodo padre_. Todos los nodos son nodos
  hijos a excepción del nodo raíz.

- **Ancestro:** Nodo que engloba al padre de dicho nodo.

- **Nieto:** Nodo que se desprende del _padre_ del **nodo padre**, es decir,
  del _ancestro_.

- **Hermanos:** Aquellos que tienen un nodo padre en común.

- **Terminal, hoja o externo:** Aquellos que no tiene hijos y, por lo tanto,
  marcan el final del árbol. En caso contrario se le denomina **nodo interno**.

- **Internos o rama:** Todos aquellos que son nodos padres o, dicho de otra
  manera, todos a quellos que no son terminales. En este tipo se excluye el nodo
  raíz.

## Subárboles

Un **subárbol** es una sección de un árbol, una parte de un ábol. Estos
subárboles están conformados desde un nodo padre de dicho árbol y todos sus
descendientes; si se dividiera desde un nodo padre n, se llamaría subárbol
raíz n.

## Tipos de árboles

<div align="center">
  <figure>
    <img
      src="https://static.platzi.com/media/user_upload/Tipos%20%C3%A1rboles-16a0eea1-ca9a-4cda-89be-e1809854ac72.jpg"
      alt="Tipos de Árbol"
      width="600px"
    >
    <figcaption>Fig. 2: Tipos de Árbol</figcaption>
  </figure>
</div>

- **Libres:** Aquellos en los que se desconoce el **nodo raíz**.
- **Degenerado:** Todos sus nodos tienen como máximo un hijo.
- **Expansión:** Aquel árbol (generalmente extraído de un grafo) el cual
  representa una conexión ponderada (un recurso asociado) con cada uno de los nodos.

<div align="center">
  <figure>
    <img
      src="https://miro.medium.com/v2/resize:fit:16000/1*CMGFtehu01ZEBgzHG71sMg.png"
      alt="Tipos de Árbol Binario"
      width="600px"
    >
    <figcaption>Fig. 3: Tipos de Árbol Binario</figcaption>
  </figure>
</div>

- **M-nario:** Cada uno de sus nodos tiene como máximo $$ m $$ hijos. Entre
  estos se encuentran los binarios (2 hijos), los ternarios (3 hijos), entre
  otros.
  - **Completo:** Sus nodos tienen o $$ m $$ hijos o ninguno.
    - **Lleno:** Todos sus nodos terminales llegan a un mismo nivel.

<div align="center">
  <figure>
    <img
      src="https://media.geeksforgeeks.org/wp-content/uploads/20230111154258/typoes1-768.png"
      alt="Arboles M-narios"
      width="600px"
    >
    <figcaption>Fig. 4: Árboles M-narios</figcaption>
  </figure>
</div>

<div style="page-break-after: always;"></div>

---

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Árboles_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 06 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12229-arboles/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Teoría de grafos_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 06 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12230-sub-arboles-vertices-y-notacion/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Árbol binario_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 07 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12232-arbol-binario/>

- Departamento de Informática - Universidad de Valladolid.
  (septiembre 10, 2011).
  _Tema 4: Árboles_.
  Recuperado el 26 de noviembre de 2023 de
  <https://www.infor.uva.es/~cvaca/asigs/doceda/tema4.pdf>
