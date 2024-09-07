# ЛЕКЦИЯ 8

$e^x \underset{x\to0}\sim 1 + x + \frac {x^2} {2!} + \frac {x^3} {3!} + o(x^3)$

$\sin x \underset{x\to0}\sim x - \frac {x^3} {3!} + \frac {x^5} {5!} - \frac {x^7} {7!} + o(x^7)$

$\cos x \underset{x\to0}\sim 1 - \frac {x^2} {2!} + \frac {x^4} {4!} - \frac {x^6} {6!} + o(x^6)$

$\arctg x \underset{x\to0}\sim x - \frac {x^3} {3} + \frac {x^5} {5} - \frac {x^7} {7} + o(x^7)$

$\ln (1+x) \underset{x\to0}\sim x - \frac {x^2} {2} + \frac {x^3} {3} - \frac {x^4} {4} + o(x^4)$

$(1+x)^p \underset{x\to0}\sim 1 + px + \frac{(p-1)px^2}{2!} + \frac{(p-2)(p-1)px^3}{3!} + o(x^3)$

$e^{i\phi} \sim 1+i\phi-\frac{x^2}{2!} - i\frac{x^3}{3!} +\frac{x^4}{4!} + i\frac{x^5}{5!}+ o(x^5)$

---

$f(x)$                $f'(x) = 3f(x)$                         $f(x) = e^{3x} \cdot C$

$(\cos\phi + i\sin\phi)' = - \sin \phi + i \cos \phi = i^2  \sin \phi + i\cos \phi = i(\cos \phi + i\sin \phi) \implies$
$\implies f'(\phi) = i \cdot f(\phi) \implies f(\phi) = e^{i\phi} \cdot C$

> $f'(x) = \lim\limits_{\Delta x \to 0} \frac {f(x + \Delta x) - f(x)} {\Delta x}$  — производная
> 

![graph.png](img/mathlectures/graph%201.png)

> $\tg \alpha = k = f'(x)$
$\tg \alpha = \frac {\Delta y} {\Delta x}$
> 

> Уравнение касательной в точке  $(x_0, y_0)$
$(y-y_0) = k (x - x_0)$
> 

## Дифференциал

> Дифференциалом функции называется величина, пропорциональная приращению независимой переменной и отличается от приращения функции на бесконечно палую величину по сравнению с приращением независимой переменной.
> 

$y - y_0 = k (x - x_0) \\ \space \space  \Delta x \space  \space  \space  \space \space \space \space \space \space \space \space \space  \space \space \space  \Delta y$

Пример:

![graph.png](img/mathlectures/graph%202.png)

Площадь: $y = x^2$

$\Delta y = (x + \Delta x)^2 - x^2 = 2x - \Delta x + (\Delta x)^2$

$\Delta y = dy + o(\Delta x)$

## Теорема о дифференциале и производной

⭐ Если функция имеет дифференциал, то она имеет и производную.

Доказательство:

$y = f(x) \space \space \space \space \space \space \space \space dy = k \Delta x$

$\Delta y = k \Delta x + o(\Delta x)$               $o(\Delta x) = \alpha \cdot \Delta x$              $\alpha \underset{\Delta x\to0}\longrightarrow 0$

$y'(x) = \frac {dy} {dx} = \frac {\Delta y} {\Delta x} = k + d \underset{\Delta x\to0}\longrightarrow k$.

---

Пример:

$\sqrt[3] {1,1}$                   $f(x) = \sqrt[3] {x}$

$f(x + \Delta x) \approx f(x) + f'(x) \cdot \Delta x$

$x = 1, \space$  $\Delta x = 0,1$               $f'(x) = 1 + \frac 1 {3 \cdot 1} \cdot 0,1$

$f' = {\large \frac 1 {3 \sqrt[3] {x^2}}}$

---

> $df(x) = f'(x) dx$
> 

## Свойство операции дифференцирования

(дифференцирование = взятие производной)

1. Линейность
$\lambda, \mu \in \mathbb R$,           $f(x), \space \space g(x)$
$(\lambda f(x) + \mu g(x))' = \lambda f'(x) + \mu g'(x)$
2. Утв. 1
$C' = 0$
Доказательство:
$\lim\limits_{\Delta x \to 0} \frac {f(x + \Delta x) - f(x)} {\Delta x} = \lim\limits_{\Delta x \to 0} \frac 0 {\Delta x} = 0$, т.к.  $f(x + \Delta x) = C$  и  $f(x) = C$
3. Утв. 2 
$(f + g)' = f' + g'$
Доказательство:
$\lim\limits_{\Delta x \to 0} \frac {(f+g) (x + \Delta x) - (f+g) (x) } {\Delta x} = \lim\limits_{\Delta x \to 0} \frac {f(x + \Delta x) - f(x)} {\Delta x} + \lim\limits_{\Delta x \to 0} \frac {g(x + \Delta x) - g(x)} {\Delta x} = \\ =f'(x) + g'(x)$
4. Утв. 3
$(f \cdot g)' = f' \cdot g + f \cdot g'$
Доказательство:
$y(x) = (f \cdot g) (x)$
$\Delta y = y(x + \Delta x) - y(x) = \\ = (f \cdot g) (x + \Delta x) - (f \cdot g) (x) = \\ =(f(x) + f'(x) (\Delta x) + o(\Delta x)) (g(x) + g'(x) (\Delta x) + o(\Delta x)) - f(x) \cdot g(x) = \\ = f(x) \cdot g(x) - f(x) \cdot g(x) + f'(x) \Delta x \cdot g(x) + f(x) \cdot g'(x) \Delta x + o(\Delta x) = \\ = (f'(x) \cdot g(x) + f(x) \cdot g'(x)) \Delta x + o(\Delta x) = \Delta y$
$\frac {\Delta y} {\Delta x} \underset{\Delta x \to 0}\longrightarrow f'(x) \cdot g(x) + f(x) \cdot g'(x)$.

Доказательство линейности:
$(\lambda f(x) + \mu g(x))' \underset{Утв \space 2}= (\lambda f(x))' + (\mu g(x))' \underset{Утв \space 3}= \lambda ' \cdot f + \lambda f' + \mu' \cdot g + \mu g' \underset{Утв \space 1}= \lambda f' + \mu g'$  

1. $\large (\frac f g) ' = \frac {f'g - fg'} {g^2}$

## Теорема Произведение сложной функции

⭐ Если $y = f(z)$  и $z = \phi (x)$, то производная $y = f(\phi (x))$ по переменной $x$ равна        $y'_x = f'_z \cdot z'_x = f'_z \cdot \phi ' _x$.

Доказательство:

$\Delta y = y'_z \cdot \Delta z = f'_z \cdot \Delta z = f'_z \cdot \phi'_x \cdot \Delta x$

> $\Delta z = \phi'_x \cdot \Delta x$
> 

$\large \frac {\Delta y} {\Delta x} = f'_z \cdot \phi' _x = \frac {df} {dz} \cdot \frac {dz} {dx} = \frac {dy} {dx}$     $(f = y, \space \space \phi = z)$

## Следствие

⭐ Композиция дифференцируемых функций — функция дифференцируемая.

