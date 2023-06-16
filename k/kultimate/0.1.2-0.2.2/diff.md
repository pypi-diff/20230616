# Comparing `tmp/kultimate-0.1.2.tar.gz` & `tmp/kultimate-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.1.2.tar", max compression
+gzip compressed data, was "kultimate-0.2.2.tar", max compression
```

## Comparing `kultimate-0.1.2.tar` & `kultimate-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1821 2023-06-14 22:57:08.956615 kultimate-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.1.2/kultimate/__init__.py
--rw-r--r--   0        0        0     1405 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/app.css
--rw-r--r--   0        0        0    18118 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/app.py
--rw-r--r--   0        0        0       64 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.1.2/kultimate/screens/addTask.py
--rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.1.2/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.1.2/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.1.2/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     2043 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     2417 2023-06-14 21:37:13.313178 kultimate-0.1.2/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.1.2/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.1.2/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.1.2/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.1.2/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.1.2/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.1.2/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-14 22:59:22.633285 kultimate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 kultimate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3303 2023-06-15 16:08:28.186725 kultimate-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.2.2/kultimate/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-15 17:00:17.893459 kultimate-0.2.2/kultimate/app.css
+-rw-r--r--   0        0        0    20867 2023-06-16 17:10:05.146824 kultimate-0.2.2/kultimate/app.py
+-rw-r--r--   0        0        0      100 2023-06-15 16:48:15.913444 kultimate-0.2.2/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.2.2/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.2.2/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.2/kultimate/screens/selectFile.py
+-rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.2.2/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.2.2/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.2/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.2/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.2/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.2/kultimate/utils/prueba.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.2/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.2/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.2/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.2/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.2/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-16 17:15:41.136831 kultimate-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 kultimate-0.2.2/PKG-INFO
```

### Comparing `kultimate-0.1.2/kultimate/app.css` & `kultimate-0.2.2/kultimate/app.css`

 * *Files 22% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ._actual > Task._active {
   color: $background-darken-3;
   border: inner $error-lighten-2;
   background: $warning-lighten-1;
 }
 
-DeleteTask, AddTask {
+DeleteTask, AddTask, SelectAFile {
   align: center middle;
 }
 
 #dialog {
   grid-size: 2;
   grid-gutter: 1 2;
   grid-rows: 1fr 3;
@@ -76,10 +76,13 @@
 #question {
   column-span: 2;
   height: 1fr;
   width: 1fr;
   content-align: center middle;
 }
 
+
 Button {
   width: 100%;
+  align: center middle;
+  content-align: center middle;
 }
```

### Comparing `kultimate-0.1.2/kultimate/app.py` & `kultimate-0.2.2/kultimate/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from pathlib import Path
 
 from textual.app import App, ComposeResult
 from textual.css.query import QueryError
 from textual.reactive import var
 from textual.widgets import Footer, Header
 
-from .screens import AddTask, DeleteTask
+from .screens import AddTask, DeleteTask, SelectAFile
 from .utils import ParserMarkdown, StagesToMarkdown
 from .widgets import Directory, Stage, StagesContainer, Task
 
 # DONE: Hay errores al navegar entre las columnas.
 
 
 class KanbanUltimate(App):
     """The main app class"""
 
     TITLE = "KUltimate"
     SUB_TITLE = "Using Kanban with Markdown"
     CSS_PATH = "app.css"
-    SCREENS = {"delete_task": DeleteTask, "add_task": AddTask}
+    SCREENS = {
+        "delete_task": DeleteTask,
+        "add_task": AddTask,
+        "select_file": SelectAFile,
+    }
 
     BINDINGS = [
         ("s", "select_file", "Select File"),
         # opción temporal, el archivo se debe guardar
         # cada que se modifique el contenido
         ("o", "add_task", "Add Task"),  # DONE: Guardar archivo
         ("ctrl+l", "mark_as_done", "Mark as Done"),  # DONE: Guardar archivo
         ("ctrl+d", "delete_task", "Delete Task"),  # DONE: Guardar archivo
         ("q", "quit", "Quit"),
         # inician las teclas sin leyendas
         ("l, right", "go_to_right"),
         ("h, left", "go_to_left"),
         ("j, down", "go_to_down"),
         ("k, up", "go_to_up"),
-        ("J, s+down", "move_down"),  # DONE: Guardar archivo
-        ("K, s+up", "move_up"),  # DONE: Guardar archivo
-        ("H, s+left", "move_left"),  # DONE: Guardar archivo
-        ("L, s+right", "move_right"),  # DONE: Guardar archivo
+        ("J, shift+down", "move_down"),  # DONE: Guardar archivo
+        ("K, shift+up", "move_up"),  # DONE: Guardar archivo
+        ("H, shift+left", "move_left"),  # DONE: Guardar archivo
+        ("L, shift+right", "move_right"),  # DONE: Guardar archivo
     ]
 
     home_user = Path.home()
     # home_directory = "Dropbox/kanban2"
     is_directory_visible = False
     total_stages = 0
     current_stage = 0
@@ -96,14 +100,63 @@
             self.list_tasks[self.current_task].add_class(
                 self.class_for_active_task,
             )
             self.__focus_task()
         except IndexError:
             pass
 
+    def __remove_class_active_for_stage(self, stage: int) -> None:
+        """remove self.class_for_active_stage"""
+        try:
+            self.list_stages[stage].remove_class(self.class_for_active_stage)
+        except IndexError:
+            pass
+
+    async def __remove_task(self, task: int) -> None:
+        """Remove task from self.list_tasks"""
+        try:
+            self.list_tasks[task].remove()
+        except IndexError:
+            pass
+
+    def __update_list_tasks(self, stage: int) -> None:
+        """Actualiza la lista de tareas"""
+        try:
+            self.list_tasks = self.list_stages[stage].query(Task)
+            self.total_tasks = len(self.list_tasks) - 1
+            self.current_task = 0
+        except QueryError:
+            self.total_tasks = 0
+            self.current_task = 0
+            pass
+
+    def __add_class_for_active_task(self, current_task: int) -> None:
+        """Add class self.class_for_active_task"""
+        try:
+            self.list_tasks[current_task].add_class(self.class_for_active_task)
+            self.list_tasks[current_task].scroll_visible(force=True)
+        except IndexError:
+            pass
+
+    def __remove_class_for_active_task(self, current_task: int) -> None:
+        """Add class self.class_for_active_task"""
+        try:
+            self.list_tasks[current_task].remove_class(
+                self.class_for_active_task,
+            )
+        except IndexError:
+            pass
+
+    def __add_class_for_active_stage(self, stage: int) -> None:
+        """Add class self.class_for_active_stage"""
+        try:
+            self.list_stages[stage].add_class(self.class_for_active_stage)
+        except IndexError:
+            pass
+
     def __activate_stage(
         self,
         old_stage: int,
         scroll_to_task: bool = True,
     ) -> None:
         """Elimina la clase self.class_for_active_stage para la
         columna old_stage y la agrega para current_stage.
@@ -191,48 +244,51 @@
                 self.__actualize_total_tasks()
                 self.current_task = self.total_tasks
                 self.__new_active_task(old_task)
 
                 # guardar al archivo
                 self.__save_to_file()
 
-        self.push_screen("add_task", get_value_from_input)
+        if self.actual_file:
+            self.push_screen("add_task", get_value_from_input)
+        else:
+            self.push_screen("select_file")
 
     def action_delete_task(self) -> None:
         """Delete task from stage"""
 
-        def check_delete_task(delete_task: bool) -> None:
+        async def check_delete_task(delete_task: bool) -> None:
             """Called when DeleteTask is dismissed"""
             if delete_task:
                 if len(self.list_tasks) > 0:
-                    self.list_tasks[self.current_task].remove()
+                    await self.list_tasks[self.current_task].remove()
                     # actualizar self.total_tasks
                     self.__actualize_total_tasks()
 
                     if self.current_task == self.total_tasks + 1:
                         self.current_task = self.total_tasks
 
                     # resaltar la nueva tarea y hacer scroll
                     self.__select_task()
 
                     # guardar al archivo
                     self.__save_to_file()
 
         self.push_screen("delete_task", check_delete_task)
 
-    def action_mark_as_done(self) -> None:
+    async def action_mark_as_done(self) -> None:
         """Send task to last stage"""
         if self.current_stage != self.total_stages:
             if self.total_tasks == 0:
                 return
 
             # copiar el texto de la tarea
             text_task_done = self.list_tasks[self.current_task].renderable
             # eliminar la tarea de la columna actual
-            self.list_tasks[self.current_task].remove()
+            await self.list_tasks[self.current_task].remove()
             # actualizar self.total_tasks y self.current_task
 
             self.__actualize_total_tasks()
 
             if self.current_task == self.total_tasks + 1:
                 self.current_task = self.total_tasks
 
@@ -398,31 +454,43 @@
 
         self.interchange_task(index)
 
         # guardar al archivo
         self.__save_to_file()
 
     async def move_task(self, new_stage) -> None:
-        """mover tarea entre columnas"""
+        """mover tarea entre columnas, esta recibe la nueva columna
+        a la cual se va a mover, por tanto, self.current_stage
+        es la columna actual"""
         if new_stage != self.current_stage:
-            # copiar texto de la tarea
+            # ambas columnas son distintas
+
+            # guardar el texto de la tarea a mover
             text_to_move = self.list_tasks[self.current_task].renderable
-            # eliminar tarea de la columna actual
-            self.list_tasks[self.current_task].remove()
-            # agregar tarea a la nueva columna
-            task_to_move = Task(text_to_move)
+            # remover la tarea de la columna actual
+            await self.__remove_task(self.current_task)
+            # DONE: Separar select y unselect stage
+            # quitar la clase self.class_for_active_stage de la columna actual
             old_stage = self.current_stage
+            self.__remove_class_active_for_stage(old_stage)
+            # actualizar self.list_tasks - creo que esto no es necesario
+            # Moverse a la nueva columna
             self.current_stage = new_stage
-            await self.list_stages[self.current_stage].mount(task_to_move)
-            self.__activate_stage(old_stage, False)
-            # deseleccionar la tarea 0
-            # self.__unselect_task()
-            # resaltar la nueva tarea
+            self.__update_list_tasks(new_stage)
+            # agregar self.class_for_active_stage a la nueva columna
+            self.__add_class_for_active_stage(new_stage)
+            # agregar la tarea a la nueva columna
+            moved_task = Task(text_to_move)
+            await self.list_stages[new_stage].mount(moved_task)
+            self.__update_list_tasks(new_stage)
             self.current_task = self.total_tasks
-            self.__select_task()
+            # agregar self.class_for_active_task a la tarea agregada
+            self.__add_class_for_active_task(self.current_task)
+            # actualizar self.list_tasks
+            pass
 
     async def action_move_left(self) -> None:
         """Mover la tarea a la columna de la izquierda. Se presionó H"""
         new_stage = self.current_stage
         if new_stage > 0:
             new_stage -= 1
         else:
@@ -447,73 +515,79 @@
         self.__save_to_file()
 
     def __save_to_file(self) -> None:
         """Guardar el archivo. Función temporal,
         pues no será llamada directamente, sino cada vez
         que se modifique el contenido"""
         if self.actual_file:
-            # stages_to_markdown = StagesToMarkdown(self.actual_file)
-            self.stages_to_markdown.structure_to_markdown(self.list_stages)
+            # actualizar stages
+            try:
+                self.list_stages = self.query(Stage)
+                self.stages_to_markdown.set_file(self.actual_file)
+                self.stages_to_markdown.structure_to_markdown(self.list_stages)
+            except QueryError:
+                pass
 
-    def unmount_stages(self) -> None:
+    async def unmount_stages(self) -> None:
         """Desmonta las columnas"""
         # DONE: Desmontar las columnas actuales - usar remove
         try:
             stages = self.query(Stage)
             for stage in stages:
-                stage.remove()
+                await stage.remove()
         except IndexError:
             pass
 
     async def mount_stages(self) -> None:
         """Monta las columnas"""
         # DONE: Montar las nuevas columnas. Usar mount
         try:
             stages_container = self.query_one("#stages_container")
-            stages = self.parser_content.get_stages()
-            tasks = self.parser_content.get_tasks()
+            board = self.parser_content.get_board()
             # DONE: Montar tareas en las columnas
-            for index, stage in enumerate(stages):
+            index = 0
+            for stage in board.keys():
                 new_stage = Stage()
-                new_stage.set_title(stage.text)
+                new_stage.set_title(stage)
                 # DONE:Errores al desplegar los movimientos entre J y K
                 # DONE: Mover tareas con H y L
                 first_task = True
-                for task in tasks[index]:
+                for task in board[stage]:
                     new_task = Task(task)
                     await new_stage.mount(new_task)
                     # DONE: Que la primer tarea obtenga el foco
                     if index == 0 and first_task:
                         new_task.focus()
                         first_task = False
                         new_task.add_class(self.class_for_active_task)
 
                 await stages_container.mount(new_stage)
+                index += 1
 
             self.get_total_stages()
 
             self.__scroll_and_focus_stage()
             # self.current_task = self.total_tasks
             self.__focus_task()
 
         except IndexError:
-            with open("/home/felipe/Dropbox/kanban2/nel.txt", "w") as ff:
+            with open("/home/felipe/Dropbox/kanban3/nel.txt", "w") as ff:
                 ff.write("nel")
 
     # DONE: Seleccionar un archivo para mostrar.
     # File selected
     async def on_directory_tree_file_selected(
         self,
         event: Directory.FileSelected,
     ) -> None:
         event.stop()
         self.actual_file = str(event.path)
         # Ocultar Directory
         self.parser_content = ParserMarkdown(self.actual_file)
         self.action_select_file()
-        self.unmount_stages()
+        await self.unmount_stages()
         await self.mount_stages()
         self.refresh()
 
 
 def main(path: str) -> None:
     KanbanUltimate(path).run()
```

### Comparing `kultimate-0.1.2/kultimate/screens/addTask.py` & `kultimate-0.2.2/kultimate/screens/addTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.2/kultimate/screens/deleteTask.py` & `kultimate-0.2.2/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.2/kultimate/utils/app_config.py` & `kultimate-0.2.2/kultimate/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.2/kultimate/utils/html_to_markdown.py` & `kultimate-0.2.2/kultimate/utils/html_to_markdown.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         # Obtener los nombres de las columnas
         for stage in stage_list:
             self.markdown_text += f"## {stage.title}\n\n"
             # Obtener las tareas para cada columna
             try:
                 tasks = stage.query(Task)
                 for task in tasks:
-                    texto = task.render()
-                    self.markdown_text += f"- {texto.markup}\n"
+                    # texto = task.render()
+                    self.markdown_text += f"- {task.renderable}\n"
             except QueryError:
                 pass
 
             self.markdown_text += "\n"
 
         print(self.markdown_text)
         # DONE: Cuando acabe la función, descomentar la última línea
```

### Comparing `kultimate-0.1.2/kultimate/utils/parser_html.py` & `kultimate-0.2.2/kultimate/utils/parser_html.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,74 +13,50 @@
         with open(self.file_path) as ff:
             content = ff.read()
 
         html_content = markdown.markdown(content)
 
         self.soup = BeautifulSoup(html_content, features="html.parser")
 
-    def get_title(self):
-        """Toma el título del documento (h1)"""
-        try:
-            h1 = self.soup.find("h1").text.strip()
-        except IndexError:
-            h1 = ""
-        return h1
-
-    def get_description(self):
-        """Obtiene la descripción del documento"""
-        try:
-            h2 = self.soup.select("h2")[0]
-            ps = h2.findPreviousSiblings("p")
-            my_list = []
-            for p in ps:
-                my_list.append(p.text)
-            my_list.reverse()
-            text = "\n\n".join(my_list)
-        except IndexError:
-            text = ""
-
-        return text
-
     def get_stages(self):
         """Obtiene todos los h2 del documento"""
         try:
             h2s = self.soup.select("h2")
         except IndexError:
             h2s = []
         return h2s
 
-    def get_stage_description(self):
-        """Obtiene la descripción de cada h2 (stage)"""
-        pass
-
     def pretty(self):
         """Imprime el html en un bonito formato"""
         return self.soup.prettify()
 
-    def get_tasks(self):
+    def get_board(self):
         """Obtiene todas las tareas de cada h2"""
+        # doing
+        # aquí es donde tengo el error, cuando no hay tareas en la
+        # primer columna empiezan las fallas
         # obtener todos los h2, y de ahí todos los li
         # DONE: Cargar las tareas desde el archivo
         tasks = {}
-        try:
-            # ¿una lista de listas? Mejor un diccionario
-            # {1:["strings", "string"], 2:["string", "string"]}
-            # primero obtener todos los h2
-            h2s = self.soup.select("h2")
-            # ahora obtener los li de cada h2
-
-            for index, h2 in enumerate(h2s):
-                uls = h2.find_next_sibling("ul")
-                lis = []
-                if uls:
-                    for li in uls.findChildren():
-                        lis.append(li.text.strip())
-
-                    tasks[index] = lis
-                else:
-                    tasks[index] = []
-
-        except IndexError:
-            tasks = {}
-            print("Hubo error")
+        # ¿una lista de listas? Mejor un diccionario
+        # {1:["strings", "string"], 2:["string", "string"]}
+        # primero obtener todos los h2
+        h2s = self.soup.find_all("h2")
+        # ahora obtener los li de cada h2
+
+        for h2 in h2s:
+            list_tasks = []
+            next_sibling = h2.find_next_sibling()
+            if next_sibling == None or next_sibling.name == "h2":
+                tasks[h2.text] = list_tasks
+                continue
+
+            if next_sibling.name == "ul":
+                for li in next_sibling.findChildren("li"):
+                    list_tasks.append(li.text.strip())
+
+                tasks[h2.text] = list_tasks
+            else:
+                tasks[h2.text] = list_tasks
+                continue
 
         return tasks
```

### Comparing `kultimate-0.1.2/kultimate/utils/process_yaml.py` & `kultimate-0.2.2/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.2/kultimate/widgets/directory.py` & `kultimate-0.2.2/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.1.2/pyproject.toml` & `kultimate-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kultimate"
-version = "0.1.2"
+version = "0.2.2"
 description = ""
 authors = ["Felipe <104157442+justafewwords4@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 textual = { extras = ["dev"], version = "^0.27.0" }
```

