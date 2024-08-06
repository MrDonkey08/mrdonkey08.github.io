---
layout: post
title: Árboles de Expansión
author: Alan Yahir Juárez Rubio
description: Qué son los árboles de expansión mínimo y máximo y cuáles son y en qué consisten los algoritmos para encontrar dichos árboles

categories:
  - matematicas
  - matematicas-discretas
  - arboles
tags:
  - arbol
  - expansion-minimo
  - expansion-maximo
  - prim
  - kruskal
  - flujo-maximo

date: 2023-01-08 14:00:00
last_updated: 2024-06-06 10:17:54

toc:
  sidebar: right
---

## Arbol de Expansión Mínimo

Un **árbol de expansión mínimo** es aquel árbol que partiendo de una raíz pueda
conectar todos los vértices buscando los caminos de menor costo. Para sacar el
costo mínimo del árbol solo basta con ir sumando el valor que tiene cada
conexión nivel por nivel, luego sumar todos los niveles.

<div align="center">
  <figure>
    <img
      src="https://static.platzi.com/media/user_upload/arbolexpansionminima-6e48d96e-36e2-4cd7-8618-ddcdf4d9a7fc.jpg"
      alt="Arboles de Expansión Mínimo"
      width="600px"
    >
    <figcaption>Fig. 1: Árbol de expansión mínimo</figcaption>
  </figure>
</div>

### Algoritmo de Prim

A continuación los pasos del **algoritmo de Prim**:

1. Escoger un nodo cualquiera.
2. Escoger el nodo asociado al nodo elegido previamente que tengan menor valor,
   menor coste.
3. En cada iteración selecciona la arista de menor peso relacionado con los
   nodos conectados.
4. Finaliza cuando todos los nodos están conectados con $$ n-1 $$ aristas, donde
   $$ n $$ es el número de nodos.
5. Para conseguir el coste total suma todas los valores de las aristas
   seleccionadas.

<div align="center">
  <figure>
    <img
      src="/assets/img/arboles/2023-01-08-prim.svg"
      alt="Algoritmo de Prim"
      width="400px"
    >
    <figcaption>Fig. 2. Algorimto de Prim</figcaption>
  </figure>
</div>

**Coste total:** 27

### Algoritmo de Kruskal

El **algoritmo de Kruskal** al igual que el _algoritmo de Prim_ sirve para
buscar el _árbol de expansión mínimo_, la diferencia es que el algoritmo de
Kruskal inicia seleccionando la arista de menor valor y después en cada
iteración se agrega la arista de menor valor del conjunto disponible.

A continuación los pasos del _algoritmo de Kruskal_:

1. Selecciona la arista menor.
2. En cada iteración agruegue la arista de menor longitud del conjunto de arcos
   disponibles.
3. El algoritmo finaliza cuando todos los vertices están conectados con
   $$ n-1 $$ arcos.

<div align="center">
  <figure>
    <img
      src="/assets/img/arboles/2023-01-08-kruskal.svg"
      alt="Algoritmo de Kruskal"
      width="400px"
    >
    <figcaption>Fig. 3. Algoritmo de Kruskal</figcaption>
  </figure>
</div>

> ##### NOTA
>
> Aplica para el agoritmo de prim y el de kruskal:
>
> - Cabe mencionar que cuando estemos haciendo este proceso no se formen ciclos
>   cerrados o rutas cerradas porque sino se estarían repitiendo caminos por los
>   cuales no se deberian pasar.
> - Esta conexión no es de orden secuencial, por lo que puedes hacer un camino
>   y si se presenta algun ciclo o ruta cerrada, puedes regresarte a cualquiera
>   de los demás nodos que ya han sido conectados y seguir conectando aquellos
>   que no están conectados.
{: .block-note }

## Árbol de Expansión Máximo

A diferencia del _árbol de expansión mínimo_, el cual busca conectar todos los
nodos entre sí con la menor cantidad de recursos, este lo que busca es
conseguir descifrar la cantidad máxima de recursos que se pueden mandar desde
un punto inicial hasta un final a partir de los caminos que se disponen y sus
respectivos flujos.

### Algoritmo de Flujo Máximo

El **algoritmo de flujo máximo** consiste en los siguientes pasos:

1. Direccionar los flujos e iniciar en ceros.
2. Obtener trayectorias buscando el mayor flujo.
3. Escoger el menor flujo de la trayectoria, esto es la arista de menor valor
   dentro de tu camino que seleccionaste.
4. Actualizar el gráfico con las capacidades mínimas, ósea, restando el valor
   de la arista del anterior paso a cada una de las aristas del camino.
5. Buscar nueva trayectoria o camina en aumento y repetir hasta que no existan
   más.

<div align="center">
  <figure>
    <img
      src="/assets/img/arboles/2023-01-08-flujo-maximo.svg"
      alt="Algoritmo de Flujo Máximo"
      width="600px"
    >
    <figcaption>Fig. 4. Algoritmo de Flujo Máximo</figcaption>
  </figure>
</div>

<div style="page-break-after: always;"></div>

---

## Referencias

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Árbol de expansión_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 07 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12231-arbol-de-expansion-minimo/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Algoritmo de Prim_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 08 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12236-algoritmo-de-prim/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Algoritmo de Kruskal_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 08 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12238-algoritmo-de-kruskal/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Algoritmo de flujo máximo_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 09 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12240-algoritmo-de-flujo-maximo/>

- [Orduz, S.](https://platzi.com/profesores/sergio-orduz-240/)
  (julio 24, 2018).
  _Algoritmo de Fleury_.
  [Curso de Matemáticas Discretas](https://platzi.com/cursos/discretas/).
  [Platzi](https://platzi.com/).
  Recuperado el 09 de enero de 2023 de
  <https://platzi.com/clases/1319-discretas/12239-algoritmo-de-fleury/>
