# Comparing `tmp/podval-3.7.tar.gz` & `tmp/podval-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.7.tar", last modified: Fri Jun 16 12:12:50 2023, max compression
+gzip compressed data, was "dist\podval-3.8.tar", last modified: Fri Jun 16 21:35:06 2023, max compression
```

## Comparing `podval-3.7.tar` & `podval-3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 12:12:50.000000 podval-3.7/
--rw-rw-rw-   0        0        0      188 2023-06-16 12:12:50.000000 podval-3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 12:12:50.000000 podval-3.7/podval/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.7/podval/__init__.py
--rw-rw-rw-   0        0        0    95923 2023-06-16 12:11:02.000000 podval-3.7/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.7/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:12:50.000000 podval-3.7/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-16 12:12:50.000000 podval-3.7/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-16 12:12:50.000000 podval-3.7/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 12:12:50.000000 podval-3.7/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.7/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-16 12:12:50.000000 podval-3.7/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 12:12:50.000000 podval-3.7/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-16 12:12:07.000000 podval-3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/
+-rw-rw-rw-   0        0        0      188 2023-06-16 21:35:06.000000 podval-3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/podval/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.8/podval/__init__.py
+-rw-rw-rw-   0        0        0    97495 2023-06-16 21:32:51.000000 podval-3.8/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.8/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.8/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 21:35:06.000000 podval-3.8/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-16 21:32:57.000000 podval-3.8/setup.py
```

### Comparing `podval-3.7/podval/exam.py` & `podval-3.8/podval/exam.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,34 @@
 ю - yu
 я - ya
 
 Заметки:
 1) Если функции совпадают в 5 буквах, пишется 6-ая (7-ая или 8-ая) (для помощи используйте Tab)
 2) Слова в () и в {} учитываются
 3) Цифры, переменные, примеры по типу 'hello world', 'l' и 'o' → 'he wrd' не учитываются.
-4) Фразы "Метод должен изменять исходный список" и " Функция должна возвращать отсортированный список." не учитываются''')
+4) Фразы "Метод должен изменять исходный список" и " Функция должна возвращать отсортированный список." не учитываются
+5) Примеры учитываются (смотрим на русские слова)
+
+Проблема с Бинарным деревом:
+1) В методе __str__ исправтьте строчку на '\н'.join(self._display(self.root)[0]) !!!н поменяйте на n!!!
+2) Найдите переменную second_line (в двух местах) и добавьтее к '\' второй такой же слэж 
+
+Задачи по группам:
+1) Лямбда-функции: fchyaks, bstsk, lpschsi, isusd, nipsu, pyaksz, chsrchd, pavzs, lpssszva, lpschsz, evpks, lichsz, nipchd, chpyaks, rvbts, ndnin, tstsks, chspvch, tnzks, kchyaks, achyaks, akvpn, lpschts, lpschz, pivia, lichsz, lpssszvch     
+2) Сортировки: kkemi, skvbg, chpobd, skdup, kkevv, skvzi, applv
+3) Классы (с дочерними): Автомобиль - khzsap, Фильм - rivgz, Продукт - sitszs, Животное - oipzs, Студент - dtibs
+4) Классы: Банк - fuvko, Круг - tstsirr, Студент - vvisv, Recipe - dtiyai, Animal - zhtsups, Student - suknf, Книга - igpkd, BankAccount - sokvv, Movie - fzhups, Прямоугольник - pppds
+5) Двусвязный список: nneei, nsitn, sdvev, sdvem, sieui, sivii, sdvek
+6) Стэк: sedkya, sepdya, chchyank
+7) Бинарное дерево поиска: pdbvn, pdbvz
+8) Очередь вар: ddnot, ddnot, upobd
+9) Хеш-таблица: tyaovkh, tyaovkhdoa
+10) Квик сорт: sbapsd
+11) Бабл сорт: psaps
+12) Инсершн сорт: vsapsa''')
 
 #1
 def fchyaks():
     print('''#Используя лямбда-функцию, найдите все числа в заданном списке, которые являются числами Фибоначчи.
 
 is_fibo = (lambda a: lambda v,fib=0,n=1: a(a,v,fib,n))(lambda f,value,fib,n: f(f,value,fib+n,fib) if fib < value else fib==value)
 
@@ -176,15 +195,15 @@
 prime_numbers = list(filter(is_prime, numbers))
 
 # Фильтрация списка на составные числа
 composite_numbers = list(filter(lambda num: not is_prime(num), numbers))
 
 prime_numbers, composite_numbers''')
     
-def susdp():
+def isusd():
     print('''#Для удаления определённых символов из заданной строки используйте лямбда-функцию. Пример: дана строка 'hello world', удалить символы 'l' и 'o' → 'he wrd'.
 
 string = 'hello world'
 characters_to_remove = ['l', 'o']
 
 # Функция для удаления символов из строки
 remove_characters = lambda s: ''.join([char for char in s if char not in characters_to_remove])
@@ -435,15 +454,15 @@
 for item in lst2:
     stack2.push(item)
 
 print(f'Стек 1: {stack1}, {square(stack1)}')
 print(f'Стек 2: {stack2}, {square(stack2)}')''')
 
 #4    
-def hzsap():
+def khzsap():
     print('''# Создайте класс АВТОМОБИЛЬ с методами, позволяющими вывести на
 # экран информацию об автомобиле, а также определить, подходит ли
 # данный автомобиль для заданных условий. Создайте дочерние классы
 # ЛЕГКОВОЙ (марка, модель, год выпуска, объем двигателя, тип
 # топлива), ГРУЗОВОЙ (марка, модель, год выпуска, грузоподъемность),
 # ПАССАЖИРСКИЙ (марка, модель, год выпуска, количество мест) со
 # своими методами вывода информации на экран и определения
@@ -865,15 +884,15 @@
 #6   
 def pyaksz():
     print('''#Используя лямбда-функцию, найдите все числа в заданном списке,
 которые являются палиндромами.
 my_list = [121, 55, 4664, 10, 12321, 88, 67876]
 palindromes = filter(lambda x: str(x) == str(x)[::-1], my_list)
 print(list(palindromes))''')
-  
+    
 def skvbg():
     print('''#Напишите программу для сортировки заданного списка строк по
 количеству гласных букв в каждой строке
 my_list = ['apple', 'peach', 'banana', 'watermelon', 'aboooooooooooba', 'lol', 'kk']
 
 def count_vowels(word):
   vowels = 'aeiouAEIOU'
@@ -1436,16 +1455,15 @@
     print('''# С помощью лямбда-функции проверьте, является ли данное число простым или нет
 is_prime = lambda num: all(num % i != 0 for i in range(2, int(num ** 0.5) + 1)) and num > 1
 print(is_prime(7))   # Output: True
 print(is_prime(20))  # Output: False''')
     
     
 def dodzp():
-    print('''#Напишите программу для поиска чисел в заданном диапазоне, которые являются суммой двух квадратов. Пример: задан диапазон от 1
-#до 50 → [1, 2, 4, 5, 8, 9, 10, 13, 16, 17, 18, 20, 25, 26, 29, 32, 34, 36, 37, 40,
+    print('''#Напишите программу для поиска чисел в заданном диапазоне, которые являются суммой двух квадратов. Пример: задан диапазон от 1 # до 50 → [1, 2, 4, 5, 8, 9, 10, 13, 16, 17, 18, 20, 25, 26, 29, 32, 34, 36, 37, 40,
 #41, 45, 49, 50]
 def sumSquare(n):
  
     s = dict()
     for i in range(1, n):
  
         if i * i > n:
@@ -2122,15 +2140,15 @@
 for s in lst:
     try:
         if s.find_conditions('Математика'):
             print(s.info())
     except:
         pass''')
     
-def psaps():
+def psapsvpk():
     print('''# Написать метод класса «Клиент», который сортирует список клиентов по возрасту с помощью алгоритма сортировки пузырьком. Метод должен изменять исходный список
 class Client():
     def __init__(self, name, age):
         self.name = name
         self.age = age
     
     def __str__(self):
@@ -2285,15 +2303,15 @@
 
 # Установка цвета животного
 animal.color = "Brown"
 
 # Вывод информации о животном с установленным цветом
 animal.display_info()''')
 
-def sovdf():
+def vsapsa():
     print('''# Написать функцию, которая принимает на вход список слов и сортирует
 # его по алфавиту с помощью алгоритма сортировки вставками. Функция
 # должна возвращать отсортированный список
 import copy
 def insertion_sort(arr):
     words = arr.copy()
     for i in range(1, len(words)):
@@ -2642,15 +2660,15 @@
 a = BankAccount(55362036, 201030405020, 'GOLOVKINA ANNA')
 print(a.info())
 
 a.currency = 'USD'
 
 print(a.info())''')
 
-def psaps():
+def psapsvpe():
     print('''#Написать функцию, которая принимает на вход список дат и сортирует
 его по возрастанию с помощью алгоритма сортировки пузырьком.
 Функция должна возвращать отсортированный список
 def bubble_sort(arr, reverse=True):
     n = len(arr)
     
     for i in range(n):
@@ -2736,15 +2754,16 @@
 
 h = HashTable(3)
 
 for i in g:
     h.insert(i.name, i)
 h.table
 ''')
-    
+
+#26
 def pivia():
     print('''Напишите лямбда-функцию, которая принимает два аргумента и возвращает их произведение.
 multiplication = lambda x,y: x*y
 print(multiplication(7,6))''')
 
 def lichsz():
     print('''Найдите числа, которые являются квадратами целых чисел, из заданного списка чисел, используя лямбда-функцию
@@ -2787,15 +2806,16 @@
 
 products = [Product('Cheese', 77), Product('Apple', 23), Product('Meat', 56), Product('Ice cream', 19)]
 
 Product.sorting(products)
 
 for i in products:
     print(i.name, i.price)''')
-    
+
+#27    
 def pppds():
     print('''Создайте класс «Прямоугольник» с атрибутами длины и ширины. Напишите методы для вычисления площади и периметра прямоугольника. Используйте магический метод eq для сравнения двух прямоугольников по площади.
 class Rectangle():
   def __init__(self, a, b):
     self.a = a
     self.b = b
```

### Comparing `podval-3.7/podval/podval.py` & `podval-3.8/podval/podval.py`

 * *Files identical despite different names*

