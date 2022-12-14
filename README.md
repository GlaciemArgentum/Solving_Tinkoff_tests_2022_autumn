# Solving_Tinkoff_tests

На данном репозитории представлены решение теста на стажировку в Тинькофф. 

На данный момент загружены только те решения заданий, которые были отправлены на проверку.
В будущем планируется дорешать некоторые или все задачи.

Условия задач в том виде, *в котором они были представлены на онлайн тесте*, расположены ниже. Также они будут находится в папках с каждой задачей:

## 1 задание

***Ограничение времени***: 1 секунда.  
***Ограничение памяти***: 256 МБ.

Ксюша недавно устроилась работать в Тинькофф. В качестве первого задания ей поручили выбрать цвета для названия нового отдела. Ксюша уже решила, что покрасит его в два цвета — желтый и черный, осталось только раскрасить.
Название отдела представляет из себя строку $s$, состоящую из нескольких слов, разделенных пробелами. Каждое слово состоит из латинских букв, суммарно в названии их ровно $n$.
Ксюша уже придумала, в какие цвета покрасит каждую букву, но хочет, чтобы раскраска получилась наиболее красивой. Слово считается *некрасивым*, если в нем есть соседние буквы, покрашенные в один цвет.
Ксюша хочет узнать, сколько слов в названии отдела окажутся *некрасивыми*, если раскрашивать их в соответствии с ее идеей. Пожалуйста, помогите ей сосчитать.

**Формат входных данных**  
В первой строке вводится число $n$ $(1 ⩽ n ⩽ 100)$ — количество букв в названии отдела.
Во второй строке вводится само название — строка $s$ $(1 ⩽ |s| ⩽ 100)$, состоящая из латинских букв и пробелов. Гарантируется, что между любыми двумя буквами не более одного пробела, строка начинается и заканчивается буквой, а также содержит ровно $n$ букв.
Втретьей строке вводится строка $b$ длины $n$, состоящая из букв $Y$ и $B$ — Ксюшина идея раскраски названия. Если $b_{i} = Y$, то $i$-ая по счету буква названия должна быть покрашена в желтый цвет; если
же $b_{i} = B$, то $i$-ая буква должна быть покрашена в черный цвет.

**Формат выходных данных**  
В единственной строке выведите число — количество некрасивых слов в раскрашенном названии отдела.

**Пример 1**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 7                             | 0                  |
| Tinkoff                       |                    |
| BYBYBYB                       |                    |

**Пример 2**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 27                            | 3                  |
| Algorithms and Data Structures|                    |
| BBBBBBBBBBBYBYYYYBBBBBBBBBВ   |                    |

## 2 задание

***Ограничение времени***: 1 секунда.  
***Ограничение памяти***: 256 МБ.

Ксюша раскрасила названия, теперь ей нужно придумать новые курсы валют.
Всем известно, что существуют только три валюты: $A$, $B$ и $C$, — и каждая из них имеет свою ценность: $a$, $b$ и $c$ соответственно. По идее Ксюши банк будет предоставлять клиентам возможность обменивать одну валюту на другую: а именно, если клиент хочет обменять валюту $A$ на валюту $B$, он сможет отдать ровно $a$ единиц валюты $A$ и получить взамен ровно $b$ единиц валюты $B$. Аналогично происходит обмен между другими валютными парами.  
У Ксюши на счету сейчас $x$, $y$ и $z$ единиц в валютах $A$, $B$ и $C$ соответственно. Она хочет узнать, сколько различных троек значений $(x, y, z)$ своего баланса она может получить, совершив некоторое количество обменов (возможно, 0). Для этого она просит вашей помощи.

**Формат входных данных**  
В первой строке вводятся три целых числа $a$, $b$ и $c$ $(1 ⩽ a, b, c ⩽ 10^9)$ — ценности валют. Во второй строке вводятся три целых числа $x$, $y$ и $z$ $(0 ⩽ x, y, z ⩽ 10^9)$ — суммы насчету у Ксюши в каждой валюте.

**Формат выходных данных**  
В единственной строке выведите целое число — количество различных троек значений, которые Ксюша может получить путем обменных операций.

**Пример 1**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 111                           | 10                 |
| 102                           |                    |

**Пример 2**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 123                           | 28                 |
| 354                           |                    |

## 3 задание

***Ограничение времени***: 1 секунда.  
***Ограничение памяти***: 256 МБ.

Для новой маркетинговой акции Ксюша придумала провести математическую лотерею. Она загадала натуральное число $n$ и напечатала на билетах пары положительных чисел $a$, $b$ такие, что $a + b = n$. Победителем лотереи будет считаться участник, получивший билет с минимальным наименьшим общим кратным (НОК) чисел $a$ и $b$.  
Ксюша хочет заранее понять, какие подходящие числа $a$ и $b$ можно выбрать, чтобы их НОК было минимально возможным. Поможете ей?

**Формат входных данных**  
В единственной строке вводится натуральное число $n$ $(2 ⩽ n ⩽ 10^9)$ — загаданное Ксюшей число $n$.

**Формат выходных данных**  
Выведите через пробел два числа $a$ и $b$ — искомую пару с минимальным НОК. Если подходящих ответов несколько, выведите любой.

**Пример 1**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 3                             | 1 2                |

**Пример 2**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 6                             | 3 3                |

**Пример 3**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 9                             | 3 6                |

## 4 задание

***Ограничение времени***: 1 секунда.  
***Ограничение памяти***: 256 МБ.

Ксюша решила попробовать себя в дизайне, поэтому теперь она разрабатывает флаг Тинькофф. Ксюша любит современное искусство, поэтому новый флаг Тинькофф будет не прямоугольником, а самым настоящим правильным $n$-угольником с длиной стороны 1. Помимо $n$-угольников Ксюше нравятся треугольники, которыми она хочет заполнить флаг. Эти треугольники при этом должны иметь вершины, совпадающие с вершинами $n$-угольника, а также не иметь общих между собой точек, в том числе вершин.  
Ксюша хочет покрыть треугольниками как можно большую часть нового флага, чтобы он не выглядел слишком пустым. Пожалуйста, посчитайте, какую максимальную площадь $n$-угольника она сможет заполнить.

**Формат входных данных**  
В единственной строке вводится целое число $n$ $(3 ⩽ n ⩽ 500)$ — число вершин $n$-угольника.

**Формат выходных данных**  
Выведите одно вещественное число — максимальную суммарную площадь, которую можно покрыть
треугольниками. Ответ будет считаться верным, если его абсолютная или относительная
погрешность не более $10^{-6}$.

**Пример 1**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 3                             | 0.433013           |

**Пример 2**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 10                            | 3.553212           |

## 5 задание

***Ограничение времени***: 2 секунда.  
***Ограничение памяти***: 256 МБ.

Благодаря стараниям Ксюши развитие Тинькофф ускорилось, а сама она стала руководителем команды! Теперь она хочет проверить, как чувствуют себя ее коллеги.  
Команда Ксюши распределена на $n$ городов, поэтому необходимо придумать маршрут их посещения. Всего существует $m$ междугородних рейсов, которыми Ксюша может воспользоваться. $i$-ый рейс ведет из города $u_{i}$ в город $v_{i}$, причем $u_{i} < v_{i}$. Все рейсы односторонние, при этом никаких других ограничений нет: между любой парой городов может существовать любое число рейсов (но все в одном направлении). Для каждого рейса известна его чётность. По чётному рейсу можно путешествовать только в чётные дни и наоборот. Можно считать, что дни нумеруются натуральными числами до бесконечность.  
Ксюша начинает поездку в городе под номером 1 и заканчивает в городе под номером $n$, путешествуя между городами только по разрешённым рейсам в дни с нужной чётностью. Для каждого города известно, что аэропорт в нем работает либо только в чётные дни, либо только в нечётные. Например, если из города $u$ разрешены только чётные рейсы в город $v$, а аэропорт в $u$ работает только по нечётным дням, то попасть из $u$ в $v$ напрямую не получится. Для командировки Ксюша выберет кратчайший по числу перелётов маршрут.  
Коля, директор Тинькофф Центра Разработки в городе $n$, хочет подготовить сюрприз к приезду Ксюши, но никак не успевает. Он хочет задержать Ксюшу, чтобы она приехала как можно позже, т.е. совершила максимально возможное число перелетов. Для этого перед началом Ксюшиной командировки он позвонит начальникам каждого аэропорта городов с номерами от 1 до $n$ с просьбой работать только в дни с нужной четностью. Помогите Коле подготовить хороший сюрприз для Ксюши и составить расписание работы аэропортов.

**Формат входных данных**  
В первой строке вводятся целые числа $n$ и $m$ $(1 ⩽ n ⩽ 5 \cdot 10^5,$ $0 ⩽ m ⩽ 5 \cdot 10^5)$ — количество городов и рейсов соответственно.  
В следующих m строках содержится описание рейсов. В $i$-ой строке записаны три целых числа $u_{i}$, $v_{i}$ и $t_i$ $(1 ⩽ u_{i}, v_{i} ⩽ n, t_{i}$ $∈$ {0, 1}) — номера городов, соединяемых $i$-ым рейсом, и его чётность (0 — чётный рейс, 1 — нечётный).

**Формат выходных данных**  
В первой строке выведите число $d$ — максимальную длину кратчайшего маршрута Ксюши, которой может добиться Коля, либо $-1$, если Коля может построить расписание работы аэропортов, чтобы Ксюша не доехала до города $n$.  Во второй строке выведите набор из 0 и 1 без пробелов — расписание работы аэропортов.

**Пример 1**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 3 3                           | -1                 |
| 1 2 0                         | 011                |
| 1 3 1                         |                    |
| 2 3 0                         |                    |

**Пример 2**
| Ввод                          | Вывод              |
|:------------------------------|:-------------------|
| 4 6                           | 3                  |
| 1 3 0                         | 1111               |
| 3 4 0                         |                    |
| 3 4 1                         |                    |
| 1 2 1                         |                    |
| 2 3 1                         |                    |
| 2 4 0                         |                    |