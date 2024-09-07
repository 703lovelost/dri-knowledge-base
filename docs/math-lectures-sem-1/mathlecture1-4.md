# ЛЕКЦИЯ 4

## Принцип Кантора вложенных отрезков

⭐ Пересечение любого семейства вложенных отрезков не пусто.

$I_0 \supset I_1 \supset I_2 \supset ...$

$I_k = [0, \frac 1 {k+1}] \space \space \space \bigcap I \neq \emptyset$

Пример:

$a_0 = 3 \\ a_1 = 3.1 \\ a_2 = 3.14 \\ \space \space \space \vdots$ 

$b_0 = 4 \\ b_1 = 3.2 \\ b_2 = 3.15 \\ \space \space \space \vdots$ 

$I_k = [a_k, b_k]$              $\bigcap\limits_{k = 0}^\infty I_k = \pi$

## Теорема о стягивающихся отрезках

⭐ Последовательность вложенных отрезков, длина которых стремится к нулю, сходится к одной точке.

> $n_k$  — строго возрастающая последовательность натуральных чисел.
$X_{n_k}$   называется подпоследовательностью последовательности $X_n$ .
> 

> $X_{n_k} \space {\overrightarrow {\scriptsize k \to \infty} }\space \large a$ ,  то число $a$ называется частичным пределом последовательности $X_n$.
> 

## Теорема Больцано-Вейерштрасса о частичных пределах

⭐ Множество частичных пределов ограниченной последовательности $X_n \in \mathbb R$ содержит наибольший и наименьший элемент и, следовательно, в $\mathbb R$ всякая ограниченная последовательность имеет сходящуюся подпоследовательность.

Доказательство (принцип Больцано - деление пополам):

$\{ x_0, \space x_1, \space x_2, ...\} \subset [a_1, b_1]$

Разделим отрезок $[a_1, b_1]$ пополам и возьмем в качестве $[a_2, b_2]$ ту половину, в которой оказалось бесконечно много членов исходной последовательности и т.д.

$[a_1, b_1] \supset [a_2, b_2] \supset ... \supset [a_n, b_n] \supset ...$

По принципу Кантора $\bigcap\limits_{i = 1}^\infty \space [a_i, b_i] \neq \emptyset$

$\xi = \bigcap\limits_{i = 1}^\infty \space [a_i, b_i]$  

Будем выбирать в отрезке $[a_i, b_i]$ какой-то член последовательности $X_n$ и обозначать его  $y_k$ . Важно чтобы номера  $n$  росли.

$y_k = X_{n_k} \longrightarrow \xi$. 

> $\lim\limits_{n \to \infty}X_n = \inf(множества \space всех \space частичных \space пределов)$  — нижний предел
> 

> $\lim\limits_{n \to \infty}X_n = \sup(множества \space всех \space частичных \space пределов)$  — верхний предел
> 

---

$(a+b)^2 = a^2 + 2ab + b^2$

$(a+b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$

$(a+b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4$

 ${\large C}_n^k = \frac {n!} {k!(n-k)!}$

## Теорема о пределе монотонной последовательности

⭐ Всякая ограниченная сверху монотонно возрастающая последовательность имеет конечный предел.

> Последовательность $X_n$ называется фундаментальной (или последовательностью Коши), если $\forall \varepsilon > 0 \space \space \exists m  \in \mathbb N= m(\varepsilon),$  т.ч. $\forall k \space$и $l > m |X_k - X_l| < \varepsilon$.
> 

## Теорема Коши

⭐ Если последовательность фундаментальна, то у неё есть предел.

Замечание: В определении фундаментальной последовательности отсутствует само значение предела, к которому сходится последовательность $X_n$.

## Критерий Коши

⭐ Последовательность $X_n \in \mathbb R$  вещественных чисел имеет конечный предел (сходится в $\mathbb R$ )  $\Leftrightarrow$ $X_n$ фундаментальна.

Доказательство:

$\Rightarrow$

$X_n \space {\overrightarrow {\scriptsize n \to \infty} } \space \large a \in \mathbb R$      $\varepsilon > 0$

$|X_n - a| \leq \frac \varepsilon 2$ ,  т.е. $\exists m \in \mathbb N$, т.ч. $\forall n \geq m \space \space \space |X_n - a| < \frac \varepsilon 2$

$|X_k - X_l| = |X_k - a + a - X_l| \leq |X_k-a| + |a - X_l| < \frac \varepsilon 2 + \frac \varepsilon 2 = \varepsilon \space \space \forall k,l \geq m$

$\Leftarrow$

$\forall \varepsilon > 0 \space \space \exists N = N(\varepsilon)$ ,  т.ч.  $\exists k, l \geq N : |X_k - X_l| > \varepsilon$

$X_n$ — фундаментальна $\implies$$X_n$ — ограничена. 

От противного: допустим, что $X_n$  — не ограничена.

$\exists$  последовательность $X_{n_k} = y_k \geq k \space \forall k \in \mathbb N$

Проверим, что $y_k$ удовлетворяет отрицанию определения фундаментальности.

 $|y_k - y_l| \geq 1 \implies \varepsilon = 1$  CONTR!

По теореме Больцано-Вейерштрасса: т.к. $X_n$ — ограничена.

$\exists X_{n_k} \space {\overrightarrow {\scriptsize k \to \infty} } \space \large a \in \mathbb R$ 

Рассмотрим $\varepsilon > 0 , \space \space m \in \mathbb N$

$|X_i - X_j| < \varepsilon \space \space \forall i,j \geq m$

$n_k\space {\overrightarrow {\scriptsize k \to \infty} } \space \large \infty$

$\exists z \in \mathbb N$ ,  т.ч. $n_k \geq m \space \space \forall k \geq z. \space \space \space \space \space \space \space \space \space \space |X_{n_k = i} - X_{n=j}| \leq \varepsilon$

$|X_n - a| \leq |X_n - X_{n_k}| + |X_{n_k} - a| < 2\varepsilon$  (неравенство треугольника).
