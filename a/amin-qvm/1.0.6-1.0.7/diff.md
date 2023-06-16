# Comparing `tmp/amin_qvm-1.0.6.tar.gz` & `tmp/amin_qvm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.6.tar", last modified: Thu Jun 15 03:04:38 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.7.tar", last modified: Fri Jun 16 16:05:26 2023, max compression
```

## Comparing `amin_qvm-1.0.6.tar` & `amin_qvm-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.467513 amin_qvm-1.0.6/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.6/LICENSE.ttxt
--rw-rw-rw-   0        0        0     6048 2023-06-15 03:04:38.465546 amin_qvm-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.434144 amin_qvm-1.0.6/amin_qvm/
--rw-rw-rw-   0        0        0    89322 2023-06-15 02:42:02.000000 amin_qvm-1.0.6/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.6/amin_qvm/__init__.py
--rw-rw-rw-   0        0        0     3843 2023-06-14 14:56:01.000000 amin_qvm-1.0.6/amin_qvm/functions.py
--rw-rw-rw-   0        0        0      543 2023-06-14 14:56:39.000000 amin_qvm-1.0.6/amin_qvm/test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:04:38.463548 amin_qvm-1.0.6/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     6048 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 03:04:38.000000 amin_qvm-1.0.6/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 03:04:38.469510 amin_qvm-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-06-15 03:04:34.000000 amin_qvm-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.673110 amin_qvm-1.0.7/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.7/LICENSE.ttxt
+-rw-rw-rw-   0        0        0     7355 2023-06-16 16:05:26.666184 amin_qvm-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.571508 amin_qvm-1.0.7/amin_qvm/
+-rw-rw-rw-   0        0        0    91665 2023-06-16 15:28:14.000000 amin_qvm-1.0.7/amin_qvm/QuantumComputer.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.7/amin_qvm/__init__.py
+-rw-rw-rw-   0        0        0     4467 2023-06-16 15:25:30.000000 amin_qvm-1.0.7/amin_qvm/functions.py
+-rw-rw-rw-   0        0        0      518 2023-06-16 11:00:36.000000 amin_qvm-1.0.7/amin_qvm/test.py
+drwxrwxrwx   0        0        0        0 2023-06-16 16:05:26.648566 amin_qvm-1.0.7/amin_qvm.egg-info/
+-rw-rw-rw-   0        0        0     7355 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 16:05:26.000000 amin_qvm-1.0.7/amin_qvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 16:05:26.674112 amin_qvm-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-06-16 15:29:06.000000 amin_qvm-1.0.7/setup.py
```

### Comparing `amin_qvm-1.0.6/LICENSE.ttxt` & `amin_qvm-1.0.7/LICENSE.ttxt`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.6/PKG-INFO` & `amin_qvm-1.0.7/amin_qvm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: amin_qvm
-Version: 1.0.6
+Name: amin-qvm
+Version: 1.0.7
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -146,7 +146,60 @@
 
    from amin_qvm.functions import grover_search
    
    # Perform Grover's search
    secret_bitstring = "1010"
    guessed_bitstring = grover_search(secret_bitstring)
    print("Guessed bitstring:", guessed_bitstring)
+
+Deutsch's Algorithm
+~~~~~~~~~~~~~~~~~~~
+.. code-block:: python
+
+   # Define your own function
+   def my_function(x):
+       # Modify this function according to your requirements
+       return x % 2 == 0
+
+   # Example usage
+   result = deutsch(my_function)
+   print("The function is:", result)
+
+WARNING: NERDS ONLY
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Normalizing Quantum States
+--------------------------
+.. image:: images/equation.png
+    :alt: an unnormalized quantum state
+
+Suppose we are given an unnormalized quantum state like the one above.
+We can turn this into an equivalent, valid quantum state by normalizing it. This function, given alpha
+and beta, normalizes this state to
+
+.. image:: images/equation2.png
+   :alt: a normalized quantum state
+
+Suppose we are given the inputs
+
+  alpha = 2.0 + 1.0j
+  beta = -0.3 + 0.4j 
+
+The function should return the vector
+
+  np.array([ 0.87287156+0.43643578j, -0.13093073+0.17457431j]) 
+
+which represents the qubit state
+
+.. image:: images/equation3.png
+   :alt: The qubit state representation
+
+Here is the code example
+
+.. code-block:: python
+
+   from amin-qvm.functions import normalize_state
+   import numpy as np
+
+   ket_0 = np.array([1, 0])
+   ket_1 = np.array([0, 1])
+   print(normalize_state(ket_0, ket_1))
+
```

### Comparing `amin_qvm-1.0.6/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.7/amin_qvm/QuantumComputer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,83 @@
 import unittest
 import re
 import random
 import itertools
 from functools import reduce
 from math import sqrt,pi,e,log
 import time
+
+def normalize_state(alpha, beta):
+    """Compute a normalized quantum state given arbitrary amplitudes.
+    
+    Args:
+        alpha (complex): The amplitude associated with the |0> state.
+        beta (complex): The amplitude associated with the |1> state.
+        
+    Returns:
+        array[complex]: A vector (numpy array) with 2 elements that represents
+        a normalized quantum state.
+    """
+
+    #[a', b'] BASED ON alpha AND beta SUCH THAT |a'|^2 + |b'|^2 = 1
+    normalized = alpha * ket_0 + beta * ket_1
+    normal = np.linalg.norm(normalized)
+    normalized = normalized/normal
+    return(normalized)
+
+def inner_product(state_1, state_2):
+    """Compute the inner product between two states.
+    
+    Args:
+        state_1 (array[complex]): A normalized quantum state vector
+        state_2 (array[complex]): A second normalized quantum state vector
+        
+    Returns:
+        complex: The value of the inner product <state_1 | state_2>.
+    """
+ 
+    ##################
+    Conjugate = np.conjugate(state_1)
+    Inner = np.dot(Conjugate, state_2)
+    ##################
+    # COMPUTE AND RETURN THE INNER PRODUCT
+
+    return  Inner
+def feature_map(qc, data, qubits):
+    # Encode the data using a Pauli feature map
+    for i, value in enumerate(data):
+        qc.execute(f"rx({value * np.pi}) q[{qubits[i]}];")
+        qc.execute(f"rz({value * np.pi}) q[{qubits[i]}];")
+
+def estimate_inner_product(qc, qubits):
+    # Estimate the inner product of the quantum states
+    for qubit in qubits:
+        qc.execute(f"h q[{qubit}];")
+    for i in range(len(qubits) - 1):
+        qc.execute(f"cx q[{qubits[i]}], q[{qubits[i + 1]}];")
+    for qubit in qubits:
+        qc.execute(f"measure q[{qubit}];")
+    return np.mean([qc.qubits[qubit].get_state() for qubit in qubits])
+
+def apply_quantum_kernel(qc, training_data, test_data):
+    num_qubits = len(training_data[0])
+    qubits = [f"q{i}" for i in range(num_qubits)]
+
+    kernel_matrix = np.zeros((len(test_data), len(training_data)))
+
+    for i, test_point in enumerate(test_data):
+        qc.reset()
+        feature_map(qc, test_point, qubits)
+        for j, training_point in enumerate(training_data):
+            qc.reset()
+            feature_map(qc, training_point, qubits)
+            kernel_matrix[i, j] = estimate_inner_product(qc, qubits)
+
+    return kernel_matrix
+
 ####
 ## Gates
 ####
 class Gate(object):
 	i_=np.complex(0,1)
 	## One qubit gates
 	# Hadamard gate
@@ -713,15 +782,15 @@
 			t q[1];
 			h q[1];
 			t q[1];
 			h q[1];
 			t q[1];
 			s q[1];
 			h q[1];
-			t q[1];
+			t q[1];  
 			h q[1];
 			t q[1];
 			s q[1];
 			h q[1];
 			bloch q[1];""")
 
 	program_test_XYZMeasureIdSdagTdag=Program("""sdg q[0];
```

### Comparing `amin_qvm-1.0.6/amin_qvm.egg-info/PKG-INFO` & `amin_qvm-1.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: amin-qvm
-Version: 1.0.6
+Name: amin_qvm
+Version: 1.0.7
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -146,7 +146,60 @@
 
    from amin_qvm.functions import grover_search
    
    # Perform Grover's search
    secret_bitstring = "1010"
    guessed_bitstring = grover_search(secret_bitstring)
    print("Guessed bitstring:", guessed_bitstring)
+
+Deutsch's Algorithm
+~~~~~~~~~~~~~~~~~~~
+.. code-block:: python
+
+   # Define your own function
+   def my_function(x):
+       # Modify this function according to your requirements
+       return x % 2 == 0
+
+   # Example usage
+   result = deutsch(my_function)
+   print("The function is:", result)
+
+WARNING: NERDS ONLY
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Normalizing Quantum States
+--------------------------
+.. image:: images/equation.png
+    :alt: an unnormalized quantum state
+
+Suppose we are given an unnormalized quantum state like the one above.
+We can turn this into an equivalent, valid quantum state by normalizing it. This function, given alpha
+and beta, normalizes this state to
+
+.. image:: images/equation2.png
+   :alt: a normalized quantum state
+
+Suppose we are given the inputs
+
+  alpha = 2.0 + 1.0j
+  beta = -0.3 + 0.4j 
+
+The function should return the vector
+
+  np.array([ 0.87287156+0.43643578j, -0.13093073+0.17457431j]) 
+
+which represents the qubit state
+
+.. image:: images/equation3.png
+   :alt: The qubit state representation
+
+Here is the code example
+
+.. code-block:: python
+
+   from amin-qvm.functions import normalize_state
+   import numpy as np
+
+   ket_0 = np.array([1, 0])
+   ket_1 = np.array([0, 1])
+   print(normalize_state(ket_0, ket_1))
+
```

### Comparing `amin_qvm-1.0.6/setup.py` & `amin_qvm-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'numpy',
     'qiskit',
     'pennylane',
     'scikit-learn',
 ]
 setup(
     name='amin_qvm',
-    version='1.0.6',
+    version='1.0.7',
     author='Amin Alogaili',
     author_email='aminalogai@gmail.com',
     description='Amin-QVM: Quantum Computing Library',
     long_description=long_description,
     url='https://github.com/amin1029384756/QVM',
     packages=['amin_qvm'],
     classifiers=[
```

