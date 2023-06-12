# Comparing `tmp/LZGraphs-0.24.tar.gz` & `tmp/LZGraphs-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LZGraphs-0.24.tar", last modified: Sun May 21 15:13:22 2023, max compression
+gzip compressed data, was "LZGraphs-0.25.tar", last modified: Mon Jun 12 07:19:22 2023, max compression
```

## Comparing `LZGraphs-0.24.tar` & `LZGraphs-0.25.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.636351 LZGraphs-0.24/
--rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.24/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.621471 LZGraphs-0.24/LZGraphs/
--rw-rw-rw-   0        0        0    27294 2023-01-16 14:08:57.000000 LZGraphs-0.24/LZGraphs/AminoAcidPositional.py
--rw-rw-rw-   0        0        0     4623 2023-01-17 13:07:44.000000 LZGraphs-0.24/LZGraphs/BOWEncoder.py
--rw-rw-rw-   0        0        0    34791 2023-05-21 14:24:04.000000 LZGraphs-0.24/LZGraphs/LZGraphBase.py
--rw-rw-rw-   0        0        0    28268 2023-05-21 08:25:24.000000 LZGraphs-0.24/LZGraphs/Naive.py
--rw-rw-rw-   0        0        0     6615 2023-05-21 14:47:47.000000 LZGraphs-0.24/LZGraphs/NodeEdgeSaturationProbe.py
--rw-rw-rw-   0        0        0    23781 2023-05-21 08:24:17.000000 LZGraphs-0.24/LZGraphs/NucleotideDoublePositional.py
--rw-rw-rw-   0        0        0     6934 2023-01-16 11:44:39.000000 LZGraphs-0.24/LZGraphs/Utilities.py
--rw-rw-rw-   0        0        0     6386 2023-01-12 07:25:58.000000 LZGraphs-0.24/LZGraphs/Visualize.py
--rw-rw-rw-   0        0        0      356 2023-01-17 13:03:13.000000 LZGraphs-0.24/LZGraphs/__init__.py
--rw-rw-rw-   0        0        0     1077 2023-05-17 13:52:35.000000 LZGraphs-0.24/LZGraphs/decomposition.py
--rw-rw-rw-   0        0        0     2378 2023-01-11 19:06:11.000000 LZGraphs-0.24/LZGraphs/misc.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.635855 LZGraphs-0.24/LZGraphs.egg-info/
--rw-rw-rw-   0        0        0     3939 2023-05-21 15:13:21.000000 LZGraphs-0.24/LZGraphs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 15:13:21.000000 LZGraphs-0.24/LZGraphs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.24/MANIFEST.in
--rw-rw-rw-   0        0        0     3939 2023-05-21 15:13:22.636351 LZGraphs-0.24/PKG-INFO
--rw-rw-rw-   0        0        0     3263 2023-01-17 11:28:03.000000 LZGraphs-0.24/README.md
--rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.24/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-05-21 15:13:22.637342 LZGraphs-0.24/setup.cfg
--rw-rw-rw-   0        0        0     1298 2023-05-21 15:08:36.000000 LZGraphs-0.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.392632 LZGraphs-0.25/
+-rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.25/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.379170 LZGraphs-0.25/LZGraphs/
+-rw-rw-rw-   0        0        0    27173 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/AminoAcidPositional.py
+-rw-rw-rw-   0        0        0     4625 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/BOWEncoder.py
+-rw-rw-rw-   0        0        0    34741 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/LZGraphBase.py
+-rw-rw-rw-   0        0        0    28270 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Naive.py
+-rw-rw-rw-   0        0        0     6600 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/NodeEdgeSaturationProbe.py
+-rw-rw-rw-   0        0        0    23649 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/NucleotideDoublePositional.py
+-rw-rw-rw-   0        0        0     6842 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Utilities.py
+-rw-rw-rw-   0        0        0     6387 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Visualize.py
+-rw-rw-rw-   0        0        0      356 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-05-21 15:14:59.000000 LZGraphs-0.25/LZGraphs/decomposition.py
+-rw-rw-rw-   0        0        0     2380 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/misc.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.392136 LZGraphs-0.25/LZGraphs.egg-info/
+-rw-rw-rw-   0        0        0     4117 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-12 07:19:22.000000 LZGraphs-0.25/LZGraphs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 07:19:22.000000 LZGraphs-0.25/LZGraphs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.25/MANIFEST.in
+-rw-rw-rw-   0        0        0     4117 2023-06-12 07:19:22.393127 LZGraphs-0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     3434 2023-06-12 07:09:33.000000 LZGraphs-0.25/README.md
+-rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.25/pyproject.toml
+-rw-rw-rw-   0        0        0      119 2023-06-12 07:19:22.393624 LZGraphs-0.25/setup.cfg
+-rw-rw-rw-   0        0        0     1331 2023-06-12 07:17:07.000000 LZGraphs-0.25/setup.py
```

### Comparing `LZGraphs-0.24/LICENSE` & `LZGraphs-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.24/LZGraphs/AminoAcidPositional.py` & `LZGraphs-0.25/LZGraphs/AminoAcidPositional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Amino Acid Positional
 import re
-from multiprocessing.pool import ThreadPool
+from time import time
 
 import networkx as nx
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
+from tqdm.auto import tqdm
 
 from .LZGraphBase import LZGraphBase
 from .decomposition import lempel_ziv_decomposition
-from tqdm.auto import tqdm
-import seaborn as sns
-from .misc import chunkify, window, choice
-from time import time
+from .misc import window
 
 
 def derive_lz_and_position(cdr3):
     lzc = lempel_ziv_decomposition(cdr3)
     aux = 0
     cumlen = []
     for sp in lzc:
```

### Comparing `LZGraphs-0.24/LZGraphs/BOWEncoder.py` & `LZGraphs-0.25/LZGraphs/BOWEncoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from collections.abc import Iterable
+
 import numpy as np
 from tqdm.auto import tqdm
-from collections.abc import Iterable
+
 from LZGraphs.decomposition import lempel_ziv_decomposition
 
 
 class LZBOW:
     """
 
          This class supplies a full suite for the conversion of repertoires into a bag of words representation
```

### Comparing `LZGraphs-0.24/LZGraphs/LZGraphBase.py` & `LZGraphs-0.25/LZGraphs/LZGraphBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+import heapq
 import re
-from time import time
+from collections import Counter
 from multiprocessing.pool import ThreadPool
+from time import time
 import networkx as nx
 import numpy as np
 import pandas as pd
-from pandas.io.json import json_normalize
-import heapq
-from .misc import chunkify, window, choice, get_dictionary_subkeys
-from collections import Counter
+from .misc import chunkify, choice, get_dictionary_subkeys
 
 
 class LZGraphBase:
     """
 
          This abstract class provides the base functionality and attributes shared between the different LZGraphs
          (excluding the Naive LZGraph).
```

### Comparing `LZGraphs-0.24/LZGraphs/Naive.py` & `LZGraphs-0.25/LZGraphs/Naive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from itertools import product
+from time import time
+
 import networkx as nx
 import numpy as np
 import pandas as pd
-from .misc import window
+
 from .decomposition import lempel_ziv_decomposition
-from time import time
+from .misc import window
 
 
 def saturation_function(x, h, k):
     """
           a version of the hill saturation function used in the "random_walk_ber_shortest" random walk method
           where based on the parameters the function controls the probability of choosing the shortest path action
           at each step
```

### Comparing `LZGraphs-0.24/LZGraphs/NodeEdgeSaturationProbe.py` & `LZGraphs-0.25/LZGraphs/NodeEdgeSaturationProbe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import random
+
 import numpy as np
+from tqdm.auto import tqdm
+
 from .AminoAcidPositional import derive_lz_and_position
+from .NucleotideDoublePositional import derive_lz_reading_frame_position
 from .decomposition import lempel_ziv_decomposition
 from .misc import window
-from .NucleotideDoublePositional import derive_lz_reading_frame_position
-from tqdm.auto import tqdm
-import itertools
 
 
 class NodeEdgeSaturationProbe:
     """
 
       The class supplies methods used to emulate the creation process of an LZGraph without actually running the full
       creation procedure, rather just accumulate a counter for the number of nodes and edges based on the provided
```

### Comparing `LZGraphs-0.24/LZGraphs/NucleotideDoublePositional.py` & `LZGraphs-0.25/LZGraphs/NucleotideDoublePositional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #Nucleotide Double Positional
-from multiprocessing.pool import ThreadPool
 
-import networkx as nx
+import re
+from time import time
+
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
-from time import time
-from . import LZGraphBase
-from .misc import chunkify, window
 from tqdm.auto import tqdm
-import re
+
+from . import LZGraphBase
 from .decomposition import lempel_ziv_decomposition
-import seaborn as sns
+from .misc import window
+
 
 def derive_lz_reading_frame_position(cdr3):
     """
          given a string this function will return the LZ sub-patterns, the reading frame position of each sub-pattern
          and the start position in the sequence of each sub-patterns in the form of 3 lists.
 
                   Parameters:
```

### Comparing `LZGraphs-0.24/LZGraphs/Utilities.py` & `LZGraphs-0.25/LZGraphs/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import networkx as nx
 import numpy as np
-from .AminoAcidPositional import AAPLZGraph
-from .Naive import NaiveLZGraph
-from .NucleotideDoublePositional import NDPLZGraph
 import pandas as pd
-import networkx as nx
 from tqdm.auto import tqdm
+
+from .Naive import NaiveLZGraph
+
+
 def restore_gene_counts(column):
     """ This function is used during the graph union operation, it converts the gene probability distribution at each
         edge back to a count vector.
                         Args:
                             column (pandas Series): An LZGraph
                         Returns:
                             pandas Series: padnas series of v and j counts instead of probabilites
```

### Comparing `LZGraphs-0.24/LZGraphs/Visualize.py` & `LZGraphs-0.25/LZGraphs/Visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+import networkx as nx
 import numpy as np
 import seaborn as sns
 from matplotlib import pylab
 
-import networkx as nx
 from .decomposition import lempel_ziv_decomposition
+
 mpl.rcParams['figure.figsize'] = (15,8)
 sns.set_context('poster')
 
 def sequence_genomic_edges_variability_plot(graph, cdr3_sample, threshold=None, figsize=None):
     """ Generate a Matplotlib plot that shows the distribution of V and J genes at each edge in a given sequence.
 
               Args:
```

### Comparing `LZGraphs-0.24/LZGraphs/decomposition.py` & `LZGraphs-0.25/LZGraphs/decomposition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import List
 
 def lempel_ziv_decomposition(sequence:str) -> List[str]:
     """
           an implementation of the LZ76 compression algorithm,
           Given a string the function will return all unique sub-patterns derived from the input string
```

### Comparing `LZGraphs-0.24/LZGraphs/misc.py` & `LZGraphs-0.25/LZGraphs/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 - `choice(options,probs)` - choose a random element from a list given a probability distribution over the elements.
 - `window(iterable, size)` - Return a sliding window generator of size "size".
 - `get_dictionary_subkeys(target)` - Returns a list of all sub dictionary keys.
 - `chunkify(L, n)` - Yield successive n-sized chunks from L.
 """
 
 from itertools import tee
+
 import numpy as np
 
+
 def choice(options,probs):
     """Choose a single random variable from a list given a probability distribution
 
       Args:
           options (list): The list of values from which a single random one should be chosen
           probs (float): Probability distribution.
```

### Comparing `LZGraphs-0.24/LZGraphs.egg-info/PKG-INFO` & `LZGraphs-0.25/LZGraphs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LZGraphs
-Version: 0.24
+Version: 0.25
 Summary: An Implementation of LZ76 Based Graphs for Repertoire Representation
-Home-page: https://github.com/MuteJester/LZGraph
-Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz
+Home-page: https://github.com/MuteJester/LZGraphs
+Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.3.tar.gz
 Author: Thomas Konstantinovsky
 Author-email: thomaskon90@gmail.com
 License: MIT
 Keywords: Graph Theory,Immunology,analytics,biology,tcell,repertoire,cdr3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,16 +45,16 @@
 
    </h2>
 
 .. raw:: html
 
    <p align="center">
 
-LZ76 Graphs and Applications in Immunology Explore the docs » View Demo
-· Report Bug · Request Feature
+LZ76 Graphs and Applications in Immunology Explore the docs » Report Bug
+· Request Feature
 
 .. raw:: html
 
    </p>
 
 .. raw:: html
 
@@ -94,14 +94,18 @@
 .. raw:: html
 
    <!-- USAGE EXAMPLES -->
 
 Usage
 -----
 
+We encourage you to either read our docs or download the ``Examples``
+folder from this repo and follow an ineractive jupyer notebook guide to
+use the different models of this repo.
+
 .. raw:: html
 
    <!-- ROADMAP -->
 
 Roadmap
 -------
```

### Comparing `LZGraphs-0.24/PKG-INFO` & `LZGraphs-0.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LZGraphs
-Version: 0.24
+Version: 0.25
 Summary: An Implementation of LZ76 Based Graphs for Repertoire Representation
-Home-page: https://github.com/MuteJester/LZGraph
-Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz
+Home-page: https://github.com/MuteJester/LZGraphs
+Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.3.tar.gz
 Author: Thomas Konstantinovsky
 Author-email: thomaskon90@gmail.com
 License: MIT
 Keywords: Graph Theory,Immunology,analytics,biology,tcell,repertoire,cdr3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,16 +45,16 @@
 
    </h2>
 
 .. raw:: html
 
    <p align="center">
 
-LZ76 Graphs and Applications in Immunology Explore the docs » View Demo
-· Report Bug · Request Feature
+LZ76 Graphs and Applications in Immunology Explore the docs » Report Bug
+· Request Feature
 
 .. raw:: html
 
    </p>
 
 .. raw:: html
 
@@ -94,14 +94,18 @@
 .. raw:: html
 
    <!-- USAGE EXAMPLES -->
 
 Usage
 -----
 
+We encourage you to either read our docs or download the ``Examples``
+folder from this repo and follow an ineractive jupyer notebook guide to
+use the different models of this repo.
+
 .. raw:: html
 
    <!-- ROADMAP -->
 
 Roadmap
 -------
```

### Comparing `LZGraphs-0.24/README.md` & `LZGraphs-0.25/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 
   <p align="center">
     LZ76 Graphs and Applications in Immunology
     <br />
     <a href="https://MuteJester.github.io/LZGraphs/"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/MuteJester/LZGraphs/wiki/">View Demo</a>
-    ·
     <a href="https://github.com/MuteJester/LZGraphs/issues">Report Bug</a>
     ·
     <a href="https://github.com/MuteJester/LZGraphs/issues">Request Feature</a>
   </p>
 </p>
 
 
@@ -55,14 +53,16 @@
 ### Installation
 ```
 pip install LZGraphs
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
+We encourage you to either read our <a href="https://MuteJester.github.io/LZGraphs/"><strong> docs </strong></a> or download the `Examples` folder from this repo and follow an ineractive
+jupyer notebook guide to use the different models of this repo.
 
 
 
 <!-- ROADMAP -->
 ## Roadmap
 
 See the [open issues](https://github.com/MuteJester/LZGraphs/issues) for a list of proposed features (and known issues).
```

#### html2text {}

```diff
@@ -3,26 +3,28 @@
           [license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
 
                                     [Logo]
                              ***** LZGraphs *****
                   LZ76 Graphs and Applications in Immunology
                              Explore_the_docs_Â»
 
-                  View_Demo Â· Report_Bug Â· Request_Feature
+                         Report_Bug Â· Request_Feature
  ## Table of Contents * [About the Project](#about-the-project) * [Usage]
 (#usage) * [Roadmap](#roadmap) * [Contributing](#contributing) * [License]
 (#license) * [Contact](#contact)  ## About The Project LZGraphs :dna: : An
 implementation of the methodology present in the XXX paper ### Installation ```
-pip install LZGraphs ```  ## Usage  ## Roadmap See the [open issues](https://
-github.com/MuteJester/LZGraphs/issues) for a list of proposed features (and
-known issues).  ## Contributing Contributions are what make the open-source
-community such a powerful place to create new ideas, inspire, and make
-progress. Any contributions you make are **greatly appreciated**. 1. Fork the
-Project 2. Create your Feature Branch (`git checkout -b feature/
-AmazingFeature`) 3. Commit your changes (`git commit -m 'Add some
+pip install LZGraphs ```  ## Usage We encourage you to either read our docs or
+download the `Examples` folder from this repo and follow an ineractive jupyer
+notebook guide to use the different models of this repo.  ## Roadmap See the
+[open issues](https://github.com/MuteJester/LZGraphs/issues) for a list of
+proposed features (and known issues).  ## Contributing Contributions are what
+make the open-source community such a powerful place to create new ideas,
+inspire, and make progress. Any contributions you make are **greatly
+appreciated**. 1. Fork the Project 2. Create your Feature Branch (`git checkout
+-b feature/AmazingFeature`) 3. Commit your changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
 license. See `LICENSE` for more information.  ## Contact [Thomas
 Konstantinovsky]() - thomaskon90@gmail.com Project Link: [https://github.com/
 MuteJester/LZGraphs](https://github.com/MuteJester/LZGraphs)  [stars-shield]:
 https://img.shields.io/github/stars/MuteJester/LZGraphs.svg?style=flat-square
 [stars-url]: https://github.com/MuteJester/LZGraphs/stargazers [issues-shield]:
```

### Comparing `LZGraphs-0.24/setup.py` & `LZGraphs-0.25/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 except ImportError:
     print("warning: pypandoc module not found, could not convert Markdown to RST")
     read_md = lambda f: open(f, 'r').read()
 
 setup(
   name = 'LZGraphs',
   packages = ['LZGraphs'],
-  version = '0.24',
+  version = '0.25',
   license='MIT',
   description='An Implementation of LZ76 Based Graphs for Repertoire Representation',
   long_description_content_type="text/markdown",
   long_description=read_md('README.md'),
   author = 'Thomas Konstantinovsky',
   author_email = 'thomaskon90@gmail.com',
-  url='https://github.com/MuteJester/LZGraph',
-  download_url='https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz',
+  url='https://github.com/MuteJester/LZGraphs',
+  download_url='https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.3.tar.gz',
   keywords = ['Graph Theory','Immunology',
               'analytics,biology','tcell','repertoire','cdr3'],   # Keywords that define your package best
     install_requires=[
         'tqdm',
-        'pandas',
+        'numpy==1.21.5',
+        'pandas==1.3.5',
         'networkx==2.8.4',
         'matplotlib==3.5.1',
         'seaborn==0.12.1'
     ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

