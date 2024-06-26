**_Oпределение 1._** Линейным дифференциальным уравнением первого порядка называется уравнение, которое можно записать в виде(2.15)
$$y'+p(x)y=f(x),$$
где $p(x)$ и $f(x)$ – заданные непрерывные функции, в частности – постоянные ( $f(x)$ – свободный член или правая часть уравнения). Будем полагать, что коэффициент уравнения $p(x)$ и свободный член $f(x)$ уравнения (2.15) непрерывны на некотором интервале (a;b) , в котором разыскивается решение уравнения ( 2.15) .

Если правая часть в уравнении (2.15), функция $f(x)$, тождественно не равна нулю на (a;b), то уравнение (2.15) называется _линейным неоднородным дифференциальным уравнением первого порядка._

Если же правая часть в уравнении (2.15), функция $f ( x)$, тождественно равна нулю на (a; b), то уравнение (2.15) принимает вид(2.16):
$$y'+p(x)y=0$$
и называется в этом случае _линейным однородным дифференциальным уравнением первого порядка_, соответствующим линейному неоднородному уравнению (2.15) (линейное однородное дифференциальное уравнение I порядка не следует смешивать с однородными дифференциальными уравнениями первого порядка, содержащими однородную функцию, которые рассматривались выше).Отметим, что линейное однородное уравнение является уравнением с разделяющимися переменными.

Иногда уравнение (2.16) называют линейным уравнением без правой части.

Существует несколько методов решения линейного дифференциального уравнения первого порядка. Рассмотрим несколько из них.

### I. Метод И. Бернулли

Решение уравнения (2.15) разыскивается в виде(2.17)
$$y=u\cdot v$$
где $u=u(x)$, $v=v(x)$ – новые неизвестные функции аргумента $x$ .

Из равенства (2.17) находят(2.18)
$$y'=u' \cdot v + u \cdot v' $$
Подставляя в уравнение (2.15.) вместо y и y ′ их выражения через u и v , согласно равенствам (2.17.) и (2.18), получают
$$u'\cdot v+ u\cdot v'+p(x)\cdot u \cdot v= f(x),$$
Далее, группируя в левой части слагаемые с общим множителем v (или u ), и, вынося общий множитель за скобки, имеют(2.19)
$$[u'+p(x)u]v+uv'=f(x)$$
В качестве функции $u(x)$ выберем одно из решений дифференциального уравнения(2.20)
$$u'+p(x)u=0$$
т. е. функция $u(x)$ подбирается так, чтобы коэффициент при v в уравнении (2.19)  , был равен нулю. Тогда функция $v(x)$ находится как общее решение уравнения(2.21)
$$u\cdot v'=f(x),$$
Подставляя полученные выражения для функцийu $u=u(x)$ и $v=v(x)$ в формулу (2.17), находят искомую функцию $y(x)$.

Таким образом, с помощью подстановки (2.17) решение линейного дифференциального уравнения первого порядка относительно неизвестной функции $y(x)$ сводится к решению двух дифференциальных уравнений с разделяющимися переменными, одно – относительно новой неизвестной функции $u(x)$, другое – относительно другой новой неизвестной функции $v(x)$.

_**Пример 1.**_ Найти решение уравнения,
$$y' + \frac{2y}{x}=x$$
удовлетворяющее начальному условию $y(1)=0$.

**_Решение._** Данное уравнение является линейным первого порядка. Здесь можно считать $p(x)= \frac{2}{x},\ f(x)=x$.
Решение данного дифференциального уравнения будем искать в виде(2.17)
$$y=u\cdot v,$$
откуда получим(2.18)
$$y'=u'v+uv'$$
Подставляя выражения для y и $y'$ из (2.17) и (2.18) в данное уравнение, получаем
$$u'v+uv'+\frac{2uv}{x}=x.$$
Группируя в левой части первое и второе слагаемые и вынося общий множитель за скобки, получим(2.23)
$$\left[  u'+\frac{2u}{x}\right]v+uv'=x$$
Подберем функцию $u$ так, чтобы выражение в квадратных скобках было равно нулю, т. е.
$$u'+\frac{2u}{x}=0$$
Решаем полученное уравнение с разделяющимися переменными и находим функцию $u$ , как его некоторое ненулевое решение:
$$\frac{du}{dx}=-\frac{2u}{x},$$
или, после разделения переменных,
$$\frac{du}{dx}=-\frac{2u}{x}, u \neq 0$$
Интегрируя, находим
$$\int\frac{du}{dx}=-2\int\frac{u}{x},$$
$$ln|u|=-2in|x|+ln|c_0|,$$
или
$$u = \frac{1}{x^2}$$
Выбирая $c_0=1$, получаем(2.24)
$$u=\frac{1}{x^2}$$
Тогда, учитывая способ выбора функции $u(x)$ из уравнения (2.23) имеем дифференциальное уравнение для нахождения второй неизвестной функции $v(x)$:
$$uv'=x,$$
или, учитывая (2.24)
$$\frac{1}{x^2}v'=x,$$
которое является дифференциальным уравнением с разделяющимися переменными относительно другой неизвестной функции $v(x)$. Решая его, получаем
$$\frac{dv}{dx}= x^3,$$
или
$$dv=x^3dx.$$
Интегрируя последнее равенство, находим
$$\int dv=\int x^3dx,$$
или(2.25)
$$v=\frac{x^4}{4}+c,$$
где $c$ – произвольная постоянная.

Перемножая найденные выражения для функций $u(x)$ и $v(x)$, находим искомое решение
$$y=uv=\frac{1}{x^2}\cdot \left( \frac{x^4}{4}+c\right).$$
Таким образом, общее решение данного линейного уравнения имеет вид
$$y(x)=\frac{x^2}{4}+\frac{c}{x^2},$$
где $c$ – произвольная постоянная.

Используя заданное начальное условие, будем иметь
$$0=\frac{1}{4}=c,$$
откуда находим
$$c=-\frac{1}{4}.$$
Тогда искомое частное решение имеет вид
$$y=\frac{x^2}{4}+\frac{1}{4x^2}.$$
**_Ответ._** $y(x)=\frac{x^2}{4}+\frac{1}{4x^2}.$ – частное решение.

### II. Метод вариации произвольной постоянной (метод Лагранжа)

Этот метод заключается в следующем:
1) находят общее решение соответствующего линейного однородного уравнения, которое будет содержать произвольную постоянную $с$ ;
2) решение исходного неоднородного дифференциального уравнения следует искать в том же виде, что и решение соответствующего однородного уравнения, но заменив постоянную с на функцию $с(x)$. Отыскав ее, находят общее решение данного линейного неоднородного уравнения.

**_Пример 2._** Решить линейное дифференциальное уравнение
$$y' +y\ cos\ x=e^{-sin\ x}.$$
**_Решение._**
1) Решаем соответствующее однородное уравнение:
$$y'+y\ cos \ x=0.$$
Это уравнение с разделяющимися переменными. Заменяя $y'$ на $\frac{dy}{dx}$ и разделяя переменные, получим
$$\frac{dy}{dx}=-y\ cos\ x,$$
или
$$\frac{dy}{y}=-cos \ x\  dx.$$
После интегрирования имеем
$$\int \frac{dy}{y}=-\int cos \ x\  dx,$$
откуда находим
$$ln|y|= - sin \ x + c_0,$$
или
$$y=e^{-sin \ x+c_0}.$$
Полагая $e^{c_0}=c$ , получаем общее решение соответствующего однородного уравнения в виде(*):
$$y=c \cdot e^{-sin \ x},$$
где $c$ – произвольная постоянная.
2) Решение исходного неоднородного дифференциального уравнения будем искать в том же виде, что и решение ( ∗ ) соответствующего однородного дифференциального уравнения, только заменяя постоянную c на функцию $c(x)$(2.26):
$$y=c(x) \cdot e^{-sin \ x}$$
Продифференцируем равенство ( 2.26) по $x$ (2.27):
$$y'=c'(x)e^{-sin \ x}-c(x) \cdot cos \ x \cdot e^{-sin \ x}$$
Подставив в исходное уравнение выражения (2.26) и (2.27)  вместо $y$ и $y'$ будем иметь:
$$c'(x)e^{-sin \ x}-c(x) \cdot cos \ x \cdot e^{-sin \ x}+c(x) \cdot cos \ x \cdot e^{-sin \ x} = e^{-sin \ x}.$$
Преобразуя полученное равенство, получаем
$$c'(x)=1,$$
или
$$\frac{dc}{dx}=1,$$
$$dc=dx,$$
откуда, после интегрирования, находим
$$\int dc=\int dx,$$
или
$$c(x)=c+c_0,$$
где $c_0$ – произвольная постоянная.

Подставляя найденное выражение для $c(x)$ в (2.26), получим общее решение исходного дифференциального уравнения
$$y=(x+c_0) \cdot e^{-sin \ x}.$$
**_Ответ:_** $y(x)=(x+c_0) \cdot e^{-sin \ x}.$ где $c_0$ – произвольная постоянная.

**_Пример._** Рассмотрим уравнение
$$y=(2x+y^3)y',$$
в котором y является функцией от $x$ . Оно не является линейным относительно $y$ .
Учитывая, что $y'=\frac{1}{x'}$, будем иметь уравнение
$$y=(2x+y3) \cdot \frac{1}{x'},$$
или
$$x'-\frac{2x}{y}=y^2,$$
которое является линейным относительно переменной $x$ , т. е. здесь $x=x(y)$ – искомая функция, $y$ – независимая переменная.

**_Определение 2._** Уравнением Я. Бернулли называется обыкновенное дифференциальное уравнение первого порядка, которое можно записать в виде(2.28):
$$y'+p(x) \cdot y=f(x) \cdot y'',\; (n \neq 0,1)$$
где $y = y(x)$ – неизвестная функция независимого переменного аргумента $x$ , $p(x)$, $f(x)$ – известные функции, коэффициенты уравнения, $y^n=[y(x)]^n$ – $n$ -я степень неизвестной функции $y(x)$.

Существует несколько способов решения уравнения Я. Бернулли. Один из них состоит в том, что если записать уравнение (2.28.) в виде
$$y^{-n} \cdot y' + p(x) \cdot y^{1-n}=f(x), \; y \neq 0,$$
то с помощью замены $z=y^{1-n}$ , где $z=z(x)$ – новая неизвестная функция, уравнение (2.29) приводится к линейному дифференциальному уравнению первого порядка, которое можно решить любым из вышеизложенных способов.

Однако, решение уравнения Я. Бернулли (2.28.) удобней искать методом И. Бернулли, т. е. в виде
$$y=u \cdot v,$$
не приводя его к линейному уравнению.

**_Пример 3._** Решить уравнение
$$y' + 2y = e^x \cdot y^2.$$
Данное уравнение является уравнением Я. Бернулли $(n = 2)$ . Решим его по методу И. Бернулли, т. е. решение будем искать в виде произведения двух функций:
$$y=u \cdot v,$$
где $u=u(x), v=v(x)$ , – новые неизвестные функции.
Найдем:
$$y'=u' \cdot v + u \cdot v'.$$
Подставим в исходное уравнение вместо y и $y'$ их выражения через $u$ и $v$ , получим
$$u' \cdot v + u \cdot v' + 2u \cdot v = e^x \cdot u^2 \cdot v^2,$$
или, после группировки слагаемых в левой части полученного равенства и вынесения общего множителя за скобки, будем иметь(2.30):
$$u' \cdot v + u \cdot [v'+2v]=e^x \cdot u^2 \cdot v^2,$$
Функцию $v(x)$ найдем как некоторое частное решение уравнения
$$v'+2v=0$$
Это уравнение с разделяющимися переменными. Разделяя переменные и интегрируя затем обе части, получим
$$\frac{dv}{dx}=-2v,$$
или
$$\int\frac{dv}{dx}=-\int2v,$$
$$ln|v|=-2x+c_0,$$
$$v=e^{-2x+c_0}.$$
Полагая $c_0=0$, получим(2.31):
$$c=e^{-2x}$$
При таком выборе функции $v(x)$ из уравнения (2.30) будем иметь следующее уравнение относительно второй неизвестной функции $u(x)$:
$$u' \cdot e^{-2x}=e^x \cdot u^2 \cdot (e^{-2x})^2,$$
или, после несложных преобразований, получим уравнение(2.32)
$$u' = e^{-x} \cdot u^2,$$
которое является уравнением с разделяющимися переменными. Разделим переменные
$$\frac{du}{dx}=e^{-x} \cdot u^2,$$
или
$$\frac{du}{u^2} = e^{-x} \cdot  dx.$$
Проинтегрируем обе части
$$\int\frac{du}{u^2} = \int e^{-x} \cdot  dx,$$
$$-\frac{1}{u}=-e^{-x}+c,$$
где $c$ – произвольная постоянная,
или
$$\frac{1}{u}=e^{-x}-c,$$
откуда находим(2.33)
$$u(x)=\frac{1}{e^{-x}-c}$$
Заметим, что, кроме полученного общего решения (2.33) уравнению (2.32) удовлетворяет функция $u = 0$, которая не может быть получена из формулы (2.33) ни при каком произвольном значении постоянной $c$ .

Таким образом, решения исходного уравнения таковы:
1) при $u=0, \ v=e^{-2x}, \ y=0.$
2) при $u(x)=\frac{1}{e^{-x}-c}, \ v=e^{-2x}, \ y=\frac{e^{-2x}}{e^{-x}-c}$

**_Ответ:_** $y(x)=\frac{e^{-2x}}{e^{-x}-c}$ – общее решение, где $c$ – произвольная постоянная, $y = 0$.