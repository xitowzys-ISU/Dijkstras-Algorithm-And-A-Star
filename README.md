**Задание следует решить двумя способами:**

+ используя алгоритм Дейкстры
+ используя алгоритм А*

**Источник: задачи олимпиады НТИ, 2016, 1 этап, трек "Автономные робототехнические системы"**

# Перевозка груза

Полигон N на M метров разбит на клетки со стороной равной одному метру. Для каждой клетки полигона нам известна средняя высота, выраженная в сантиметрах. В центре одной из клеток стоит робот, который может двигаться только из центра одной клетки в центр другой, и только в том случае, если эти клетки имеют общую сторону. Еще одно ограничение, которое наложено конструкцией робота — невозможность перемещаться между клетками, если их средние высоты отличаются более, чем на 100 сантиметров.

Также нам интересны на этом полигоне две другие клетки — в одной из них лежит груз, в другую должен прибыть робот после того, как заберет груз. Для того чтобы забрать груз, роботу нужно просто заехать в клетку, в которой он находится.

Какой минимальный путь должен пройти робот, чтобы попасть из начальной клетки в конечную, забрав перед этим груз? Груз не влияет на движение робота. Гарантируется, что искомый путь существует.

**Формат входных данных:**

В первой строке даны два натуральных числа N и M, разделенных пробелом — размеры полигона (1 = N, M = 300). В следующих N строках даны по M целых неотрицательных чисел, разделенных пробелами, — средние высоты ячеек, выраженные в сантиметрах. Высоты ячеек не превышают 10 000 000.

В следующей строке дано начальное положение робота — два целых числа, разделенные пробелом. Первое число задает строку, второе — номер клетки в строке. Строки нумеруются начиная с 00 и заканчивая N-1, а клетки в строках — от 00 до M-1. В двух следующих строках в аналогичном формате описываются положение груза и конечная клетка.

**Пример ввода:**
```python
2 3
0 1000 0
0 0 0
0 0
0 2
1 1
```
**Формат выходных данных:**

Выведите единственное целое число — расстояние в метрах, которое необходимо проехать роботу, чтобы доставить груз в конечную клетку.

**Пример вывода:**
```python
6
```
