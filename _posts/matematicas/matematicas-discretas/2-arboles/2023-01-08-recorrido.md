---
layout: post
title: Recorrido de Árboles
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - matematicas-discretas
  - arboles
tags:
  - arbol

date: 2023-01-08 14:00:00
last_updated: 2024-06-04 17:58:52

toc:
  sidebar: right
---

## Recorridos

El **recorrido** de un **arbol** es el proceso de visitar de una manera
sistemática, exactamente una vez, cada nodo de un árbol. Los recorridos más
comunes son:

- **Preorden**: raíz-izq-der
- **Inorden**: izq-raíz-der
- **Posorden**: izq-der-raíz

<div align="center">
  <figure>
    <img
      src="https://media.geeksforgeeks.org/wp-content/uploads/20230623123129/traversal.png"
      width="600px"
    >
    <figcaption>Fig. 1: Recorrido de árboles</figcaption>
  </figure>
</div>

### Recorrido de Expresiones Aritméticas

Los árboles también nos sirven para representar expresiones aritméticas, para
ello debe cumplir con las siguientes condiciones:

- Los vértices terminales son operandos
- Los vértices internos son operadores
- La raíz siempre debe ser un operador

Así como vimos las diferentes formas para recorrer un árbol, las expresiones
aritméticas tienen también sus propias formas:

- **Pre fijo**: raíz-izq-der
- **In fijo**: izq-raíz-der
- **Pos fijo**: izq-der-raíz

<div align="center">
  <figure>
    <img
      src="https://i.ibb.co/kxdsKDt/expr-arth-to-tree-tranversal-02-03-2020-21-04.jpg"
      width="600px"
    >
    <figcaption>
      Fig. 2: Recorrido de expresiones aritméticas a través de árboles
    </figcaption>
  </figure>
</div>

<div style="page-break-after: always;"></div>

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Recorrido de árboles_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 08 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12233-recorrido-de-arboles/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Expresiones aritméticas_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 08 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12234-expresiones-aritmeticas/>
