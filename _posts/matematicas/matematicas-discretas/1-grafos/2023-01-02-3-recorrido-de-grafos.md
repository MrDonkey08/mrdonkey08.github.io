---
layout: post
title: Recorrido de Grafos
author: Alan Yahir Juárez Rubio
description: Qué son y en qué consisten los grados, los caminos, las cadenas y los ciclos de un grafo.

categories:
  - matematicas
  - matematicas-discretas
  - grafos
tags:
  - grafos
  - grafo_no_dirigido
  - camino
  - ciclo
  - cadena

date: 2023-01-02 17:00:00
last_updated: 2024-06-04 16:11:55

toc:
  sidebar: right
---

## Grado de un Vértice

El **grado de un vértice** es el número de aristas o conexiones que tiene un
nodo con otros nodos.

$$\delta(v) = \text{número de aristas incidentes en } v$$

Existe una propiedad matemática que establece que la suma de los grados de
todos los vértices de un grafo es igual al doble del número de aristas del grafo:

$$\sum \delta(v) = 2 |E|$$

## Caminos

Un **camino** es una secuencia de vértices conectados por aristas, que permite
ir de un nodo a otro a través de las conexiones del grafo.

> ##### NOTA
>
> Si en un grafo hay más de dos vértices con grado impar, es imposible recorrer
> cada una de las aristas sin repetir nodos.
{: .block-note }

## Caminos, Cadenas y Ciclos

- **Cadena:** Es una sucesión de vértices y aristas donde las aristas pueden
  repetirse, pero no necesariamente los vértices.

- **Camino:** Es una sucesión de vértices y aristas donde no se repite ningún
  vértice ni arista.

- **Ciclo:** Es un recorrido que comienza y termina en el mismo vértice, sin
  repetir aristas.

- **Cadena Cerrada:** Es un ciclo en el cual se pueden repetir vértices, pero
  no aristas.

## Conectividad en Grafos

- **Grafo Conexo:** Un grafo es conexo si existe al menos un camino entre cada
  par de vértices. En otras palabras, todos los nodos están interconectados.

- **Grafo No Conexo:** Un grafo es no conexo si existe al menos un par de
  vértices entre los cuales no hay camino. Es decir, el grafo está dividido en
  componentes desconectados.

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Grados, caminos, cadenas y ciclos_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 02 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12222-grados-caminos-cadenas-y-ciclos/>
