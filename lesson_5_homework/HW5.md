## 1. Напишите программу, которая проверяет последнюю цифру числа.Если последняя цифра числа 3, то вывести True иначе вывести False.

- Код 
```python
number = int(input("Введите число: "))

def check_last_digit(number):
    if str(number)[-1] == "3":
        return True
    else:
        return False
result = check_last_digit(number)
print (result)
```
- Результат выполнения кода 
```console
Введите число: 23
True
Введите число: 16
False
```
## 2. Напишите программу, которая выводит True, если хотя бы одно из чисел number_1, number_2, number_3 отрицательно. Если нет вывести False. Числа вводятся с клавиатуры в одной строке.

- Код 
```python
number_1 = int(input("Введите число: "))
number_2 = int(input("Введите число: "))
number_3 = int(input("Введите число: "))
if number_1 < 0 or number_2 < 0 or number_3 < 0:
    print (True)
else:
    print (False)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: -3
Введите число: 2
True
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: 2
Введите число: 3
False
```
## 3. Верно ли что, целые number_1, number_2 имеют одинаковую четность. 

- Код 
```python
number_1 = int(input("Введите число: "))
number_2 = int(input("Введите число: "))

if number_1 % 2 == number_2 % 2:
    print (True)
else:
    print (False)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 2
Введите число: 2
True
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 4
Введите число: 5
False
```
## 4. Даны три стороны треугольника side_a, side_b, side_c. Выведите equilateral если треугольник равносторонний, isosceles если равнобедренный и scalene если разносторонний

- Код 
```python
side_a = int(input("Введите число: "))
side_b = int(input("Введите число: "))
side_c = int(input("Введите число: "))

if side_a == side_b == side_c:
    print ("equilateral")
elif side_a == side_b != side_c:
    print ("isosceles")
elif side_a != side_b == side_c:
    print ("isosceles")
elif side_a == side_c != side_b: 
    print ("isosceles")
elif side_a != side_b != side_c :
    print ("scalene")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 2
Введите число: 2
Введите число: 1
isosceles
PS C:\git\tms-py61>
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: 2
Введите число: 3
scalene
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: 1
Введите число: 1
equilateral
```
## 5. Найти количество четных чисел среди заданных трех целых чисел. В ответе вывести количество четных чисел.


- Код 
```python
number_a = int(input("Введите число: "))
number_b = int(input("Введите число: "))
number_c = int(input("Введите число: "))

count = 0

if number_a % 2 == 0:
    count = count + 1
if number_b % 2 == 0:
    count = count + 1
if number_c % 2 == 0:
    count = count + 1

print (f"Количество чётных чисел: {count}")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: 2
Введите число: 3
Количество чётных чисел: 1
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите число: 1
Введите число: 1
Введите число: 1
Количество чётных чисел: 0
```

## 6. Дано двузначное число. Определить является ли сумма его цифр двузначным числом. 


- Код 
```python
number = int(input("Введите двузначное число: "))

if number > 99 or number < 9:
    print ("Вы ввели не двузначное число") 
elif (number % 10 + number / 10) > 99 or (number % 10 + number / 10) < 9 :
    print ("Сумма цифр введённого числа не является двузначным числом")
else:
    print ("Сумма цифр введённого числа является двузначным числом")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите двузначное число: 1
Вы ввели не двузначное число
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите двузначное число: 12
Сумма цифр введённого числа не является двузначным числом
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите двузначное число: 88
Сумма цифр введённого числа является двузначным числом
```

## 7. Дано четырёхзначное число. Проверить, одинаковы ли все цифры в нём. 


- Код 
```python
number = list(map(int, input("Введите четырёхзначное число: ")))

if len(number) != 4:
    print ("Вы ввели не четырёхзначное число")
elif number[0] == number[1] == number[2] == number[3]:
    print ("Все цифры в числе равны")
else:
    print ("Цифры в числе не равны")  
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите четырёхзначное число: 12345
Вы ввели не четырёхзначное число
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите четырёхзначное число: 1
Вы ввели не четырёхзначное число
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите четырёхзначное число: 1234
Цифры в числе не равны
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите четырёхзначное число: 1111
Все цифры в числе равны
```

## 8. Напишите программу, принимающую на вход год и выводящую "Високосный", если в этом году действительно 366 дней, и "Не високосный" иначе. Год считается високосным, если его номер делится на 4, но не делится на 100 или же делится на 400

- Код 
```python
year = int(input("Введите год: "))
if year % 4 == 0 and year % 100 != 0 or year % 400 == 0:
    print ("Год високосный")
else:
    print ("Год не високосный")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите год: 2024
Год високосный
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите год: 2025
Год не високосный
```
## 9. Вывести на экран число "10" 20 раз столбиком.
- Код 
```python
number = 10
for _ in range (20):
    print (number)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
10
```

## 10. Даны два числа start и stop. Составить программу вывода на экран всех чисел от start до stop.
- Код 
```python
start = int(input("Введите первое число:"))
stop = int(input("Введите последнее число:"))

for i in range (start, stop + 1):
    print (i)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите первое число:1
Введите последнее число:5
1
2
3
4
5
```

## 11. Выведите на экран в одну строку числа от 100 до  -100 включительно.
- Код 
```python
for i in range (100, -100, -1):
    print (i, end=" ")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
100 99 98 97 96 95 94 93 92 91 90 89 88 87 86 85 84 83 82 81 80 79 78 77 76 75 74 73 72 71 70 69 68 67 66 65 64 63 62 61 60 59 58 57 56 55 54 53 52 51 50 49 48 47 46 45 44 43 42 41 40 39 38 37 36 35 34 33 32 31 30 29 28 27 26 25 24 23 22 21 20 19 18 17 16 15 14 13 12 11 10 9 8 7 6 5 4 3 2 1 0 -1 -2 -3 -4 -5 -6 -7 -8 -9 -10 -11 -12 -13 -14 -15 -16 -17 -18 -19 -20 -21 -22 -23 -24 -25 -26 -27 -28 -29 -30 -31 -32 -33 -34 -35 -36 -37 -38 -39 -40 -41 -42 -43 -44 -45 -46 -47 -48 -49 -50 -51 -52 -53 -54 -55 -56 -57 -58 -59 -60 -61 -62 -63 -64 -65 -66 -67 -68 -69 -70 -71 -72 -73 -74 -75 -76 -77 -78 -79 -80 -81 -82 -83 -84 -85 -86 -87 -88 -89 -90 -91 -92 -93 -94 -95 -96 -97 -98 -99
```
## 12. Найти сумму всех целых чисел от 100 до 500 включительно.
- Код 
```python
sum = 0
for i in range (100, 500 + 1):
    sum = sum + i
print (sum)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
120300
```
## 13. Найти произведение всех целых чисел от 5 до 20 включительно.
- Код 
```python
multiplication = 1
for i in range (5, 20 + 1):
    multiplication = multiplication * i
print (multiplication)
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
101370917007360000
```
## 14. Дано натуральное число n. Вывести на экран факториал этого числа. Например: 5! = 1 * 2 * 3 * 4 * 5 = 120

- Код 
```python
number = int(input("Введите натуральное число: "))

if number < 0:
    print("Значение не может быть отрицательным")
elif number == 0:
    print("Факториал равен: 1")
else:
    factorial = 1
    for i in range(1, number + 1):
        factorial *= i
    print(f"Факториал равен: {factorial}")
```
- Результат выполнения кода 
```console
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите натуральное число: -1
Значение не может быть отрицательным
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите натуральное число: 0
Факториал равен: 1
PS C:\git\tms-py61> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/git/tms-py61/lesson_5_homework/main.py
Введите натуральное число: 23
Факториал равен: 25852016738884976640000
```