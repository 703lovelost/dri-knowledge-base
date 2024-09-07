# ЛЕКЦИЯ 12

> Размерностью векторного пространства $V$ ( $\dim V$) называется количество векторов в базисе.
> 

Пример:

$P_n(x) = \{ a_0\cdot x^n + ... + a_n \space | \space a_i \in \mathbb R  \}$

Базис $P_n$   

 $\overrightarrow e_1 = 1$  

 $\overrightarrow e_2 = x$ 

 $\overrightarrow e_3 = x^2$

$\vdots$

$\overrightarrow e_{n+1} = x^n$

$\dim P_n = n + 1$

$a_0x^n + ... + a_n = a_0 \overrightarrow e_{n+1} + a_1 \overrightarrow e_n + ... + a_n \overrightarrow e_1$

> Координаты вектора $\overrightarrow v$  в  базисе  $\varepsilon_1, ... , \varepsilon_n$  — это коэффициенты в разложении вектора $\overrightarrow v$  по базису :  $\overrightarrow v = \sum \limits^n_{i = 1} v  _i \cdot \overrightarrow \varepsilon_i$ ,                    $v = (v_1, ..., v_n)$.
> 

Замечание: бывают бесконечномерные векторные пространства. 

$e^x = 1 + x + \frac {x^2} {2!} + ... + \frac {x^n} {n!} = \sum\limits^\infty_{k = 0} \frac {x^k} {k!}$
Координаты $e^x$ как бесконечного ряда равны 
$e^x = (1, 1, \frac 1 2, \frac 1 {3!} , ... , \frac 1 {n!}, ...)$

## Теорема

⭐ Пусть $V$  — векторное пространство над $\mathbb R$ с базисом $(e_1, e_2, ..., e_n)$. Тогда имеют место следующие утверждения:
1. $\forall \space v \in V$ можно представить единственным образом в виде линейной комбинации векторов $e_1, ..., e_n$.
2. Всякую систему из $s < n$ линейно независимых векторов $f_1, ..., f_s$  можно дополнить до базиса.

Доказательство:

1. Рассмотрим систему из векторов $\{ v, e_1, ..., e_n \}$.

Существует нетривиальная линейная комбинация $\alpha v + \alpha_1e_1 + ... + \alpha_ne_n = 0$.

$\alpha \neq 0$  (т.к. $e_1 ... e_n$ — базис).

$v = - \Large \frac {\alpha_1} {\alpha} \normalsize e_1 - \Large \frac {\alpha_2} {\alpha} \normalsize e_2 - ... - \Large \frac {\alpha_n} {\alpha} \normalsize e_n$

Пусть  $v = \beta_1 e_1 + ... + \beta_n e_n = \gamma_1e_1 + ... + \gamma_n e_n$
$(\beta_1 - \gamma_1)e_1 + ... + (\beta_n - \gamma_n)e_n = 0$,
т.к.    $e_1 ... e_n$   — базис, то такая линейная комбинация может быть только тривиальной $\implies \beta_i = \gamma_i$.

1. Рассмотрим набор $f_1, ..., f_n , e_1, ..., e_n$.

Этот набор линейно зависим. Будем выкидывать по порядку из этого набора вектора, которые могут быть выражены через предыдущие. 
Никакой из $f_j \space (j = 1 .. . s)$ выкинут не будет. Получим:
$f_i, ..., f_s, e_{i_1}, e_{i_2}, ..., e_{i_{n-s}}$.

## Изоморфизм

Пример:

$P_2(x) \cong \mathbb R^3 \{ (\alpha, \beta, \gamma ) \space | \space \alpha, \beta, \gamma \in \mathbb R \}$

$P_2(x) = \{ ax^2 + bx + c \space | \space a, b, c \in \mathbb R \} \space \longmapsto \space (a, b , c)$

> Два пространства $V$  и  $W$  называются изоморфными, если существует биективное (взаимно однозначное) отображение  $f : V \mapsto W$ ,  т.ч. 
$f(\alpha v_1 + \beta v_2) = \alpha f(v_1) + \beta f (v_2)$ ,         $v_1, v_2 \in V$.
> 

$f(x) = ax$      $a \neq 0, a \in \mathbb R$  —  изоморфизм (линейно)

$f(x) = x^3$   — не изоморфизм

$f : \mathbb R^2 \longmapsto \mathbb R^3$  —  не изоморфизм, т.к. не сюрьективно.

---

> $f : X \longrightarrow Y$  инъективно, если  $\forall \space \space x_1 \neq x_2  \space \space \space f(x_1) \neq f(x_2)$.
> 

> $f : X \longrightarrow Y$  сюрьективно, если  $\forall \space \space y \in Y \space \space \space \exists \space \space \space x \in X$ ,   т.ч.  $f(x) = y$.
> 

## Теорема об изоморфных векторных пространствах

⭐ Все векторные пространства одинаковой размерности  $n$   над  $\mathbb R$  изоморфны. Более того, все они изоморфны $\mathbb R ^n$.


Доказательство:

Рассмотрим произвольный базис   $e_1, ..., e_n$   в   $V$.

$v = \alpha_1 e_1 + \alpha_2 e_2 + ... + \alpha_n e_n$   (← линейно, т.к. при сложении векторов их координаты складываются).

$v  \overset {f}\longmapsto \left( \begin{array}{rcl}  \alpha_1 \\ \alpha_2 \\ \vdots \\ \alpha_n \end{array} \right) \in \mathbb R^n$    

(Координатный изоморфизм. Не единственный и зависит от выбора базиса)

$V \overset {f}\longmapsto \mathbb R^n$

$\overrightarrow v = \alpha_1 e_1 +  ... + \alpha_n e_n$
$\overrightarrow w = \beta_1 e_1 +  ... + \beta_n e_n$
$\overrightarrow v + \overrightarrow w = (\alpha_1 + \beta_1)e_1 + ... + (\alpha_n + \beta_n) e_n$

$\overrightarrow v + \overrightarrow w \longmapsto \left( \begin{array}{rcl}  \alpha_1 + \beta_1\\ \alpha_2 + \beta_2\\ \vdots \\ \alpha_n + \beta_n\end{array} \right)$

$\lambda \overrightarrow v \longmapsto \left( \begin{array}{rcl}  \lambda \alpha_1 \\ \lambda \alpha_2 \\ \vdots \\ \lambda \alpha_n \end{array} \right)$
