# Comparing `tmp/loosers-0.0.10.tar.gz` & `tmp/loosers-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loosers-0.0.10.tar", last modified: Fri Jun 16 18:36:56 2023, max compression
+gzip compressed data, was "loosers-0.0.11.tar", last modified: Fri Jun 16 21:24:18 2023, max compression
```

## Comparing `loosers-0.0.10.tar` & `loosers-0.0.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 18:36:56.300352 loosers-0.0.10/
--rw-rw-rw-   0        0        0      124 2023-06-16 18:36:56.300352 loosers-0.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 18:36:56.284726 loosers-0.0.10/loosers/
--rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 loosers-0.0.10/loosers/__init__.py
--rw-rw-rw-   0        0        0   188553 2023-06-16 18:00:23.000000 loosers-0.0.10/loosers/tvz.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:36:56.300352 loosers-0.0.10/loosers.egg-info/
--rw-rw-rw-   0        0        0      124 2023-06-16 18:36:56.000000 loosers-0.0.10/loosers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-16 18:36:56.000000 loosers-0.0.10/loosers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 18:36:56.000000 loosers-0.0.10/loosers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 18:36:56.000000 loosers-0.0.10/loosers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-06-16 18:36:56.300352 loosers-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-16 18:33:59.000000 loosers-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.350631 loosers-0.0.11/
+-rw-rw-rw-   0        0        0      124 2023-06-16 21:24:18.350631 loosers-0.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.335006 loosers-0.0.11/loosers/
+-rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 loosers-0.0.11/loosers/__init__.py
+-rw-rw-rw-   0        0        0   190232 2023-06-16 21:12:44.000000 loosers-0.0.11/loosers/tvz.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.350631 loosers-0.0.11/loosers.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-16 21:24:18.350631 loosers-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-16 21:23:22.000000 loosers-0.0.11/setup.py
```

### Comparing `loosers-0.0.10/loosers/tvz.py` & `loosers-0.0.11/loosers/tvz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os.path
 
 
 class izi:
     def pract(number=''):
+        #1
         sklad = {
 #1-17-19
             'Написать программу с':'Написать программу с интерактивным консольным меню (т.е. вывод списка действий по цифрам) по вычислению площади круга (родительский класс), длины окружности (подкласс) и объема шара (подкласс) по задаваемому с клавиатуры радиусу. Содержание меню: 1. Вычислить площадь круга. 2. Вычислить длину окружности. 3. Вычислить объем шара.\n\
 \n\
 from math import pi\n\
 class RoundOne():\n\
 def __init__(self, radius):\n\
@@ -401,15 +402,15 @@
 print(f"Загрузка самолета {plane3.name}: {load3}%")\n\
 print(f"Загрузка самолета {plane4.name}: {load4}%")\n\
 print(f"Загрузка самолета {plane5.name}: {load5}%")\n\
 \n\
 # Определение всех имен самолетов, летящих по одному маршруту\n\
 planes = [plane1, plane2, plane3, plane4, plane5]\n\
 matching_planes = Plane.find_planes_by_route(planes, "New York - London")\n\
-print(f"Самолеты, летящие по маршруту "New York - London": {matching_planes}")\n\
+print(f"Самолеты, летящие по маршруту New York - London: {matching_planes}")\n\
 \n\
 # Определение средней загрузки всех самолетов\n\
 average_load = Plane.calculate_average_load(planes)\n\
 print(f"Средняя загрузка всех самолетов: {average_load}")'
             ,
 #7-54
             'Дано предложение без':'7.	Дано предложение без знаков препинания. Превратить предложение в список слов. При помощи механизма map/filter/reduce отбросить у каждого слова последнюю букву и склеить в одну строку те обрезанные слова, длина которых больше 5. \n\
@@ -419,18 +420,18 @@
 s.split())))))) \n\
 \n\
 \n\
 \n\
 \n\
 \n\
 Дано предложение без знаков препинания. Превратить предложение в список слов. При помощи механизма map/filter/reduce найти количество слов, длина которых больше 4 и склеить их в одну строку (20 баллов)\n\
-lst = «eeny meeny money moe do they love u no they dont»\n\
-lst = lst.split(« «)\n\
+lst = "eeny meeny money moe do they love u no they dont"\n\
+lst = lst.split(" ")\n\
 a = list(filter(lambda x: len(x)>4, lst)) # отбирает только слова больше 4 сим-в\n\
-print(««.join(a))'
+print("".join(a))'
             ,
 #9-29
             'Дан список S':'9.	Дан список S состоящий из N различных элементов. Вывести индексы четных элементов списка. Использовать встроенные функции высшего порядка.\n\
 s = [1, 2, 3, 4]\n\
 print(list(map(lambda x: print(s.index(x)) if x % 2 == 0 else x, s)))\n\
 \n\
 \n\
@@ -438,20 +439,27 @@
 \n\
 \n\
 Дан список S состоящий из N различных элементов. Вывести индексы четных элементов списка. Использовать функции высшего порядка. (20 баллов)\n\
 s = [1, 2, 3, 4, 5, 6]\n\
 list(map(lambda x: print(s.index(x)) if x % 2 == 0 else x, s))'
             ,
 #10-18-52
-            'Построить базовый класс':'Задание: построить базовый класс с указанными в таблице полями и методами:\n\
+            'Построить базовый класс':'КОМПЬЮТЕРЫ Задание: построить базовый класс с указанными в таблице полями и методами:\n\
 - конструктор; - функция, которая определяет «качество» объекта – Q по заданной формуле; - метод вывода информации об объекте.\n\
 Построить дочерний класс (класс-потомок), который содержит:\n\
 - дополнительное поле P;\n\
 - функция, которая определяет «качество» объекта дочернего класса – Qp и перегружает функцию качества родительского класса (Q), выполняя вычисление по новой формуле.\n\
 Создать проект для демонстрации работы: ввод и вывод информации об объектах классов\n\
+Поля и методы базового класса	Поля и методы дочернего класса\n\
+Компьютер:\n\
+- наименование процессора;\n\
+- тактовая частота процессора (МГц);\n\
+- объем оперативной памяти (Мб);\n\
+- Q = (0,1·частота) + память	P: объем накопителя SSD (Гб)\n\
+- Qp = Q +0,5P\n\
 \n\
 class Computer:\n\
     def __init__(self, processor_name, processor_speed, memory):\n\
         self.processor_name = processor_name\n\
         self.processor_speed = processor_speed\n\
         self.memory = memory\n\
 \n\
@@ -488,26 +496,69 @@
 quality2 = computer2.calculate_quality()\n\
 print(f"Quality: {quality2}")\n\
 \n\
 \n\
 \n\
 \n\
 \n\
-Построить базовый класс с указанными в таблице полями и методами:\n\
+Задание: построить базовый класс с указанными в таблице полями и методами:\n\
 - конструктор; - функция, которая определяет «качество» объекта – Q по заданной формуле; - метод вывода информации об объекте.\n\
 Построить дочерний класс (класс-потомок), который содержит:\n\
 - дополнительное поле P;\n\
 - функция, которая определяет «качество» объекта дочернего класса – Qp и перегружает функцию качества родительского класса (Q), выполняя вычисление по новой формуле.\n\
-Создать проект для демонстрации работы: ввод и вывод информации об объектах классов.\n\
+Создать проект для демонстрации работы: ввод и вывод информации об объектах классов. (20 баллов)\n\
+Поля и методы базового класса Поля и методы дочернего класса\n\
+Автомобиль:\n\
+- марка автомобиля;\n\
+- мощность двигателя (кВт);\n\
+- число мест;\n\
+- Q = 0,1·мощность ·число мест P: год выпуска\n\
+- Qp = Q - 1,5·(T-P),\n\
+где T – текущий год\n\
+\n\
+import datetime\n\
+\n\
+class Car:\n\
+    def init(self, marka, moshnost, chislo_mest):\n\
+        self.marka = marka\n\
+        self.moshnost = moshnost\n\
+        self.chislo_mest = chislo_mest\n\
+    \n\
+    def kachestvo(self):\n\
+        return 0.1 * self.moshnost * self.chislo_mest\n\
+    \n\
+    def info(self):\n\
+        print("Марка:", self.marka)\n\
+        print("Мощность двигателя (кВт):", self.moshnost)\n\
+        print("Число мест:", self.chislo_mest)\n\
+        print("Качество:", self.kachestvo())\n\
+\n\
+class ChildCar(Car):\n\
+    def init(self, marka, moshnost, chislo_mest, date):\n\
+        super().init(marka, moshnost, chislo_mest)\n\
+        self.P = date\n\
+    \n\
+    def kachestvo(self):\n\
+        year1 = datetime.datetime.now().year\n\
+        T = year1\n\
+        return super().kachestvo() - 1.5 * (T - self.P)\n\
+    \n\
+#Пример\n\
+car1 = Car("БМВ", 100, 5)\n\
+car2 = ChildCar("МЕРСЕДЕС", 150, 4, 2015)\n\
 \n\
+car1.info()\n\
+print()  \n\
+car2.info()\n\
 \n\
 \n\
 \n\
 \n\
-Задание: построить базовый класс с указанными в таблице полями и методами:\n\
+\n\
+КОМПЬЮТЕРЫ Задание: построить базовый класс с указанными в таблице полями и методами:\n\
 - конструктор; - функция, которая определяет «качество» объекта – Q по заданной формуле; - метод вывода информации об объекте.\n\
 Построить дочерний класс (класс-потомок), который содержит:\n\
 - дополнительное поле P;\n\
 - функция, которая определяет «качество» объекта дочернего класса – Qp и перегружает функцию качества родительского класса (Q), выполняя вычисление по новой формуле.\n\
 Создать проект для демонстрации работы: ввод и вывод информации об объектах классов. (20 баллов)\n\
 Поля и методы базового класса	Поля и методы дочернего класса\n\
 Компьютер:\n\
@@ -612,28 +663,14 @@
     return a+b+c\n\
 func(10,-1,-1)\n\
 \n\
 \n\
 \n\
 \n\
 \n\
-Реализовать декоратор с именем not_sum, который генерирует исключительную ситуацию, если декорируемая функция вернула отрицательное значение суммы трех чисел.\n\
-\n\
-def not_sum(func):\n\
-    def wrapper(*args):\n\
-        result = func(*args)\n\
-        if result < 0:\n\
-            raise Exception("Сумма трех чисел отрицательна")\n\
-        return result\n\
-    return wrapper\n\
-\n\
-# Пример использования декоратора\n\
-@not_sum\n\
-def calculate_sum(a, b, c):\n\
-    return a + b + c\n\
 \n\
 # Пример данных\n\
 a = 5\n\
 b = -10\n\
 c = 15\n\
 \n\
 try:\n\
@@ -850,51 +887,65 @@
 '
             ,
 #22
             'Создайте класс Заказ':'Создайте класс Заказ(Order), у которого есть свойства код_товара(code), цена(price), количество(count) и методы __init__ и __str__. Создайте 2 класса-потомка: Опт(Opt) и Розница(Retail). В этих классах создайте методы __init__, __str__ и сумма_заказа (summa), позволяющий узнать стоимость заказа. Для опта стоимость единицы товара составляет 95% от цены, а при покупке более 500 штук – 90% цены. В розницу стоимость единицы товара составляет 100% цены. Стоимость заказа равна произведению цены на количество. Создайте список, содержащий по 2 объекта каждого класса (Order, Opt, Retail). Для этого списка:\n\
 •	выведите информацию о каждом объекте с помощью метода __str__;\n\
 •	найдите общую стоимость заказов для объектов Opt и Retail. (20 баллов)\n\
 class Order:\n\
-    def _init (self, code, price, count):\n\
+    def __init__(self, code, price, count):\n\
         self.code = code\n\
         self.price = price\n\
         self.count = count\n\
+    \n\
     def __str__(self):\n\
-        return f"Товар {self.code} в стоимость {self.price} за шт. \\n\
-в количестве {self.count} шт."\n\
+        return f"Товар {self.code} стоимостью {self.price} за шт.\nв количестве {self.count} шт."\n\
+\n\
+\n\
 class Opt(Order):\n\
-    def _init (self, code, price, count):\n\
-        super().__init (code, price, count)\n\
+    def __init__(self, code, price, count):\n\
+        super().__init__(code, price, count)\n\
         if count <= 500:\n\
             self.summa = price * count * 0.95\n\
         else:\n\
             self.summa = price * count * 0.9\n\
+    \n\
     def __str__(self):\n\
-        return  f"Товар {self.code} в стоимость {self.price} за шт. \\n\
-в количестве {self.count} шт. Итоговая цена: {self.summa}"\n\
+        return f"Товар {self.code} стоимостью {self.price} за шт.\nв количестве {self.count} шт. Итоговая цена: {self.summa}"\n\
+    \n\
+    def summa_zakaza(self):\n\
+        return self.summa\n\
+\n\
+\n\
 class Retail(Order):\n\
-    def _init_(self, code, price, count):\n\
-        super().__init (code, price, count)\n\
+    def __init__(self, code, price, count):\n\
+        super().__init__(code, price, count)\n\
         self.summa = price * count\n\
-        def __str_ (self):\n\
-            return f"Товар {self.code} в стоимость {self.price} за шт. \\n\
-в количестве {self.count} шт. Итоговая цена: {self.summa}"\n\
+    \n\
+    def __str__(self):\n\
+        return f"Товар {self.code} стоимостью {self.price} за шт.\nв количестве {self.count} шт. Итоговая цена: {self.summa}"\n\
+    \n\
+    def summa_zakaza(self):\n\
+        return self.summa\n\
 \n\
-#Пример\n\
+\n\
+# Пример\n\
 a = Order("молоко_1", 80, 40)\n\
 b = Order("молоко_2", 98, 10)\n\
 c = Opt("шоколад_1", 119, 700)\n\
 d = Opt("шоколад_2", 39, 300)\n\
 e = Retail("хлеб", 48, 2)\n\
 f = Retail("мороженое", 99, 1)\n\
+\n\
 orders = [a, b, c, d, e, f]\n\
 for elem in orders:\n\
-    print (elem)\n\
-print(sum([c.summa, d.summa]))\n\
-print(sum([e.summa, f.summa]))\n\
+    print(elem)\n\
+\n\
+opt_retail_orders = [c, d, e, f]\n\
+total_opt_retail_sum = sum(order.summa_zakaza() for order in opt_retail_orders)\n\
+print(f"Общая стоимость заказов для объектов Opt и Retail: {total_opt_retail_sum}")\n\
 '
             ,
 #23
             'Создать класс Деньги':'Создать класс Деньги для работы с денежными суммами. Число должно быть представлено списком, состоящим из рублей и копеек. Реализовать сложение, вычитание, деление сумм, деление денежных сумм. (20 баллов)\n\
 class M():\n\
     summa = [0, 0]\n\
 \n\
@@ -930,15 +981,15 @@
     global string\n\
     while n:\n\
         string += str(n % 10)\n\
         n //= 10\n\
         return func(n)\n\
 \n\
 \n\
-string = ''\n\
+string = ""\n\
 func(int(input()))\n\
 print(string)'
             ,
 #28
             'Создайте класс Студент':'Создайте класс Студент, имеющий: \n\
 •	закрытый атрибут Имя – строка, содержащая фамилию; \n\
 •	метод __init__. При создании объекта указывается имя, список Дисциплины пустой; \n\
@@ -954,19 +1005,19 @@
     def put(self, subject: str, mark: int):\n\
         self.__subjects.setdefault (subject, mark)\n\
 \n\
     @property\n\
     def passed(self):\n\
         return list(self.__subjects.items())\n\
 \n\
-me = Student(«Kondrashov»)\n\
-me.put(«Math», 5)\n\
-me.put(«Programming», 5)\n\
-me.put(«History», 4)\n\
-print (me.passed)'
+me = Student("Kondrashov")\n\
+me.put("Math", 5)\n\
+me.put("Programming", 5)\n\
+me.put("History", 4)\n\
+print(me.passed)'
             ,
 #30-36
             'Дан однонаправленный связный':'Дан однонаправленный связный список. Вставить элемент после n-го элемента списка. (20 баллов)\n\
 class Node:\n\
     def __init__(self, data=None):\n\
         self.data = data\n\
         self.next = None\n\
@@ -1021,15 +1072,15 @@
 linked_list.insert_at_head("Элемент 4")\n\
 \n\
 print("Список до вставки:")\n\
 linked_list.display()\n\
 \n\
 linked_list.insert_after(1, "Вставленный элемент")\n\
 \n\
-print("\nСписок после вставки:")\n\
+print("Список после вставки:")\n\
 linked_list.display()\n\
 \n\
 \n\
 \n\
 \n\
 \n\
 Дан однонаправленный связный список. Удалить каждый второй элемент списка.\n\
@@ -1043,14 +1094,41 @@
     current = head\n\
     while current and current.next:\n\
         next_node = current.next\n\
         current.next = next_node.next\n\
         next_node = None\n\
         current = current.next\n\
     return head\n\
+head = Node(1)\n\
+node2 = Node(2)\n\
+node3 = Node(3)\n\
+node4 = Node(4)\n\
+node5 = Node(5)\n\
+\n\
+head.next = node2\n\
+node2.next = node3\n\
+node3.next = node4\n\
+node4.next = node5\n\
+\n\
+print("Исходный список:")\n\
+current = head\n\
+while current:\n\
+    print(current.data, end=" -> ")\n\
+    current = current.next\n\
+print("None")\n\
+\n\
+\n\
+head = delete_every_second_node(head)\n\
+\n\
+print("Список после удаления каждого второго узла:")\n\
+current = head\n\
+while current:\n\
+    print(current.data, end=" -> ")\n\
+    current = current.next\n\
+print("None")\n\
 '
             ,
 #31
             'Создать декоратор tol':'Создать декоратор tol(len, fill) с параметрами len и fill. Декоратор превращает результат декорируемой функции в список состоящий из len элементов. Если исходная функция возвращает меньше заданного количества элементов, то оставшиеся места заполняются значениями fill, в случае, если количество возвращаемых элементов больше len, то хвост последовательности отбрасывается.\n\
 \n\
 def tol(length, fill):\n\
     def decorator(func):\n\
@@ -1108,73 +1186,47 @@
     def display(self):\n\
         current = self.head\n\
         while current:\n\
             print(current.data, end=" ")\n\
             current = current.next\n\
         print()\n\
 # Создание связанного списка из строки\n\
-string = «Eeny, meeny, miney, moe; Catch a tiger by his toe.»\n\
+string = "Eeny, meeny, miney, moe; Catch a tiger by his toe."\n\
 linked_list = LinkedList()\n\
 for char in string:\n\
     linked_list.insert(char)\n\
 # Удаление элементов с гласными буквами\n\
 linked_list.remove_vowels()\n\
 # Вывод связанного списка\n\
-linked_list.display()'
+linked_list.display()\n\'
             ,
 #33
-            'Создать базовый класс':'Реализовать однонаправленный связанный список (реализовать класс для элементов списка). Преобразовать строку «Eeny, meeny, miney, moe; Catch a tiger by his toe.» в связный список символов строки и удалить из него все элементы содержащие гласные буквы.\n\
+            'Создать базовый класс':'Создать базовый класс по следующей предметной области. Известны оклад (зарплата) и ставка процента подоходного налога. Определить размер подоходного налога и сумму, получаемую на руки. Исходными данными являются величина оклада (переменная oklad, выражаемая числом) и ставка подоходного налога (переменная procent, выражаемая числом). Размер налога (переменная nalog) определяется как oklad∗procent/100, а сумма, получаемая на руки (переменная summa) — как oklad-nalog. \n\
 \n\
-class Node:\n\
-    def __init__(self, data):\n\
-        self.data = data\n\
-        self.next = None\n\
-class LinkedList:\n\
-    def __init__(self):\n\
-        self.head = None\n\
-    def insert(self, data):\n\
-        new_node = Node(data)\n\
-        if self.head is None:\n\
-            self.head = new_node\n\
-        else:\n\
-            current = self.head\n\
-            while current.next:\n\
-                current = current.next\n\
-            current.next = new_node\n\
-    def remove_vowels(self):\n\
-        if self.head is None:\n\
-            return\n\
-        current = self.head\n\
-        previous = None\n\
-        vowels = set("aeiouyAEIOUY")\n\
-        while current:\n\
-            if current.data in vowels:\n\
-                if previous:\n\
-                    previous.next = current.next\n\
-                else:\n\
-                    self.head = current.next\n\
-                current = current.next\n\
-            else:\n\
-                previous = current\n\
-                current = current.next\n\
-    def display(self):\n\
-        current = self.head\n\
-        while current:\n\
-            print(current.data, end=" ")\n\
-            current = current.next\n\
-        print()\n\
-# Создание связанного списка из строки\n\
-string = «Eeny, meeny, miney, moe; Catch a tiger by his toe.»\n\
-linked_list = LinkedList()\n\
-for char in string:\n\
-    linked_list.insert(char)\n\
-# Удаление элементов с гласными буквами\n\
-linked_list.remove_vowels()\n\
-# Вывод связанного списка\n\
-linked_list.display()'
+class Salary:\n\
+    def __init__(self, oklad, procent):\n\
+        self.oklad = oklad\n\
+        self.procent = procent\n\
+    def calculate_tax(self):\n\
+        nalog = self.oklad * self.procent / 100\n\
+        return nalog\n\
+    def calculate_net_salary(self):\n\
+        nalog = self.calculate_tax()\n\
+        summa = self.oklad - nalog\n\
+        return summa\n\
+# Пример использования\n\
+oklad = 1000000\n\
+procent = 13\n\
+salary = Salary(oklad, procent)\n\
+nalog = salary.calculate_tax()\n\
+summa = salary.calculate_net_salary()\n\
+print(f"Размер налога: {nalog}")\n\
+print(f"Сумма на руки: {summa}")\n\
+\n\
+'
             ,
 #35
             'Описать рекурсивные функции':'Описать рекурсивные функции Fact(N) и Fact2(N) вещественного типа, вычисляющие значения факториала N! и двойного факториала N!! соответственно (N > 0 — параметр целого типа).\n\
 def Fact(N):\n\
     if N == 0 or N == 1:\n\
         return 1\n\
     else:\n\
@@ -1252,18 +1304,18 @@
     def __init__(self, sort, country, weight):\n\
         self.index = Mango.generate_next_index()\n\
         self.sort = sort\n\
         self.country = country\n\
         self.weight = weight\n\
         \n\
     def price(self):\n\
-        return f»the price is {self.weight * 100}»\n\
+        return f"the price is {self.weight * 100}"\n\
     \n\
     def __str__(self):\n\
-        return f»Сорт манго - {self.sort}, страна - {self.country}, вес - {self.weight}»\n\
+        return f"Сорт манго - {self.sort}, страна - {self.country}, вес - {self.weight}"\n\
 \n\
 class Banana(Mango):\n\
     next_index = 0\n\
     \n\
     @classmethod\n\
     def generate_next_index(cls):\n\
         index = cls.next_index\n\
@@ -1291,22 +1343,22 @@
         super().__init__(sort, country, weight)\n\
         self.index = Apple.generate_next_index()\n\
         self.count = count\n\
         \n\
     def price(self):\n\
         return super().price()\n\
         \n\
-a1 = Apple(«red», «USA», 2, 3)\n\
+a1 = Apple("red", "USA", 2, 3)\n\
 a1.next_index\n\
-a2 = Apple(«blue», «Kazakhstan», 1, 4)\n\
+a2 = Apple("blue", "Kazakhstan", 1, 4)\n\
 a2.next_index\n\
-m = Mango(«dope», «Brazil», 0.2)\n\
-m1 = Mango(«aloa», «Brazil», 0.5)\n\
-m2 = Mango(«waergsedrgearg», «Rushka», 123)\n\
-m2.next_index'
+m = Mango("dope", "Brazil", 0.2)\n\
+m1 = Mango("aloa", "Brazil", 0.5)\n\
+m2 = Mango("waergsedrgearg", "Rushka", 123)\n\
+m2.next_index\n\'
             ,
 #38
             'Расположить по алфавиту':'Расположить по алфавиту имена владельцев и, соответственно, вывести информацию об их машинах.  Использовать алгоритм сортировки выбором.\n\
 \n\
 def selection_sort(owners, cars):\n\
     n = len(owners)\n\
     for i in range(n-1):\n\
@@ -1315,23 +1367,23 @@
             if owners[j] < owners[min_index]:\n\
                 min_index = j\n\
         if min_index != i:\n\
             owners[i], owners[min_index] = owners[min_index], owners[i]\n\
             cars[i], cars[min_index] = cars[min_index], cars[i]\n\
 \n\
 # Пример данных владельцев и их машин\n\
-owners = [«Alice», «Charlie», «Bob», «Eve»]\n\
-cars = [«Toyota», «Ford», «Honda», «BMW»]\n\
+owners = ["Alice", "Charlie", "Bob", "Eve"]\n\
+cars = ["Toyota", "Ford", "Honda", "BMW"]\n\
 \n\
 # Вызываем сортировку выбором\n\
 selection_sort(owners, cars)\n\
 \n\
 # Выводим информацию об отсортированных владельцах и их машинах\n\
 for i in range(len(owners)):\n\
-    print(f»Владелец: {owners[i]}, Машина: {cars[i]}»)'
+    print(f"Владелец: {owners[i]}, Машина: {cars[i]}")\n\'
             ,
 #39
             'Описать рекурсивную функцию':'Описать рекурсивную функцию Root (а, b, ε), которая методом деления отрезка пополам находит с точностью ε корень уравнения f(x) = 0 на отрезке [а, b] (считать, что ε > 0, а < b, f(a) – f(b) < 0 и f(x) — непрерывная и монотонная на отрезке [а, b] функция).\n\
 \n\
 def Root(a, b, ε):\n\
     c = (a + b) / 2  # Находим середину отрезка\n\
     if abs(f(c)) < ε:\n\
@@ -1549,20 +1601,20 @@
         self.first = None\n\
         self.last = None\n\
         self.lenght = 0\n\
 \n\
     def __str__(self):\n\
         if self.first != None:\n\
             current = self.first\n\
-            out = «LinkedList [« +str(current.value) +» «\n\
+            out = "LinkedList [" +str(current.value) +" "\n\
             while current.next != None:\n\
                 current = current.next\n\
-                out += str(current.value) + « «\n\
-            return out + «]»\n\
-        return «LinkedList []»\n\
+                out += str(current.value) + " "\n\
+            return out + "]"\n\
+        return "LinkedList []"\n\
     def add(self, x):\n\
         self.lenght+=1\n\
         if self.first == None:\n\
             self.last = self.first = Node(x, None)\n\
         else:\n\
             self.last.next = self.last = Node(x, None)\n\
             \n\
@@ -1590,15 +1642,17 @@
     for j in range(L2.lenght):\n\
         if current1.value == current2.value:\n\
             L3.add(current1.value)\n\
         current2 = current2.next\n\
     current1 = current1.next\n\
 print(L1)\n\
 print(L2)\n\
-print(L3)'
+print(L3)\n\
+
+'
             ,
 #48
             'Создать класс Профиль':'Создать класс Профиль местности, который хранит последовательность высот, вычисленных через равные промежутки по горизонтали. Методы: наибольшая высота, наименьшая высота, перепад высот (наибольший, суммарный), крутизна (тангенс угла наклона; наибольшая, средняя), сравнение двух профилей одинаковой длины (по перепаду, по крутизне). (20 баллов)\n\
 class Profile:\n\
     def __init__(self, heights):\n\
         self.heights = heights\n\
 \n\
@@ -1702,30 +1756,30 @@
             t.right_child = self.right_child\n\
             self.right_child = t\n\
             \n\
     def set_parent(self, node):\n\
         self.parent = BinaryNode(node)\n\
         \n\
     def __str__(self):\n\
-        return «{} ({}, {})».format(str(self.get_val()), str(self.get_left_child()), str(self.get_right_child()))\n\
+        return "{} ({}, {})".format(str(self.get_val()), str(self.get_left_child()), str(self.get_right_child()))\n\
     \n\
 def in_order(node):\n\
     if node:\n\
         in_order(node.left_child)\n\
-        print(node.get_val(), end = « «)\n\
+        print(node.get_val(), end = " ")\n\
         in_order(node.right_child)\n\
         \n\
 r = BinaryNode(5)\n\
 r.set_left_child(7)\n\
 r.set_right_child(6)\n\
 r.get_left_child().set_left_child(10)\n\
 r.get_left_child().set_right_child(30)\n\
 r.set_right_child(20)\n\
 r.__str__()\n\
-in_order(r)'
+in_order(r)\n\'
             ,
 #51-55
             'В одномерном массиве':'В одномерном массиве целых чисел найти количество пар элементов разного знака. (пара — это два рядом стоящих элемента). (20 баллов)\n\
 counter = 0 # счетчик для пар \n\
 array = [1, -1, 2, 4 ,5, -6, 2, 3]\n\
 for i in range(len(array)-1):\n\
     if array[i] < 0 and array[i+1] > 0: # проверка знаков\n\
@@ -1924,14 +1978,15 @@
 while current:\n\
     print(current.data, end=" ")\n\
     current = current.next'}
 
         print(sklad[number])
 
     def theory(number=''):
+        #1
         sklad = {'Концепция класса и': 'Класс — в объектно-ориентированном программировании, представляет собой шаблон для создания объектов, обеспечивающий начальные значения состояний: инициализация полей-переменных и реализация поведения функций или методов.\n\
 Объект — некоторая сущность в цифровом пространстве, обладающая определённым состоянием и поведением, имеющая определенные свойства (атрибуты) и операции над ними (методы). Как правило, при рассмотрении объектов выделяется то, что объекты принадлежат одному или нескольким классам, которые определяют поведение (являются моделью) объекта. Термины «экземпляр класса» и «объект» взаимозаменяемы.\n\
 Парадигма ООП построена на 3 основных принципах:\n\
 Инкапсуляция – сокрытие данных, т. е. классы не имеют прямого доступа к полям друг друга, а взаимодействие между ними осуществляется через публичные методы.\n\
 Наследование – название говорит само за себя. Дочерний класс наследует свойства и методы родительского, тем самым реализуя повторное использование. \n\
 Полиморфизм – это способность одного и того же объекта вести себя по-разному в зависимости от того, в контексте какого класса он используется. Полиморфизм связан с созданием перегружаемых виртуальных методов.\n\
 '
@@ -2073,15 +2128,15 @@
 update_wrapper()\n\
 Используется для обновления метаданных функции-обертки, данными из некоторых атрибутов оборачиваемой функции. Обеспечивает лучшую читаемость и возможность повторного использования кода.\n\
 @lru_cache\n\
 lru_cache — это декоратор. То есть обёртка, которая может изменить поведение функции, не меняя её код. Lru_cache даёт выбранной функции кэширование, чтобы фиксировать результаты тяжеловесных вычислений, запросов или других операций.\n\
 '
                  ,
 #5
-                 'функции граждане': '5.Концепция «функции – граждане первого класса» в языке программирования, поддержка этой концепции в Python. Специфика лямбда-функций в Python их возможности и ограничения. Типичные сценарии использования лямбда-функций в Python.\n\
+                 'Концепция функции граждане': '5.Концепция «функции – граждане первого класса» в языке программирования, поддержка этой концепции в Python. Специфика лямбда-функций в Python их возможности и ограничения. Типичные сценарии использования лямбда-функций в Python.\n\
 \n\
 Концепция «функции – граждане первого класса» в языке программирования, поддержка этой концепции в Python\n\
    Концепция «функции – граждане первого класса» в языке программирования\n\
 Функции в языке программирования считаются гражданами первого класса, если они демонстрируют следующие характеристики.\n\
 •	Их можно хранить в переменных.\n\
 •	Их можно хранить в структурах данных.\n\
 •	Их можно пропустить как аргумент к функции.\n\
@@ -2215,15 +2270,15 @@
        fn(arg)\n\
    return wrapper\n\
 @param_transfer\n\
 def print_sqrt(num):\n\
    print(num**0.5)'
                  ,
 #9                 
-                 'Концепция map/filter/reduce. Реализация':'9.Концепция map/filter/reduce. Реализация map/filter/reduce в Python и пример их использования.\n\
+                 'Концепция map filter':'9.Концепция map/filter/reduce. Реализация map/filter/reduce в Python и пример их использования.\n\
 \n\
 В Python функция map принимает два аргумента: функцию и аргумент составного типа данных, например, список. map применяет к каждому элементу списка переданную функцию. Например, вы прочитали из файла список чисел, изначально все эти числа имеют строковый тип данных, чтобы работать с ними - нужно превратить их в целое число:\n\
 old_list = [1, 2, 3, 4, 5,6, 7]\n\
 new_list = list(map(int, old_list))\n\
 print (new_list)\n\
 [1, 2, 3, 4, 5, 6, 7]\n\
 \n\
```

