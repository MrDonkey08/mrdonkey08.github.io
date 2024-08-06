---
layout: post
title: Caminos y Ciclos Eulerianos y Hamiltonianos
author: Alan Yahir Juárez Rubio
description: En qué consisten los caminos y ciclos hamiltonianos y cómo identificarlos

categories:
  - matematicas
  - matematicas-discretas
  - grafos
tags:
  - grafo
  - grafo_no_dirigido
  - camino
  - ciclo
  - camino
  - euler
  - hamilton

date: 2023-01-02 14:00:00
last_updated: 2024-06-04 21:56:16

toc:
  sidebar: right
---

## Camino Euleriano

Un **camino euleriano** es aquel **camino** o recorrido que puedes realizar sin
repetir las aristas y pasando por todos las aristas.

Para saber si un camino es euleriano, se tiene que analizar los grados de cada
uno de los nodos de dicho grafo.

### Cómo saber si existe un camino euleriano

Para identificar si existe en un grafo existe un _camino euleriano_ tenemos que:

- Si un grafo tiene un solo un nodo con grado non, para hacer el camino
  euleriano tenemos que empezar y terminar en dicho nodo con grado impar.

- Si tienes dos vértices con grado non, tienes que iniciar en uno de los dichos
  nodos y terminar en el otro para descubrir el camino euleriano.

## Ciclo Euleriano

Un **ciclo euleriano** al igual que el _camino euleriano_ busca recorrer todos
los nodos sin repetir aristas, la diferencia es que el ciclo busca que el
recorrido termine en el mismo punto de partida.

Para saber si existe un **ciclo euleriano**, tenemos que analizar los nodos de
un grafo. Si dicho grafo no tiene nodos impares, entonces existe un **ciclo
euleriano**.

### Algoritmo de Fleury

El **algoritmo de Fleury** va a encontrar un **ciclo euleriano**. Los pasos del
_algoritmo de Fleury_ son:

1. Verificar que el grado de todos los nodos es par. Si no lo son, no es un
   ciclo euleriano.
2. Realizar un circuito cerrado, sin importar que no se encluyan todos los nodos.
3. En cada nueva iteración realizar un nuevo camino cerrado visitando aristas
   que no han sido visitadas.
4. Reemplazar cada nuevo circuito en el inicial hasta visitar todas las
   aristas.

<div align="center">
  <figure>
    <img
      src="/assets/img/2023-01-02-Fleury.svg"
      alt="Algoritmo de Fleury"
      width="600px"
    >
    <figcaption>Fig. 1: Algorimto de Fleury</figcaption>
  </figure>
</div>

> ##### CONSEJO
>
> Un _ciclo euleriano_ se ha hecho correctamente si el número de veces que el
nodo aparece en el ciclo euleriano es la mitad del grado que tiene en el grafo.
{: .block-tip }

## Caminos Hamiltoniano

Un **camino hamiltoniano** es aquel en el que visitas a todas los vértices sin
repetir aristas.

Para afirmar que hay un _camino hamiltoniano_ se debe cumplir la condición donde
la suma del grado de los dos grados más pequeños de los vertices es mayor o
igual al número de vértices menos uno:

$$\text{Grado}\left(u\right)+\text{Grado}\left(v\right)\geq n-1$$

donde $n$ es el número de vértices del grafo.

> ##### NOTA
>
> Si un grafo no cumple con esta condición, no significa que no sea hamiltoniano,
> sino que simplemente no se puede asegurar que sea un _camino hamiltoniano_
{: .block-note}

## Ciclo Hamiltoniano

El **ciclo hamiltoniano** al igual que el _camino hamiltoniano_, busca visitar
todos los nodos sin repetir aristas. Adicionalmente, el _ciclo hamiltoniano_
busca finalizar en el punto de partida.

## Grafos Hamiltoniano

Los **grafos hamiltonianos** son todos aquellos que no poseen un _ciclo hamiltoniano_.

Si en un grafo uno de los nodos tiene grado uno, entonces no existe _camino hamiltoniano_ y, por ende, no es un _grafo hamiltoniano_.

<div style="page-break-after: always;"></div>

---

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Caminos y ciclos eulerianos_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 02 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12223-caminos-y-ciclos-eulerianos/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Caminos y ciclos hamiltonianos_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 02 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12224-caminos-y-ciclos-hamiltonianos/>
