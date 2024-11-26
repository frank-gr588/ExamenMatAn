# Вопросы по математическому анализу (часть 1, 2024)

**Лектор:** Морозова А.В.

## 1. **Понятие числовой последовательности.** Предел числовой последовательности, сходящиеся и расходящиеся последовательности, примеры.
### Понятие числовой последовательности

**Числовая последовательность** — это функция, определенная на множестве натуральных чисел, значения которой являются числами. Иными словами, это упорядоченный набор чисел, записанный в определенной последовательности.

### Предел числовой последовательности

Число $A$ называют **пределом числовой последовательности** $\{a_n\}$, если для любого положительного числа $\epsilon$ существует такое натуральное число $N$, что для всех $n > N$ выполняется неравенство $|a_n - A| < \epsilon$


**Предел числовой последовательности** — это значение, к которому стремятся элементы последовательности при неограниченном увеличении номера элемента. Если такая величина существует, то последовательность называется **сходящейся**. В противном случае, если элементы последовательности не приближаются к какому-либо числу, последовательность называется **расходящейся**.

### Примеры

1. **Сходящаяся последовательность - имеет предел
   - Последовательность $\frac{1}{n}$ при $n \to \infty$ стремится к 0.
   - Последовательность $\left(1 + \frac{1}{n}\right)^n$ при $n \to \infty$ стремится к числу $e$ (основание натурального логарифма).

2. **Расходящаяся последовательность** - не имеет предела
   - Последовательность $n$ при $n \to \infty$ стремится к бесконечности.
   - Последовательность $(-1)^n$ не имеет предела, так как она колеблется между -1 и 1.



## 2. **Теорема о единственности предела последовательности.**


### Теорема о единственности предела последовательности

**Теорема:**  Последовательность $\{a_n\}$ не может иметь двух различных пределов.


**Док-во:** Пусть последовательность $\{a_n\}$ имеет пределом число $A$. Докажем, что тогда никакое число $B \neq A$ не может быть пределом $\{a_n\}$. Для этой цели возьмем $\varepsilon$-окрестности точек $A$ и $B$ столь малыми, чтобы они не пересекались, например, возьмем $\varepsilon = \frac{|B - A|}{3}$ 

Так как $\lim_{n \to \infty} a_n = A$, то вне интервала $(A - \varepsilon, A + \varepsilon)$, в частности, в интервале $(B - \varepsilon, B + \varepsilon)$ может располагаться лишь конечное число точек из последовательности $\{a_n\}$. Поэтому число $B$ и не может быть пределом последовательности $\{a_n\}$.

## 3. **Ограниченная последовательность.** Теорема об ограниченности сходящейся последовательности. (б. д.) Пример.

### Теорема об ограниченности сходящейся последовательности

**Теорема:** Всякая сходящаяся последовательность ограничена, т. е. существуют числа $m$ и $М$ такие, что $m \leq a_n \leq M$
### Пример
$1, 0, 1, 0, 1$



## 4. **Арифметические действия над сходящимися последовательностями.**
### Арифметические действия над сходящимися последовательностями

Если $\{a_n\}$ и $\{b_n\}$ — две сходящиеся числовые последовательности с пределами $A$ и $B$ соответственно, то справедливы следующие свойства:

1. **Сумма последовательностей:**
   Если $\lim_{n \to \infty} a_n = A$ и $\lim_{n \to \infty} b_n = B$, то
   $$\lim_{n \to \infty} (a_n + b_n) = A + B.$$

2. **Разность последовательностей:**
   Если $\lim_{n \to \infty} a_n = A$ и $\lim_{n \to \infty} b_n = B$, то
   $$\lim_{n \to \infty} (a_n - b_n) = A - B.$$

3. **Произведение последовательностей:**
   Если $\lim_{n \to \infty} a_n = A$ и $\lim_{n \to \infty} b_n = B$, то
   $$\lim_{n \to \infty} (a_n \cdot b_n) = A \cdot B.$$

4. **Частное последовательностей:**
   Если $\lim_{n \to \infty} a_n = A$, $\lim_{n \to \infty} b_n = B$ и $B \neq 0$, то
   $$\lim_{n \to \infty} \left(\frac{a_n}{b_n}\right) = \frac{A}{B}.$$

### Пример

Рассмотрим две последовательности $a_n = \frac{1}{n}$ и $b_n = \frac{2}{n}$. Обе последовательности сходятся к нулю при $n \to \infty$.

1. **Сумма:**
   $$\lim_{n \to \infty} \left(\frac{1}{n} + \frac{2}{n}\right) = \lim_{n \to \infty} \frac{3}{n} = 0.$$

2. **Разность:**
   $$\lim_{n \to \infty} \left(\frac{2}{n} - \frac{1}{n}\right) = \lim_{n \to \infty} \frac{1}{n} = 0.$$

3. **Произведение:**
   $$\lim_{n \to \infty} \left(\frac{1}{n} \cdot \frac{2}{n}\right) = \lim_{n \to \infty} \frac{2}{n^2} = 0.$$

4. **Частное:**
   $$\lim_{n \to \infty} \left(\frac{\frac{1}{n}}{\frac{2}{n}}\right) = \lim_{n \to \infty} \frac{1}{2} = \frac{1}{2}.$$

Эти свойства позволяют выполнять арифметические операции над сходящимися последовательностями и находить пределы новых последовательностей, образованных этими операциями.
## 5. **Определение предела функции «на языке последовательностей» (предел по Гейне).** Теорема о единственности предела.
### Определение предела функции «на языке последовательностей» (предел по Гейне)

**Предел функции по Гейне** — Пусть функция $f(x)$ задана на произвольном множестве $E$ действительных чисел и пусть точка $x_0 \in E$. Функция $f(x)$ называется непрерывной в точке $x_0$, если для любой последовательности точек $\{x_n\}$, $x_n \in E$, сходящейся к точке $x_0$, соответствующая последовательность $\{f(x_n)\}$ значений функции сходится к $f(x_0)$.


### Теорема о единственности предела

**Теорема:** Если функция $f(x)$ имеет предел в точке $x_0$, то этот предел единственный.

### Пример

Рассмотрим функцию $f(x) = \frac{1}{x}$ при $x \to \infty$. Для любой последовательности $\{x_n\}$, стремящейся к бесконечности, последовательность $\{\frac{1}{x_n}\}$ будет стремиться к нулю. Таким образом, предел функции $f(x)$ при $x \to \infty$ равен нулю, и этот предел единственный.
## 6. **Ограниченная функция (ограниченная сверху, снизу).** Теорема об ограниченности функции, имеющей предел (конечный).
### Ограниченная функция

**Ограниченная функция** — это функция, значения которой не выходят за пределы некоторого интервала. Функция $f(x)$ называется ограниченной:

- **Сверху**, если существует такое число $M$, что для всех $x$ из области определения $f(x) \leq M$.
- **Снизу**, если существует такое число $m$, что для всех $x$ из области определения $f(x) \geq m$.
- **Ограниченной**, если она ограничена и сверху, и снизу, то есть существует такое число $K$, что $|f(x)| \leq K$ для всех $x$ из области определения.

### Теорема об ограниченности функции, имеющей предел (конечный)

**Теорема:** Если функция $f(x)$ имеет конечный предел $L$ при $x \to x_0$, то существует такая окрестность точки $x_0$, в которой функция $f(x)$ ограничена.

### Пример

Рассмотрим функцию $f(x) = \frac{1}{x}$ при $x \to \infty$. Предел этой функции равен нулю. Для любой окрестности точки $\infty$ (например, для всех $x > N$), функция $f(x)$ ограничена сверху числом $\frac{1}{N}$ и снизу числом $0$. Таким образом, функция $f(x)$ ограничена в этой окрестности.

Эти понятия и теорема важны для анализа поведения функций и их пределов.

## 7. **Арифметические действия с пределами функции.** Предел суперпозиции.
### Арифметические действия с пределами функции

Если функции $f(x)$ и $g(x)$ имеют пределы при $x \to x_0$, то справедливы следующие свойства:

1. **Сумма пределов:**
   Если $\lim_{x \to x_0} f(x) = A$ и $\lim_{x \to x_0} g(x) = B$, то
   $$\lim_{x \to x_0} (f(x) + g(x)) = A + B.$$

2. **Разность пределов:**
   Если $\lim_{x \to x_0} f(x) = A$ и $\lim_{x \to x_0} g(x) = B$, то
   $$\lim_{x \to x_0} (f(x) - g(x)) = A - B.$$

3. **Произведение пределов:**
   Если $\lim_{x \to x_0} f(x) = A$ и $\lim_{x \to x_0} g(x) = B$, то
   $$\lim_{x \to x_0} (f(x) \cdot g(x)) = A \cdot B.$$

4. **Частное пределов:**
   Если $\lim_{x \to x_0} f(x) = A$, $\lim_{x \to x_0} g(x) = B$ и $B \neq 0$, то
   $$\lim_{x \to x_0} \left(\frac{f(x)}{g(x)}\right) = \frac{A}{B}.$$

### Предел суперпозиции

**Теорема о пределе суперпозиции:** Если функция $g(x)$ стремится к $y_0$ при $x \to x_0$, и функция $f(y)$ непрерывна в точке $y_0$, то
$$\lim_{x \to x_0} f(g(x)) = f\left(\lim_{x \to x_0} g(x)\right) = f(y_0).$$

### Пример

Рассмотрим функции $f(x) = x^2$ и $g(x) = \sin(x)$. Найдём предел суперпозиции $f(g(x))$ при $x \to 0$.

1. Найдём предел $g(x)$ при $x \to 0$:
   $$\lim_{x \to 0} \sin(x) = 0.$$

2. Так как $f(y) = y^2$ непрерывна в точке $y = 0$, то
   $$\lim_{x \to 0} (\sin(x))^2 = \left(\lim_{x \to 0} \sin(x)\right)^2 = 0^2 = 0.$$

Таким образом, предел суперпозиции $f(g(x)) = (\sin(x))^2$ при $x \to 0$ равен 0.

Эти свойства и теорема позволяют выполнять арифметические операции с пределами функций и находить пределы сложных функций.





## 8. **Теоремы о пределах функции:** о предельном переходе в неравенство, о сжатой функции. Первый замечательный предел.
### Теоремы о пределах функции

#### Теорема о предельном переходе в неравенство

Если функции $f(x)$ и $g(x)$ имеют пределы при $x \to x_0$, и для всех $x$ из некоторой окрестности точки $x_0$ выполняется неравенство $f(x) \leq g(x)$, то
$$\lim_{x \to x_0} f(x) \leq \lim_{x \to x_0} g(x).$$

#### Теорема о сжатой функции (теорема о двух милиционерах)

Если для всех $x$ из некоторой окрестности точки $x_0$ выполняется неравенство $f(x) \leq h(x) \leq g(x)$, и $\lim_{x \to x_0} f(x) = \lim_{x \to x_0} g(x) = L$, то
$$\lim_{x \to x_0} h(x) = L.$$

### Первый замечательный предел

Первый замечательный предел:
$$\lim_{x \to 0} \frac{\sin x}{x} = 1.$$

Этот предел часто используется в анализе для нахождения пределов более сложных функций.

### Пример

Рассмотрим функцию $h(x) = x \sin \frac{1}{x}$ при $x \to 0$. Мы можем использовать теорему о сжатой функции, чтобы показать, что $\lim_{x \to 0} h(x) = 0$. Для этого заметим, что $-x \leq x \sin \frac{1}{x} \leq x$, и пределы $-x$ и $x$ при $x \to 0$ равны нулю.


## 9. **Предел функции на бесконечности.**
### Предел функции на бесконечности
**Определение.** Число $A$ называют пределом функции $f(x)$ при $x$, стремящемся к бесконечности, и пишут 
$$\lim_{x \to \infty} f(x) = A$$ 
если для любого $\epsilon > 0$ существует число $N > 0$ такое, что для всех $x$, удовлетворяющих 
условию $|x| > N$, верно неравенство $|f(x) - A| < \epsilon$.


### Пример

Рассмотрим функцию $f(x) = \frac{1}{x}$. При $x \to \infty$ функция стремится к нулю:
$$\lim_{x \to \infty} \frac{1}{x} = 0.$$

Для любого $\epsilon > 0$ мы можем найти такое число $M$, что для всех $x > M$ выполняется $|\frac{1}{x} - 0| < \epsilon$. Например, если $\epsilon = 0.01$, то $M = 100$.

Эти понятия важны для анализа поведения функций при больших значениях аргумента.

## 10. **Бесконечно большие функции.**
**Определение.** Если для любого, как угодно большого, числа $M > 0$ существует такое  число $\delta > 0$, что для всех $x \neq x_0$, удовлетворяющих условию  $|x - x_0| < \delta$, выполняется неравенство $|f(x)| > M$,  то функцию $f(x)$ называют бесконечно большой функцией при $x \to x_0$ и пишут 
$$\lim_{x \to x_0} f(x) = \infty.$$ 
При этом говорят также, что $f(x)$ при $x \to x_0$ имеет бесконечный предел.


1. Функция $f(x) = \frac{1}{x}$ является бесконечно большой при $x \to 0$.
2. Функция $g(x) = x^2$ является бесконечно большой при $x \to \infty$.

### Свойства бесконечно больших функций

1. **Сумма бесконечно больших функций**: Если $f(x)$ и $g(x)$ — бесконечно большие функции при $x \to x_0$, то $f(x) + g(x)$ также является бесконечно большой функцией при $x \to x_0$.
2. **Произведение бесконечно большой функции на ограниченную**: Если $f(x)$ — бесконечно большая функция при $x \to x_0$, а $g(x)$ — ограниченная функция при $x \to x_0$, то $f(x) \cdot g(x)$ также является бесконечно большой функцией при $x \to x_0$.

Эти понятия и свойства важны для анализа поведения функций при стремлении аргумента к определённым значениям.

## 11. **Теорема о пределе монотонной и ограниченной функции.** Второй замечательный предел.
### Теорема о пределе монотонной и ограниченной функции

**Теорема:** Если функция $f(x)$ монотонно возрастает или убывает и ограничена на некотором интервале, то она имеет конечный предел на этом интервале.

**Пример:** Рассмотрим функцию $f(x) = \frac{1}{x}$ при $x \to \infty$. Эта функция монотонно убывает и ограничена снизу нулем. Следовательно, по теореме, она имеет предел при $x \to \infty$, и этот предел равен нулю.

### Второй замечательный предел

**Второй замечательный предел:**
$$\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e,$$


## 12. **Бесконечно малые функции.** Теорема о сумме бесконечно малых функций.
 Если $a(x)$ и $f(x)$ — б. м. ф. при $x \to x_0$, то их сумма $a(x) + f(x)$ есть также б. м. ф. при $x \to x_0$.

Возьмем любое $\epsilon > 0$. Так как $a(x)$ — б. м. ф. при $x \to x_0$, то найдется $\delta_1 > 0$ такое, что для всех $x \neq x_0$, удовлетворяющих условию $|x - x_0| < \delta_1$, верно неравенство $\epsilon |a(x)| < 2$. (1)

По условию $f(x)$ также б. м. ф. при $x \to x_0$, поэтому найдется $\delta_2 > 0$, такое, что  для всех $x \neq x_0$, удовлетворяющих условию $|x - x_0| < \delta_2$, верно неравенство $\epsilon |f(x)| < 2$. (2)

Положим $\delta = \min\{\delta_1, \delta_2\}$. Тогда для всех $x \neq x_0$, удовлетворяющих условию $|x - x_0| < \delta$, будут одновременно верны неравенства (1) и (2). Поэтому $\epsilon |a(x) + f(x)| \leq |a(x)| + |f(x)| < 2 + 2 = \epsilon$ для всех $x \neq x_0$, $|x - x_0| < \delta$. 
Это означает, что сумма $a(x) + f(x)$ есть б. м. ф. при $x \to x_0$.


## 13. **Теорема о произведении бесконечно малой функции на ограниченную, следствия.**

**Теорема 6 (произведение б. м. ф. на ограниченную функцию)**. Если функция $a(x)$ является б. м. ф. при $x \to x_0$, а функция $f(x)$ ограничена в окрестности точки $x_0$, то произведение $a(x)f(x)$ есть б. м. ф. при $x \to x_0$.

По условию функция $f(x)$ ограничена в окрестности точки $x_0$. Это означает, что существуют такие числа $\delta_1 > 0$ и $M > 0$, что 
$$|f(x)| \leq M \forall x \in (x_0 - \delta_1, x_0 + \delta_1).$$
Возьмем любое $\epsilon > 0$. Так как по условию $a(x)$ - б. м. ф. при $x \to x_0$, то найдется такое $\delta_2 > 0$, что для всех $x \neq x_0$, удовлетворяющих условию $$|x - x_0| < \delta_2,$$ будет верно неравенство 
$$|a(x)| < \epsilon.$$
Положим $\delta = \min\{\delta_1, \delta_2\}$. Тогда для всех 
$$x \neq x_0,$$
удовлетворяющих условию 
$$|x - x_0| < \delta,$$ будут одновременно верны неравенства 
$$|f(x)| \leq M$$ и $$|a(x)| < \epsilon.$$
Поэтому 
$$|a(x)f(x)| = |a(x)| \cdot |f(x)| < \epsilon \cdot M = \epsilon \forall x, x \neq x_0, |x - x_0| < \delta.$$
Это означает, что произведение $a(x)f(x)$ есть б. м. ф. при $x \to x_0$.

### Теорема о произведении бесконечно малой функции на ограниченную

**Теорема:** Если $f(x)$ — бесконечно малая функция при $x \to x_0$, а $g(x)$ — ограниченная функция при $x \to x_0$, то произведение $f(x) \cdot g(x)$ также является бесконечно малой функцией при $x \to x_0$.

**Доказательство (без подробностей):** Поскольку $f(x)$ стремится к нулю, а $g(x)$ ограничена, то произведение $f(x) \cdot g(x)$ также стремится к нулю, что и означает, что $f(x) \cdot g(x)$ является бесконечно малой функцией.

### Следствия

1. **Произведение с константой:** Если $f(x)$ — бесконечно малая функция при $x \to x_0$, и $c$ — константа, то $c \cdot f(x)$ также является бесконечно малой функцией при $x \to x_0$.
2. **Сумма бесконечно малых функций:** Если $f(x)$ и $g(x)$ — бесконечно малые функции при $x \to x_0$, то их сумма $f(x) + g(x)$ также является бесконечно малой функцией при $x \to x_0$.

### Пример

Рассмотрим функции $f(x) = \frac{1}{x}$ и $g(x) = \sin(x)$ при $x \to \infty$. Функция $f(x)$ является бесконечно малой, а $g(x)$ — ограниченной. Следовательно, их произведение $\frac{\sin(x)}{x}$ также является бесконечно малой функцией при $x \to \infty$.

## 14. **Теорема об отношении б.м.ф. и функции, имеющей предел.** Связь функции имеющей предел с её пределом и б. м. ф.
**Теорема 7**. Если $a(x)$ - б. м. ф. при $x \to x_0$, а функция $f(x)$ имеет в точке $x_0$ предел, отличный от нуля, то частное $\frac{a(x)}{f(x)}$ есть б. м. ф. при $x \to x_0$.

Док-во:
Представим частное $\frac{a(x)}{f(x)}$ в виде 
$$\frac{a(x)}{f(x)} = a(x) \cdot \frac{1}{f(x)}.$$
В силу леммы функция $\frac{1}{f(x)}$ ограничена в проколотой окрестности точки $x_0$ и, следовательно, $a(x) \cdot \frac{1}{f(x)}$ - б. м. ф. при $x \to x_0$ как произведение б. м. ф. на ограниченную.

Условие $\lim f(x) \neq 0$ является существенным. Рассмотрим, например, функции $a(x) = x$ и $f(x) = x^2$, являющиеся б. м. ф. при $x \to 0$. Частное $\frac{x}{x^2} = \frac{1}{x}$, $x \neq 0$, очевидно, не является б. м. ф. при $x \to 0$, так что отношение двух бесконечно малых в общем случае не есть бесконечно малая функция.








### Теорема об отношении бесконечно малой функции и функции, имеющей предел

**Теорема:** Если $f(x)$ имеет конечный предел $A$ при $x \to x_0$, и $g(x)$ является бесконечно малой функцией при $x \to x_0$, то отношение $\frac{g(x)}{f(x)}$ также является бесконечно малой функцией при $x \to x_0$.

### Связь функции, имеющей предел, с её пределом и бесконечно малой функцией

Если функция $f(x)$ имеет предел $A$ при $x \to x_0$, то её можно представить в виде:
$$f(x) = A + \alpha(x),$$
где $\alpha(x)$ — бесконечно малая функция при $x \to x_0$.

### Пример

Рассмотрим функцию $f(x) = x + \sin(x)$ при $x \to 0$. Предел этой функции равен нулю:
$$\lim_{x \to 0} (x + \sin(x)) = 0.$$

Мы можем представить $f(x)$ в виде:
$$f(x) = 0 + (x + \sin(x)),$$
где $\alpha(x) = x + \sin(x)$ является бесконечно малой функцией при $x \to 0$.

Эти понятия и теорема важны для анализа поведения функций и их пределов.


## 15. **Бесконечно большие функции.** Теоремы о связи бесконечно больших и бесконечно малых функций. Пример.

### Бесконечно большие функции

**Бесконечно большая функция** — это функция $f(x)$, которая при стремлении аргумента $x$ к некоторому значению $x_0$ становится и остаётся по абсолютной величине больше любого наперёд заданного числа. Формально, функция $f(x)$ называется бесконечно большой при $x \to x_0$, если
$$\lim_{x \to x_0} f(x) = \infty.$$

### Теоремы о связи бесконечно больших и бесконечно малых функций

1. **Теорема 1:** Если $f(x)$ — бесконечно большая функция при $x \to x_0$, то $\frac{1}{f(x)}$ является бесконечно малой функцией при $x \to x_0$.
2. **Теорема 2:** Если $g(x)$ — бесконечно малая функция при $x \to x_0$, то $\frac{1}{g(x)}$ является бесконечно большой функцией при $x \to x_0$, при условии, что $g(x) \neq 0$.

### Пример

Рассмотрим функцию $f(x) = x$ при $x \to \infty$. Эта функция является бесконечно большой при $x \to \infty$. Следовательно, функция $\frac{1}{x}$ является бесконечно малой при $x \to \infty$.

Эти теоремы и примеры важны для анализа поведения функций и их пределов.

## 16. **Сравнение б. м. ф.** Символы о и O.

### Сравнение бесконечно малых функций

**Бесконечно малая функция** — это функция, которая стремится к нулю при стремлении аргумента к некоторому значению. Для сравнения бесконечно малых функций используются символы \(o\) и \(O\).

### Символ \(o\) (малое о)

Функция \(f(x)\) называется $o(g(x))\) при \(x \to x_0\), если
$$\lim_{x \to x_0} \frac{f(x)}{g(x)} = 0.$$
Это означает, что \(f(x)\) стремится к нулю быстрее, чем \(g(x)\).

### Символ \(O\) (большое О)

Функция \(f(x)\) называется \(O(g(x))\) при \(x \to x_0\), если существует такое положительное число \(M\) и окрестность точки \(x_0\), что для всех \(x\) из этой окрестности выполняется неравенство
$$|f(x)| \leq M |g(x)|.$$
Это означает, что \(f(x)\) ограничена по абсолютной величине функцией \(g(x)\) умноженной на константу.

### Пример

Рассмотрим функции \(f(x) = x^2\) и \(g(x) = x\) при \(x \to 0\):
- \(f(x) = x^2\) является \(o(x)\), так как \(\lim_{x \to 0} \frac{x^2}{x} = \lim_{x \to 0} x = 0\).
- \(f(x) = x^2\) также является \(O(x^2)\), так как \(\frac{x^2}{x^2} = 1\), и это неравенство выполняется для всех \(x\).

Эти символы помогают анализировать поведение функций и их пределов.


Рассмотрим функцию $f(x) = x$ при $x \to \infty$. Эта функция является бесконечно большой при $x \to \infty$. Следовательно, функция $\frac{1}{x}$ является бесконечно малой при $x \to \infty$.

Эти теоремы и примеры важны для анализа поведения функций и их пределов.

## 17. **Эквивалентные бесконечно малые и их свойства.** Теорема о замене на эквивалентные при вычислении предела, следствие. Таблица эквивалентных бесконечно малых, главная степенная часть функции.

### Эквивалентные бесконечно малые и их свойства

**Эквивалентные бесконечно малые функции** — это функции, которые стремятся к нулю при одном и том же пределе и имеют одинаковый порядок малости. Формально, функции $f(x)$ и $g(x)$ называются эквивалентными бесконечно малыми при $x \to a$, если
$$\lim_{x \to a} \frac{f(x)}{g(x)} = 1.$$

### Теорема о замене на эквивалентные при вычислении предела

**Теорема:** Если $f(x) \sim g(x)$ при $x \to a$, то предел $\lim_{x \to a} \frac{h(x)}{f(x)}$ равен пределу $\lim_{x \to a} \frac{h(x)}{g(x)}$, то есть
$$\lim_{x \to a} \frac{h(x)}{f(x)} = \lim_{x \to a} \frac{h(x)}{g(x)}.$$

**Следствие:** При вычислении пределов можно заменять бесконечно малые функции на эквивалентные им, что упрощает процесс нахождения пределов.

### Таблица эквивалентных бесконечно малых

Примеры эквивалентных бесконечно малых функций при $x \to 0$:
- $\sin(x) \sim x$
- $\tan(x) \sim x$
- $1 - \cos(x) \sim \frac{x^2}{2}$
- $\ln(1 + x) \sim x$

### Главная степенная часть функции

**Главная степенная часть функции** — это часть разложения функции в ряд Тейлора, которая доминирует при стремлении аргумента к нулю. Например, для функции $f(x) = x^3 + 2x^2 + x$ при $x \to 0$ главной степенной частью является $x$.

### Пример

Рассмотрим функцию $f(x) = \ln(1 + x)$ при $x \to 0$. Мы знаем, что $\ln(1 + x) \sim x$. Следовательно, при вычислении предела $\lim_{x \to 0} \frac{\ln(1 + x)}{x}$ можно заменить $\ln(1 + x)$ на $x$, и получим:
$$\lim_{x \to 0} \frac{\ln(1 + x)}{x} = \lim_{x \to 0} \frac{x}{x} = 1.$$

## 18. **Односторонние пределы.** Теорема о связи между односторонними пределами и пределом функции.

### Односторонние пределы

**Односторонний предел** — это предел функции, при котором аргумент стремится к предельной точке с одной стороны. Различают два типа односторонних пределов:
- **Левосторонний предел** (предел слева): $\lim_{x \to a-} f(x)$
- **Правосторонний предел** (предел справа): $\lim_{x \to a+} f(x)$

### Определения

- **Левосторонний предел** функции $f(x)$ в точке $a$ существует и равен $L$, если для любой последовательности $\{x_n\}$, стремящейся к $a$ слева (то есть $x_n < a$), последовательность значений $\{f(x_n)\}$ стремится к $L$.
- **Правосторонний предел** функции $f(x)$ в точке $a$ существует и равен $L$, если для любой последовательности $\{x_n\}$, стремящейся к $a$ справа (то есть $x_n > a$), последовательность значений $\{f(x_n)\}$ стремится к $L$.

### Теорема о связи между односторонними пределами и пределом функции

**Теорема:** Функция $f(x)$ имеет предел в точке $a$ тогда и только тогда, когда существуют оба односторонних предела в этой точке и они равны. То есть,
$$\lim_{x \to a} f(x) = L \iff \lim_{x \to a-} f(x) = L \text{ и } \lim_{x \to a+} f(x) = L.$$

### Пример

Рассмотрим функцию $f(x)$, определенную следующим образом:
$$
f(x) = \begin{cases} 
2x, & \text{если } x < 1 \\
3, & \text{если } x = 1 \\
x + 1, & \text{если } x > 1 
\end{cases}
$$

Для точки $x = 1$:
- Левосторонний предел: $\lim_{x \to 1-} f(x) = \lim_{x \to 1-} 2x = 2$
- Правосторонний предел: $\lim_{x \to 1+} f(x) = \lim_{x \to 1+} (x + 1) = 2$

Так как оба односторонних предела равны, предел функции в точке $x = 1$ существует и равен 2:
$$\lim_{x \to 1} f(x) = 2.$$

## 19. **Понятие функции, непрерывной в точке.** Непрерывность функции в точке справа, слева. Примеры. Теорема о необходимом и достаточном условии непрерывности функции в точке.

#### Понятие функции, непрерывной в точке

Функция $f(x)$ называется **непрерывной в точке** $x_0$, если:
1. Существует предел $\lim_{x \to x_0} f(x)$.
2. Существует значение функции $f(x_0)$.
3. Предел функции в точке равен значению функции в этой точке: $\lim_{x \to x_0} f(x) = f(x_0)$.

### Непрерывность функции в точке справа и слева

- **Непрерывность справа**: Функция $f(x)$ непрерывна в точке $x_0$ справа, если $\lim_{x \to x_0^+} f(x) = f(x_0)$.
- **Непрерывность слева**: Функция $f(x)$ непрерывна в точке $x_0$ слева, если $\lim_{x \to x_0^-} f(x) = f(x_0)$.

### Примеры

1. **Пример 1**: Функция $f(x) = x^2$ непрерывна в любой точке, так как предел $\lim_{x \to x_0} x^2 = x_0^2$ совпадает со значением функции $f(x_0) = x_0^2$.
2. **Пример 2**: Функция $f(x) = \frac{\sin x}{x}$ непрерывна в любой точке, кроме $x = 0$, так как в точке $x = 0$ функция не определена.

### Теорема о необходимом и достаточном условии непрерывности функции в точке

Функция $f(x)$ непрерывна в точке $x_0$ тогда и только тогда, когда для любой последовательности $\{x_n\}$, сходящейся к $x_0$, последовательность значений $\{f(x_n)\}$ сходится к $f(x_0)$.

### Формулировка теоремы

Если $\lim_{n \to \infty} x_n = x_0$, то $\lim_{n \to \infty} f(x_n) = f(x_0)$.

### Доказательство

1. Пусть $\{x_n\}$ — последовательность, сходящаяся к $x_0$.
2. По определению предела функции, $\lim_{x \to x_0} f(x) = f(x_0)$.
3. Следовательно, $\lim_{n \to \infty} f(x_n) = f(x_0)$.

Таким образом, функция $f(x)$ непрерывна в точке $x_0$.


## 20. **Устойчивость знака непрерывной функции.**
### Устойчивость знака непрерывной функции

**Устойчивость знака непрерывной функции** означает, что если функция $f(x)$ непрерывна в точке $x_0$ и $f(x_0) \neq 0$, то существует такая окрестность точки $x_0$, в которой функция сохраняет свой знак.

### Формулировка теоремы

Если функция $f(x)$ непрерывна в точке $x_0$ и $f(x_0) \neq 0$, то существует такая окрестность точки $x_0$, в которой знак функции совпадает со знаком $f(x_0)$.

### Пример

Пусть $f(x) = x^2 - 1$. Рассмотрим точку $x_0 = 2$:
- $f(2) = 2^2 - 1 = 3$, то есть $f(2) > 0$.
- Функция $f(x)$ непрерывна в точке $x_0 = 2$.
- Следовательно, существует такая окрестность точки $x_0 = 2$, в которой $f(x) > 0$.

Таким образом, в окрестности точки $x_0 = 2$ функция $f(x)$ сохраняет свой знак.



## 21. **Основные элементарные функции, их классификация, непрерывность элементарных функций.**
### Основные элементарные функции

**Элементарные функции** — это функции, которые можно выразить с помощью конечного числа операций сложения, вычитания, умножения, деления, взятия корней и композиции над основными функциями. К основным элементарным функциям относятся:

1. **Полиномиальные функции**: $f(x) = a_n x^n + a_{n-1} x^{n-1} + \ldots + a_1 x + a_0$, где $a_i$ — коэффициенты.
2. **Рациональные функции**: $f(x) = \frac{P(x)}{Q(x)}$, где $P(x)$ и $Q(x)$ — полиномы.
3. **Экспоненциальные функции**: $f(x) = a^x$, где $a > 0$.
4. **Логарифмические функции**: $f(x) = \log_a(x)$, где $a > 0$ и $a \neq 1$.
5. **Тригонометрические функции**: $f(x) = \sin(x)$, $f(x) = \cos(x)$, $f(x) = \tan(x)$ и т.д.
6. **Обратные тригонометрические функции**: $f(x) = \arcsin(x)$, $f(x) = \arccos(x)$, $f(x) = \arctan(x)$ и т.д.
7. **Гиперболические функции**: $f(x) = \sinh(x)$, $f(x) = \cosh(x)$, $f(x) = \tanh(x)$ и т.д.
8. **Обратные гиперболические функции**: $f(x) = \operatorname{arsinh}(x)$, $f(x) = \operatorname{arcosh}(x)$, $f(x) = \operatorname{artanh}(x)$ и т.д.

### Классификация элементарных функций

Элементарные функции можно классифицировать следующим образом:

1. **Алгебраические функции**: функции, которые можно выразить с помощью конечного числа операций сложения, вычитания, умножения, деления и взятия корней. Примеры: полиномы, рациональные функции.
2. **Трансцендентные функции**: функции, которые не являются алгебраическими. Примеры: экспоненциальные, логарифмические, тригонометрические и гиперболические функции.

### Непрерывность элементарных функций

Все элементарные функции **непрерывны на своих областях определения**. Это означает, что для любой элементарной функции $f(x)$ и любой точки $x_0$ из её области определения выполняется:

$$\lim_{x \to x_0} f(x) = f(x_0)$$

### Примеры непрерывности

1. **Полиномиальные функции**: Полиномы непрерывны на всей числовой прямой $\mathbb{R}$.
2. **Рациональные функции**: Непрерывны на всей числовой прямой, за исключением точек, где знаменатель равен нулю.
3. **Экспоненциальные и логарифмические функции**: Непрерывны на своих областях определения. Например, $e^x$ непрерывна на $\mathbb{R}$, а $\log(x)$ непрерывна на $(0, \infty)$.
4. **Тригонометрические функции**: Непрерывны на всей числовой прямой $\mathbb{R}$.
5. **Гиперболические функции**: Непрерывны на всей числовой прямой $\mathbb{R}$.


## 22. **Операции над непрерывными функциями.** Переход к пределу под знаком непрерывной функции.

**Операции над непрерывными функциями**

Рассмотрим основные операции над непрерывными функциями и переход к пределу под знаком непрерывной функции.

1. **Сумма и разность функций**
   Если $f(x)$ и $g(x)$ непрерывны в точке $a$, то функции $f(x) + g(x)$ и $f(x) - g(x)$ также непрерывны в точке $a$.

2. **Произведение функций**
   Если $f(x)$ и $g(x)$ непрерывны в точке $a$, то функция $f(x) \cdot g(x)$ непрерывна в точке $a$.

3. **Частное функций**
   Если $f(x)$ и $g(x)$ непрерывны в точке $a$ и $g(a) \neq 0$, то функция $\frac{f(x)}{g(x)}$ непрерывна в точке $a$.

4. **Переход к пределу под знаком непрерывной функции**
   Если $f(x)$ непрерывна в точке $a$ и $\lim_{x \to a} g(x) = L$, то $\lim_{x \to a} f(g(x)) = f(L)$.

Эти свойства позволяют выполнять различные операции с непрерывными функциями, сохраняя их непрерывность.

## 23. **Теорема о непрерывности сложной функции.**

**Теорема о непрерывности сложной функции**

Если функция $u = \varphi(x)$ непрерывна в точке $x_0$, а функция $y = f(u)$ непрерывна в точке $u_0 = \varphi(x_0)$, то сложная функция $y = f[\varphi(x)]$ непрерывна в точке $x_0$[.

**Доказательство:**

По условию функция $u = \varphi(x)$ в точке $x_0$ имеет предел, равный $\varphi(x_0) = u_0$. Кроме того, функция $y = f(u)$ непрерывна в точке $u_0$. На основании теоремы о переходе к пределу под знаком непрерывной функции сложная функция $y = f[\varphi(x)]$ в точке $x_0$ имеет предел, равный $f(u_0) = f[\varphi(x_0)]$:

$$
\lim_{x \to x_0} f[\varphi(x)] = f[\varphi(x_0)]
$$

что означает непрерывность сложной функции $f[\varphi(x)]$ в точке $x_0$.


## 24. **Замечательные пределы:** $$\lim_{x \to 0} \frac{\sin x}{x}$$ и $$\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x$$ и следствия из них.


**Следствия из первого замечательного предела**

1. **Предел функции синуса**:
   $$\lim_{x \to 0} \frac{\sin x}{x} = 1$$

2. **Предел функции тангенса**:
   $$\lim_{x \to 0} \frac{\tan x}{x} = 1$$

3. **Предел функции арксинуса**:
   $$\lim_{x \to 0} \frac{\arcsin x}{x} = 1$$

**Следствия из второго замечательного предела**

1. **Предел экспоненциальной функции**:
   $$\lim_{x \to 0} (1 + x)^{\frac{1}{x}} = e$$

2. **Предел логарифмической функции**:
   $$\lim_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e$$

3. **Предел функции натурального логарифма**:
   $$\lim_{x \to 0} \frac{\ln(1 + x)}{x} = 1$$

## 25. **Точки разрыва функции и их классификация:** точка разрыва первого рода, скачок функции, точка устранимого разрыва, точка разрыва второго рода, примеры.


### Точка разрыва первого рода
**Определение**: Точка $x = a$ называется точкой разрыва первого рода функции $f(x)$, если существуют конечные односторонние пределы $\lim_{x \to a^-} f(x)$ и $\lim_{x \to a^+} f(x)$, но они не равны между собой.

**Пример**:
$$
f(x) = 
\begin{cases} 
x, & \text{если } x < 1 \\
2, & \text{если } x = 1 \\
x + 1, & \text{если } x > 1 
\end{cases}
$$
Точка $x = 1$ является точкой разрыва первого рода.

### Скачок функции
**Определение**: Скачок функции в точке $x = a$ — это разность между значениями односторонних пределов функции в этой точке: $\Delta f = \lim_{x \to a^+} f(x) - \lim_{x \to a^-} f(x)$.

**Пример**:
$$
f(x) = 
\begin{cases} 
x, & \text{если } x < 1 \\
2, & \text{если } x = 1 \\
x + 1, & \text{если } x > 1 
\end{cases}
$$
Скачок функции в точке $x = 1$ равен $2 - 1 = 1$.

### Точка устранимого разрыва
**Определение**: Точка $x = a$ называется точкой устранимого разрыва функции $f(x)$, если существуют конечные односторонние пределы $\lim_{x \to a^-} f(x)$ и $\lim_{x \to a^+} f(x)$, и они равны между собой, но $f(a)$ не равно этому значению или не определено.

**Пример**:
$$
f(x) = 
\begin{cases} 
\frac{x^2 - 1}{x - 1}, & \text{если } x \neq 1 \\
3, & \text{если } x = 1 
\end{cases}
$$
Точка $x = 1$ является точкой устранимого разрыва, так как $\lim_{x \to 1} f(x) = 2$, но $f(1) = 3$.

### Точка разрыва второго рода
**Определение**: Точка $x = a$ называется точкой разрыва второго рода функции $f(x)$, если хотя бы один из односторонних пределов $\lim_{x \to a^-} f(x)$ или $\lim_{x \to a^+} f(x)$ не существует или равен бесконечности.

**Пример**:
$$
f(x) = 
\begin{cases} 
\frac{1}{x - 1}, & \text{если } x \neq 1 \\
0, & \text{если } x = 1 
\end{cases}
$$
Точка $x = 1$ является точкой разрыва второго рода, так как пределы $\lim_{x \to 1^-} f(x)$ и $\lim_{x \to 1^+} f(x)$ не существуют.

## 26. **Понятие непрерывности функции на интервале и на отрезке, функции кусочно-непрерывные на отрезке.**
Вот краткое изложение понятия непрерывности функции на интервале и на отрезке, а также кусочно-непрерывных функций:

- **Непрерывность на интервале**: Функция $f(x)$ непрерывна на интервале, если она непрерывна в каждой точке этого интервала.
- **Непрерывность на отрезке**: Функция $f(x)$ непрерывна на отрезке $[a,b]$, если она непрерывна на интервале $(a,b)$ и имеет пределы в точках $a$ и $b$, совпадающие со значениями функции в этих точках.
- **Кусочно-непрерывные функции**: Функция называется кусочно-непрерывной на отрезке, если она непрерывна на каждом подотрезке, на который можно разбить исходный отрезок, и имеет конечное число точек разрыва первого рода.




## 27. **Первая теорема Больцано — Коши (о существовании корня).** Вторая теорема Больцано — Коши (о промежуточном значении непрерывной функции).
**Теорема 19 (Коши) (о промежуточных значениях непрерывной функции)**

Пусть функция $f(x)$ непрерывна на отрезке $[a, b]$, причем $f(a) = A$, $f(b) = B$. Тогда каким бы ни было число $C$, заключенное между числами $A$ и $B$, на отрезке $[a, b]$ найдется по крайней мере одна точка $\alpha$ такая, что $f(\alpha) = C$.


## 28. **Первая теорема Вейерштрасса (об ограниченности непрерывной функции).** Вторая теорема Вейерштрасса (о наибольшем и наименьшем значении функции на отрезке).

(первая теорема Вейерштрасса), Если функция $j(x)$ непрерывна на отрезке $[а, Ь]$, то она ограничена на нем, т. е. существует такое число $К > О$, что для всех $х \in [а, Ь]$ верно неравенство $|j(x)| \leq К$.

(вторая теорема Вейерштрасса). Если функция $f(x)$ непрерывна на отрезке $[а, Ь]$, то она достигает на этом отрезке своих точной нижней и верхней граней, т. е. на отрезке $[а, Ь]$ найдутся такие точки $\zeta$ и $\eta$, что 
$f(\zeta) = m = \inf f(x), x \in [а, Ь]$ 
$f(\eta) = M = \sup f(x), x \in [а, Ь]$.


## 29. **Понятия монотонной и строго монотонной функции.** Теорема о непрерывности обратной функции (формулировка).

Функция $f(x)$ называется монотонной на $[а, Ь]$, если она на $[а, Ь]$ только неубывающая (в частности, возрастающая) или только невозрастающая (в частности, убывающая). Возрастающие и убывающие функции часто называют также строго монотонными
