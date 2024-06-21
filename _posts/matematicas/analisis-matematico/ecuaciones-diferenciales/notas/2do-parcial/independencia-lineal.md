## Independencia lineal

Definición: Consideremos las funciones $f_1, f_2, f_3, \dots, f_n$.

1. Diremos que estas funciones son **linealmente independientes** si los únicos números que satisfacen la ecuación $cf_1, cf_2, cf_3, \dots, cf_n = 0$ son los números $c_1 = c_2 = c_3 = \dots = c_n = 0$
2. Diremos que estas funciones son **linealmente dependiendes** si no son **línealmente independientes**.
3. El **Wronskiano** de $f_1, f_2, f_3, \dots, f_n$ se define como el **determinante**

$$
W \left(f_1, f_2, f_3, \dots, f_n \right) =
\begin{vmatrix}
f_1           & f_2           & f_3           & \dots  & f_n \\
f_1\:'        & f_2\:'        & f_3\:'        & \dots  & f_n\:' \\
f_1\:''       & f_2\:''       & f_3\:''       & \dots  & f_n\:'' \\
\vdots        & \vdots        & \vdots        & \ddots & \vdots\\
{f_1}^{(n-1)} & {f_2}^{(n-1)} & {f_3}^{(n-1)} & \dots  & {f_{n}} ^{(n-1)} \
\end{vmatrix}
$$

> [!IMPORTANT] En Wronskiano
>
> Si $|D| = 0 \to$ sistema **linealmente dependiente**
> Si $|D| \neq 0 \to$ sistema **linealmente independiente**

> [!NOTE]
>
> El **Wronskiano** se puede aplicar para **sistemas homogéneos** y **heterogéneos**
