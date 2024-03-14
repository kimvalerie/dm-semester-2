# dm-semester-2

## Определения

1. [Инцидентность вершин и ребер](#инцидентность-вершин-и-ребер)
2. [Смежность вершин и ребер](#смежность-вершин-и-ребер)
3. [Изолированная вершина](#изолированная-вершина)
4. [Висячая вершина](#висячая-вершина)
5. [Мультиграф](#мультиграф)
6. [Псевдограф](#псевдограф)
7. [Матрица смежности](#матрица-смежности)
8. [Матрица инцедентности](#матрица-инцедентности)
9. [Кратные дуги](#кратные-дуги)
10. [Симметричные дуги](#симметричные-дуги)
11. [Направленный граф](#направленный-граф)
12. [Лемма о рукопожатиях](#лемма-о-рукопожатиях)
13. [Подграф и надграф](#подграф-и-надграф)
14. [Частичный граф](#частичный-граф)
15. [Объединение и пересечение графов](#объединение-и-пересечение-графов)
16. [Подразбиение ребра](#подразбиение-ребра)
17. [Отождествление вершин](#отождествление-вершин)
18. [Стягивание ребра](#стягивание-ребра)
19. [Регулярный граф, степень регулярности](#регулярный-граф-степень-регулярности)
20. [Хроматическое число](#хроматическое-число)
21. [Клика, кликовое число](#клика-кликовое-число)
22. [Изоморфизм графов](#изоморфизм-графов)
23. [Путь и замкнутый путь](#путь-и-замкнутый-путь)
24. [Цепь и цикл](#цепь-и-цикл)
25. [Простая цепь и простой цикл](#простая-цепь-и-простой-цикл)
26. [Связность (достижимость) вершин, компонента связности](#связность-достижимость-вершин-компонента-связности)
27. [Сильная связность вершин, компонента сильной связности](#сильная-связность-вершин-компонента-сильной-связности)
28. [Описание кратных ребер в матрице смежности и матрице инцидентности](#описание-кратных-ребер-в-матрице-смежности-и-матрице-инцидентности)
29. [Дополнение графа](#дополнение-графа)
30. [Двудольный граф](#двудольный-граф)
31. [Реберная двусвязность](#реберная-двусвязность)
32. [Мост](#мост)
33. [Вершинная двусвязность](#вершинная-двусвязность)
34. [Точка сочленения](#точка-сочленения)
35. [Блок](#блок)
36. [Лемма о цикле и мосте](#лемма-о-цикле-и-мосте)
37. [Разрезающее множество и разрез](#разрезающее-множество-и-разрез)
38. [Гомеоморфизм графов](#гомеоморфизм-графов)
39. [Дерево](#дерево)
40. [Эксцентриситет](#эксцентриситет)
41. [Радиус](#радиус)
42. [Диаметр](#диаметр)
43. [Центр](#центр)
44. [Граф блоков и точек сочленения](#граф-блоков-и-точек-сочленения)
45. [Граф компонент реберной двусвязности](#граф-компонент-реберной-двусвязности)
46. [Остов графа](#остов-графа)
47. [Фундаментальная система циклов](#фундаментальная-система-циклов)
48. [Безопасное ребро](#безопасное-ребро)
49. [⟨S, T⟩ разрез](#⟨s-t⟩-разрез)

## Инцидентность вершин и ребер

> *x* — ребро с концами *u* и *v*, *{u, v}*, тогда *x* инцидентно *u* и *v*, *u* и *v* инцидентны *x*

## Смежность вершин и ребер

> вершины *u* и *v* называются смежными, если являются концами
одного ребра

> ребра *x* и *y* называются смежными, если имеют общую вершину

## Изолированная вершина

> Изолированная вершина — вершина
без петель также не являющаяся концом ни одного из ребер

## Висячая вершина

> Висячая вершина — вершина, в которую вдет только одно ребро, которое в свою очередь также называется висячим

## Мультиграф

> Мультиграф — граф с
параллельными ребрами

## Псевдограф

Псевдограф — граф, который может содержать:

* петли
* и/или параллельные ребра

## Матрица смежности

Матрица смежности — матрица A [V x V] , в которой в ячейке a_ij записано

* (неориентир.): число ребер, соединяющих вершины V_i и V_j.

* (ориентир.): a_ij = 1, если из V_i в V_j идет дуга, иначе 0

## Матрица инцедентности

> Матрица инцидентности (для **неориентированного** графа) — матрица A размера |V|x|E|, для которой a_ij = 1, если вершина v_i инцидентна ребру e_j, иначе a_ij = 0

> Матрица инцидентности (для **ориентированного** графа) — матрица A размера |V|x|E|, для которой a_ij = 1, если вершина v_i начало дуги e_j, a_ij = -1, если вершина v_i конец дуги e_j, иначе a_ij = 0

## Кратные дуги

> Несколько дуг с совпадающими начальными и конечными вершинами.

## Симметричные дуги

> Дуги вида (*u*, *v*) и (*v*, *u*) в некотором графе.

*u*, *v* ∊ V(G)

(*u*, *v*), (*v*, *u*) ∊ E(G)

## Направленный граф

> Направленный граф — граф без
симметричных ориентированных
ребер (дуг).

## Лемма о рукопожатиях

Неориентированный граф:

> Сумма степеней всех вершин графа — четное число, равное удвоенному числу ребер графа.

> Следствие: произвольный граф содержит четное число вершин нечетной
степени.

Ориентированный граф:

> Сумма входящих и исходящих степеней всех вершин графа — четное число, равно удвоенному числу дуг графа.

## Подграф и надграф

> Граф G'(V', E') является **подграфом** G(V, E), если V' ⊆ V, E' ⊆ E. Таким образом каждая вершина или ребро подграфа являются вершиной или ребром исходного графа.

> **Надграф** — граф, полученный путем добавления
новых ребер и/или вершин в исходный граф.

## Частичный граф

> Частичный граф — состоящий из множества вершин исходного графа и подмножества множества ребер.

*Каждый граф частичен сам себе.*

## Объединение и пересечение графов

> Объединение графов G(V, E) и G'(V', E') — объединяет множества вершин и ребер этих графов

> Пересечение графов G(V, E) и G'(V', E') — пересекает множества вершин и ребер этих графов

## Подразбиение ребра

> Подразбиение ребра — операция, состоящая из удаления ребра *e_0* = (*u*, *v*) и добавления двух новых ребер *e_1* = (*u*, *q*), *e_2* = (*q*, *v*) где *q* — новая вершина степени 2.

## Отождествление вершин

> Если v и v' — вершины различных компонент графа G, то мы можем создать новый граф G' путём отождествления v и v' в G в новую вершину v в G'.

## Стягивание ребра

> Ребро *e* удаляется, а две его инцидентные вершины, *u* и *v*, сливаются в новую вершину *w*, где рёбра, инцидентные *w*, соответствуют рёбрам, инцидентным либо *u*, либо *v*. Ребро инцидентное *u* и *v* переходит в петлю на *w*.

*Частный случай отождествления вершин*

## Регулярный граф, степень регулярности

> Регулярный (однородный) граф — такой граф что степени всех его вершин равны.

> Cтепень регулярности — степень вершины регулярного графа.

## Хроматическое число

> Хроматическим числом графа называется минимальное число цветов, которыми можно раскрасить вершины графа так, что никакое ребро не будет иметь начало и конец одного цвета.

## Клика, кликовое число

> Кликой в неориентированном графе G = (V,E) называется подмножество вершин C ⊆ V, такое что для любых двух вершин в C существует ребро, их соединяющее. Эквивалентно утверждению, что подграф, порождённый 
C, является полным.

> Кликовое число графа — это число вершин в наибольшей клике графа.

## Изоморфизм графов

> Графы G и G' изоморфны — между их множествами вершин существует взаимно-однозначное
соответствие с сохранением смежности.

## Путь и замкнутый путь

> Путь — последовательность вида v_1, e_1, v_2, e_2, ... v_n, e_n, v_n+1 где e_i ∊ E, v_i ∊ V.

> Замкнутый путь — такой путь что его конец и начало совпадают (v_1 = v_n+1).

## Цепь и цикл

> Цепь — путь без повторяющихся ребер.

> Цикл — замкнутая цепь.

## Простая цепь и простой цикл

> Простая цепь — цепь без повторяющихся вершин (а следовательно и ребер).

> Простой цикл — замкнутая простая цепь *n* ≥ 3.

## Связность (достижимость) вершин, компонента связности

> Вершины *u* и *v* связаны, если в графе существует путь *u* --> *v*.

> Компонента связности это максимальный по включению связный подграф.

> Граф связен, если состоит из одной компоненты связности. В противном случае граф называется несвязным.

*Связность — отношение эквивалентности.*

## Сильная связность вершин, компонента сильной связности

> Сильная связность пары вершин — есть как путь u --> v, так и v --> u.

*Минимальная компонента сильной связности – вершина!*

## Описание кратных ребер в матрице смежности и матрице инцидентности

Матрица смежности:

> В **неориентированном** графе кратные ребра кратно увеличивают значения в симметричных ячейках **(i, j) и (j, i)**.

> Если i = j, то в **неориентированном**
графе петля учитывается **дважды**.

> Если i = j, то в **ориентированном**
графе петля учитывается **единожды**.

> В **ориентированном** графе кратные дуги кратно
увеличивают значение в ячейке **(i, j)**.

Матрица инцидентности:

**очев.** (см. определение)

## Дополнение графа

> Дополнение графа до полного — добавляет в исходный граф ребра до полного и удаляет ребра исходного.

## Двудольный граф

> Двудольный граф — это граф, множество вершин которого можно так разбить на два непересекающихся подмножества (доли) V_1 и V_2, что никакие две вершины из одной доли не смежны.

## Реберная двусвязность

> Вершины u и v графа G называются реберно двусвязными, если между ними существует два реберно непересекающихся пути.

## Мост

> Мост — ребро, при удалении которого, граф становится несвязным.

## Вершинная двусвязность

> Ребра графа являются вершинно двусвязными, если существуют два вершинно непересекающиеся
пути, соединяющие их концы.

## Точка сочленения

> Точка сочленения — вершина, при удалении которой, увеличивается
число компонент связности.

## Блок

> Блок — максимальный неразделимый подграф.

*Связный граф неразделим, если не содержит точек сочленения.*

## Лемма о цикле и мосте

> Ребро является мостом тогда и только тогда, когда оно не принадлежит ни одному циклу.

## Разрезающее множество и разрез

> Разрезающее множество — множество ребер графа, при удалении которых число компонент связности увеличивается.

> Разрез — минимальное по включению разрезающее множество графа.

## Гомеоморфизм графов

> Графы *G* и *G'* изоморфны если изоморфны некоторый *G_0*, являющийся подразбиением *G*, и, некоторый *G_0'*, являющийся подразбиением *G'*.

## Дерево

> Связный ациклический граф.

## Эксцентриситет

> Эксцентриситет *v* — расстояние до самой дальней от *v* вершины графа.

## Радиус

> Радиусом графа называется минимальный эксцентриситет среди всех его вершин.

## Диаметр

> Диаметром графа называется максимальный эксцентриситет среди всех вершин графа.

## Центр

> Вершина, эксцентриситет которой равен радиусу.

## Граф блоков и точек сочленения

> Двудольный граф, где одна доля — точки сочленения, другая — блоки, сжатые в виде вершин.

## Граф компонент реберной двусвязности

> Cвязный граф, где компоненты реберной двусвязности сжаты в виде вершин и соединяются мостами исходного графа.

## Остов графа

> Cвязный, ацикличный, частичный граф исходного графа.

> Минимальное остовное дерево графа G = (V, E) — это его ациклический связный подграф, в который входят все его вершины, обладающий минимальным суммарным весом ребер.

## Фундаментальная система циклов

> Множество циклов графа, ассоциированное с остовом (полученное путем поочередного добавления каждого ребра из множества удаленных ребер к остову).

## Безопасное ребро

*Пусть G' — подграф некоторого минимального остовного дерева графа G = (V, E).*

> Ребро (*u*, *v*) ∉ *G'* называется безопасным, если при добавлении его в *G'*, *G'* ∪ {(*u*, *v*)} также является подграфом некоторого минимального остовного дерева графа *G*.

## ⟨S, T⟩ разрез

Разрезом неориентированного графа *G* = (*V*, *E*) называется разбиение *V* на два непересекающихся подмножества: *S* и *T* = *V* ∖ *S*. Обозначается как ⟨*S*, *T*⟩.

Ребро (*u*, *v*) ∈ *E* пересекает разрез ⟨*S*, *T*⟩, если один из его концов принадлежит множеству *S*, а другой — множеству *T*.
