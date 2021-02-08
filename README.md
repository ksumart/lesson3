# lesson3
v1
# номер 2
  def exe_2(**kwargs):
    return list(kwargs.values())

def exe_2_use():
    print(exe_2(name=input('Enter name:'),
                s_name=input('Enter second name:')
                birth_date=input('Enter birth day:')
                l_town=input('Enter live town:')
                email=input('Enter email:')
                tel=input('Enter tel number:')
 #
    name = input('enter name')
    surname = input('enter surname')
    year = int(input('enter year'))
    city = input('enter city')
    email = input('enter email')
    telephone = input('input telephone')

 def my_func (name, surname, year, city, email, telephone)
      return ' '.join([name, surname, year, city, email, telephone])
 print(my_func)

#  Реализовать функцию my_func(), которая принимает три позиционных
#  аргумента, и возвращает сумму наибольших двух аргументов.
#
def my_func(arg1 , arg2, arg3):
     if arg1 >= arg3 and arg2 >= arg3:
          return arg1 + arg2
      elif arg1 > arg2 and arg1 < arg3:
          return arg1 + arg3
      else:
          return arg2 + arg3

   print(f'Result - {my_func(int(input("enter first argument ")), int(input("enter second argument ")), int(input("enter third argument ")))}')
#Программа запрашивает у пользователя строку чисел, разделенных
 # пробелом. При нажатии Enter должна выводиться сумма чисел.
 #Пользователь может продолжить ввод чисел, разделенных пробелом и
 #снова нажать Enter. Сумма вновь введенных чисел будет добавляться
 #к уже подсчитанной сумме. Но если вместо числа вводится специальный
# символ, выполнение программы завершается. Если специальный символ
 #введен после нескольких чисел, то вначале нужно добавить сумму этих
 #чисел к полученной ранее сумме и после этого завершить программу.


  def my_sum ():
     sum_res = 0
     ex = False
     while ex == False:
         number = input('Input numbers or Q for quit - ').split()

          res = 0
         for el in range(len(number)):
             if number[el] == 'q' or number[el] == 'Q':
                 ex = True
                 break
             else:
                 res = res + int(number[el])
         sum_res = sum_res + res
         print(f'Current sum is {sum_res}')
     print(f'Your final sum is {sum_res}')


  my_sum()
  #Реализовать функцию int_func(), принимающую слово из маленьких
 #латинских букв и возвращающую его же, но с прописной первой буквой.
 #Например, print(int_func(‘text’)) -> Text.
 #Продолжить работу над заданием. В программу должна попадать
 #строка из слов, разделенных пробелом. Каждое слово состоит
 #из латинских букв в нижнем регистре. Сделать вывод исходной
 #строки, но каждое слово должно начинаться с заглавной буквы.
 #Необходимо использовать написанную ранее функцию int_func().

 def int_func (*args):
     word = input("Input words ")
     print(word.title())
     return
 int_func()
# Реализовать скрипт, в котором должна быть предусмотрена
#   функция расчета заработной платы сотрудника. В расчете
#   необходимо использовать формулу:
#   (выработка в часах*ставка в час) + премия.
#   Для выполнения расчета для конкретных значений необходимо
#   запускать скрипт с параметрами.


   from sys import argv

   name, time, salary, bonus = argv
  try:
      time = int(time)
      salary = int(salary)
      bonus = int(bonus)
      res = time * salary + bonus
      print(f'заработная плата сотрудника  {res}')
  except ValueError:
      print('Not a number')

#1 Реализовать функцию, принимающую два числа
 #(позиционные аргументы) и выполняющую их деление.
 #Числа запрашивать у пользователя,
 #предусмотреть обработку ситуации деления на ноль.



  def div(*args):

      try:
         arg1 = int(input("Input dividend "))
         arg2 = int(input("Input divider "))
         res = arg1 / arg2
     except ValueError:
         return 'Value error'
     except ZeroDivisionError:
         return "Wrong devider! You can't use zero as a devider"

     return res

     if arg2 != 0:
    return arg1 / arg2
     else:
         print("Wrong number! Devider can't be null")
