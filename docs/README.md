# Документация по библиотеке
Geometric lib это библиотека помогающая находить периметр и площадь некоторых фигур.
Данное решение работает с 4 фигурами: треугольник, квадрат, прямоугольник и окружность.
## square.py

Работа с квадратом

- def area(a)

Данная функция принимает на вход значение стороны квадрата и возвращает его площадь

Формула:

S = a²

Пример вызова:

area(2)

Возвращаемое значение:

4

- def perimeter(a)

Данная функция принимает на вход значение стороны квадрата и возвращает его периметр

Формула:

P = 4a

Пример вызова:

perimeter(2)

Возвращаемое значение:

8

## circle.py

Работа с окружностью

- def area(r)

Данная функция принимает на вход значение радиуса окружности и возвращает её площадь

Формула:

S = πR²

Пример вызова:

area(2)

Возвращаемое значение:

12.56...

- def perimeter(a)

Данная функция принимает на вход значение радиуса окружности и возвращает длину окружности

Формула:

P = 2πR

Пример вызова:

perimeter(2)

Возвращаемое значение:

12.56...

## triangle.py

Работа с треугольником

- def existing(a, b, c)

Данная функция принимает три значения, длины сторон треугольника, и возвращает true, если треугольник существует, false в противном случае

Правило:

Для каждой суммы двух сторон верно неравенство: a + b > c

Пример вызова:

existing(1, 1, 1)

Возвращаемое значение:

true

- def area(a, b, c)

Данная функция принимает три значения, длины сторон треугольника, и если треугольник с данными сторонами существует, то функция возвращает его площадь, иначе -1

Формула:

S = (p * (p - a) * (p - b) * (p - c)) ** 0.5

Пример вызова:

area(3, 4, 5)

Возвращаемое значение:

8

- def perimeter(a, b, c)

Данная функция принимает три значения, длины сторон треугольника, и если треугольник с данными сторонами существует, то функция возвращает его периметр, иначе -1

Формула:

P = a + b + c

Пример вызова:

perimeter(1, 1, 1)

Возвращаемое значение:

3

## Rectangle.py


Работа с прямоугольником

- def area(a, b)

Данная функция принимает на вход значения сторон прямоугольником и возвращает его площадь

Формула:

S = a * b

Пример вызова:

area(2, 3)

Возвращаемое значение:

6

- def perimeter(a, b)

Данная функция принимает на вход значения сторон прямоугольником и возвращает его периметр

Формула:

P = 2 * (a + b)

Пример вызова:

perimeter(2, 3)

Возвращаемое значение:

10

## Unit тесты
Для каждой функции написаны unit тесты, проверяющие правильность работы.

Полное прохождение тестов показывает, что каждая функция:

-Правильно считает площадь/периметр

-Способна работать с большими числами

-Правильно обрабатывает отрицательные числа

-Правильно обрабтывает нестандартные входные данные

Для запуска тестов, нужно в терминале написать следующую команду:

python.exe -m unittest "название тестируемого файла".py

## История изменений библиотеки

- 8ba9aeb3cea847b63a91ac378a2a6db758682460 Circle and square added

- d078c8d9ee6155f3cb0e577d28d337b791de28e2 Docs added

- c62e24f728a67ff5de3fc0b71ba9425999f2ee7b first commit, adding new file

- 82b42442900d5dee1dcb26c9d978334c39ac1755 Исправление ошибки в файле commit_n_2

- 48df452123d7fc27a9ca65e7abf0f2916847e453 удалени ненужных файлов

- 8f58de7fe025e0c3be5e174e3331453aef2a9506 добавлен файл rectangle

- 3a237f44fcbcb83e43a96f255decab597d05576e Добавление файла triangle.py, с подробными комментариями

- 34583af5bef6db14098f807e27600b72f8ac422d Добавление подробных коментариев в файлы circle.py, Rectangle.py, square.py

- 76fe54662b88e6d94503a65c673526608a2aeb7f Добавлены unit тесты
