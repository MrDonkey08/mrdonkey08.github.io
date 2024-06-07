---
layout: post
title: Introducción a los Grafos
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - matematicas-discretas
  - grafos
tags:
  - grafo
  - digrafo
  - grafo_dirigido
  - grafo_no_dirigido

date: 2023-01-02 12:00:00
last_updated: 2024-06-05 15:21:47

toc:
  sidebar: right
---

Los **grafos** son modelos matemáticos que sirven para representar las
relaciones entre objetos de un conjunto.

Un **gráfico** o **grafo** es un conjunto de vértices, o nodos, que están conectados
a través de aristas, líneas o conexiones.

## Tipos de grafos

- **Grafo simple**: Aquel que en sus vertices no tiene ni **aristas paralelas**
  ni **lazos**

- **Multígrafo**: Aquel que tiene **aristas paralelas**, pero no lazos.

- **Pseudografo**: Aquel que tiene **aristas paralelas** y **lazos**.

- **Grafo Ponderado**: Este cuenta con un valor dentro de las conexiones, esto
  puede verse como el costo, o recurso, de una ruta de nodos.

- **Grafo Dirigido o Dígrafo**: Establece una dirección en las conexiones, la
  cual se representa con una flecha.
  - **Multígrafo Dirigido**: Cuenta con dirección en las conexiones y puede
    haber múltiples conexiones entre dos nodos.

## Partes de un Grafo

- **Vertices**: Son los puntos que representas objetos dentro de la gráfica

- **Aristas**: Son las lineas que unen a los vertices para indicar su relación
  entre estos.

- **Aristas adyacentes**: Aristas que convergen en el mismo vertice.

- **Aristas multiples o paralelas**: Son aquellas que están conectados a dos
  vertices en común.

- **Lazo**: Arista cuyo vertice incide sobre sí mismo, es decirm el vertice
  sale y regresa del mismo vértice.

<div style="page-break-after: always;"></div>

---

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Teoría de grafos_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 02 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12221-teoria-de-grafos/>
