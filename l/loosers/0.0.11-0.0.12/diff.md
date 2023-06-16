# Comparing `tmp/loosers-0.0.11.tar.gz` & `tmp/loosers-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loosers-0.0.11.tar", last modified: Fri Jun 16 21:24:18 2023, max compression
+gzip compressed data, was "loosers-0.0.12.tar", last modified: Fri Jun 16 21:38:25 2023, max compression
```

## Comparing `loosers-0.0.11.tar` & `loosers-0.0.12.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.350631 loosers-0.0.11/
--rw-rw-rw-   0        0        0      124 2023-06-16 21:24:18.350631 loosers-0.0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.335006 loosers-0.0.11/loosers/
--rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 loosers-0.0.11/loosers/__init__.py
--rw-rw-rw-   0        0        0   190232 2023-06-16 21:12:44.000000 loosers-0.0.11/loosers/tvz.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:24:18.350631 loosers-0.0.11/loosers.egg-info/
--rw-rw-rw-   0        0        0      124 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 21:24:18.000000 loosers-0.0.11/loosers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-06-16 21:24:18.350631 loosers-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-16 21:23:22.000000 loosers-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:38:25.612619 loosers-0.0.12/
+-rw-rw-rw-   0        0        0      124 2023-06-16 21:38:25.612619 loosers-0.0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 21:38:25.602622 loosers-0.0.12/loosers/
+-rw-rw-rw-   0        0        0       18 2023-06-05 15:45:24.000000 loosers-0.0.12/loosers/__init__.py
+-rw-rw-rw-   0        0        0   190213 2023-06-16 21:37:03.000000 loosers-0.0.12/loosers/tvz.py
+drwxrwxrwx   0        0        0        0 2023-06-16 21:38:25.611618 loosers-0.0.12/loosers.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-06-16 21:38:25.000000 loosers-0.0.12/loosers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-16 21:38:25.000000 loosers-0.0.12/loosers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 21:38:25.000000 loosers-0.0.12/loosers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 21:38:25.000000 loosers-0.0.12/loosers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-16 21:38:25.614617 loosers-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-16 21:37:41.000000 loosers-0.0.12/setup.py
```

### Comparing `loosers-0.0.11/loosers/tvz.py` & `loosers-0.0.12/loosers/tvz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1193,15 +1193,15 @@
 string = "Eeny, meeny, miney, moe; Catch a tiger by his toe."\n\
 linked_list = LinkedList()\n\
 for char in string:\n\
     linked_list.insert(char)\n\
 # Удаление элементов с гласными буквами\n\
 linked_list.remove_vowels()\n\
 # Вывод связанного списка\n\
-linked_list.display()\n\'
+linked_list.display()'
             ,
 #33
             'Создать базовый класс':'Создать базовый класс по следующей предметной области. Известны оклад (зарплата) и ставка процента подоходного налога. Определить размер подоходного налога и сумму, получаемую на руки. Исходными данными являются величина оклада (переменная oklad, выражаемая числом) и ставка подоходного налога (переменная procent, выражаемая числом). Размер налога (переменная nalog) определяется как oklad∗procent/100, а сумма, получаемая на руки (переменная summa) — как oklad-nalog. \n\
 \n\
 class Salary:\n\
     def __init__(self, oklad, procent):\n\
         self.oklad = oklad\n\
@@ -1350,15 +1350,15 @@
 a1 = Apple("red", "USA", 2, 3)\n\
 a1.next_index\n\
 a2 = Apple("blue", "Kazakhstan", 1, 4)\n\
 a2.next_index\n\
 m = Mango("dope", "Brazil", 0.2)\n\
 m1 = Mango("aloa", "Brazil", 0.5)\n\
 m2 = Mango("waergsedrgearg", "Rushka", 123)\n\
-m2.next_index\n\'
+m2.next_index'
             ,
 #38
             'Расположить по алфавиту':'Расположить по алфавиту имена владельцев и, соответственно, вывести информацию об их машинах.  Использовать алгоритм сортировки выбором.\n\
 \n\
 def selection_sort(owners, cars):\n\
     n = len(owners)\n\
     for i in range(n-1):\n\
@@ -1375,15 +1375,15 @@
 cars = ["Toyota", "Ford", "Honda", "BMW"]\n\
 \n\
 # Вызываем сортировку выбором\n\
 selection_sort(owners, cars)\n\
 \n\
 # Выводим информацию об отсортированных владельцах и их машинах\n\
 for i in range(len(owners)):\n\
-    print(f"Владелец: {owners[i]}, Машина: {cars[i]}")\n\'
+    print(f"Владелец: {owners[i]}, Машина: {cars[i]}")'
             ,
 #39
             'Описать рекурсивную функцию':'Описать рекурсивную функцию Root (а, b, ε), которая методом деления отрезка пополам находит с точностью ε корень уравнения f(x) = 0 на отрезке [а, b] (считать, что ε > 0, а < b, f(a) – f(b) < 0 и f(x) — непрерывная и монотонная на отрезке [а, b] функция).\n\
 \n\
 def Root(a, b, ε):\n\
     c = (a + b) / 2  # Находим середину отрезка\n\
     if abs(f(c)) < ε:\n\
@@ -1642,17 +1642,15 @@
     for j in range(L2.lenght):\n\
         if current1.value == current2.value:\n\
             L3.add(current1.value)\n\
         current2 = current2.next\n\
     current1 = current1.next\n\
 print(L1)\n\
 print(L2)\n\
-print(L3)\n\
-
-'
+print(L3)'
             ,
 #48
             'Создать класс Профиль':'Создать класс Профиль местности, который хранит последовательность высот, вычисленных через равные промежутки по горизонтали. Методы: наибольшая высота, наименьшая высота, перепад высот (наибольший, суммарный), крутизна (тангенс угла наклона; наибольшая, средняя), сравнение двух профилей одинаковой длины (по перепаду, по крутизне). (20 баллов)\n\
 class Profile:\n\
     def __init__(self, heights):\n\
         self.heights = heights\n\
 \n\
@@ -1771,15 +1769,15 @@
 r = BinaryNode(5)\n\
 r.set_left_child(7)\n\
 r.set_right_child(6)\n\
 r.get_left_child().set_left_child(10)\n\
 r.get_left_child().set_right_child(30)\n\
 r.set_right_child(20)\n\
 r.__str__()\n\
-in_order(r)\n\'
+in_order(r)'
             ,
 #51-55
             'В одномерном массиве':'В одномерном массиве целых чисел найти количество пар элементов разного знака. (пара — это два рядом стоящих элемента). (20 баллов)\n\
 counter = 0 # счетчик для пар \n\
 array = [1, -1, 2, 4 ,5, -6, 2, 3]\n\
 for i in range(len(array)-1):\n\
     if array[i] < 0 and array[i+1] > 0: # проверка знаков\n\
```

