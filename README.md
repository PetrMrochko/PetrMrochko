TASK01

a = 90

b = 5

value = a + b

print(value)

value = "Такой ответ"

print(value)

TASK02

time_in_second = int(input("Введите время в секундах >>> "))

import datetime

sec = time_in_second

res = datetime.timedelta(seconds =sec)

print(res)

TASK03

shislo_N = input('Введите число >>> ')

if shislo_N.isdigit():

    print(sum([int(shislo_N * i) for i in range(1, 4)]))
else:
    print('Entered wrong value. Bye.')
    
    quit()
    
    TASK04
number = int(input("Введите число: "))

number = abs(number)

figure = number % 10

number = number // 10

while number > 0:

    if number & 10 > figure:
        figure = number % 10
    number = number // 10
    
print(figure)   

TASK05

Revenue = int(input("Выручка за период: "))

Overheads = int(input("Издержки за период :"))

Income = Revenue - Overheads

if Revenue > Overheads:
    print("Фирма работает с прибылью")

else:
    print("Фирма работает с убытком")

if Revenue > Overheads:
    print("Рентабельность выручки = ", Income / Revenue)
    
if Revenue > Overheads:
    Stuff_number = int(input("Численность сотрудников: "))
    print("Прибыль фирмы в расчете на одного сотрудника: ", Income / Stuff_number)
    
TASK06

a = int(input('Количесво км в 1-й день пробежки: '))

b = int(input('Количество километров, к которому стремится спортсмен за одну пробежку: '))

day = 1

cur_result = a

while cur_result < b:
    cur_result = cur_result*1.1
    day += 1

print(f'На {day}-й день спортсмен достиг результата — не менее {b} км')
