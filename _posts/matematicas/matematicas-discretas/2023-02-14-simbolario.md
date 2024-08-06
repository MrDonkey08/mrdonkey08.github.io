---
layout: post
title: "Simbolario: Conjuntos y Lógica Matemática"
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - matematicas-discretas
tags:
  - guia-de-studio
  - simbolario

date: 2023-02-14
last_updated: 2024-07-27 12:23

toc:
  beginning: true

pretty_table: true
---

## Conjuntos

|                   Símbolo                    |        Nombre        | Significado                                                                         |
| :------------------------------------------: | :------------------: | :---------------------------------------------------------------------------------- |
|                $$ A\cup B $$                 |        Unión         | Todos los elementos de $$ A $$ y $$ B $$                                            |
|                $$ A\cap B $$                 |     Intersección     | Elementos en común entre $$ A $$ y $$ B $$                                          |
| $$ A^c $$ , $$ A\: ' $$ o $$ \overline{A} $$ |     Complemento      | Elementos que no pertenecen a $$ A $$ , pero sí al conjunto universal               |
|             $$ A\backslash B $$              | Complemento relativo | Elementos que pertenecen a $$ A $$ , pero no a $$ B $$                              |
|             $$ A-B $$ o $$ AB $$             |      Diferencia      | Elementos en $$ A $$ , pero no en $$ B $$                                           |
|      $$ A\Delta B $$ o $$ A\ominus B $$      | Diferencia simétrica | Elementos que no tienen en comun $$ A $$ y $$ B $$                                  |
|               $$ A\times B $$                | Producto cartesiano  | Conjunto de pares ordenados de $$ A $$ y $$ B $$                                    |
|                  $$ A=B $$                   |       Igualdad       | Ambos conjuntos tienen los mismos elementos                                         |
|              $$ A\subseteq B $$              |     Subconjunto      | Cada elemento de $$ A $$ está en $$ B $$                                            |
|               $$ A\subset B $$               |  Subconjunto propio  | Cada elemento de $$ A $$ está en $$ B $$ , pero $$ B $$ tiene más elementos         |
|             $$ A\not\subset B $$             |  No es subconjunto   | $$ A $$ no es subconjunto de $$ B $$                                                |
|              $$ A\supseteq B $$              |    Superconjunto     | A tiene los mismos de elementos que $$ B $$ , o más                                 |
|               $$ A\supset B $$               | Superconjunto propio | $$ A $$ tiene elemetos de $$ B $$ y más                                             |
|             $$ A\not\supset B $$             | No es superconjunto  | $$ A $$ no es un superconjunto de $$ B $$                                           |
|              $$ \varnothing $$               |    Conjunto vacío    | Conjunto sin elementos                                                              |
|                 $$ \Bbb U $$                 |  Conjunto universal  | Todos los valores posibles (en el área de interés)                                  |
|                  $$ P(A) $$                  |  Conjunto potencia   | Todos los subconjuntos de $$ A $$ . Si \ $$ A = n $$ , entonces \# $$ P(A) = 2^n $$ |
|        \# $$ A $$ o $$ \mid A\mid $$         |     Cardinalidad     | Número de elementos del conjunto $$ A $$                                            |

## Clasificación de Números

| Notación                                                      |         Nombre          | Definición                                                                                                                                   |
| :------------------------------------------------------------ | :---------------------: | -------------------------------------------------------------------------------------------------------------------------------------------- |
| $$ \Bbb{N} = \Bbb{N}\_{1}= \Bbb{Z}^{+} = \{1, 2, 3,\dots\} $$ |    Números Naturales    | Son el conjunto de números que sirven para contar.                                                                                           |
| $$ \Bbb{N}\_{0} = \Bbb{N}^{0} = \{0, 1, 2, 3,\dots\} $$       | Números Naturales con 0 | -                                                                                                                                            |
| $$ \Bbb Z = \{\dots, -2, -1, 0, 1, 2,\dots\} $$               |     Números Enteros     | Son el conjunto de números naturales, sus opuestos (negativos) y el cero.                                                                    |
| $$ \Bbb Q = \{\frac {p}{q} \mid \;p,q ∈ \Bbb{Z} \} $$         |   Números Racionales    | Son el conjunto de números que se pueden representar con una razón (cociente) de dos enteros                                                 |
| $$ \Bbb{I} = \{a \mid a \in \Bbb{R}, a \notin \Bbb{Q}\} $$    |  Números Irracionales   | Son el conjunto de números que tiene decimal infinito no periódico y, por lo tanto, no se puede representar como el cociente de dos enteros. |
| $$ \Bbb R = \{a \mid a \in (-∞, ∞)\} $$                       |     Números Reales      | Es el conjunto que contiene a los números racionales e irracionales.                                                                         |
| $$ I = \{bi \mid b \in \Bbb{R}, i \in I\} $$                  |   Números Imaginarios   | Son producto del número real por la unidad imaginaria: $$ i=\sqrt{-1} $$                                                                     |
| $$ \Bbb C = \{a+bi \mid a \in \Bbb{R}, bi \in I\} $$          |    Números Complejos    | Comprende los números reales y los imaginarios.                                                                                              |

## Relaciones

|            Símbolo            |          Nombre          | Significado                                                                           |
| :---------------------------: | :----------------------: | :------------------------------------------------------------------------------------ |
|         $$ x\ R\ y $$         |         Relación         | $$ (x,y)\in R $$                                                                      |
| $$ R^{-1} $$ o $$ R^{\sim} $$ |         Inversa          | Conjunto de pares ordenados que cambian su posición $$ (a,b)\to (b,a) $$              |
|        $$ R\circ S $$         |       Composición        | Elemento en común en sus extremos. Además $$ T\circ (S\circ R) = (T\circ S)\circ R $$ |
|         $$ a\ R\ a $$         |        Reflexiva         | $$ R $$ es reflexiva $$ ≡ ∀a \left(a\ R\ a\right) $$                                  |
|      $$ a\ \not R\ a $$       |       No reflexiva       | $$ R $$ es reflexiva $$ ≡ ∀a \left(a\ \not R\ a\right) $$                             |
|               -               |        Simétrica         | $$ R $$ es simétrica ≡ $$ ∀a\ ∀b \left(a\ R\ b ⇒ b\ R\ a\right) $$                    |
|               -               |      Antisimétrica       | R es antisimétrica $$ ≡ ∀a\ ∀b \left(a\ R\ b ∧ b\ R\ a ⇒ a = b\right) $$              |
|               -               |        Transitiva        | R es transitiva $$ ≡ ∀a\ ∀b\ ∀c\ (a\ R\ b ∧ b\ R\ c ⇒ a\ R\ c) $$                     |
|               -               | Relación de equivalencia | Reflexiva, simétrica y transitiva                                                     |
|         $$ \preceq $$         |      Orden Parcial       | Reflexivo, antisimétrico y transitivo                                                 |

## Operadores de Conjuntos

|               Símbolo                |          Nombre           | Significado     |     |
| :----------------------------------: | :-----------------------: | :-------------- | --- | --- |
| $$ \mid $$ <br> $$ / $$ <br> $$ : $$ |             -             | Tal que         |     |     |
|            $$ \forall $$             |  Cuantificador universal  | Para todo       |     |
|              $$ \in $$               |             -             | Pertenece       |     |
|             $$ \notin $$             |             -             | No pertenece    |     |
|            $$ \exists $$             | Cuantificador existencial | Existe          |     |
|            $$ \nexists $$            |             -             | No existe       |     |
|           $$ \nexists ! $$           |             -             | Existe un único |     |
|                  {}                  |         Conjunto          | -               |     |

## Conectores Lógicos

|                                            Símbolo                                             |                                      Ejemplo                                       | Nombre                | Significado                          |
| :--------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------: | --------------------- | ------------------------------------ |
|          $$ \neg $$ <br> $$ \sim $$ <br> $$ ! $$ <br> $$ ' $$ <br> $$ \overline{} $$           | $$ \neg P $$ <br> $$ \sim P $$ <br> $$ !P $$ <br> $$ P' $$ <br> $$ \overline{P} $$ | Negación              | no                                   |
|                                 $$ \wedge $$ <br> $$ \cdot $$                                  |                                  $$ P \wedge Q $$                                  | Conjunción            | y                                    |
|                          $$ \vee $$ <br> $$ + $$ <br> $$ \mid\mid $$                           |                                   $$ P \vee Q $$                                   | Disyunción            | o                                    |
|                        $$ \to $$ <br> $$ \implies $$ <br> $$ \supset $$                        |                                   $$ P \to Q $$                                    | Condicional           | si... entonces, implica              |
|               $$ \leftrightarrow $$ <br> $$ \equiv $$ <br> $$ \Leftrightarrow $$               |                             $$ P \leftrightarrow Q $$                              | Bicondicional         | si y solo si                         |
|                                        $$ \downarrow $$                                        |                                $$ P \downarrow Q $$                                | Negación conjunta     | ni... ni                             |
| $$ \nleftrightarrow $$ <br> $$ \oplus $$ <br> $$ \not\equiv $$ <br> $$ W $$ <br> $$ \veebar $$ |                             $$ P \nleftrightarrow Q $$                             | Disyunción excluyente | o bien... o bien                     |
|                                        $$ \therefore $$                                        |                                $$ P \therefore Q $$                                | Conclusión            | luego, por lo tanto, en consecuencia |
|                                         $$ \because $$                                         |                                 $$ P \because Q $$                                 | Porque                | -                                    |
|                              $$ \top $$ <br> $$ T $$ <br> $$ 1 $$                              |                                         -                                          | Tautología            | siempre verdadero                    |
|                              $$ \bot $$ <br> $$ F $$ <br> $$ 0 $$                              |                                         -                                          | Contradicción         | siempre falso                        |

<div style="page-break-after: always;"></div>

---

## Referencias

- Wikipedia
  (s.f.).
  _Conectiva lógica_.
  <https://es.wikipedia.org/wiki/Conectiva_l%C3%B3gica>

- Wikipedia
  (s.f.).
  _Símbolos lógicos_.
  <https://es.wikipedia.org/wiki/Anexo:S%C3%ADmbolos_l%C3%B3gicos>

- Wikipedia
  (s.f.).
  _Álgebra de conjuntos_.
  <https://es.wikipedia.org/wiki/Operaciones_con_conjuntos>

- [Rodo, P.](https://economipedia.com/author/P.rodo) (01 de agosto, 2020).
  _Números imaginarios_.
  <https://economipedia.com/definiciones/numeros-imaginarios.html>

- Wikipedia
  (s.f.).
  _Anexo: Símbolos matemáticos_.
  <https://es.wikipedia.org/wiki/Anexo:S%C3%ADmbolos_matem%C3%A1ticos>

- Wikipedia
  (s.f.).
  _Natural number_.
  <https://en.wikipedia.org/wiki/Natural_number>

- [Rodó,P.](https://economipedia.com/author/P.rodo)
  (11 de septiembre de 2019).
  _Números reales_.
  <https://economipedia.com/definiciones/numeros-reales.html>

- Wikipedia
  (s.f.).
  _Número natural_.
  <https://es.wikipedia.org/wiki/N%C3%BAmero_natural>

<!--
https://www.quora.com/What-is-the-symbol-for-the-set-of-Irrational-numbers
https://es.wikipedia.org/wiki/Teor%C3%ADa_de_conjuntos
-->
