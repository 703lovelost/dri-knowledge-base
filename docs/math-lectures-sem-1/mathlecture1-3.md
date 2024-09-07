# ЛЕКЦИЯ 3

## Аксиома граней

Любое подмножество $X \subset \mathbb R$ имеет точные верхнюю и нижнюю грани из $\overline {\mathbb R}$.

$\sup \emptyset = -\infty$

$\inf \emptyset = +\infty$

> Монотонная последовательность - это или возрастающая, или убывающая последовательность
> 

## Теорема Вейерштрасса определения монотонной последовательности

⭐ На  $\mathbb R$  всякая монотонная последовательность имеет предел

Доказательство:

Пусть $X_n$  — возрастающая последовательность и $X = \{ x_0, x_1, ..., x_n,... \} \subset \mathbb R$.

$h : \sup X$            $h > -\infty$       и      $U \in \mathcal N(h)$

$\exists \space m \in \mathbb N$ ,  такая что $h - \varepsilon < x_m$ , потому что $h = \sup X$.

$\forall n \geq m \space \space \space X_m \leq X_n \leq h$ , потому что последовательность $X_n$  —  возрастающая. 

 

> Хвост последовательности - это все элементы последовательности, начиная с некоторого по определению предела  $h = \lim\limits_{n \to \infty} X_n$.
Для убывающей последовательности аналогично.
> 

**Первый замечательный предел**

$$
\lim\limits_{x \to 0}\frac {\sin x} x = 1
$$

**Второй замечательный предел**

$$
e = \lim\limits_{n\to\infty} (1+\frac1n)^n
$$

## Теорема о неравенстве пределов

⭐ Пусть $X_n$   и  $Y_n$   — последовательности, такие что $X_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a$     $Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large b$    .  Тогда:
1.  Если   $a < b$ ,  то  $X_n < Y_n$  при  $n \to \infty$
2.  Если $X_n \leq Y_n$  при  $n \to \infty$ ,  то $a \leq b$
Неравенство начинает выполняться с некоторого  $N \in \mathbb N$.

Доказательство:

1. $a < b$               $c \in (a, b)$
    
    $U = (-\infty, c)  \space \space \in  \mathcal N(a)$
    
    $V = (c, +\infty)  \space \space \in  \mathcal N(b)$
    
    $U \cap V = \emptyset$
    
    $\forall n > m_1$  ,   $X_n \in U$                  $\forall n > m_2 \space, \space \space Y_n \in V$
    
    $m = \max (m_1, m_2) \implies \forall n > m \space \space X_n <Y_n$
    
2. $\forall n > m_1 \space \space \space Y_n \geq X_n$
    
    Допустим, что  $b < a$ .  Тогда по пункту 1    $\exists m_2 \in \mathbb N$  ,  т.ч.
    
    $X_n > Y_n \space \space \space \forall n > m_2$$m = \max(m_1, m_2) \implies \forall n > m$   CONTR!
    

## Теорема о трех последовательностях (о двух милиционерах)

⭐ Пусть $X_n, \space U_n, \space V_n$   —  последовательности, такие что 
$X_n \in [U_n, \space V_n]$    и   $\lim\limits_{n \to \infty} U_n = \lim\limits_{n \to \infty} V_n = a$ 
Тогда $\lim\limits_{n \to \infty} X_n = a$.

Доказательство:

$V = (a - \varepsilon, a + \varepsilon) \in \mathcal N(a)$

$\exists m_1 \in \mathbb N$  , т.ч.  $U_n \in V \space \space \forall n>m_1$

$\exists m_2 \in \mathbb N$  , т.ч.  $U_n \in V \space \space \forall n>m_2$   

$\exists m_3 \in \mathbb N$  , т.ч.  $X_n \in [U_n, V_n] \space \space \forall n>m_3$ 

$\forall  n \geq \max(m_1, m_2, m_3) \space \space X_n \in V$ ,  по определению $\lim\limits_{n \to \infty} X_n = a$

> Топологическое определение предела последовательности:
$X_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a \in \mathbb R \Longleftrightarrow \forall U \in \mathcal N(a) \space \space \exists m \in \mathbb N$ ,  т.ч. 
$\forall n \geq m \space \space X_n \in U$
> 

## Теорема о сумме пределов

⭐ Сумма пределов является пределом суммы.
Если  $X_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a$  и  $Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large b$  и  $a + b$   определено, $(X + Y)_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a+b$

Доказательство (неравенство треугольника):

Пусть $a$ и $b \in \mathbb R$,   $\varepsilon > 0$

$|(X_n + Y_n) - (a+b)| \leq |X_n - a| + |Y_n - b| \leq \frac \varepsilon 2 + \frac \varepsilon 2 = \varepsilon \implies \\ \implies (X+Y) \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a + b$
Пусть   $b = + \infty$ ,  $a > -\infty$
$t \in \mathbb R, \space \space c \in (-\infty, a)$
$X_n > c \space , \space Y_n > t - c$   при $n \to \infty$
$X_n + Y_n > t \implies X + Y \space {\overrightarrow {\scriptsize n \to \infty} } \space + \infty$ . 

## Теорема о произведении пределов

⭐ Произведение пределов является пределом произведения.
Если  $X_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a$  и  $Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large b$  и  $a \cdot b$   определено, $(X \cdot Y)_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a \cdot b$

Доказательство:

$a \cdot b \in \mathbb R$
$|X_n \cdot Y_n - a \cdot b| = |X_n \cdot Y_n - Y_n \cdot a + Y_n \cdot a - a \cdot b| = \\ =|(X_n - a)Y_n + a (Y_n - b)| \leq |Y_n| \cdot |X_n - a| + |a| \cdot |Y_n - b| \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0$

## Лемма об умножении на бесконечно малую

⭐ Если $X_n$  ограничена, а  $Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0$ ,  то $(X \cdot Y)_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0$

Доказательство:

$X_n$  — ограничена 

$\forall n : X_n \in [a, b]$ 

$a \cdot Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0\leq X_n \cdot Y_n \leq b \cdot Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0 \implies X_n \cdot Y_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large 0$.

## Теорема о пересекающихся отрезках

⭐ Пересечение любого множества $M$ **попарно** пересекающихся отрезков тоже является отрезком, т.е. не пусто.

