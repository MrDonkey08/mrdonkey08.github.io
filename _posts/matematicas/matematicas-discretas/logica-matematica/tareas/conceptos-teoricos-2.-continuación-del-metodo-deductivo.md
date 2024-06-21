# Continuación del Método deductivo

## Pruebas de inválidez

Es obvio que, para un argumento inválido no existe una prueba formal de validez. Pero, si no se puede hallar una prueba de validez para un argumento, eso no quiere decir que sea inválido y que no se pueda construir dicha prueba.

A continuación se describe un método que está muy relacionado con el de las tablas de verdad, pero que es mucho más breve, en el cual se prueba la invalidez de un argumento hallando un único caso en el que se asignan valores de verdad a las variables del enunciado de tal forma que las premisas sean verdaderas y la conclusión falsa, lo que lleva a concluir que la forma argumental es inválida.

### Ejemplo 1

Probar la invalidez del siguiente argumento por el método de asignar valores de verdad.

1. f → r
2. p → r
3. ∴ f → p

Para probar que este argumento es inválido sin tener que construir una tabla de verdad completa, es necesario tener claro que un condicional es falso solamente si su antecedente es verdadero y su consecuente falso, utilizando este hecho se procede a asignar valores de verdad a las proposiciones de la conclusión, es decir, si F es verdadero y P es falso, entonces, la conclusión es falsa. Si a la proposición R se le asigna el valor verdadero, ambas premisas se convierten en verdaderas, porque un condicional es verdadero siempre que su consecuente sea verdadero. Lo anterior permite afirmar que si a las proposiciones F y R se les asigna un valor verdadero y a la proposición P un valor falso, entonces el argumento tendrá premisas verdaderas y una conclusión falsa, con lo cual queda probado que el argumento es inválido.

Con este método lo que realmente se hace es construir un renglón de la tabla de verdad del argumento indicado, la relación se puede observar más claramente cuando los valores de verdad se escriben horizontalmente, de la siguiente forma:

|  F  |  R  |  P  | F→R | P→R | F→P |
| :-: | :-: | :-: | :-: | :-: | :-: |
|  V  |  V  |  F  |  V  |  V  |  F  |

Nótese que es posible pasar de premisas verdaderas a conclusión falsa:

#### Argumento Invalido

Un argumento se prueba inválido mostrando que por lo menos en un renglón de su tabla de verdad todas las premisas son verdaderas pero su conclusión es falsa.

### Ejemplo 2

Si Sandra es inteligente y estudia mucho, sacará buenas calificaciones y aprobará el curso. Si Sandra estudia mucho pero no es inteligente, sus esfuerzos serán apreciados y si sus esfuerzos son apreciados, aprobará el curso. Si Sandra es inteligente, entonces estudia mucho. Luego, Sandra aprobará el curso.

Tomando el siguiente lenguaje simbólico

I: Sandra es inteligente
S: Sandra estudia mucho
G: Sandra sacará buenas calificaciones
P: Sandra aprobará el curso
A: los esfuerzos de Sandra serán apreciados
Se pueden establecer las siguientes premisas:

1. (i ∧ s) → (g ∧ p)
2. [(s ∧ ∼ i) → t ] ∧ [t → p]
3. i → s
4. ∴ p

Este argumento es inválido porque con cualquiera de las siguientes asignaciones de valores de verdad la conclusión P es falsa.

|  I  |  S  |  G  |  T  |  P  |
| :-: | :-: | :-: | :-: | :-: |
|  F  |  F  |  V  |  F  |  F  |

ó

|  I  |  S  |  G  |  T  |  P  |
| :-: | :-: | :-: | :-: | :-: |
|  F  |  F  |  F  |  F  |  F  |

### Ejemplo 3

Si la inflación continua, entonces las tasas de interés permanecerán altas. Si la inflación continúa, entonces si las tasas de interés permanecen altas, descenderá la actividad comercial. Si las tasas de interés permanecen altas, entonces si la actividad comercial decrece, el desempleo aumenta. Así, si el desempleo aumenta, continuará la inflación.

Tomando el siguiente lenguaje simbólico:

P: la inflación continúa
Q: las tasas de interés permanecen altas
R: descenderá la actividad comercial
S: el desempleo aumenta

Se pueden establecer las siguientes premisas:

1. p → q
2. p → (q → r)
3. q → (r → s) / ∴ s → p

Este argumento es inválido porque la siguiente asignación de valores de verdad hace las premisas verdaderas pero la conclusión falsa:

| P   | Q   | R   | S   | P→Q | P→(Q→R) | Q→(R→S) | S→P |
| --- | --- | --- | --- | --- | ------- | ------- | --- |
| F   | F   | F   | V   | V   | V       | V       | F   |

## La inconsistencia de un razonamiento

El objetivo de esta prueba es detectar si hay consistencia o inconsistencia al interior de las hipótesis. Basta con encontrar una proposición que sea contradictoria con otra para declarar que el conjunto de proposiciones en su totalidad es inconsistente. De un conjunto inconsistente de hipótesis puede concluirse tanto p como ~p, lo cual contradice el principio de no-contradicción (~(p ∧ ~p)).

Este método propone buscar la posible presencia de (P ∧ ~P) entre las hipótesis. Esta búsqueda puede realizarse por medio de una tabla de verdad. Sin embargo, si hablamos de 6 o más premisas, el trabajo de elaborar las 2n combinaciones (26 = 64, 27 = 128, 28 = 256, etc.) de las premisas es demasiado. La otra manera de realizar esta búsqueda es de una manera indirecta siguiendo estos pasos:

1. Se introduce la negación de la conclusión como una hipótesis adicional.
2. Partiendo de esta nueva hipótesis se trata de deducir una contradicción de cualquiera de las proposiciones del conjunto.
3. De conseguirse una contradicción, afirmamos que el teorema es válido, de otro modo, el teorema es una falacia.

Algunos autores conocen esta prueba formal como prueba por contradicción o como reducción al absurdo.

### Ejemplo 1

Sea H = [a → (b ∨ c), b →~a, d →~c, a ], C = ~d

Listando las hipótesis y la negación de la conclusión, tenemos:

1. a → (b ∨ c) (hipótesis)

2. b →~a (hipótesis)

3. d →~c (hipótesis)

4. a (hipótesis)

5. d (negación de la conclusión)

Desarrollando la prueba, resulta:

6. b ∨ c (modus ponens de 4. y 1.)

7. ~c (modus ponens de 5. y 3.)

8. b (silogismo disyuntivo de 6. y 7.)

9. ~a (modus ponens de 8. y 2.)

10. a ∧ ~a Contradicción (de Conjunción de 4. y 9.)

Dado que encontramos la contradicción a ∧ ~a, podemos concluir que el teorema es válido.

### Ejemplo 2

Sean las hipótesis H={a ∧ b, a →c}, y la conclusión C = b∧c. Se desea saber si se trata de un teorema válido.

Listando las hipótesis y la negación de la conclusión, tenemos:

1. a ∧ b (hipótesis)

2. a →c (hipótesis)

3. ~( b∧c) (negación de la conclusión)

4. ~b ∨ ~c (leyes de DeMorgan, regla 8b)

5. a (Simplificación de 1.)

6. c (Modus ponens de 5. y 2.)

7. b (Simplificación de 1.)

8. ~b (Silogismo disyuntivo de 4. y 6.)

9. b∧~b Contradicción (conjunción de 7. y 8.)

Nota que la demostración pudo seguir otro camino a partir de 7.:

7. b

8. ~c (Silogismo disyuntivo de 4. y 7.)

9. c∧~c Contradicción (conjunción de 7. y 8.)

En cualquier caso, dado que encontramos una contradicción, queda demostrado que el teorema es válido.

### Ejemplo 3

Sea el teorema H =[ ~f → b ∧ t, b ∧ f], C = ~t. Se desea saber si se trata de un teorema válido o de una falacia.

Listando las hipótesis y la negación de la conclusión, se obtiene:

1. ~f → b ∧ t (hipótesis)

2. b ∧ f (hipótesis)

3. t (negación de la conclusión)

4. b (simplificación de 2.)

5. b ∧ t (conjunción de 3. y 4.)

6. f (simplificación de 2.)

7. ~f (??, regla ??)

No hay regla alguna que me permita obtener ~f a partir de 1., que sería lo necesario para formar la contradicción f ∧ ~f. Por tanto, esto debe hacernos sospechar que se trata de una falacia.
