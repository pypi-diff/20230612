# Comparing `tmp/aisp-0.1.1.tar.gz` & `tmp/aisp-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisp-0.1.1.tar", last modified: Thu Jun  8 16:10:38 2023, max compression
+gzip compressed data, was "aisp-0.1.21.tar", last modified: Mon Jun 12 18:30:51 2023, max compression
```

## Comparing `aisp-0.1.1.tar` & `aisp-0.1.21.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.136405 aisp-0.1.1/
--rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.133383 aisp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6852 2023-06-08 15:06:17.000000 aisp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.100382 aisp-0.1.1/aisp/
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.129382 aisp-0.1.1/aisp/NSA/
--rw-rw-rw-   0        0        0      116 2023-05-28 13:47:18.000000 aisp-0.1.1/aisp/NSA/__init__.py
--rw-rw-rw-   0        0        0    48346 2023-06-08 15:27:54.000000 aisp-0.1.1/aisp/NSA/_negativeSelection.py
--rw-rw-rw-   0        0        0     8040 2023-06-08 15:52:49.000000 aisp-0.1.1/aisp/_base.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.119385 aisp-0.1.1/aisp.egg-info/
--rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1349 2023-06-08 15:56:51.000000 aisp-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 16:10:38.137386 aisp-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.276323 aisp-0.1.21/
+-rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.21/LICENSE
+-rw-rw-rw-   0        0        0     7908 2023-06-12 18:30:51.275325 aisp-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.21/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.248329 aisp-0.1.21/aisp/
+drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.272324 aisp-0.1.21/aisp/NSA/
+-rw-rw-rw-   0        0        0      140 2023-06-12 18:29:52.000000 aisp-0.1.21/aisp/NSA/__init__.py
+-rw-rw-rw-   0        0        0    50866 2023-06-12 18:20:04.000000 aisp-0.1.21/aisp/NSA/_negativeSelection.py
+-rw-rw-rw-   0        0        0     8811 2023-06-12 16:38:13.000000 aisp-0.1.21/aisp/_base.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.262325 aisp-0.1.21/aisp.egg-info/
+-rw-rw-rw-   0        0        0     7908 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1443 2023-06-12 18:29:11.000000 aisp-0.1.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:30:51.277328 aisp-0.1.21/setup.cfg
```

### Comparing `aisp-0.1.1/LICENSE` & `aisp-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `aisp-0.1.1/PKG-INFO` & `aisp-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.1
+Version: 0.1.21
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
 Project-URL: Tracker, https://github.com/AIS-Package/aisp/issues
-Keywords: Artificial Immune Systems,classification,Natural computing,machine learning,artificial intelligence
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -65,15 +64,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -175,15 +174,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/README.md` & `aisp-0.1.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -151,15 +151,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/aisp/NSA/_negativeSelection.py` & `aisp-0.1.21/aisp/NSA/_negativeSelection.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,23 @@
         * algorithm(``str``), Set the algorithm version:
 
                 * ``'default-NSA'``: Default algorithm with fixed radius.
                 * ``'V-detector'``: This algorithm uses a variable radius for anomaly detection in feature spaces.
 
             Defaults to ``'default-NSA'``.
 
-        * cell_bounds (``bool``): If set to ``True``, this option limits the generation of detectors to 
-            the space within the plane between 0 and 1. 
+        * non_self_label (``str``): This variable stores the label that will be assigned when the data has only one 
+        output class, and the sample is classified as not belonging to that class. Defaults to ``'non-self'``.
+        * cell_bounds (``bool``): If set to ``True``, this option limits the generation of detectors to the space within 
+        the plane between 0 and 1. This means that any detector whose radius exceeds this limit is discarded, 
+        this variable is only used in the ``V-detector`` algorithm. Defaults to ``False``.
+        * p (``float``): This parameter stores the value of ``p`` used in the Minkowski distance. The default is ``2``, which 
+        represents normalized Euclidean distance. Different values of p lead to different variants of the Minkowski 
+        distance [learn more](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
+       
         * detectors (``dict``): This variable stores a list of detectors by class.
         * classes (``npt.NDArray``): list of output classes.
         
     ---
 
     A classe ``RNSA`` (Algoritmo de Seleção Negativa de Valor Real) tem a finalidade de classificação e identificação 
     de anomalias através do método self e not self . 
@@ -56,32 +63,38 @@
 
                 * ``'default-NSA'``: Algoritmo padrão com raio fixo.
                 * ``'V-detector'``: Este algoritmo utiliza um raio variável para a detecção de anomalias em espaços 
                     de características. 
 
             Defaults to ``'default-NSA'``.
 
-        * cell_bounds (``bool``):  Se definido como ``True``, esta opção limita a geração dos detectores ao espaço 
-            do plano compreendido entre 0 e 1.
-       
+        * non_self_label (``str``): Esta variável armazena o rótulo que será atribuído quando os dados possuírem 
+        apenas uma classe de saída, e a amostra for classificada como não pertencente a essa classe. Defaults to ``'non-self'``.
+        * cell_bounds (``bool``):  Se definido como ``True``, esta opção limita a geração dos detectores ao espaço do plano 
+        compreendido entre 0 e 1. Isso significa que qualquer detector cujo raio ultrapasse esse limite é descartado, 
+        e esta variável é usada exclusivamente no algoritmo ``V-detector``.
+        * p (``float``): Este parâmetro armazena o valor de ``p`` utilizada na distância de Minkowski. O padrão é ``2``, o que significa 
+        distância euclidiana normalizada. Diferentes valores de p levam a diferentes variantes da distância de 
+        Minkowski [saiba mais](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
         
         * detectors (``dict``): Essa variável armazena uma lista com detectores por classes.
         * classes (``npt.NDArray``): lista com as classes de saída.
     """
+    
     def __init__(
         self, 
         N: int = 100, 
         r: float = 0.05, 
         r_s: float = 0.0001, 
         k: int = 1, 
         metric: Literal['manhattan', 'minkowski', 'euclidean'] = 'euclidean', 
         max_discards: int = 1000, 
         seed: int = None, 
         algorithm: Literal['default-NSA', 'V-detector'] ='default-NSA', 
-        **kwargs: Dict[str, Union[bool, str]]
+        **kwargs: Dict[str, Union[bool, str, float]]
     ):
         """
         Negative Selection class constructor (``RNSA``).
 
         Details:
         ---
             This method initializes the ``detectors``, ``classes``, ``k``, ``metric``, ``N``, ``r``, ``r_S``, 
@@ -93,15 +106,15 @@
             * r (``float``): Radius of the detector. Defaults to ``0.05``.
             * r_s (``float``): rₛ Radius of the ``X`` own samples. Defaults to ``0.0001``.
             * k (``int``): Number of neighbors near the randomly generated detectors to perform the
             distance average calculation. Defaults to ``1``.
             * metric (``str``): Way to calculate the distance between the detector and the sample:
 
                 * ``'Euclidean'`` ➜ The calculation of the distance is given by the expression: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
-                * ``'minkowski'`` ➜ The calculation of the distance is given by the expression: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ, In this project ``p == 2``.
+                * ``'minkowski'`` ➜ The calculation of the distance is given by the expression: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ.
                 * ``'manhattan'`` ➜ The calculation of the distance is given by the expression: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|) .
 
             Defaults to ``'euclidean'``.
 
             * max_discards (``int``): This parameter indicates the maximum number of consecutive detector discards, aimed at preventing a 
             possible infinite loop in case a radius is defined that cannot generate non-self detectors. Defaults to ``1000``.
             * seed (``int``): Seed for the random generation of values in the detectors. Defaults to ``None``.
@@ -115,15 +128,17 @@
 
             - ``**kwargs``:
                     - non_self_label (``str``): This variable stores the label that will be assigned when the data has only one 
                     output class, and the sample is classified as not belonging to that class. Defaults to ``'non-self'``.
                     - cell_bounds (``bool``): If set to ``True``, this option limits the generation of detectors to the space within 
                     the plane between 0 and 1. This means that any detector whose radius exceeds this limit is discarded, 
                     this variable is only used in the ``V-detector`` algorithm. Defaults to ``False``.
-
+                    - p (``float``): This parameter stores the value of ``p`` used in the Minkowski distance. The default is ``2``, which 
+                    represents normalized Euclidean distance. Different values of p lead to different variants of the Minkowski 
+                    distance [learn more](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
         ---
 
         Construtor da classe de Seleção negativa (``RNSA``).
 
         Details:
         ---
             Este método inicializa os atributos ``detectors``, ``classes``, ``k``, ``metric``, ``N``, ``r`` e ``seed``.
@@ -134,15 +149,15 @@
             * r (``float``): Raio do detector. Defaults to ``0.05``.
             * r_s (``float``): O valor de ``rₛ`` é o raio das amostras próprias da matriz ``X``. Defaults to ``0.0001``.
             * k (``int``): Quantidade de vizinhos próximos dos detectores gerados aleatoriamente para efetuar o 
             cálculo da média da distância. Defaults to ``1``.
             * metric (``str``): Forma para se calcular a distância entre o detector e a amostra: 
 
                 * ``'euclidiana'`` ➜ O cálculo da distância dá-se pela expressão: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
-                * ``'minkowski'``  ➜ O cálculo da distância dá-se pela expressão: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ, Neste projeto ``p == 2``.
+                * ``'minkowski'``  ➜ O cálculo da distância dá-se pela expressão: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ.
                 * ``'manhattan'``  ➜ O cálculo da distância dá-se pela expressão: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|).
 
             Defaults to ``'euclidean'``.
 
             * max_discards (``int``): Este parâmetro indica o número máximo de descartes de detectores em sequência, que tem como objetivo evitar um 
             possível loop infinito caso seja definido um raio que não seja possível gerar detectores do não-próprio. Defaults to ``1000``.
             * seed (``int``): Semente para a geração randômica dos valores nos detectores. Defaults to ``None``.
@@ -155,14 +170,17 @@
 
             - ``**kwargs``:
                     - non_self_label (``str``): Esta variável armazena o rótulo que será atribuído quando os dados possuírem 
                     apenas uma classe de saída, e a amostra for classificada como não pertencente a essa classe. Defaults to ``'non-self'``.
                     - cell_bounds (``bool``):  Se definido como ``True``, esta opção limita a geração dos detectores ao espaço do plano 
                     compreendido entre 0 e 1. Isso significa que qualquer detector cujo raio ultrapasse esse limite é descartado, 
                     e esta variável é usada exclusivamente no algoritmo ``V-detector``.
+                    - p (``float``): Este parâmetro armazena o valor de ``p`` utilizada na distância de Minkowski. O padrão é ``2``, o que significa 
+                    distância euclidiana normalizada. Diferentes valores de p levam a diferentes variantes da distância de 
+                    Minkowski [saiba mais](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
         """
         
         if metric == 'manhattan' or metric == 'minkowski' or metric == 'euclidean':
             self.metric = metric
         else:
             self.metric = 'euclidean'
 
@@ -194,18 +212,25 @@
 
         if algorithm == 'V-detector':
             self._Detector = namedtuple("Detector", "position radius")
             self._algorithm: str = algorithm
         else:
             self._Detector = namedtuple("Detector", "position")
             self._algorithm: str = 'default-NSA'
-            
+
+        if max_discards > 0:
+            self.max_discards: int = max_discards
+        else:
+            self.max_discards: int = 1000
+
+        # Obtém as variáveis do kwargs.
+        self.p: float = kwargs.get('p', 2)
         self._cell_bounds: bool = kwargs.get('cell_bounds', False)
         self.non_self_label: str = kwargs.get('non_self_label', 'non-self')
-        self.max_discards: int = max_discards
+        
         self.detectors: Union[dict, None] = None
         self.classes: npt.NDArray = None
 
     def fit(self, X: npt.NDArray, y: npt.NDArray, verbose: bool = True):
         """
         The function ``fit(...)``, performs the training according to ``X`` and ``y``, using the method
         negative selection method(``NegativeSelect``).
```

### Comparing `aisp-0.1.1/aisp/_base.py` & `aisp-0.1.21/aisp/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,40 +9,50 @@
     and therefore are considered essential for the overall functioning of the system.
 
     ---
 
     A classe base contém funções que são utilizadas por mais de uma classe do pacote, 
     e por isso são consideradas essenciais para o funcionamento geral do sistema.
     """
-    def __init__(self, metric: str = 'euclidean'):
+    def __init__(self, metric: str = 'euclidean', p: float = 2):
         """
         Parameters:
         ---
         * metric (``str``): Way to calculate the distance between the detector and the sample:
 
                 * ``'Euclidean'`` ➜ The calculation of the distance is given by the expression: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
-                * ``'minkowski'`` ➜ The calculation of the distance is given by the expression: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ , In this project ``p == 2``.
+                * ``'minkowski'`` ➜ The calculation of the distance is given by the expression: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ.
                 * ``'manhattan'`` ➜ The calculation of the distance is given by the expression: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|) .
         
+        
+        * p (``float``): This parameter stores the value of ``p`` used in the Minkowski distance. 
+        The default is ``2``, which represents normalized Euclidean distance. Different values of p lead to 
+        different variants of the Minkowski distance [learn more](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
+
         ---
 
         Parameters:
         ---
         * metric (``str``): Forma para se calcular a distância entre o detector e a amostra: 
 
                 * ``'euclidiana'`` ➜ O cálculo da distância dá-se pela expressão: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
-                * ``'minkowski'``  ➜ O cálculo da distância dá-se pela expressão: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ , Neste projeto ``p == 2``.
+                * ``'minkowski'``  ➜ O cálculo da distância dá-se pela expressão: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p).
                 * ``'manhattan'``  ➜ O cálculo da distância dá-se pela expressão: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|).
 
             Defaults to ``'euclidean'``.
+        
+        * p (``float``): Este parâmetro armazena o valor de ``p`` utilizada na distância de Minkowski.
+          O padrão é ``2``, o que significa distância euclidiana normalizada. Diferentes valores de p levam a 
+          diferentes variantes da distância de Minkowski [saiba mais](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.minkowski.html).
         """
         if metric == 'manhattan' or metric == 'minkowski' or metric == 'euclidean':
-            self.metric = metric
+            self.metric: str = metric
         else:
-            self.metric = 'euclidean'
+            self.metric: str = 'euclidean'
+        self.p: float = p
 
     def _distance(self, u: npt.NDArray, v: npt.NDArray):
         """
         Function to calculate the distance between two points by the chosen ``metric``.
 
         Parameters:
         ---
@@ -65,15 +75,15 @@
         Returns:
         ---
             * Distância (``double``) entre os dois pontos.
         """
         if self.metric == 'manhattan':
             return cityblock(u, v)
         elif self.metric == 'minkowski':
-            return minkowski(u, v, 2)
+            return minkowski(u, v, self.p)
         else:
             return euclidean(u, v)
         
     def _check_and_raise_exceptions_fit(self, X: npt.NDArray = None, y: npt.NDArray = None, _class_: Literal['RNSA', 'BNSA'] = 'RNSA'):
         """
         Function responsible for verifying fit function parameters and throwing exceptions if the verification is not successful.
```

### Comparing `aisp-0.1.1/aisp.egg-info/PKG-INFO` & `aisp-0.1.21/aisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.1
+Version: 0.1.21
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
 Project-URL: Tracker, https://github.com/AIS-Package/aisp/issues
-Keywords: Artificial Immune Systems,classification,Natural computing,machine learning,artificial intelligence
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -65,15 +64,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -175,15 +174,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/pyproject.toml` & `aisp-0.1.21/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aisp"
-version = "0.1.1"
+version = "0.1.21"
 authors = [
   { name="João Paulo da Silva Barros", email="jpsilvabarr@gmail.com" },
 ]
 
 maintainers = [
   { name="Alison Zille Lopes",  email="alisonzille@gmail.com"},
 ]
@@ -31,17 +31,22 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "numpy>=1.22.4",
     "scipy>=1.8.1",
-    "tqdm==4.64.1",
+    "tqdm>=4.64.1",
 ]
 
+[tool.poetry]
+readme = "README.md"
+
+repository = "https://github.com/AIS-Package/aisp"
+
 keywords = ["Artificial Immune Systems", "classification", "Natural computing", "machine learning", "artificial intelligence"]
 
 [project.urls]
 Homepage = "https://ais-package.github.io/"
 Documentation = "https://ais-package.github.io/docs/intro"
 "Source Code" = "https://github.com/AIS-Package/aisp"
 Tracker = "https://github.com/AIS-Package/aisp/issues"
```

