## 1. Напишите функцию minimum вычисляющую минимум двух чисел.

- Код 
```python
number_one = int(input("Введите первое число:"))
number_two = int(input("Введите первое число:"))

def minimum (value1, value2):
    return min(value1, value2)


print (f"Наименьшее число: {minimum(value1=number_one, value2=number_two)}")
```
- Результат выполнения кода 
```console
Введите первое число:357
Введите первое число:88
Наименьшее число: 88
```

## 2. Найдите минимальное из четырёх чисел с помощью функции написанной в предыдущей  задаче. Новую функцию не создавать! Использовать функцию из предыдущей задачи!

- Код 
```python
number_one = int(input("Введите первое число:"))
number_two = int(input("Введите первое число:"))
number_three = int(input("Введите первое число:"))
number_four = int(input("Введите первое число:"))

def minimum (value1, value2):
    return min(value1, value2)


print (f"Наименьшее число: {minimum(value1=minimum(value1=number_one, value2=number_two), value2=minimum(value1=number_three, value2=number_four))}")
```
- Результат выполнения кода 
```console
Введите первое число:77
Введите первое число:46
Введите первое число:11
Введите первое число:83
Наименьшее число: 11
```

## 3. Даны четыре действительных числа: x1, y1, x2, y2. Напишите функцию distance(x1, y1, x2, y2), вычисляющую расстояние между точкой (x1, y1) и (x2, y2). Считайте четыре действительных числа и выведите результат работы этой функции.

- Код 
```python
from math import sqrt

def distance(x1, y1, x2, y2):
    return sqrt((x2-x1) ** 2 + (y2-y1) ** 2)

coordinate_x1 = float(input("Введите первое число:"))
coordinate_x2 = float(input("Введите первое число:"))
coordinate_y1 = float(input("Введите первое число:"))
coordinate_y2 = float(input("Введите первое число:"))

print (f"Длина отрезка равна: {distance(x1=coordinate_x1, x2=coordinate_x2, y1=coordinate_y1, y2=coordinate_y2)}")
```
- Результат выполнения кода 
```console
Введите первое число:10
Введите первое число:15
Введите первое число:24
Введите первое число:23
Длина отрезка равна: 5.0990195135927845
```