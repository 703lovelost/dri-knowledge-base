# ЛЕКЦИЯ 14

> Пусть $V$ — векторное пространство размерности $n$ и $(e_1, ..., e_n)$ — старый базис, а $(e_1', ..., e_n')$ — новый базис.
$e_1' = a_{11} \overrightarrow e_1 + a_{21} \overrightarrow e_2 + a_{31} \overrightarrow e_3 + ... + a_{n1} \overrightarrow e_n$
$e_2' = a_{12} \overrightarrow e_1 + a_{22} \overrightarrow e_2 + a_{32} \overrightarrow e_3 + ... + a_{n2} \overrightarrow e_n$
$\vdots$
$e_n' = a_{1n} \overrightarrow e_1 + a_{2n} \overrightarrow e_2 + a_{3n} \overrightarrow e_3 + ... + a_{nn} \overrightarrow e_n$
$A = (a_{ij}) = \left( \begin{array} {rcl} a_{11} & a_{12} & a_{13} & ... & a_{1n} \\ a_{21} & a_{22} & a_{23} & ... & a_{2n} \\ \vdots & \vdots &  \vdots & & \vdots \\ a_{n1} & a_{n2} & a_{n3} & ... & a_{nn}\end{array} \right)$ — **матрица перехода** от старого базиса к новому.
> 

$v = \lambda_1 e_1 + ... + \lambda_n e_n = \lambda_1' e_1' + ... + \lambda_n' e_n' = \\ \lambda_1' (a_{11} e_1 + a_{21} e_2 + ... + a_{n1} e_n) + \lambda_2' (a{12} e_1 + a_{22} e_2 + ... + a_{n2} e_n) +... + \\ + \lambda_n' (a_{1n} e_1 + a_{2n} e_2 ++ a_{nn} e_n) = \\ e_1 (a_{11} \lambda_1' + a_{12} \lambda_2' + ... + a_{1n} \lambda_n') + e_2 (a_{21} \lambda_1' + a_{22} \lambda_2' + ... + a_{2n} \lambda_n') + ... + \\ + e_n (a_{n1} \lambda_1' + a_{n2} \lambda_2' + ... + a_{nn} \lambda_n')$ 

$\left\{ \begin{array} {rcl} a_{11} \lambda_1' + a_{12} \lambda_2' +...+ a_{1n} \lambda_n' = \lambda_1 \\ a_{21} \lambda_1' + a_{22} \lambda_2' +...+ a_{2n} \lambda_n' = \lambda_2 \\ ... \\ a_{n1} \lambda_1' + a_{n2} \lambda_2' +...+ a_{nn} \lambda_n' = \lambda_n \end{array} \right.$

$A \cdot \overrightarrow \lambda_1 = \lambda$        $\overrightarrow \lambda = A^{-1} \cdot \overrightarrow \lambda'$

$(\lambda_1, ... , \lambda_n)$ — координаты $v$ в старом базисе

$(\lambda_1', ... , \lambda_n')$ — координаты $v$ в новом базисе 

---

> **Обратная матрица**
$A^{-1} \cdot A = A \cdot A^{-1}= E = Id$
$(A^{-1})_{ij} = \Large \frac {1} {\det A} \normalsize (\alpha_{ij})$ ,  где 
$\alpha_{ij} = (-1)^{i + j} \cdot \det M_{ij}$ ( $M_{ij}$ — это матрица $A$  без i-й строки и j-го столбца ).
> 

## Матричное уравнение

$A \cdot X = E$
$X = A^{-1}$

$\det (A \cdot X) = \det A \cdot \det X$                      $\det E = 1$

## Аффинные пространства

> Пусть $\mathbb A$ —  некоторое множества элементов, которые будем называть точками и обозначать $A, B, C, ...$  и пусть $V$  — векторное пространство над $\R$. 
Множество $\mathbb A$  называется аффинным пространством, ассоциируемым с $V$ ,  если задана операция $\mathbb A \times V \longmapsto \mathbb A$ .
> 

$(A, \overrightarrow v) \mapsto B$
$A + \overrightarrow v = B$

![Untitled](img/mathlectures/Untitled%205.png)

**Свойства:**

1. $A + \overrightarrow 0 = A$
2. $\forall \space \space A, B \in \mathbb A \space \space \space \exists ! \space \space v \in V$ ,   т.ч.  $A + v = B$.
3. $A + (\overrightarrow v + \overrightarrow u) = (A + \overrightarrow v ) + \overrightarrow u$

Замеч.

1. Точки можно складывать и умножать на скаляр
2. Есть особый вектор $\overrightarrow 0$.    Нулевой точки нет.

Аффинная система координат

![Untitled](img/mathlectures/Untitled%206.png)

$(0, e_1, ... , e_n)$ — базис ассоциированного векторного пространства $V$. 

> Аффинное преобразование   $\Phi (x) = Ax + b$ 
$A$ — линейная часть,  $b$ — сдвиг.
> 

Замеч. Умножение комплексных чисел и умножение матрицы вида $\left( \begin{array} {rcl} x & -y \\ y & x\end{array} \right)$
это одно и то же ($z  = x + iy$).

## Евклидовы пространства

> $(V, <\cdot \space , \space \cdot >)$ — векторное пространство, наделенное билинейной операцией.
$<\cdot \space, \space \cdot > : V \times V \longmapsto \R \space (\mathbb C)$
> 

Билинейное  $\Leftrightarrow$  линейное по обеим переменным. 

$<u,v> = \sum\limits_{i = 1}^n u_i v_i$

1. $<v, v > \space \ge 0 \space \space \forall \space \space v \in V$ 
$<v , v> = 0 \Leftrightarrow \overrightarrow v = \overrightarrow  0$
2. $<\overrightarrow u, \overrightarrow v> = <\overrightarrow v, \overrightarrow u>$
3. $<\alpha u + \beta v, w> = \alpha <u, w> + \beta <v, w>$

Пример:

$P(x) = \{ ax^2 + bx + c \space | \space  a, b, c \in \R  \}$

$e_1 = 1 \\ e_2 = x \\ e_3 = x^2$

$ax^2 + bx + c \longmapsto (a, b, c)$

$\alpha x^2 + \beta x + \gamma \longmapsto (\alpha, \beta, \gamma )$

> Нормой (или длиной) вектора $v$  в  $V$   называется операция
 $\| v \| = | v | = \sqrt{<v, v>}$.
> 

Пример:

$f, g \in C([0, 1])$  — непрерывные на $[0, 1]$ функции

$<f , g> = \int\limits_0^1 f(x) g(x) \space dx$

$<u, v> = \sum\limits_{i = 1}^n u_i v_i$

$<\alpha f + \beta h \space , \space g> = \int\limits_0^1 (\alpha f , \space \beta h) \cdot g  = \alpha \int\limits^1_0 f \cdot g + \beta \int\limits^1_0 h \cdot g \\= \alpha <f, g> + \beta <h, g>$

## Неравенство Коши-Буняковского

⭐ $|<u, v>| \space \leq \space  |u| \cdot |v|$      $\forall u, v \in V$

Доказательство:

Рассмотрим вектор  $\lambda u = v$

$<\lambda u - v, \lambda u - v> \space \geq \space 0$ 

$\lambda^2<u, u> - 2 \lambda <u, v> + <v, v> \space \geq \space 0$

$D \leq 0$

$D = 4 <u, v>^2 - 4 <u, u> \cdot <v, v> \space \leq \space 0$

$<u, v>^2 \space \leq \space |u|^2 \cdot |v|^2$

$|<u, v>| \space \leq \space |u| \cdot |v|$

---

$-1 < \Large \frac {<u, v>} {|u| \cdot |v|} \normalsize < 1$
               $\cos (\widehat{u, v})$

> Векторы $\overrightarrow u$  и  $\overrightarrow v$   называются перпендикулярными (ортогональными) $u \perp v$ ,   если $<u, v> = 0 \space \Leftrightarrow \space \widehat {u, v} = \Large \frac \pi 2$
> 

## Теорема Пифагора

⭐ $c^2 = a^2 + b^2$

![Untitled](img/mathlectures/Untitled%207.png)

$\overrightarrow w = \overrightarrow u + \overrightarrow v$                               $<u, v> = 0$  $(u \perp v)$

$c^2 = |w|^2 = <w, w> = <u + v, u + v> = <u, u> + 2 <u, v> + <v, v> = a^2 + b^2$.

Пример:

$|\overrightarrow u | = |\overrightarrow v | \implies  \overrightarrow u + \overrightarrow v  \perp \overrightarrow u - \overrightarrow v$

$< u + v , u - v> = <u, u> - <v, v> = 0 \implies a^2 - b^2 = (a + b)(a - b)$

![Untitled](img/mathlectures/Untitled%208.png)

## Неравенство треугольника

⭐ $|u \pm v| \space \leq \space |u| + |v|$

Доказательство:

$<u \pm v, u \pm v> = <u, u> \pm 2 <u,v> + <v, v> = |u|^2 \pm 2<u, v> + |v|^2 \overset {К-Б} \leq |u|^2 \pm 2 |u| \cdot |v| + |v|^2 = (|u| \pm |v|)^2$  .

Пример:

В пространстве функций  $f, g \in C[0, 1]$

$|f| = (\int\limits^1_0 f^2(x) \space dx)^{1/2}$

**Неравенство Минковского**

$\left( \int\limits^1_0 (f(x) \pm g(x))^2 dx \right)^{1/2} = \left( \int\limits^1_0 f^2(x)dx \right)^{1/2} + \left( \int\limits^1_0 g^2(x)dx \right)^{1/2}$ 