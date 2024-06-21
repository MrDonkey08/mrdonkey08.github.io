# Problemas de valor inicial con la transformada de Laplace

## Transformada de una derivada

Si $Y(S) = \mathcal{L} \{y\:'(t) \}$, entonces

$$
\begin{array}{l}
\mathcal{L} \{y\:'(t) \}  &=& sY(S) - y(0) \\
\mathcal{L} \{y\:''(t) \} &=& s^{2}Y(S) - sY(0) - y(0)\\
\mathcal{L} \{y\:'''(t) \} &=& s^{3}Y(S) - s^{2}Y(0) - sY(0) - y(0)\\
\mathcal{L} \{y^{(n)}(t) \} &=& s^{n}Y(S) - s^{n-1}Y(0) - \cdots -sY^{(n-2)}(0) - y^{(n-2)}(0)\\
\end{array}
$$
