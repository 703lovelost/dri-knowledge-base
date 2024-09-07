# ЛЕКЦИЯ 2

$(a,b) = \{x\in\mathbb R: a<x<b \}$  — интервал

$[a,b] = \{x\in\mathbb R: a\leq x \leq b \}$  — отрезок

$[a,b) = [a, b] \backslash \{ b \}$ — полуинтервал

> Промежуток - интервал или отрезок
> 

## Комплексные числа

$\mathbb C$   — complex

$\mathbb R \space \oplus \space i \mathbb R$             $i = \sqrt {-1}$

$z = x + iy, \space x,y \in \mathbb R$

$Re \space z = x$  — вещественная часть числа $z$

$Im \space z = y$  — мнимая часть

Сложение

$(x_1 + iy_1) + (x_2 + iy_2) = (x_1 + x_2) + i (y_1 + y_2)$

Умножение 

$(x_1 + iy_1) \space \cdot \space (x_2 + iy_2) = (x_1 \cdot x_2 - y_1 \cdot y_2) + i(y_1x_2 - x_1y_2)$

$z = \overline {(x+iy)} = x - iy$  — комплексное сопряжение

$|z| = |(x, y)| = \sqrt {x^2 + y^2} = \sqrt {z \cdot z}$  — модуль комплексного числа

$|z| = 1$   — единичная окружность

## Формула Эйлера

$$
\cos \phi + i\sin \phi = e^{i\phi}
$$

$e^{i\pi} = -1$

## Числовые последовательности

> Числовая последовательность $x_0, x_1, x_2, ... , x_n, ...$   — это функция из $\mathbb N$ в $\mathbb R$ , т.е. каждому номеру из $n$  сопоставляется вещественное число $x_n$. 
$X : \mathbb N \to \mathbb R$
> 

Пример:

$X_n = \frac 1 {n+1}$             $1, \frac 1 2, \frac 1 3, \frac 1 4, ..., \frac 1 n ...$

$n \to \infty$            ${1 \over {n+1}} \to 0$ 

> $X_n$  — стационарная последовательность, если
$\exists n_0\in\mathbb N\ \space \forall n,k\in \mathbb N, n > n_0, k > n_0: X_n = X_k$
> 

> Ограниченная последовательность 
$Y_n = (-1)^n$           $Y_n = -1, 1, -1, 1....$
> 

> Последовательность $X_n$  — убывающая (строго), если
$\forall m,n \in \mathbb N \space при \space m < n \space X_m \geq X_n \space (X_m > X_n)$
> 

> Возрастающая  последовательность - аналогично
> 

> Отображение $f : A \longmapsto B$   —  функция $f(a) = b, \space a \in A, b \in B$
> 

> Число  $a \in \mathbb R$ называется пределом последовательности $X_n,$   если 
$\forall \varepsilon > 0 \space \exists \space N = N(\varepsilon) \in \mathbb N,$    такая что $\forall n > N(\varepsilon) \space |X_n - a| < \varepsilon$.
$\lim\limits_{n \to \infty} X_n = a$
> 

> Элементарная окрестность точки $p \in \mathbb R$ —  это интервал $(p - \varepsilon, \space p + \varepsilon)$   для некоторого $\varepsilon > 0$.
> 

> Множество $U \subset \mathbb R$   называется окрестностью точки $p \in \mathbb R$,  если оно содержит некоторую элементарную окрестность точки $p$.
> 

Множество всех окрестностей точки $p$ обозначается $\mathcal N(p)$. 

## Теорема о единственности предела

⭐ Если $X_n \longrightarrow a$   и  $X_n \longrightarrow b$  при $n \to \infty$  , то $a = b$.

Доказательство:

Пусть $U \in \mathcal N(a) \space и \space V \in \mathcal N(b).$ Существуют  два числа $m_1$  и  $m_2 \in \mathbb N$ ,   такие что  $\forall n > m_1 \space \space \space X_n \in U$    и     $\forall n > m_2 \space\space\space X_n \in V$.

$N = \max \{m_1, \space m_2\} \implies X_n \in U \cap V \implies$ любые две окрестности точек  $a$   и  $b$ пересекаются $\implies a = b$. 

> Расширенная числовая прямая -    $\overline {\mathbb R} = \mathbb R \space \cup \space \{-\infty\} \space \cup \space \{+ \infty \}$
> 

> Множество чисел $S \subset \overline {\mathbb R}$   называется ограниченным, если
$\exists \space u, h \in \mathbb R,$   т.ч.  $u \leq S \leq h.$
$u$  — нижняя грань  $S$.    $h$  — верхняя грань $S$.
> 

> $\sup S = \min \{ h \in \overline {\mathbb R} : S \leq h\}$  — супремум $S$  (точная верхняя грань).
> 

> $\inf S = \max \{ u \in \overline {\mathbb R} : u \leq S\}$  — инфинум $S$  (точная нижняя грань).
> 

Примеры:

$\sup \space \mathbb N = \infty$

$\inf \space \mathbb N = 0$

$\sup (0, 1) = 1$

$\inf (0,1) = 0$
