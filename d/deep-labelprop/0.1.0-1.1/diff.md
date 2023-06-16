# Comparing `tmp/deep-labelprop-0.1.0.tar.gz` & `tmp/deep-labelprop-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-labelprop-0.1.0.tar", last modified: Wed Mar 30 12:03:20 2022, max compression
+gzip compressed data, was "deep-labelprop-1.1.tar", last modified: Fri Jun 16 15:15:38 2023, max compression
```

## Comparing `deep-labelprop-0.1.0.tar` & `deep-labelprop-1.1.tar`

### file list

```diff
@@ -1,42 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 12:03:20.251692 deep-labelprop-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-03-30 12:03:20.251692 deep-labelprop-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 12:03:20.247692 deep-labelprop-0.1.0/deep_labelprop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-03-30 12:03:19.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-03-30 12:03:20.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 12:03:19.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 12:03:17.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-03-30 12:03:20.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-30 12:03:20.000000 deep-labelprop-0.1.0/deep_labelprop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 12:03:20.247692 deep-labelprop-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4807 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 12:03:20.251692 deep-labelprop-0.1.0/labelprop/
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/DataLoading.py
--rw-r--r--   0 runner    (1001) docker     (121)     9484 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/LabelProp.py
--rw-r--r--   0 runner    (1001) docker     (121)    10694 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/Pretraining_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/api.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/labelprop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/napari_entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/script.py
--rw-r--r--   0 runner    (1001) docker     (121)    11577 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/train.py
--rw-r--r--   0 runner    (1001) docker     (121)    12553 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/labelprop/voxelmorph2d.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-03-30 12:03:20.251692 deep-labelprop-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 12:03:20.251692 deep-labelprop-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-03-30 12:03:01.000000 deep-labelprop-0.1.0/tests/test_labelprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:38.626175 deep-labelprop-1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18092 2023-06-16 15:15:28.000000 deep-labelprop-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-16 15:15:38.626175 deep-labelprop-1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-06-16 15:15:28.000000 deep-labelprop-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:38.622176 deep-labelprop-1.1/deep_labelprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 15:15:38.000000 deep-labelprop-1.1/deep_labelprop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:38.626175 deep-labelprop-1.1/labelprop/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10000 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/DataLoading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2307 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/MultiLevelNet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10694 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/Pretraining_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8632 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38210 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/lightning_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9749 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/napari_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3958 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18898 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20182 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/voxelmorph2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-06-16 15:15:28.000000 deep-labelprop-1.1/labelprop/weight_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:15:38.626175 deep-labelprop-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-16 15:15:28.000000 deep-labelprop-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:15:38.626175 deep-labelprop-1.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      403 2023-06-16 15:15:28.000000 deep-labelprop-1.1/tests/test_labelprop.py
```

### Comparing `deep-labelprop-0.1.0/labelprop/LabelProp.py` & `deep-labelprop-1.1/labelprop/Pretraining_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import torch.nn.functional as F
 import pytorch_lightning as pl
 import kornia
 from .voxelmorph2d import VxmDense,NCC,Grad,Dice
-
+from pprint import pprint
+from monai.metrics import compute_meandice
 class LabelProp(pl.LightningModule):
 
     @property
     def automatic_optimization(self):
         return False
     def norm(self, x):
         
@@ -15,26 +16,30 @@
             x = kornia.enhance.normalize_min_max(x)
         elif len(x.shape)==3:
             x= kornia.enhance.normalize_min_max(x[:, None, ...])[:,0, ...]
         else:
             x = kornia.enhance.normalize_min_max(x[None, None, ...])[0, 0, ...]
         return x
     
+   
+
 
-    def __init__(self,n_channels=1,n_classes=2,learning_rate=5e-3,weight_decay=1e-8,way='up',shape=256,selected_slices=None,losses={},by_composition=False):
+    def __init__(self,n_channels=1,n_classes=2,learning_rate=1e-3,weight_decay=1e-8,way='up',shape=256,selected_slices=None,losses={},by_composition=False):
         super().__init__()
         self.n_classes = n_classes
         self.learning_rate=learning_rate
         self.weight_decay=weight_decay
         self.selected_slices=selected_slices #Used in validation step 
         if isinstance(shape,int):shape=[shape,shape]
         self.registrator= VxmDense(shape,bidir=False,int_downsize=1,int_steps=7)
         self.way=way #If up, learning only "forward" transitions (phi_i->j with j>i). Other choices : "down", "both". Bet you understood ;)
         self.losses=losses
         self.by_composition=by_composition
+        self.delta=1
+        self.mean_dice=0
         print('Losses',losses)
         self.save_hyperparameters()
 
     def apply_deform(self,x,field):
         """Apply deformation to x from flow field
         Args:
             x (Tensor): Image or mask to deform (BxCxHxW)
@@ -43,28 +48,55 @@
             Tensor: Transformed image
         """        
         return self.registrator.transformer(x,field)
     
     def compose_list(self,flows):
         flows=list(flows)
         compo=flows[-1]
-        for flow in reversed(flows[:-1]):
-            compo=self.compose_deformation(flow,compo)
+        if len(flows)>1:
+            for flow in reversed(flows[:-1]):
+                compo=self.compose_deformation(flow,compo)
         return compo
     def compose_deformation(self,flow_i_k,flow_k_j):
         """ Returns flow_k_j(flow_i_k(.)) flow
         Args:
             flow_i_k 
             flow_k_j
         Returns:
             [Tensor]: Flow field flow_i_j = flow_k_j(flow_i_k(.))
         """        
         flow_i_j= flow_k_j+self.apply_deform(flow_i_k,flow_k_j)
         return flow_i_j
 
+    def apply_successive_transformations(self,moving,flows):
+        """
+        Args:
+            moving (Tensor): Moving image (BxCxHxW)
+            flows ([Tensor]): List of deformation fields (Bx2xHxW)
+        Returns:
+            Tensor: Transformed image
+        """
+        if len(flows)==0:
+            return moving
+        else:
+            return self.apply_deform(self.apply_successive_transformations(moving,flows[:-1]),flows[-1])
+        
+    def multi_class_dice(self,pred_with_logits,target):
+        """
+        Args:
+            pred_with_logits: Predicted mask with logits
+            target: Target mask
+        """
+        preds=self.hardmax(pred_with_logits,1)
+        preds=torch.stack([preds[:,0],1-preds[:,0]],1)
+        target=torch.stack([target[:,0],1-target[:,0]],1)
+        dice=-Dice().loss(preds,target)
+        return dice
+      
+
     def forward(self, moving,target,registration=True):
         """
         Args:
             moving (Tensor): Moving image (BxCxHxW)
             target ([type]): Fixed image (BxCxHxW)
             registration (bool, optional): If False, also return non-integrated inverse flow field. Else return the integrated one. Defaults to False.
         Returns:
@@ -88,137 +120,136 @@
         loss_trans=0
         if moved!=None:
             loss_ncc=NCC().loss(moved,target)
         if moved_mask!=None:
             loss_seg= Dice().loss(moved_mask,target_mask)
         if field!=None:
             loss_trans=Grad().loss(field,field) #Recommanded weight for this loss is 1 (see Voxelmorph paper) 
-        return loss_ncc+loss_seg+loss_trans
+        return loss_ncc+loss_seg+2*loss_trans
 
     def blend(self,x,y):
         #For visualization
         x=self.norm(x)
         blended=torch.stack([y,x,x])
         return blended
 
     def training_step(self, batch, batch_nb):
         X,Y=batch # X : Full scan (1x1xLxHxW) | Y : Ground truth (1xCxLxHxW)
         y_opt=self.optimizers()
         loss=[]
-        chunks=[]
-        chunk=[]
-        loss_up=[]
-        loss_down=[]
-        dices_prop=[]
+        chunk=[None,None]
+
         #Identifying chunks (i->j)
         for i in range(X.shape[2]):
             y=Y[:,:,i,...]
             if len(torch.unique(torch.argmax(y,1)))>1:
-                chunk.append(i)
-            if len(chunk)==2:
-                chunks.append(chunk)
-                chunk=[i]
+                if chunk[0]==None:
+                    chunk[0]=i
+                else:
+                    chunk[1]=i
+
         if self.current_epoch==0:
-            print(chunks)
+            print(chunk)
+        y_opt.zero_grad()
+        #Sequences of flow fields (field_up=forward, field_down=backward)
+        fields_up=X.shape[2]*[None]
+        print(len(fields_up))
+        fields_down=X.shape[2]*[None]
         
-        for chunk in chunks:
-            y_opt.zero_grad()
-            #Sequences of flow fields (field_up=forward, field_down=backward)
-            fields_up=[]
-            fields_down=[]
-            for i in range(chunk[0],chunk[1]):
+        if self.mean_dice>0.98:
+            self.delta+=1
+        dices=[]
+
+        # loss=torch.stack(loss).sum()
+        # self.manual_backward(loss,retain_graph=True)
+        loss=[]
+        for j in range(chunk[0],chunk[1]):
                 #Computing flow fields and loss for each hop from chunk[0] to chunk[1]
-                x1=X[:,:,i,...]
-                x2=X[:,:,i+1,...]
-                if not self.way=='down':
-                    moved_x1,field_up=self.forward(x1,x2)
-                    loss_up.append(self.compute_loss(moved_x1,x2,field=field_up))
-                    fields_up.append(field_up)
-
-                if not self.way=='up':
-                    moved_x2,field_down=self.forward(x2,x1)#
-                    fields_down.append(field_down)
-                    moved_x2=self.registrator.transformer(x2,field_down)
-                    loss_down.append(self.compute_loss(moved_x2,x1,field=field_down))
-    
-            #Better with mean
-            if self.way=='up':
-                loss=torch.stack(loss_up).mean()
-            elif self.way=='down':
-                loss=torch.stack(loss_down).mean()
-            else:
-                loss_up=torch.stack(loss_up).mean()
-                loss_down=torch.stack(loss_down).mean()
-                loss=(loss_up+loss_down)
-            
-            # Computing registration from the sequence of flow fields
-            if not self.way=='down':
-                prop_x_up=X[:,:,chunk[0],...]
-                prop_y_up=Y[:,:,chunk[0],...]
-                if self.by_composition:
-                    composed_fields_up=self.compose_list(fields_up)
-                    prop_x_up=self.apply_deform(prop_x_up,composed_fields_up)
-                    prop_y_up=self.apply_deform(prop_y_up,composed_fields_up)
-                else:
-                    for field_up in fields_up:
-                        prop_x_up=self.apply_deform(prop_x_up,field_up)
-                        prop_y_up=self.apply_deform(prop_y_up,field_up)
-                
-                if self.losses['compo-reg-up']:
-                    loss+=self.compute_loss(prop_x_up,X[:,:,chunk[1],...])
-                if self.losses['compo-dice-up']:
-                    dice_loss=self.compute_loss(moved_mask=prop_y_up,target_mask=Y[:,:,chunk[1],...])
-                    loss+=dice_loss
-                    dices_prop.append(dice_loss)
-
-            if not self.way=='up':
-                prop_x_down=X[:,:,chunk[1],...]
-                prop_y_down=Y[:,:,chunk[1],...]
-                if self.by_composition:
-                    composed_fields_down=self.compose_list(fields_down[::-1])
-                    prop_x_down=self.apply_deform(prop_x_down,composed_fields_down)
-                    prop_y_down=self.apply_deform(prop_y_down,composed_fields_down)
-                else:
-                    for field_down in reversed(fields_down):
-                        prop_x_down=self.apply_deform(prop_x_down,field_down)
-                        prop_y_down=self.apply_deform(prop_y_down,field_down)
-
-                if self.losses['compo-reg-down']:
-                    loss+=self.compute_loss(prop_x_down,X[:,:,chunk[0],...])
-                if self.losses['compo-dice-down']:
-                    dice_loss=self.compute_loss(moved_mask=prop_y_down,target_mask=Y[:,:,chunk[0],...])
-                    loss+=dice_loss
-                    dices_prop.append(dice_loss)
+                x1=X[:,:,j,...]
+                x2=X[:,:,j+1,...]
+                moved_x1,field_up=self.forward(x1,x2)
+                loss.append(self.compute_loss(moved_x1,x2,field=field_up))
+                fields_up[j]=(field_up)
+                moved_x2,field_down=self.forward(x2,x1)#
+                fields_down[j]=(field_down)
+                moved_x2=self.registrator.transformer(x2,field_down)
+                loss.append(self.compute_loss(moved_x2,x1,field=field_down))
+
+        for i in range(chunk[0],chunk[1]+1):
+            up_idx=i+self.delta
+            down_idx=i-self.delta
+            moving_x=X[:,:,i,...]
+            moving_y=Y[:,:,i,...]
+            if up_idx>chunk[1] : 
+                up_idx=chunk[1]
+            if i<chunk[1]:
+                composed_field_up=self.compose_list(fields_up[i:up_idx])
+                prop_y_up=self.apply_deform(moving_y,composed_field_up)
+                prop_x_up=self.apply_deform(moving_x,composed_field_up)
+                # prop_y_up=self.apply_successive_transformations(moving_y,fields_up[i:up_idx])
+                # prop_x_up=self.apply_successive_transformations(moving_x,fields_up[i:up_idx])
+                loss.append(self.compute_loss(prop_x_up,X[:,:,up_idx]))
+                d_loss_up=[]
+                # for lab in range(Y.shape[1]):
+                #     if len(torch.unique(Y[:,lab,up_idx]))>1:
+                #         d_loss_up.append(self.compute_loss(moved_mask=prop_y_up[:,lab],target_mask=Y[:,lab,up_idx]))
+                d_loss_up.append(self.compute_loss(moved_mask=prop_y_up,target_mask=Y[:,:,up_idx]))
+                d_loss_up=torch.stack(d_loss_up).sum()*100
+                dices.append(self.multi_class_dice(prop_y_up,Y[:,:,up_idx].detach()))
+                loss.append(d_loss_up)
+
+            if i>chunk[0]:
+                if down_idx<chunk[0] : 
+                    down_idx=chunk[0]
+
+                composed_field_down=self.compose_list(fields_down[down_idx:i][::-1])
+                prop_y_down=self.apply_deform(moving_y,composed_field_down)
+                prop_x_down=self.apply_deform(moving_x,composed_field_down)
+                # prop_y_down=self.apply_successive_transformations(moving_y,fields_down[down_idx:i][::-1])
+                # prop_x_down=self.apply_successive_transformations(moving_x,fields_down[down_idx:i][::-1])
+                loss.append(self.compute_loss(prop_x_down,X[:,:,down_idx]))
+                d_loss_down=[]
+                # for lab in range(Y.shape[1]):
+                #     if len(torch.unique(Y[:,lab,down_idx]))>1:
+                #         d_loss_down.append(self.compute_loss(moved_mask=prop_y_down[:,lab],target_mask=Y[:,lab,down_idx]))
+                d_loss_down.append(self.compute_loss(moved_mask=prop_y_down,target_mask=Y[:,:,down_idx]))
+                d_loss_down=torch.stack(d_loss_down).sum()*100
+                dices.append(self.multi_class_dice(prop_y_down,Y[:,:,down_idx].detach()))
+                loss.append(d_loss_down)
+
+        loss=torch.stack(loss).sum()
+        self.manual_backward(loss,retain_graph=True)
+        y_opt.step()
+        loss=[]
+
 
 
             #Additionnal loss to ensure sequences (images and masks) generated from "positive" and "negative" flows are equal
             # if self.way=='both':
             #     #This helps
             #     if self.losses['bidir-cons-dice']:
             #         loss+=self.compute_loss(moved_mask=prop_y_down,target_mask=prop_y_up)
             #     #This breaks stuff
             #     if self.losses['bidir-cons-reg']:
             #         loss+=self.compute_loss(prop_x_up,prop_x_down)
 
-            self.log_dict({'loss':loss},prog_bar=True)
-            self.manual_backward(loss)
-            y_opt.step()
-            loss_up=[]
-            loss_down=[]
             # self.logger.experiment.add_image('x_true',X[0,:,chunk[0],...])
             # self.logger.experiment.add_image('prop_x_down',prop_x_down[0,:,0,...])
             # self.logger.experiment.add_image('x_true_f',X[0,:,chunk[1],...])
             # self.logger.experiment.add_image('prop_x_up',prop_x_up[0,:,-1,...])
-        
-        if len(dices_prop)>0:
-            dices_prop=-torch.stack(dices_prop).mean()
-            self.log('val_accuracy',dices_prop)
-            print(dices_prop)
-        else:
-            self.log('val_accuracy',self.current_epoch)
+        self.mean_dice=torch.stack(dices).mean()
+        print('Dices : ',self.mean_dice)
+        print('Delta :',self.delta)
+        self.log('val_accuracy',self.mean_dice*self.delta)
+        # if len(dices_prop)>0:
+        #     dices_prop=-torch.stack(dices_prop).mean()
+        #     self.log('val_accuracy',dices_prop)
+        #     print(dices_prop)
+        # else:
+        #     self.log('val_accuracy',self.current_epoch)
         return loss
 
     def register_images(self,moving,target,moving_mask):
         moved,field=self.forward(moving,target,registration=True)
         return moved,self.apply_deform(moving_mask,field),field
 
     def configure_optimizers(self):
```

### Comparing `deep-labelprop-0.1.0/setup.py` & `deep-labelprop-1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
-
-requirements = ['kornia==0.5.8',
-    'medpy==0.4.0',
-    'monai==0.6.0',
-    'nibabel==3.2.1',
-    'pytorch_lightning==1.3.8',
-    'torch==1.10.2',
-    'torchio==0.18.47',
-    'torchvision==0.11.3',
-    "flask"]
+requirements = [
+'Flask==2.1.0',
+'kornia==0.6.12',
+'monai==0.8.1',
+'nibabel==3.2.1',
+'numpy',
+'plotext==4.2.0',
+'lightning']
 
 test_requirements = [ ]
 
-dependency_links = ['https://download.pytorch.org/whl/cu111']
-
+dependency_links = []
+with open('README.md') as f:
+    readme = f.read()
 setup(
     author="Nathan Decaux",
     author_email='nathan.decaux@imt-atlantique.fr',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
+    entry_points = {
+        'console_scripts': [
+            'labelprop = labelprop.cli:cli',                  
+        ],              
+    },
     description="Label propagation using deep registration",
+    long_description = readme,
+    long_description_content_type = 'text/markdown',
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='labelprop',
     name='deep-labelprop',
     packages=find_packages(include=['labelprop', 'labelprop.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nathandecaux/labelprop',
-    version='0.1.0',
+    version='1.1',
     zip_safe=False,
 )
```

