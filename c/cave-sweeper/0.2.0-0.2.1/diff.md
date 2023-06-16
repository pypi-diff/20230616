# Comparing `tmp/cave_sweeper-0.2.0.tar.gz` & `tmp/cave_sweeper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_sweeper-0.2.0.tar", max compression
+gzip compressed data, was "cave_sweeper-0.2.1.tar", max compression
```

## Comparing `cave_sweeper-0.2.0.tar` & `cave_sweeper-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-11 20:24:03.431189 cave_sweeper-0.2.0/README.md
--rw-r--r--   0        0        0     5666 2023-05-11 20:56:44.465333 cave_sweeper-0.2.0/cave_sweeper/field_slot.py
--rw-r--r--   0        0        0      117 2023-05-11 20:56:44.458751 cave_sweeper-0.2.0/cave_sweeper/mine_sweeper.py
--rw-r--r--   0        0        0     4429 2023-05-11 20:56:44.471839 cave_sweeper-0.2.0/cave_sweeper/renderers.py
--rw-r--r--   0        0        0       55 2023-05-05 22:02:44.764403 cave_sweeper-0.2.0/cave_sweeper/settings.py
--rw-r--r--   0        0        0      188 2023-05-05 21:13:27.324715 cave_sweeper-0.2.0/cave_sweeper/utils.py
--rw-r--r--   0        0        0      368 2023-05-11 20:58:11.365039 cave_sweeper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 cave_sweeper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-11 20:24:03.431189 cave_sweeper-0.2.1/README.md
+-rw-r--r--   0        0        0      461 2023-06-16 15:11:47.585389 cave_sweeper-0.2.1/cave_sweeper/button.py
+-rw-r--r--   0        0        0     5850 2023-06-16 17:51:09.344038 cave_sweeper-0.2.1/cave_sweeper/field_slot.py
+-rw-r--r--   0        0        0      117 2023-05-11 20:56:44.458751 cave_sweeper-0.2.1/cave_sweeper/mine_sweeper.py
+-rw-r--r--   0        0        0     4950 2023-06-16 17:52:03.060155 cave_sweeper-0.2.1/cave_sweeper/renderers.py
+-rw-r--r--   0        0        0       55 2023-05-05 22:02:44.764403 cave_sweeper-0.2.1/cave_sweeper/settings.py
+-rw-r--r--   0        0        0     1160 2023-06-16 15:21:29.829832 cave_sweeper-0.2.1/cave_sweeper/style_checker.py
+-rw-r--r--   0        0        0      188 2023-05-05 21:13:27.324715 cave_sweeper-0.2.1/cave_sweeper/utils.py
+-rw-r--r--   0        0        0      368 2023-06-16 17:53:34.739658 cave_sweeper-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 cave_sweeper-0.2.1/PKG-INFO
```

### Comparing `cave_sweeper-0.2.0/cave_sweeper/field_slot.py` & `cave_sweeper-0.2.1/cave_sweeper/field_slot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from tkinter import Button, Frame, messagebox
+from tkinter import Button, Frame, messagebox, ttk
 from random import randint
 from cave_sweeper.utils import count_digits
 from cave_sweeper.settings import DIFFICULTY_MAPPING
 
 
 class Field(Frame):
 
@@ -22,14 +22,20 @@
         self._mines = []
 
         # a counter to keep track of how many buttons have been
         # opened or flagged
         self.swept = 0
 
     @property
+    def btn_size(self):
+        first_btn = self.all_buttons.get((0,0))
+        first_btn.update()
+        return first_btn.winfo_width(), first_btn.winfo_height()
+
+    @property
     def columns(self):
         return int(os.environ.get("MINEFIELD_COLUMNS", 8))
 
     @property
     def rows(self):
         return int(os.environ.get("MINEFIELD_ROWS", 8))
```

### Comparing `cave_sweeper-0.2.0/cave_sweeper/renderers.py` & `cave_sweeper-0.2.1/cave_sweeper/renderers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 import os
-from tkinter import Tk, Label, Radiobutton, ttk, StringVar, Button, Frame
+from tkinter import Tk, Label, ttk, StringVar, Frame, N, W, E, S
 from cave_sweeper.field_slot import Field
-from cave_sweeper.utils import count_digits
 
 
 def render_selection_window():
     def _render_minefield_window():
         os.environ["MINEFIELD_COLUMNS"] = cols_combo.get()
         os.environ["MINEFIELD_ROWS"] = rows_combo.get()
         os.environ["DIFFICULTY"] = difficulty.get()
         selection_window.destroy()
         render_minefield_window()
 
     selection_window = Tk()
     selection_window.title("Pick your settings")
-    selection_window.geometry("350x400")
+    selection_frame = ttk.Frame(selection_window, padding="50 50 50 50")
+    selection_frame.grid(column=0, row=0, sticky=(N, E, W, S))
+    selection_window.columnconfigure(0, weight=1)
+    selection_window.rowconfigure(0, weight=1)
+
+    #ROW1
+    rows_combo_label = ttk.Label(master=selection_frame, text="Rows: ")
+    rows_combo_label.grid(row=1, column=1, sticky=W)
 
-    rows_combo_label = Label(master=selection_window, text="Rows: ")
-    rows_combo_label.place(x=125, y=150)
-
-    rows_combo = ttk.Combobox(selection_window, width=5)
+    rows_combo = ttk.Combobox(selection_frame, width=5)
     rows_combo['values'] = (10, 15, 20, 25)
+    rows_combo.state(["readonly"])
     rows_combo.set(10)
-    rows_combo.place(x=170, y=150)
+    rows_combo.grid(row=1, column=2, sticky=E)
 
-    cols_combo_label = Label(master=selection_window, text="Cols: ")
-    cols_combo_label.place(x=125, y=175)
+    #ROW 2
+    cols_combo_label = ttk.Label(master=selection_frame, text="Cols: ")
+    cols_combo_label.grid(row=2, column=1, sticky=W)
 
-    cols_combo = ttk.Combobox(selection_window, width=5)
+    cols_combo = ttk.Combobox(selection_frame, width=5)
     cols_combo['values'] = (10, 15, 20, 25)
+    cols_combo.state(["readonly"])
     cols_combo.set(10)
-    cols_combo.place(x=170, y=175)
+    cols_combo.grid(row=2, column=2, sticky=E)
 
+    #ROW 3
     difficulty = StringVar()
     difficulty.set("easy")
 
-    rb_easy = Radiobutton(master=selection_window, text="Easy", variable=difficulty, value="easy")
-    rb_easy.place(x=125, y=225)
-
-    rb_hard = Radiobutton(master=selection_window, text="Hard", variable=difficulty, value="hard")
-    rb_hard.place(x=200, y=225)
+    rb_easy = ttk.Radiobutton(master=selection_frame, text="Easy", variable=difficulty, value="easy")
+    rb_easy.grid(row=3, column=1, sticky=W)
 
-    btn_ok = Button(master=selection_window, text="OK", width=4, height=2, command=_render_minefield_window)
-    btn_ok.place(x=100, y=300)
+    rb_hard = ttk.Radiobutton(master=selection_frame, text="Hard", variable=difficulty, value="hard")
+    rb_hard.grid(row=3, column=2, sticky=E)
 
-    btn_close = Button(master=selection_window, text="Close", width=4, height=2, command=selection_window.quit)
-    btn_close.place(x=200, y=300)
+    #ROW 4
+    btn_ok = ttk.Button(master=selection_frame, text="OK", width=4, command=_render_minefield_window)
+    btn_ok.grid(row=4, column=1, sticky=W)
+
+    btn_close = ttk.Button(master=selection_frame, text="Close", width=4, command=selection_window.quit)
+    btn_close.grid(row=4, column=2, sticky=E)
+
+    # adds extra spacing between widgets and the borders of 'selection_frame'
+    for child in selection_frame.winfo_children():
+        child.grid_configure(padx=5, pady=5)
 
     selection_window.mainloop()
 
 
 def render_minefield_window():
     MINEFIELD_COLUMNS = int(os.environ.get("MINEFIELD_COLUMNS", 8))
     MINEFIELD_ROWS = int(os.environ.get("MINEFIELD_ROWS", 8))
     countdown_time = MINEFIELD_COLUMNS * MINEFIELD_COLUMNS * 2
 
     root = Tk()
     # styling of the main app window
     root.title("Minefield")
-    root.geometry(f"{MINEFIELD_COLUMNS*48 + 20}x{MINEFIELD_ROWS*38 + 130}")
-    root.resizable(width=True, height=True)
     root.configure(bg="lightgray")
 
     # display
-    display_frame = Frame(master=root, bg="grey21", width=MINEFIELD_COLUMNS*48, height=100)
+    display_frame = ttk.Frame(master=root, width=MINEFIELD_COLUMNS*48, height=100)
     display_frame.place(x=10, y=10)
 
     # label to display amount of fields remaining
-    remaining_label = Label(master=display_frame, bg="dim gray")
+    remaining_label = ttk.Label(master=display_frame, background="black", foreground="brown1")
     remaining_label.config(
         font=("consolas", 50),
-        width=count_digits(MINEFIELD_COLUMNS * MINEFIELD_ROWS),
-        height=1,
-        fg="brown1",
         text=MINEFIELD_COLUMNS * MINEFIELD_ROWS
     )
     remaining_label.place(x=10, y=14)
 
 
     # label to display amount of mines
     mines_label = Label(master=display_frame, bg="dim gray")
@@ -131,9 +138,13 @@
             countdown_time -= 1
             root.after(1000, update_label)
         else:
             mf_frame.game_over(timeout=True)
             pass
 
     root.after(1000, update_label)
+
     # renders the app window
+    mine_btn_width, mine_btn_heigth = mf_frame.btn_size
+    root.geometry(f"{MINEFIELD_COLUMNS*mine_btn_width + 20}x{MINEFIELD_ROWS*mine_btn_heigth + 130}")
+    root.resizable(width=False, height=False)
     root.mainloop()
```

