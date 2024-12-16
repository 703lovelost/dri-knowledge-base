# ЛЕКЦИЯ 1

> Множество - совокупность некоторых элементов.
> 

**Обозначения**

$\forall - квантор \space всеобщности$ (для каждого)

$\exists - квантор \space существования$ (существует)

$\exists!$  — существует единственное

$\rceil -$   отрицание

$$
A \cup B = \{ q \in \mathbb R : q \in A \space \lor \space q \in B \} \space - объединение \space множеств 
$$

$$
A \cap B = \{ q \in \mathbb R : q \in A \space \land \space q \in B \} \space - пересечение \space множеств
$$

$$
A \backslash B = \{  q \in A : q \notin B \}    \space -разность\space множеств
$$

$$
A = B \iff \forall p \in A \implies p \in B, \space \forall p \in B \implies p \in A \space - равенство \space множеств 
$$

$$
( \space \forall p \in A \implies p \in B) \implies A \subset B \space - подмножество
$$

$$
A \times B = \{ (a, b) : a \in A, \space b \in B\} \space - декартово \space произведение
$$

Пример:

$\mathbb R$ - вещественные числа. 

Плоскость - $\mathbb R^2 = \mathbb R \times \mathbb R = \{ (p_x, \space p_y) : p_x \in \mathbb R, p_y \in \mathbb R \}$

  

## Множества чисел

$\mathbb N$  - натуральные числа

$\mathbb N = \{ 0, 1, 2, 3...\}$

$\cap$

$\mathbb Z$  - целые числа

$\mathbb Z = \{... -2, -1, 0, 1, 2 ...\} = \mathbb N \cup \{-1\cdot n:n\in\mathbb N\} \cup \{0\}$

$\cap$

$\mathbb Q$  - рациональные числа 

$\mathbb Q = \{ \frac{m}{n} : m \in \mathbb Z, \space n \in \mathbb N \backslash \{ 0 \} \}$

$\cap$

$\mathbb R$  - вещественные числа

$e, \sqrt 2, \pi \in \mathbb R \space\backslash \space \mathbb Q$  - иррациональные числа

$\sqrt 2$   -  корень полинома с рациональными коэффициентами - $x^2 - 2 = 0$

$\pi$ -  не является корнем такого полинома - трансцендентное число 

$\cap$

$\mathbb C$ - комплексные числа 

$\mathbb C = \{ x + iy : x, y \in \mathbb R\}$  

$\space i = \sqrt {-1}$   -  мнимая единица

$\cap$

$\mathbb H$   -  кватернионы

$\mathbb H = \{ x + iy + jz + kw : x, \space y,\space z \in \mathbb R\}$

$i, \space j, \space  k$ - три мнимые единицы

## Основная теорема алгебры

Пусть   $p(z) = a_o \cdot z^n + a_1 \cdot z^{n-1} + ... \space+ a_n$ 

$a_i \in \mathbb C$ , то все его  $n$   корней тоже являются комплексными числами

$a = 0,(9)$          $b = 1$      $a = b$,    т.к.

$10a = 9,(9)$

$10a - a = 9a = 9 \implies a = 1$

## Принцип математической индукции

⭐ Пусть утверждение $W(n)$ , зависящее от натурального числа $n$, истинно при $n = 0, 1, 2 , 3, ..., n_0$.   $\forall n \in \mathbb N$   утверждение $W(n+1)$  является следствием $W(n).$  Тогда $W(n)$ истинно $\forall n \in \mathbb N.$

Доказательство (от противного):

$S = \{ n \in \mathbb N : W(n) \space ложно\} \neq \emptyset$

$m = \min(S)$

Тогда $m - 1 \notin S \implies W(m-1)$    -  истинно  $\implies W(m)$  - истинно. CONTR!
