# ЛЕКЦИЯ 13

## Матрицы

> Матрицей размерности $m \times n$ называется таблица, состоящая из $m$   строк и $n$  столбцов, элементами которой являются числа из $\mathbb R \space (\mathbb C)$.
> 

> Матрицы размерности $m \times 1$ называют столбцами. 
Матрицы размерности $1 \times n$ называют строками
> 

Утв.   Матрицы образуют векторное пространство размерности $m \times n$. 

Пример:

$2 \left( \begin{array}{rcl}  2 & 3 & 1 \\ 7 & 5 & 0 \end{array} \right) + 3 \left( \begin{array}{rcl}  -1 & 0 & 2 \\ 10 & 5 & 0 \end{array} \right) = \left( \begin{array}{rcl}  1 & 6 & 8 \\ 44 & 25 & 0 \end{array} \right)$

Если $m = n$ ,   то матрица называется квадратной.

> $B$ называется транспонированной матрицей $A_{m \times n}$, если 
$b_{ij} = a_{ji}$             $j = 1 ... m$                $i = 1 ... n$
и обозначается $A^T$.
> 

$\left [ \left( \begin{array}{rcl}  1 &  2 &  {-1} \\ 3 & 0 & 2  \end{array} \right) \right]^T = \left[ \begin{array}{rcl}  1 &3 \\ 2 & 0 \\ {-1} & 2 \end{array} \right]$

## Умножение матриц

$\overrightarrow v = (v_1, ... , v_n)_{1 \times n} \in V$

$\left( \begin{array}{rcl}  v_1 \\ \vdots \\ v_n \end{array} \right)_{n \times 1} = \sum\limits^{n}_{i = 1} u_i v_i$                     $<\overrightarrow u, \overrightarrow v>$

$A_{m \times n} \cdot B_{n \times k} = C_{m \times k}$

$\begin{array}{rcl} \overrightarrow \alpha_1  \\ \overrightarrow \alpha_2\\ \vdots \\ \overrightarrow \alpha_m \end{array}$$\left( \begin{array}{rcl}  a_{11} & ... & a_{1n}\\ a_{21} & ... & a_{2n} \\ \vdots & \vdots & \vdots \\ a_{m1} & ... & a_{mn} \end{array} \right)$$\cdot$ $\left( \begin{array}{rcl}  b_{11}  & b_{12} & ... &b_{1k}\\ b_{21} & b_{22} & ... & b_{2k} \\ \vdots & \vdots & \vdots \\b_{n1}& b_{n2} & ... & b_{nk} \end{array} \right)$  $=$
                                                                          $\overrightarrow \beta_1 \space \space \overrightarrow \beta_2 \space \space\space \space\space \space\space \space \overrightarrow \beta_k$
 $= C =$ $\left( \begin{array}{rcl}  <\alpha_1, \beta_1>  & <\alpha_1, \beta_2> & ... & <\alpha_1, \beta_k>\\  \vdots  & \vdots & \vdots & \vdots \\ <\alpha_m, \beta_1> & <\alpha_m , \beta_2> & ... & <\alpha_m, \beta_k> \end{array} \right)$

Пример:

$\left( \begin{array}{rcl}  1 & 2 \\ 3 & 4 \\ 5 & 6 \end{array} \right)_{3 \times 2}$$\cdot$ $\left( \begin{array}{rcl}  1 & 5 & {-1} \\ 0 & 4 & 3 \end{array} \right)_{2 \times 3}$ $=$ $\left( \begin{array}{rcl}  11 & 8 & 5 \\ 23 & 16 & 9 \\ 35 & 24 & 13 \end{array} \right)_{3 \times 3}$

Замеч:  $A \cdot B \neq B \cdot A$  в общем случае

Замеч: Если умножать квадратные матрицы, то будут получаться тоже квадратные.

> Единичная матрица
$E_{n \times n} = Id_{n \times n} = I_{n \times n}$
$A_{n \times n} \cdot E_{n \times n} = E_{n \times n} \cdot A_{n \times n} = A_{n \times n}$
$\delta_{ij} = \left\{ \begin{array}{rcl} 1, \space i = j \\ 0, \space i \neq j \end{array} \right.$

$E = \left( \begin{array}{rcl}  1 & 0 & 0 & ... & 0 \\ 0 & 1  & 0  & ... & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & ... & 1 \end{array} \right)$
> 

## Свойства умножения матриц

1. $A \cdot B \neq B \cdot A$   нет коммутативности
2. $(A \cdot B) \cdot C = A \cdot ( C \cdot B)$   ассоциативность
3. $(A_{n \times k} + B_{n \times k }) \cdot C_{k \times l} = A \cdot C + B \cdot C$
4. Не для всех $A$   $\exists \space \space A^{-1}$   обратная матрица
$A^{-1} \cdot A = A \cdot A^{-1} = E$

$<M_{n \times n}, \space  + \space , \space \cdot >$  — умножение матриц

## Определитель (детерминант) матрицы

(только для квадратных матриц)

$a \in \mathbb R$      $a = a_{1 \times 1}$        $\det a = a$

$\det \left( \begin{array}{rcl} a & b \\ c & d\end{array} \right)_{2 \times 2} = \left| \begin{array}{rcl} a & b \\ c & d\end{array} \right| = ad - bc$

## Лемма

⭐ $\det \left( \begin{array}{rcl} a & b \\ c & d\end{array} \right) = \pm S$

![Untitled](img/mathlectures/Untitled%203.png)

Доказательство:

![Untitled](img/mathlectures/Untitled%204.png)

$\cos \alpha = \Large \frac {<u, v>} {|u| \cdot |v|}$

$S_{uv} = |u| \cdot |v| \cdot \sin \alpha = \sqrt{a^2 + b^2} \cdot \sqrt{c^2 + d^2} \cdot \sqrt{1 - \Large (\frac {<(a, b), (c, d)>} {\sqrt{a^2 + b^2} \cdot \sqrt{c^2 + d^2}}) \normalsize ^2} =$  $\Large \frac {\sqrt{a^2 + b^2}} {\sqrt{a^2 + b^2}} \cdot \frac {\sqrt{c^2 + d^2}} {\sqrt{c^2 + d^2}} \cdot \normalsize \sqrt{(a^2 + b^2)(c^2 + d^2) - (a \cdot c + b \cdot d)} =$ 

$= a^2 c^2 + a^2 d^2 + b^2 c^2 + b^2 d^2 - a^2 c^2 - 2abcd - b^2 d^2 =$  

 $= \sqrt {a^2 d^2 - 2abcd + b^2c^2} = \pm (ad - bc)$ . 

---

$\left| \begin{array}{rcl} a & b \\ c & d\end{array} \right| = ad - bc$

$\left| \begin{array}{rcl} c & d \\ a & b\end{array} \right| = cb - ad = - \left| \begin{array}{rcl} a & b \\ c & d\end{array} \right|$

$|A| = \left| \left( \begin{array}{rcl} a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \\ \vdots & \vdots & \vdots \\ c_1 & c_2 & c_3\end{array} \right) \right|  =$  $a_1 \left| \begin{array} {rcl} b_2 & b_3 \\  c_2 & c_3\end{array}\right|$ —  $a_2 \left| \begin{array} {rcl} b_1 & b_3 \\  c_1 & c_3\end{array}\right|$ + $a_3 \left| \begin{array} {rcl} b_1 & b_2 \\  c_1 & c_2\end{array}\right|$ $=$  
$= a_1 b_2 c_3 - a_1 b_3 c_2 - a_2 b_1 c_3 + a_2 b_3 c_1 + a_3 b_1 c_2 - a_3 b_2 c_1 =$ 
$= \sum\limits^{3!}_{перест-ки \space i, j ,k} a_i b_j c_k$

## Свойства определителя

1. $\det A = \det A^T$
2. $\det \left( \begin{array} {rcl} \lambda a \\ b \space \\ c \space \end{array} \right)$ $= \lambda \det \left( \begin{array} {rcl} a \\ b \\ c  \end{array} \right)$
3. $\det \left( \begin{array} {rcl} a' + \tilde a \\ b \space \space \space \space \\ c \space \space \space \space \end{array} \right)$ $=$  $\det \left( \begin{array} {rcl} a' \\ b  \space \\ c \end{array} \right) + \det \left( \begin{array} {rcl} \tilde a \\ b  \\ c  \end{array} \right)$
4. Если векторы, составляющие матрицу линейно зависимы, то ее определитель равен 0.
5. $\det \left( \begin{array} {rcl}  a \\ b \\ c \end{array} \right) = - \det \left( \begin{array} {rcl} b \\ a \\ c \end{array} \right)$
6. $\det (A + B) \neq \det A + \det B$
7. $\det (A \cdot B) = \det A \cdot \det B$

## Системы линейных уравнений

$\begin{array} {rcl} I \\ II \\ III \end{array} \left\{ \begin{array} {rcl} a_1x + b_1y + c_1z = d_1 \\ a_2x + b_2y + c_2z = d_2  \\ a_3x + b_3y + c_3z = d_3  \end{array} \right.$

$A \overrightarrow x = \overrightarrow d$

$A = \left( \begin{array} {rcl} a  & b & c \\ \vdots & \vdots & \vdots \end{array} \right)$       $\overrightarrow x = \left( \begin{array} {rcl} x \\ y \\ z \end{array} \right)$       $\overrightarrow d = \left( \begin{array} {rcl} d_1 \\ d_2 \\ d_3 \end{array} \right)$

### Метод Крамера

$x_0 = \Large \frac {1} {\det A} \cdot \normalsize \det \left( \begin{array} {rcl} a  & b & c \\ \vdots & \vdots & \vdots \end{array} \right)$

$y_0 = \Large \frac {1} {\det A} \cdot \normalsize \det \left( \begin{array} {rcl} a  & d & c \\ \vdots & \vdots & \vdots \end{array} \right)$

$z_0 = \Large \frac {1} {\det A} \cdot \normalsize \det \left( \begin{array} {rcl} a & b & d \\ \vdots & \vdots & \vdots \end{array} \right)$

Доказательство:

$I \cdot \left| \begin{array} {rcl} b_2 & c_2 \\ b_3 & c_3 \end{array} \right| - II \left| \begin{array} {rcl} b_1 & c_1 \\ b_3 & c_3 \end{array} \right| + III \left| \begin{array} {rcl} b_1 & c_1 \\ b_2 & c_2 \end{array} \right|$

$x \left( a_1\left| \begin{array} {rcl} b_2 & c_2 \\ b_3 & c_3 \end{array} \right| - a_2 \left| \begin{array} {rcl} b_1 & c_1 \\ b_3 & c_3 \end{array} \right| + a_3 \left| \begin{array} {rcl} b_1 & c_1 \\ b_2 & c_2 \end{array} \right| \right) +$ 

$+ \space y \left( b_1\left| \begin{array} {rcl} b_2 & c_2 \\ b_3 & c_3 \end{array} \right| - b_2 \left| \begin{array} {rcl} b_1 & c_1 \\ b_3 & c_3 \end{array} \right| + b_3 \left| \begin{array} {rcl} b_1 & c_1 \\ b_2 & c_2 \end{array} \right| \right) +$ 

 $+ \space z \left( c_1\left| \begin{array} {rcl} b_2 & c_2 \\ b_3 & c_3 \end{array} \right| - c_2 \left| \begin{array} {rcl} b_1 & c_1 \\ b_3 & c_3 \end{array} \right| + c_3 \left| \begin{array} {rcl} b_1 & c_1 \\ b_2 & c_2 \end{array} \right| \right) =$

$=  d_1\left| \begin{array} {rcl} b_2 & c_2 \\ b_3 & c_3 \end{array} \right| - d_2 \left| \begin{array} {rcl} b_1 & c_1 \\ b_3 & c_3 \end{array} \right| + d_3 \left| \begin{array} {rcl} b_1 & c_1 \\ b_2 & c_2 \end{array} \right|$  

### Метод Гаусса

$\left( \begin{array} {rcl} a_1 & b_1 & c_1 & d_1 \\ a_2 & b_2 & c_2 & d_2 \\ a_3 & b_3 & c_3 & d_3 \\ a_4 & b_4 & c_4 & d_4 \end{array} \right)$$\cdot$ $\left( \begin{array} {rcl} x  \\ y \\ z \\ u \end{array} \right)$ $= \left( \begin{array} {rcl} f_1 \\ f_2 \\ f_3 \\ f_4 \end{array} \right)$

$a_1 x + b_1 y + c_1 z + d_1 u  = f_1 \space \space \space I$
$a_2 x + ... + d_2 u = f_2 \space \space \space II$

$II - \Large \frac {a_2} {a_1} \normalsize I \Longleftrightarrow ox$ 

$\left( \begin{array} {rcl} a_1 & b_1 & c_1 & d_1 \\ 0 & b_2 & c_2 & d_2 \\ 0 & b_3 & c_3 & d_3 \\ 0 & b_4 & c_4 & d_4 \end{array} \right)$ $\left( \begin{array} {rcl} x \\ y \\ z \\ u \end{array} \right)$$= \left( \begin{array} {rcl} f_1 \\ f_2 \\ f_3 \\ f_4 \end{array} \right)$

$0  = \left\{ \begin{array} {rcl} \neq 0 \space , \space \space решений \space нет \\ = 0 \space ,\space \space есть & \end{array} \right.$

$\left( \begin{array} {rcl} a_1 & b_1 & c_1 \\ 0 & b_2 & c_2 \\ 0 & 0 & 0\end{array} \right) \space \left( \begin{array} {rcl} x \\ y \\ z \end{array} \right)$  $= \left( \begin{array} {rcl} f_1 \\ f_2 \\ 0\end{array} \right)$

---

**Диагональная матрица**
$\left( \begin{array} {rcl} a_{11} & \space & \space & \space \\ \space & a_{22} & \space & \LARGE 0 \\  &\space & \ddots & \space \\ \LARGE0 \space & \space & \space & a_{nn}\end{array} \right)$  $\left( \begin{array} {rcl} x_1 \\ x_2 \\ \vdots \\ x_n \end{array} \right)$   $= \left( \begin{array} {rcl} f_1 \\ f_2 \\ \vdots \\ f_n\end{array} \right)$

**Треугольная матрица**

$\left( \begin{array} {rcl} a_{11} & \space & \space & \space \\ \space & a_{22} & \space & \LARGE * \\  &\space & \ddots & \space \\ \LARGE0 \space & \space & \space & a_{nn}\end{array} \right)$   $\left( \begin{array} {rcl} x_1 \\ x_2 \\ \vdots \\ x_n \end{array} \right)$  $= \left( \begin{array} {rcl} f_1 \\ f_2 \\ \vdots \\ f_n\end{array} \right)$
