# ЛЕКЦИЯ 11

## Векторные (Линейные) пространства

> Векторным (линейным) пространством  $V$  над коэффициентами из $\mathbb R \space (\mathbb C)$  называется множество элементов (векторов), удовлетворяющее следующим аксиомам:
$V, \space +$  (сложение векторов),  $\cdot$  (умножение на скаляр из $\mathbb R \space (\mathbb C)$  )
1.  $\overrightarrow x + \overrightarrow y = \overrightarrow y + \overrightarrow x$    (коммутативность)
2.  $(\overrightarrow x + \overrightarrow y ) + \overrightarrow z = \overrightarrow x + (\overrightarrow y + \overrightarrow z)$  (ассоциативность)
3.  $\exists \space \overrightarrow 0$
4.  $\forall \space \space \overrightarrow x \in V \space \space \exists \space \space -\overrightarrow x$  (обратный по сложению вектор) 
$- \overrightarrow x + \overrightarrow x = \overrightarrow 0$
5.  $1 \cdot \overrightarrow x = \overrightarrow x$       $\overrightarrow x \in V$
6.  $(\alpha \cdot \beta) \overrightarrow x = \alpha (\beta \cdot \overrightarrow x)$       $\alpha, \beta \in \mathbb R$
7.  $(\alpha + \beta) \cdot \overrightarrow x = \alpha \cdot \overrightarrow x + \beta \cdot \overrightarrow x$    (дистрибутивность)
8.  $\alpha \cdot (\overrightarrow x + \overrightarrow y) = \alpha \cdot \overrightarrow x + \alpha \cdot \overrightarrow y$  (дистрибутивность)
> 

$\mathcal P_n = \{ a_0x^n + a_1x^{n-1} + ... + a_n \}$  — полиномы степени $n$

$C([0, 1])$ — множество непрерывных на отрезке $[0, 1]$  функций.

> $\overrightarrow a, \overrightarrow b \in V$  называются коллинеарными, если $\exists \space \space k \in \mathbb R$ ,  т.ч.  $\overrightarrow b = k \cdot \overrightarrow a$  или  $\overrightarrow a = k \cdot \overrightarrow b$.
Т.е. координаты  $\overrightarrow a$  и  $\overrightarrow b$  пропорциональны.
> 

> Векторы $\overrightarrow a, \overrightarrow b, \overrightarrow c \in V$ называются компланарными, если  существует плоскость, в которой они все лежат. Т.е.   $\exists \space \space \lambda, \mu \in \mathbb R$  , т.ч.     $\overrightarrow c = \lambda \cdot \overrightarrow a + \mu \cdot \overrightarrow b$ .
> 

> Линейной комбинацией векторов $\overrightarrow V_1 , ... , \overrightarrow V_k \in V$ называется вектор вида $\sum \limits^k_{i = 1} \lambda_i\cdot \overrightarrow V_i$  $\lambda_i \in \mathbb R$.   $(\lambda_1 \cdot \overrightarrow V_1 + ... + \lambda_k \cdot \overrightarrow V_k)$.
> 

> Нетривиальной линейной комбинацией называется комбинация,  у которой не все $\lambda_i$  равны нулю.
> 

> $\overrightarrow 0 = \lambda \overrightarrow a + \mu \overrightarrow b - 1 \overrightarrow c$
Компланарность трёх векторов $\overrightarrow a, \overrightarrow b, \overrightarrow c \space \Longleftrightarrow \space$ не существует непрерывной линейной комбинации $a, b , c$ ,  равной нулевому вектору.
> 

> Линейной оболочкой  $span(A)$ для $A \subset V$ называется множество векторов $\overrightarrow v$ ,  каждый из которых может быть представление в видел линейной комбинации векторов из $A$,  т.е.  $\overrightarrow v = \lambda_1 \overrightarrow u_1 + ... + \lambda_k \overrightarrow u_k$          $\lambda_i \in R \space \space \space \space \space \overrightarrow u_i \in A$.
> 

> Векторным подпространством называется подмножество, которое само является векторным пространством.
> 

Пример:

Подпространство в $\mathbb R ^ 3 = \{ (x , y , z) \}$:

$\mathbb R^2 \times |0| =$   пространство $0xy$

Все плоскости, проходящие через начало координат (т.е. $\overrightarrow0$) являются векторными подпространствами в  $\mathbb R^3$.

Аналогично, все прямые, проходящие через 0 также являются векторными подпространствами.

 

## Линейно независимые вектора

> Векторы $\overrightarrow V_1, \overrightarrow V_2, ..., \overrightarrow V_k \space \in \space V$ называются линейно зависимыми, если существует неприрывная линейная комбинация $\sum\limits^k_{i =  1} \lambda_i \overrightarrow V_i = 0$.
> 

> Система векторов называется линейно независимой , если такой линейной комбинации не существует.
> 

> Максимальный (по включению) набор векторов векторного пространства $V$ называется базисом данного пространства.
> 

Пример:

Стандартный базис в $\mathbb R ^n$ — это набор векторов 
$\overrightarrow e_1 = (1, 0, 0,..., 0)$
$\overrightarrow e_2 = (0, 1, 0, ..., 0)$
$\vdots$
$\overrightarrow e_n = (0, 0 , 0, ..., 1)$.

> Координатами вектора $\overrightarrow v$ называются коэффициенты в разложении по базису $\overrightarrow v = \lambda_1 \overrightarrow e_1 + \lambda_2 \overrightarrow e_2 + ... + \lambda_n \overrightarrow e_n$.
> 

![Untitled](img/mathlectures/Untitled%202.png)

$(0, \overrightarrow e_1, \overrightarrow e_2 )$ — положительно ориентированный базис.
