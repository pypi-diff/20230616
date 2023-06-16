# Comparing `tmp/podval-3.5.tar.gz` & `tmp/podval-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.5.tar", last modified: Wed Jun 14 19:36:42 2023, max compression
+gzip compressed data, was "dist\podval-3.6.tar", last modified: Fri Jun 16 07:44:23 2023, max compression
```

## Comparing `podval-3.5.tar` & `podval-3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/
--rw-rw-rw-   0        0        0      188 2023-06-14 19:36:42.000000 podval-3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/podval/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.5/podval/__init__.py
--rw-rw-rw-   0        0        0    86591 2023-06-14 19:36:17.000000 podval-3.5/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.5/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.5/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 19:36:42.000000 podval-3.5/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 19:36:42.000000 podval-3.5/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-14 19:36:28.000000 podval-3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:44:23.000000 podval-3.6/
+-rw-rw-rw-   0        0        0      188 2023-06-16 07:44:23.000000 podval-3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 07:44:23.000000 podval-3.6/podval/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.6/podval/__init__.py
+-rw-rw-rw-   0        0        0    93676 2023-06-16 07:42:56.000000 podval-3.6/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.6/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:44:23.000000 podval-3.6/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-16 07:44:23.000000 podval-3.6/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-16 07:44:23.000000 podval-3.6/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:44:23.000000 podval-3.6/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.6/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-16 07:44:23.000000 podval-3.6/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:44:23.000000 podval-3.6/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-16 07:44:11.000000 podval-3.6/setup.py
```

### Comparing `podval-3.5/podval/exam.py` & `podval-3.6/podval/exam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+def _help():
+    print('''
+Алфавит:
+ж - zh
+х - kh
+ц - ts
+ч - ch
+ш - sh
+щ - shch
+ю - yu
+я - ya
+
+Заметки:
+1) Если функции совпадают в 5 буквах, пишется 6-ая (7-ая) (для помощи используйте Tab)
+2) Слова в () и в {} учитываются
+3) Цифры, переменные, примеры по типу 'hello world', 'l' и 'o' → 'he wrd' не учитываются.
+4) Фразы "Метод должен изменять исходный список" и " Функция должна возвращать отсортированный список." не учитываются''')
+
 #1
 def fchyaks():
     print('''#Используя лямбда-функцию, найдите все числа в заданном списке, которые являются числами Фибоначчи.
 
 is_fibo = (lambda a: lambda v,fib=0,n=1: a(a,v,fib,n))(lambda f,value,fib,n: f(f,value,fib+n,fib) if fib < value else fib==value)
 
 # Заданный список чисел
@@ -1200,15 +1218,15 @@
 #9    
 def pavzs():
     print('''#Используя лямбда-функцию, отсортировать список строковых значений в алфавитном порядке.
 fruits = ['apple', 'Orage', 'peach', 'kiwi', 'Banana', 'grapes', 'Lemon']
 sorted(fruits, key=lambda x: x[0].lower())''')
     
     
-def lpsss():
+def lpssszva():
     print('''#Найдите все анаграммы в заданном списке строк с помощью лямбда-функции
 words = ['нос','апельсин', 'собака', 'тапок', 'топка',  'автор', 'шакал',  'отвар', 'товар', 'алкаш', 'шкала', 'кот', 'капот', 'покат', 'ток', 'сон', 'кошка']
 anagrams_dict = {}
 for w in words:
   key = ''.join(sorted(w))
   anagrams_dict[key] = []
   for ww in words:
@@ -1539,15 +1557,15 @@
 else:
     print("I need to buy some ingredients")
 
 recipe.cuisine_type = "Italian"
 print(recipe.cuisine_type)''')
 
     
-def siidm():
+def sbapsd():
     print('''#Написать метод класса «Заказ», который сортирует список заказов по
 #дате с помощью алгоритма быстрой сортировки. Метод должен
 #изменять исходный список.
 
 
 class Order:
     def __init__(self, id, date, amount):
@@ -1614,53 +1632,60 @@
     
 def rvbts():
     print('''# в) Используя лямбда-функцию, найдите все строки в заданном списке строк, которые содержат только буквы верхнего регистра
 st = ['RHGR', 'EGHTYHegF', 'rehGr', 'GETG', 'wqgre', 'qwergjb', 'eGt']
 C = list(filter(lambda a: a.isupper(), st))
 print(C)''')
     
-def tyaovkh():
+def tyaovkhdoa():
     print('''#Реализовать класс хеш-таблицы для хранения объектов класса «Книга». 
 #Хеш-функция должна основываться на поле «автор книги». Если две
 #книги имеют одного и того же автора, они должны храниться в одной
 #ячейке таблицы
 
 # реализация хеш-таблицы методом цепочек
 class HashTable:
     def __init__(self, size):
         self.size = size
         self.table = [[] for _ in range(self.size)]
 
     def hash_function(self, key):
         return hash(key) % self.size
 
-    def insert(self, book):
-        index = self.hash_function(book.author)
-        self.table[index].append(book.name)
+    def insert(self, key, value):
+        slot = self.hash_function(key)
+        for pair in self.table[slot]:
+            if pair[0] == key:
+                pair.append(value)
+                return
+        self.table[slot].append([key, value])
 
-    def find(self, author):
-        index = self.hash_function(author)
-        return self.table[index]
-        
+    def find(self, key):
+        slot = self.hash_function(key)
+        for pair in self.table[slot]:
+            if pair[0] == key:
+                return pair[1]
+        return None
+    
 class Book:
     def __init__(self, author, name):
         self.author = author
         self.name = name
 
     def __str__(self):
         return f"Автор: {self.author}, название: {self.name}"
-        
+    
 books = HashTable(6)
 books_list = [Book('Pushkin', 'Boris Godunov'), Book('Dostoevskiy', 'Prestuplenie i nakazanie'),
               Book('Pushkin', 'Evgeniy Onegin')]
 for b in books_list:
-    books.insert(b)
+    books.insert(b.author,b.name)
     print(b)
-
-print(books.find('Pushkin'))''')
+    
+books.table''')
 
 #14    
 def ndnin():
     print('''#а) Используя лямбда-функцию, найдите все числа в заданном списке, которые делятся на 3 и не делятся на 5.
 import numpy as np
 lst = np.random.randint(1, 100, 30)
 A = list(filter(lambda a: (a % 3 == 0)*(a % 5 != 0), lst))
@@ -2097,15 +2122,15 @@
 for s in lst:
     try:
         if s.find_conditions('Математика'):
             print(s.info())
     except:
         pass''')
     
-def siidm():
+def psaps():
     print('''# Написать метод класса «Клиент», который сортирует список клиентов по возрасту с помощью алгоритма сортировки пузырьком. Метод должен изменять исходный список
 class Client():
     def __init__(self, name, age):
         self.name = name
         self.age = age
     
     def __str__(self):
@@ -2572,8 +2597,164 @@
                 if (arr[j] < arr[j + 1]):
                     arr[j], arr[j + 1] = arr[j + 1], arr[j]
     return arr
 
 a = ['2004-06-29', '2005-01-17', '2004-02-03', '2004-05-26', '1980-06-18', '1978-02-18', '1953-10-24', '1951-08-31', '2011-01-09']
 
 bubble_sort(a)
-''')
+''')
+    
+#25
+def fzhups():
+    print('''Опишите класс Movie, заданный названием, режиссером, годом выпуска и продолжительностью. Включите в описание класса методы: вывода информации о фильме на экран, проверки, является ли фильм длинным (продолжительность больше 2 часов), и свойство, позволяющее установить жанр фильма.
+class Movie:
+    def __init__(self, name, director, year, time, genre = None):
+        self.name = name
+        self.director = director
+        self.year = year
+        self.time = time
+        self.genre = genre
+
+    def set_genre(self, genre):
+        self.genre = genre
+
+    def get_data(self):
+            print(f'Name of film is : {self.name}, The director is : {self.director}, Year of publication is : {self.year}, Duration is : {self.time} minutes')
+        if self.genre:
+            print(f'The genre is: {self.genre}')
+
+    def check_time(self):
+        if self.time > 120:
+            print(f'The film {self.name} lats more 120 minutes')
+        else:
+            print(f'The film {self.name} lats less 120 minutes')
+movie1 = Movie('The Green Mile', 'Ton Khencks', 1999, 189)
+movie2 = Movie('Mountain', 'Jo Dain', 2017, 90)
+
+movie1.check_time()
+movie1.set_genre('Drama, Thriller')
+movie1.get_data()
+
+movie2.check_time()
+movie2.set_genre('Drama, Thriller')
+movie2.get_data()''')
+    
+def tyaovkhdon():
+    print('''#Реализовать класс хеш-таблицы для хранения объектов класса «Товар». Хеш-функция должна основываться на поле «название #товара». Если два товара имеют одинаковое название, они должны храниться в одной ячейке таблицы.
+class Good():
+    def __init__(self, name, price):
+        self.name = name
+        self.price = price
+
+g = [Good('Pork', 100), Good('Pork', 120), Good('Jam', 40), Good('Meat', 300), Good('Lemon', 30), Good('Kale', 25)]
+class HashTable:
+    def __init__(self, size):
+        self.size = size
+        self.table = [[] for _ in range(self.size)]
+
+    def hash_function(self, key):
+        return hash(key) % self.size
+
+    def insert(self, key, value):
+        slot = self.hash_function(key)
+        for pair in self.table[slot]:
+            if pair[0] == key:
+                pair.append(value)
+                return
+        self.table[slot].append([key, value])
+
+    def find(self, key):
+        slot = self.hash_function(key)
+        for pair in self.table[slot]:
+            if pair[0] == key:
+                return pair[1]
+        return None
+
+h = HashTable(3)
+
+for i in g:
+    h.insert(i.name, i)
+h.table
+''')
+    
+def pivia():
+    print('''Напишите лямбда-функцию, которая принимает два аргумента и возвращает их произведение.
+multiplication = lambda x,y: x*y
+print(multiplication(7,6))''')
+
+def lichsz():
+    print('''Найдите числа, которые являются квадратами целых чисел, из заданного списка чисел, используя лямбда-функцию
+numbers = [1,2,4,5,8,9,10,12,14,16,19,25]
+result = list(filter(lambda x: int(x**0.5)**2 == x, numbers))
+print(result)''')
+    
+def lpssszvch():
+    print('''Напишите программу для подсчёта целых чисел в заданном смешанном списке с помощью лямбда-функции.
+numbers = [1, 3.24, 6, 8, 5.45, 10]
+result = list(filter(lambda x: isinstance(x, int), numbers))
+print(result)''')
+    
+def sbapsts():
+    print('''Написать метод класса «Товар», который сортирует список товаров по цене с помощью алгоритма быстрой сортировки. Метод должен изменять исходный список.
+class Product():
+    def __init__(self, name, price):
+        self.name = name
+        self.price = price
+     
+    def __str__(self):
+        return f"Продукты: {self.name}, Цена: {self.price}"
+    
+    @staticmethod
+    def sorting(arr):
+        def quick_sort(arr):
+            if len(arr) <= 1:
+                return arr
+            else:
+                pivot = arr[0]
+                left = []
+                right = []
+                for i in range(1, len(arr)):
+                    if arr[i].price < pivot.price:
+                        left.append(arr[i])
+                    else:
+                        right.append(arr[i])
+                return quick_sort(left) + [pivot] + quick_sort(right)
+        arr[:] = quick_sort(arr)
+
+products = [Product('Cheese', 77), Product('Apple', 23), Product('Meat', 56), Product('Ice cream', 19)]
+
+Product.sorting(products)
+
+for i in products:
+    print(i.name, i.price)''')
+    
+def pppds():
+    print('''Создайте класс «Прямоугольник» с атрибутами длины и ширины. Напишите методы для вычисления площади и периметра прямоугольника. Используйте магический метод eq для сравнения двух прямоугольников по площади.
+class Rectangle():
+  def __init__(self, a, b):
+    self.a = a
+    self.b = b
+
+  def Perimeter(self):
+    return 2*(self.a + self.b)
+
+  def Square(self):
+    return self.a*self.b
+
+  def __eq__(self, other):
+    if isinstance(other, Rectangle): #проверка принадлежности классу
+      return self.Square == other.Square
+    False
+figure1 = Rectangle(20,16)
+figure2 = Rectangle(10,32)
+
+square1 = figure1.Square()
+square2 = figure2.Square()
+
+print('Perimetr is: ', figure1.Perimeter())
+print('Square is: ', figure1.Square())
+print('Perimetr is: ', figure2.Perimeter())
+print('Square is: ', figure2.Square())
+if  square1 == square2:
+  print('square1 and square2 are equal')
+else:
+  print(False)''')
```

### Comparing `podval-3.5/podval/podval.py` & `podval-3.6/podval/podval.py`

 * *Files identical despite different names*

