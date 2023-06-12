# Comparing `tmp/cmsis_stream-1.3.0-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 76157 bytes, number of entries: 67
+Zip file size: 80185 bytes, number of entries: 67
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -24,17 +24,17 @@
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
 -rw-rw-rw-  2.0 fat     6665 b- defN 23-Jun-06 08:34 cmsis_stream/cg/scheduler/config.py
--rw-rw-rw-  2.0 fat    41606 b- defN 23-Jun-05 08:22 cmsis_stream/cg/scheduler/description.py
--rw-rw-rw-  2.0 fat     1784 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    36807 b- defN 23-Jun-06 05:54 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat    41853 b- defN 23-Jun-09 07:44 cmsis_stream/cg/scheduler/description.py
+-rw-rw-rw-  2.0 fat    10849 b- defN 23-Jun-09 12:50 cmsis_stream/cg/scheduler/graphviz.py
+-rw-rw-rw-  2.0 fat    37754 b- defN 23-Jun-12 08:33 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-05 09:45 cmsis_stream/cg/scheduler/standard.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
 -rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
@@ -43,27 +43,27 @@
 -rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple.cproject.yml
 -rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 -rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
 -rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
 -rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
 -rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/vht.clayer.yml
--rw-rw-rw-  2.0 fat    16526 b- defN 23-Jun-06 08:40 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-06 08:40 cmsis_stream/cg/scheduler/templates/cg_status.h
--rw-rw-rw-  2.0 fat      431 b- defN 23-Jun-01 13:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-02 07:46 cmsis_stream/cg/scheduler/templates/cmsis.py
--rw-rw-rw-  2.0 fat      674 b- defN 23-Jun-01 13:13 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
--rw-rw-rw-  2.0 fat      297 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
+-rw-rw-rw-  2.0 fat    16526 b- defN 23-Jun-12 11:34 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-12 11:34 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat      434 b- defN 23-Jun-12 07:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
+-rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsis.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
 -rw-rw-rw-  2.0 fat     1111 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
--rw-rw-rw-  2.0 fat     3185 b- defN 23-Jun-01 11:18 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
+-rw-rw-rw-  2.0 fat     3305 b- defN 23-Jun-12 05:32 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
 -rw-rw-rw-  2.0 fat     4482 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/commonc.cpp
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/defineConfig.h
--rw-rw-rw-  2.0 fat     4848 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/dot_template.dot
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3506 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6457 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/RECORD
-67 files, 221209 bytes uncompressed, 65603 bytes compressed:  70.3%
+-rw-rw-rw-  2.0 fat     1427 b- defN 23-Jun-12 05:39 cmsis_stream/cg/scheduler/templates/defineConfig.h
+-rw-rw-rw-  2.0 fat     7826 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/dot_template.dot
+-rw-rw-rw-  2.0 fat     7555 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4046 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6473 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/RECORD
+67 files, 242775 bytes uncompressed, 69603 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -153,17 +153,14 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsis.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
-Comment: 
-
 Filename: cmsis_stream/cg/scheduler/templates/code.cpp
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/code.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/code.py
@@ -177,26 +174,29 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/LICENSE.txt
+Filename: cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
+Comment: 
+
+Filename: cmsis_stream-1.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/METADATA
+Filename: cmsis_stream-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/WHEEL
+Filename: cmsis_stream-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/entry_points.txt
+Filename: cmsis_stream-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/top_level.txt
+Filename: cmsis_stream-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.3.0.dist-info/RECORD
+Filename: cmsis_stream-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/description.py

```diff
@@ -28,15 +28,15 @@
 import networkx as nx
 import numpy as np 
 import math 
 
 from sympy import Matrix
 from sympy.core.numbers import ilcm,igcd
 
-from .graphviz import gengraph
+from .graphviz import gengraph,gen_precompute_graph,Style
 from .ccode import gencode as c_gencode
 from .pythoncode import gencode as p_gencode
 
 from .node import *
 from .config import *
 from .standard import Duplicate
 
@@ -185,14 +185,18 @@
 
          # Prefix used to generate the class names
         # of the duplicate nodes like Duplicate2,
         # Duplicate3 ...
         self.duplicateNodeClassName = "Duplicate"
 
 
+    def graphviz(self,f,config=Configuration(),style=Style.default_style()):
+        """Write graphviz into file f""" 
+        gen_precompute_graph(self,f,config,style=style)
+
     def computeTopologicalSortOfNodes(self):
         remaining = self._sortedNodes.copy()
 
         while len(remaining)>0:
             toremove = []
             for n in remaining:
                 if n.nbOutputsForTopologicalSort == 0:
@@ -1105,14 +1109,14 @@
         """Write graphviz into file f""" 
         c_gencode(self,directory,config)
 
     def pythoncode(self,directory,config=Configuration()):
         """Write graphviz into file f""" 
         p_gencode(self,directory,config)
 
-    def graphviz(self,f,config=Configuration()):
+    def graphviz(self,f,config=Configuration(),style=Style.default_style()):
         """Write graphviz into file f""" 
-        gengraph(self,f,config)
+        gengraph(self,f,config,style=style)
```

## cmsis_stream/cg/scheduler/graphviz.py

```diff
@@ -23,28 +23,340 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ############################################
 from jinja2 import Environment, PackageLoader, select_autoescape
 import pathlib
 import os.path
 
-def gengraph(sched,f,config):
+
+
+class Style:
+    _DEFAULT_STYLE = {
+    # Graph global settings
+     "graph_background"      : "white"       # Color of graph background
+    ,"graph_font"            : "Times-Roman" # Font used in the graph
+
+    # Node settings
+    ,"node_color"            : "none"        # Fill color of any node
+    ,"node_boundary_color"   : "black"       # Boundary color of any node
+    ,"node_label_size"       : "14.0"        # Font size of node labels
+    ,"node_label_color"      : "black"       # Color of node labels
+
+    # Special node settings (Constant node and delay box)
+    ,"special_node_border"   : "1"           # Thickness of node boundary
+
+    # Node port settings
+    ,"port_sample_color"     : "blue"        # Color of number of samples
+    ,"port_sample_font_size" : "12.0"        # Font size of number of samples
+
+    ,"port_font_color"       : "black"       # Color of a port
+    ,"port_font_size"        : "12.0"        # Font size of a port
+
+    # Edge settings
+    ,"edge_color"            : "black"       # Color of any edge
+    ,"edge_label_size"       : "12.0"        # Font size of any edge label
+    ,"edge_label_color"      : "black"       # Color of any edge label
+    ,"edge_style"            : "solid"       # Edge style (dashed, dotted ...)
+    ,"arrow_size"            : 0.5           # Arrow size at end of edge
+
+    }
+
+    _DARK_STYLE = {
+         "graph_background"      : "black"
+        ,"node_boundary_color"   : "white"
+        ,"node_label_color"      : "white"
+
+        ,"port_font_color"       : "white"
+
+        ,"port_sample_color"     : "green"
+
+        ,"edge_color"            : "white"
+        ,"edge_label_color"      : "white"
+
+    }
+
+    def __getitem__(self,name):
+        """Present styles from the dictionary as keys"""
+        if name in self._s:
+           return(self._s[name])
+        raise IndexError 
+
+    # Set default styles when a valuie for a style
+    # is not available in the current style
+    def _cleanStyle(self):
+        for k in Style._DEFAULT_STYLE:
+            if not k in self._s:
+                self._s[k] = Style._DEFAULT_STYLE[k]
+
+    def __init__(self,style=_DEFAULT_STYLE):
+        self._s = style 
+        # Force missing values to default values
+        self._cleanStyle()
+
+    # Create a style object with the default style
+    @classmethod
+    def default_style(cls):
+        return cls(style=cls._DEFAULT_STYLE)
+
+    # Create a style object with the dark style
+    @classmethod
+    def dark_style(cls):
+        return cls(style=cls._DARK_STYLE)
+
+    
+    # Check if an edge is a FIFO (post-schedule graph)
+    # or a pair of ios (pre-schedule graph)
+    def isFIFO(self,edge):
+        return (not (type(edge) is tuple))
+
+    # Return the length of a FIFO or none
+    # if the edge is not a FIFO (pre-schedule)
+    # graph
+    # But, in pre-schedule graph this function is
+    # never called
+    def fifoLength(self,edge):
+        if self.isFIFO(edge):
+            return(edge.length)
+        else:
+            return None
+
+    # Get the src node of an edge
+    def edgeSrcNode(self,edge):
+        if not (self.isFIFO(edge)):
+            return(edge[0].owner)
+        else:
+           return(edge.src.owner)
+
+    # Get the dst node of and egde
+    def edgeDstNode(self,edge):
+        if not (self.isFIFO(edge)):
+            return(edge[1].owner)
+        else:
+           return(edge.dst.owner)
+
+    # Get the src port of an edge
+    def edgeSrcPort(self,edge):
+        if not (self.isFIFO(edge)):
+            return(edge[0])
+        else:
+           return(edge.src)
+
+    # Get the dst port of and egde
+    def edgeDstPort(self,edge):
+        if not (self.isFIFO(edge)):
+            return(edge[1])
+        else:
+           return(edge.dst)
+
+    # Get port ID on item (input or output)
+    def getPort(self,item,i,input=False):
+        if input:
+            return(item.inputPortFromID(i))
+        else:
+            return(item.outputPortFromID(i))
+          
+
+    ############################
+    #
+    # NORMAL NODE CUSTOMIZATION
+    #
+
+    # fill color value
+    def node_color(self,node):
+        return(self["node_color"])
+
+    # Boundary color value
+    def node_boundary_color(self,node):
+        return(self["node_boundary_color"])
+
+    # Color of node label
+    def node_label_color(self,node):
+        return(self["node_label_color"])
+
+    # Font size of node label
+    def node_label_size(self,node):
+        return(self["node_label_size"])
+
+    # Node label
+    def node_label(self,node):
+        return node.graphvizName
+
+    ############################
+    #
+    # DELAY NODE CUSTOMIZATION
+    #
+
+    # fill color value
+    def delay_color(self,delay_value):
+        return(self["node_color"])
+
+    # delay boundary thickness
+    def delay_border(self,delay_value):
+        return(self["special_node_border"])
+
+    # delay boundary color
+    def delay_boundary_color(self,delay_value):
+        return(self["node_boundary_color"])
+
+    # delay label color
+    def delay_label_color(self,delay_value):
+        return(self["node_label_color"])
+
+    # delay label size
+    def delay_label_size(self,delay_value):
+        return(self["node_label_size"])
+
+    ############################
+    #
+    # CONST NODE CUSTOMIZATION
+    #
+
+    # fill color value
+    def const_color(self,const_name):
+        return(self["node_color"])
+
+    # const node boundary thickness
+    def const_border(self,const_name):
+        return(self["special_node_border"])
+
+    # const node boundary color
+    def const_boundary_color(self,const_name):
+        return(self["node_boundary_color"])
+
+    # const label color
+    def const_label_color(self,const_name):
+        return(self["node_label_color"])
+
+    # const label font size
+    def const_label_size(self,const_name):
+        return(self["node_label_size"])
+
+    
+    ############################
+    #
+    # NODE PORT CUSTOMIZATION
+    #
+
+    # Color of number of samples produced or
+    # consumed by a port
+    def port_sample_color(self,nb_sample):
+        return(self["port_sample_color"])
+
+    # Font size of number of samples produced or
+    # consumed by a port
+    def port_sample_font_size(self,nb_sample):
+        return(self["port_sample_font_size"])
+
+    # Color of a port
+    def port_font_color(self,item,i,input=False):
+        # item.outputNames[0]
+        return(self["port_font_color"])
+
+    # Font size of a port
+    def port_font_size(self,item,i,input=False):
+        return(self["port_font_size"])
+
+    ############################
+    #
+    # NORMAL EDGE CUSTOMIZATION
+    #
+
+    # edge color
+    def edge_color(self,edge):
+        return(self["edge_color"])
+
+    # edge label color
+    def edge_label_color(self,edge):
+        return(self["edge_label_color"])
+
+    # edge label font size
+    def edge_label_size(self,edge):
+        return(self["edge_label_size"])
+
+    # edge style (dashed, dotted ...)
+    def edge_style(self,edge):
+        return(self["edge_style"])
+
+    # Label on the edge
+    # (By default datatype and number of samples)
+    def edge_label(self,fifo,typeName,length):
+        return f"{typeName}({length})"
+
+    ############################
+    #
+    # DELAY EDGE CUSTOMIZATION
+    #
+
+    # edge color for the edge entering a delay box
+    def delay_edge_color(self,srcPort,nb_samples):
+        return(self["edge_color"])
+
+    # edge style for the edge entering the delay box
+    # (dashed, dotted ...)
+    def delay_edge_style(self,srcPort,nb_samples):
+        return(self["edge_style"])
+
+    ############################
+    #
+    # CONST EDGE CUSTOMIZATION
+    #
+
+    # Color of edge connecting a constant node
+    def const_edge_color(self,name,dstPort):
+        return(self["edge_color"])
+
+    # Style of edge connecting a constant node
+    # (dashed, dotted)
+    def const_edge_style(self,name,dstPort):
+        return(self["edge_style"])
+
+# Generate a graph before schedule computation
+# It is working with a graph that ha sno FIFOs but only
+# edges (pair of input / output ports)
+def gen_precompute_graph(g,f,config,style=Style.default_style()):
+    env = Environment(
+       loader=PackageLoader("cmsis_stream.cg.scheduler"),
+       autoescape=select_autoescape(),
+       trim_blocks=True
+    )
+
+    constObjs = list(set([x[0] for x in g.constantEdges]))
+    template = env.get_template("precompute_dot_template.dot")
+
+    nbFifos = len(g.edges)
+
+    print(template.render(style=style,
+      graph=g,
+      nodes=g.nodes,
+      edges=g.edges,
+      fifos=g.edges,
+      nbFifos=nbFifos,
+      constEdges=g.constantEdges,
+      nbConstEdges=len(g.constantEdges),
+      constObjs=constObjs,
+      config=config
+      ),file=f)
+
+# Work with a graph after schedule computation
+# It has access to schedule information and FIFOs
+def gengraph(sched,f,config,style=Style.default_style()):
 
     env = Environment(
        loader=PackageLoader("cmsis_stream.cg.scheduler"),
        autoescape=select_autoescape(),
        trim_blocks=True
     )
     
     constObjs = list(set([x[0] for x in sched.constantEdges]))
     template = env.get_template("dot_template.dot")
 
     nbFifos = len(sched._graph._allFIFOs)
 
-    print(template.render(graph=sched,
+    print(template.render(style=style,
+      graph=sched,
       nodes=sched.nodes,
       edges=sched.edges,
       fifos=sched._graph._allFIFOs,
       nbFifos=nbFifos,
       constEdges=sched.constantEdges,
       nbConstEdges=len(sched.constantEdges),
       constObjs=constObjs,
```

## cmsis_stream/cg/scheduler/node.py

```diff
@@ -569,19 +569,28 @@
 
 
     @property
     def graphvizName(self):
         """Name for graph vizualization"""
         return ("%s<BR/>(%s)" % (self.nodeName,self.typeName))
 
+    def inputPortFromID(self,i):
+        r = sorted(list(self._inputs.keys()))
+        k = r[i]
+        return self._inputs[k]
+    
+    def outputPortFromID(self,i):
+        r = sorted(list(self._outputs.keys()))
+        k = r[i]
+        return self._outputs[k]
+
     @property
     def inputNames(self):
         return sorted(list(self._inputs.keys()))
 
-
     @property
     def outputNames(self):
         return sorted(list(self._outputs.keys()))
 
     @property
     def hasManyInputs(self):
         return len(self._inputs.keys())>1
@@ -617,28 +626,38 @@
     
 
 class GenericSink(BaseNode):
     """A sink in the dataflow graph""" 
 
     def __init__(self,name):
         BaseNode.__init__(self,name)
+        self._isPureNode = False
+    
+    @property
+    def isPureNode(self):
+        return self._isPureNode
 
     @property
     def typeName(self):
         return "void"
 
     def addInput(self,name,theType,theLength):
         self._inputs[name]=Input(self,name,theType,theLength)
 
 
 class GenericSource(BaseNode):
     """A source in the dataflow graph""" 
 
     def __init__(self,name):
         BaseNode.__init__(self,name)
+        self._isPureNode = False
+    
+    @property
+    def isPureNode(self):
+        return self._isPureNode
 
     @property
     def typeName(self):
         return "void"
 
     def addOutput(self,name,theType,theLength):
         self._outputs[name]=Output(self,name,theType,theLength)
@@ -942,54 +961,57 @@
     @property
     def typeName(self):
         return "OverlapAdd"
 
 
 
 
+class ArgLength():
+    def __init__(self,n,sample_unit=True):
+        self.name = n 
+        self.sample_unit = sample_unit
+
+
 # Pure compute functions
 # It is supporting unary function (src,dst,blockize)
 # and binary functions (sraa,srcb, dst, blocksize)
 # For cmsis, the prefix arm and the type suffix are not needed
 # if class Dsp is used
 class GenericFunction(GenericNode):
     # Number of function node of each category
     # Used to generate unique ID and names when
     # unique names are required
     # like for creating the graph where each call to
     # the same function must be identified as a
     # separate node
     NODEID={}
-    PUREID=1
-
 
     ENV = Environment(
        loader=PackageLoader("cmsis_stream.cg.scheduler"),
        autoescape=select_autoescape(),
        lstrip_blocks=True,
        trim_blocks=True
     )
     
     CTEMPLATE = ENV.get_template("cmsis.cpp")
     CCHECKTEMPLATE = ENV.get_template("cmsisCheck.cpp")
-    CNODETEMPLATE = ENV.get_template("cmsisNode.cpp")
 
     PYTEMPLATE = ENV.get_template("cmsis.py")
 
-    def __init__(self,funcname,theType,length):
+    def __init__(self,funcname,argsDesc):
         if not (funcname in GenericFunction.NODEID):
             GenericFunction.NODEID[funcname]=1 
 
-        GenericFunction.PUREID = GenericFunction.PUREID + 1
         GenericNode.__init__(self,"%s%d" % (funcname,GenericFunction.NODEID[funcname]))
 
         self._hasState = False
-        self._length = length 
+        #self._length = length 
         self._nodeName = funcname
         self._isPureNode = True
+        self._argsDesc = argsDesc
 
         GenericFunction.NODEID[funcname]=GenericFunction.NODEID[funcname]+1
 
     @property
     def realInputs(self):
         return self._realInputs
     
@@ -1027,24 +1049,14 @@
     def datatypeForConstructor(self):
         return self._datatypeForConstructor
 
     @property
     def genericConstructorArgs(self):
         return self._genericConstructorArgs
     
-    
-    
-    
-    @property 
-    def nodeKind(self):
-        if (self._realInputs + self._realOutputs) == 2:
-           return "GenericNode"
-        else:
-           return "GenericNode21"
-
 
     @property
     def hasState(self):
         return self._hasState
     
 
     @property
@@ -1053,91 +1065,138 @@
 
     # Prepare for code generation.
     # All those values are used in the
     # code generation template
     # They are both used for the run part
     # and the prepareForRunning part
     def _prepareForCodeGen(self,ctemplate=True):
-       if ctemplate:
-         theType=self._inputs[self.inputNames[0]].ctype
-       else:
-         theType=self._inputs[self.inputNames[0]].nptype
-       # For cyclo static scheduling, nbSamples may be a list
-       # and in this case we are using the max value
-       nbSamples = self._inputs[self.inputNames[0]].nbSamples
-       if isinstance(nbSamples,int):
-          theLen = self._inputs[self.inputNames[0]].nbSamples
-       else:
-          theLen = np.max(nbSamples)
+       
        theId = 0
        # List of buffer and corresponding fifo to initialize buffers
        inputs=[]
        outputs=[]
        # List of buffers variable to declare
        ptrs=[]
 
        # Argument names (buffer or constant node)
-       args=[]
        inargs=[]
        outargs=[]
 
        argsStr=""
        inArgsStr=""
        outArgsStr=""
        inputId=1
        outputId=1
+       fifoToBuf = {}
        for io in self.inputNames:
             ioObj = self._inputs[io] 
             if ioObj.constantNode:
                # Argument is name of constant Node
-               args.append(ioObj.constantNode.name)
                inargs.append(ioObj.constantNode.name)
+               fifoToBuf[io] = ioObj.constantNode.name
             else:
+               if ctemplate:
+                    the_type = ioObj.ctype
+               else:
+                    the_type = ioObj.nptype
                # Argument is a buffer created from FIFO
                buf = "i%d" % theId
-               ptrs.append(buf)
-               args.append(buf)
+               ptrs.append((the_type,buf))
                inargs.append(buf)
-               if self.realInputs == 1:
-                  readFuncName="getReadBuffer"
-               else:
-                  readFuncName="getReadBuffer%d"%inputId
+               fifoToBuf[io] = buf
+               
                # Buffer and fifo
-               inputs.append((buf,self.listOfargs[theId],readFuncName))
+               nb = ioObj.nbSamples
+               inputs.append((buf,self.listOfargs[theId],nb))
                inputId = inputId + 1
             theId = theId + 1
        for io in self.outputNames:
+            ioObj = self._outputs[io] 
+            if ctemplate:
+                the_type = ioObj.ctype
+            else:
+                the_type = ioObj.nptype
             buf = "o%d" % theId
-            ptrs.append(buf)
-            args.append(buf)
+            ptrs.append((the_type,buf))
             outargs.append(buf)
-            writeFuncName="getWriteBuffer"
-
-            outputs.append((buf,self.listOfargs[theId],writeFuncName))
+            fifoToBuf[io] = buf
+            nb = ioObj.nbSamples
+            outputs.append((buf,self.listOfargs[theId],nb))
             outputId = outputId + 1
             theId = theId + 1
 
+       sched = []
+       if self.schedArgs:
+            for lit in self.schedArgs:
+                sched.append(lit.arg)
+
+       args=[]
+       # inargs and outargs are used for Python version
+       # of a pure function
+       inargs=[] 
+       outargs=[]
+       for a in self._argsDesc:
+           # Name of an IO
+           if isinstance(a,str):
+              args.append(fifoToBuf[a])
+              if a in self._inputs:
+                 inargs.append(fifoToBuf[a])
+              else:
+                 outargs.append(fifoToBuf[a])
+           # ID of a special argument (literal or C
+           # variable)
+           elif isinstance(a,int):
+              args.append(sched[a])
+              inargs.append(sched[a])
+           # FIFO lengths
+           else:
+              # Length description for an IO
+              # For Python, length is derived from
+              # the array so it is not passed as
+              # argument and those arguments
+              # are ignored for the generated Python API
+              nb = None 
+              the_type = None
+              isInput = False
+              # Get the type and the number of samples
+              # for the IO
+              if a.name in self._inputs:
+                 isInput = True
+                 nb = self._inputs[a.name].nbSamples
+                 if ctemplate:
+                    the_type = self._inputs[a.name].ctype
+                 else:
+                    the_type = self._inputs[a.name].nptype
+              if a.name in self._outputs:
+                 nb = self._outputs[a.name].nbSamples
+                 if ctemplate:
+                    the_type = self._outputs[a.name].ctype
+                 else:
+                    the_type = self._outputs[a.name].nptype
+              
+              if a.sample_unit:
+                 args.append(f"{nb}")
+              else:
+                 args.append(f"sizeof({the_type})*{nb}")
+                 
+
        argsStr="".join(joinit(args,","))
        inArgsStr="".join(joinit(inargs,","))
        outArgsStr="".join(joinit(outargs,","))
 
-       return ({"theType" : theType,
-               "nb" : theLen,
-               "ptrs" : ptrs,
+       return ({"ptrs" : ptrs,
                "args" : argsStr,
                "inArgsStr" : inArgsStr,
                "outArgsStr" :outArgsStr,
                "inputs":inputs, 
                "outputs":outputs})
 
     def cCheck(self,asyncDefaultSkip=True):
         params = self._prepareForCodeGen(True)
-        result=Dsp.CCHECKTEMPLATE.render(func=self._nodeName,
-           theType = params["theType"],
-           nb = params["nb"],
+        result=GenericFunction.CCHECKTEMPLATE.render(func=self._nodeName,
            ptrs = params["ptrs"],
            args = params["args"],
            inputs=params["inputs"], 
            outputs=params["outputs"],
            node=self,
            asyncDefaultSkip = asyncDefaultSkip
            )
@@ -1145,82 +1204,52 @@
         
 
     # To clean
     def cRun(self,config,ctemplate=True):
        params = self._prepareForCodeGen(ctemplate)
 
        if ctemplate:
-              result=Dsp.CTEMPLATE.render(func=self._nodeName,
-               theType = params["theType"],
-               nb = params["nb"],
+              result=GenericFunction.CTEMPLATE.render(func=self._nodeName,
                ptrs = params["ptrs"],
                args = params["args"],
                inputs=params["inputs"], 
                outputs=params["outputs"],
                node=self
                )
        else:
-           result=Dsp.PYTEMPLATE.render(func=self._nodeName,
-            theType = params["theType"],
-            nb = params["nb"],
+           result=GenericFunction.PYTEMPLATE.render(func=self._nodeName,
             ptrs = params["ptrs"],
             args = params["args"],
             inArgs= params["inArgsStr"], 
             outArgs= params["outArgsStr"], 
             inputs=params["inputs"], 
             outputs=params["outputs"],
             node=self
             )
        return(result)
 
     
 class Unary(GenericFunction):
     def __init__(self,funcname,theType,length,input_name="i",output_name="o"):
-        GenericFunction.__init__(self,funcname,theType,length)
+        GenericFunction.__init__(self,funcname,
+            [input_name
+            ,output_name
+            ,ArgLength(output_name)])
+
+
 
         self.addInput(input_name,theType,length)
         self.addOutput(output_name,theType,length)
 
 
 class Binary(GenericFunction):
     def __init__(self,funcname,theType,length,input_names=["ia","ib"],output_name="o"):
-        GenericFunction.__init__(self,funcname,theType,length)
+        GenericFunction.__init__(self,funcname,
+            [input_names[0]
+            ,input_names[1]
+            ,output_name
+            ,ArgLength(output_name)])
 
         self.addInput(input_names[0],theType,length)
         self.addInput(input_names[1],theType,length)
         
-        self.addOutput(output_name,theType,length)
-
-
-    
-
-
-BINARYOP=["scale","add","and","mult","not","or","sub","xor","cmplx_mult_cmplx","cmplx_mult_real"
-]
-
-class Dsp(GenericFunction):
-
-    def __init__(self,name,theType,length,input_name="i",input_names=["ia","ib"],output_name="o"):
-        # Some different graph functions correspond to the same
-        # DSP function like IFFT
-        # So we rename the cmsis function to call the same function
-        
-        cmsisname = "arm_%s_%s" % (name,theType.dspExtension)
-        GenericFunction.__init__(self, cmsisname,theType,length)
-        self._binary=True
-        
-        if name in BINARYOP:
-            self.addInput(input_names[0],theType,length)
-            self.addInput(input_names[1],theType,length)
-            self._binary=True
-        else:
-           self.addInput(input_name,theType,length)
-           self._binary=False
-        
-        self.addOutput(output_name,theType,length)
-
-    
-
-    @property
-    def typeName(self):
-        return "CMSIS-DSP"
-  
+        self.addOutput(output_name,theType,length)
```

## cmsis_stream/cg/scheduler/templates/cmsis.cpp

```diff
@@ -1,15 +1,15 @@
 
                   {
 
 {% for ptr in ptrs %}
-                   {{theType}}* {{ptr}};
+                   {{ptr[0]}}* {{ptr[1]}};
 {% endfor %}
 {% for ptr in inputs %}
-                   {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{nb}});
+                   {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{ptr[2]}});
 {% endfor %}
 {% for ptr in outputs %}
-                   {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{nb}});
+                   {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{ptr[2]}});
 {% endfor %}
-                   {{func}}({{args}},{{nb}});
+                   {{func}}({{args}});
                    cgStaticError = 0;
                   }
```

## cmsis_stream/cg/scheduler/templates/cmsis.py

```diff
@@ -1,10 +1,10 @@
 
 {% for ptr in inputs %}
-       {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{nb}})
+       {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{ptr[2]}})
 {% endfor %}
 {% for ptr in outputs %}
-       {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{nb}})
+       {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{ptr[2]}})
 {% endfor %}
        {{outArgs}}[:]=dsp.{{func}}({{inArgs}})
        cgStaticError = 0
```

## cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp

```diff
@@ -1,14 +1,14 @@
                     
                     bool canRun=true;
 {% for ptr in inputs %}
-                    canRun &= !({{ptr[1].access}}willUnderflowWith({{nb}}));
+                    canRun &= !({{ptr[1].access}}willUnderflowWith({{ptr[2]}}));
 {% endfor %}
 {% for ptr in outputs %}
-                    canRun &= !({{ptr[1].access}}willOverflowWith({{nb}}));
+                    canRun &= !({{ptr[1].access}}willOverflowWith({{ptr[2]}}));
 {% endfor %}
 
                     if (!canRun)
                     {
 {% if asyncDefaultSkip %}
                       cgStaticError = CG_SKIP_EXECUTION_ID_CODE;
 {% else %}
```

## cmsis_stream/cg/scheduler/templates/codeSwitch.cpp

```diff
@@ -30,14 +30,15 @@
             {% if config.eventRecorder -%}
             EventRecord2 (Evt_Node, schedule[id], 0);
             {% endif -%}
             CG_BEFORE_NODE_EXECUTION;
 
             {% if config.asynchronous -%}
             cgStaticError = 0;
+            CG_ASYNC_BEFORE_NODE_CHECK;
             switch(schedule[id])
             {
                 {% for nodeID in range(nbNodes) -%}
                 case {{nodeID}}:
                 {
                     {% if not nodes[nodeID].isPureNode -%}
                     {%- if not config.heapAllocation -%}
@@ -54,17 +55,20 @@
 
                 {% endfor -%}
 
                 default:
                 break;
             }
 
+            CG_ASYNC_AFTER_NODE_CHECK;
+
             if (cgStaticError == CG_SKIP_EXECUTION_ID_CODE)
             { 
               cgStaticError = 0;
+              CG_NODE_NOT_EXECUTED;
               continue;
             }
 
             {% if config.eventRecorder -%}
             if (cgStaticError<0)
             {
                 EventRecord2 (Evt_Error, cgStaticError, 0);
```

## cmsis_stream/cg/scheduler/templates/defineConfig.h

```diff
@@ -48,8 +48,26 @@
 
 #if !defined(CG_BEFORE_NODE_EXECUTION)
 #define CG_BEFORE_NODE_EXECUTION
 #endif
 
 #if !defined(CG_AFTER_NODE_EXECUTION)
 #define CG_AFTER_NODE_EXECUTION
-#endif
+#endif
+
+{% if config.asynchronous -%}
+#if !defined(CG_AFTER_NODE_EXECUTION)
+#define CG_AFTER_NODE_EXECUTION
+#endif
+
+#if !defined(CG_NODE_NOT_EXECUTED)
+#define CG_NODE_NOT_EXECUTED
+#endif
+
+#if !defined(CG_ASYNC_BEFORE_NODE_CHECK)
+#define CG_ASYNC_BEFORE_NODE_CHECK
+#endif
+
+#if !defined(CG_ASYNC_AFTER_NODE_CHECK)
+#define CG_ASYNC_AFTER_NODE_CHECK
+#endif
+{% endif %}
```

## cmsis_stream/cg/scheduler/templates/dot_template.dot

```diff
@@ -3,113 +3,113 @@
 {{node.nodeName}}{% else %}
 {% if not node.hasManyIOs %}{{node.nodeID}}:i{% else %}{{node.nodeID}}:{{theio.name}}{% endif %}
 {% endif %}
 {%- endmacro %}
 
 {% macro edgelabel(ioport,name) -%}
 {% if not ioport.owner.isDuplicateNode %}
-,{{name}}=<<TABLE BORDER="0" CELLPADDING="2"><TR><TD><FONT COLOR="blue" POINT-SIZE="12.0" >{{ioport.nbSamples}}</FONT>
+,{{name}}=<<TABLE BORDER="0" CELLPADDING="4"><TR><TD><FONT COLOR="{{style.port_sample_color(ioport.nbSamples)}}" POINT-SIZE="{{style.port_sample_font_size(ioport.nbSamples)}}" >{{ioport.nbSamples}}</FONT>
 </TD></TR></TABLE>>{% endif %}
 {%- endmacro %}
 
 {% macro constdst(theID) -%}
 {{constEdges[theID][1].owner.nodeID}}:{{constEdges[theID][1].name}}
 {% endmacro -%}
 
 {% macro delayBoxID(id) -%}{{fifos[id].src.owner.nodeID}}{{fifos[id].dst.owner.nodeID}}Delay{%- endmacro %}
 
 {% macro delayBox(edge) -%}
 {% if fifos[edge].hasDelay %}
 {{delayBoxID(edge)}} [label=<
-<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+<TABLE color="{{style.delay_boundary_color(fifos[edge].delay)}}" bgcolor="{{style.delay_color(fifos[edge].delay)}}" BORDER="0" CELLBORDER="{{style.delay_border(fifos[edge].delay)}}" CELLSPACING="0" CELLPADDING="4">
   <TR>
-    <TD ALIGN="CENTER" PORT="i">{{fifos[edge].delay}}</TD>
+    <TD ALIGN="CENTER" PORT="i"><FONT COLOR="{{style.delay_label_color(fifos[edge].delay)}}" POINT-SIZE="{{style.delay_label_size(fifos[edge].delay)}}">{{fifos[edge].delay}}</FONT></TD>
   </TR>
 </TABLE>>];
 {% endif %}
 {%- endmacro %}
 
 digraph structs {
-    node [shape=plaintext]
+    bgcolor = "{{style['graph_background']}}"
+    node [shape=plaintext,color="{{style['node_boundary_color']}}",fontcolor="{{style['node_label_color']}}",fontname="{{style['graph_font']}}"]
 {% if config.horizontal %}
     rankdir=LR
 {% endif %}
-    edge [arrowsize=0.5]
-    fontname="times"
+    edge [arrowsize="{{style['arrow_size']}}",color="{{style['edge_color']}}",fontcolor="{{style['edge_label_color']}}",fontname="{{style['graph_font']}}"]
 
 {% for item in nodes %}
 
 {% if item.isDuplicateNode %}
-{{item.nodeID}} [shape=point,label={{item.nodeName}}]
+{{item.nodeID}} [shape=point,label="{{item.nodeName}}"]
 {% else %}
 {% if not item.hasManyIOs %}
 {{item.nodeID}} [label=<
-<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+<TABLE color="{{style.node_boundary_color(item)}}" bgcolor="{{style.node_color(item)}}" BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
   <TR>
-    <TD ALIGN="CENTER" PORT="i">{{item.graphvizName}}</TD>
+    <TD ALIGN="CENTER" PORT="i"><FONT COLOR="{{style.node_label_color(item)}}" POINT-SIZE="{{style.node_label_size(item)}}">{{ style.node_label(item) }}</FONT></TD>
   </TR>
 </TABLE>>];
 {% else %}
 
 {% if not config.horizontal %}
 
 {{item.nodeID}} [label=<
-<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+<TABLE color="{{style.node_boundary_color(item)}}" bgcolor="{{style.node_color(item)}}" BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
   <TR>
     {% for id in range(0,item.maxNbIOs) -%}
     {% if item.inputNames[id] -%}
     {% set input %}{{item.inputNames[id]}}{% endset %}
-    <TD PORT="{{input}}"><FONT POINT-SIZE="9.0">{{input}}</FONT></TD>
+    <TD PORT="{{input}}"><FONT POINT-SIZE="{{style.port_font_size(item,id,input=True)}}" COLOR="{{style.port_font_color(item,id,input=True)}}">{{input}}</FONT></TD>
     {% else %}
     <TD></TD>
     {%- endif %}
     {%- endfor %}
   </TR>
   <TR>
-    <TD ALIGN="CENTER" COLSPAN="{{item.maxNbIOs}}">{{ item.graphvizName }}</TD>
+    <TD ALIGN="CENTER" COLSPAN="{{item.maxNbIOs}}"><FONT COLOR="{{style.node_label_color(item)}}" POINT-SIZE="{{style.node_label_size(item)}}">{{ style.node_label(item) }}</FONT></TD>
   </TR>
   <TR>
     {% for id in range(0,item.maxNbIOs) -%}
     {% if item.outputNames[id] -%}
     {% set output %}{{item.outputNames[id]}}{% endset %}
-    <TD PORT="{{output}}"><FONT POINT-SIZE="9.0">{{output}}</FONT></TD>
+    <TD PORT="{{output}}"><FONT POINT-SIZE="{{style.port_font_size(item,id)}}" COLOR="{{style.port_font_color(item,id)}}">{{output}}</FONT></TD>
     {% else %}
     <TD></TD>
     {%- endif %}
     {%- endfor %}
   </TR>
 </TABLE>>];
 {% else %}
 {{item.nodeID}} [label=<
-<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+<TABLE color="{{style.node_boundary_color(item)}}" bgcolor="{{style.node_color(item)}}" BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
   <TR>
 {% if item.inputNames[0] is defined %}
-    <TD PORT="{{item.inputNames[0]}}"><FONT POINT-SIZE="9.0">{{item.inputNames[0]}}</FONT></TD>
+    <TD PORT="{{item.inputNames[0]}}"><FONT POINT-SIZE="{{style.port_font_size(item,0,input=True)}}" COLOR="{{style.port_font_color(item,0,input=True)}}">{{item.inputNames[0]}}</FONT></TD>
 {% else %}
     <TD></TD>
 {% endif %}
-    <TD ALIGN="CENTER" ROWSPAN="{{item.maxNbIOs}}">{{ item.graphvizName }}</TD>
+    <TD ALIGN="CENTER" ROWSPAN="{{item.maxNbIOs}}"><FONT COLOR="{{style.node_label_color(item)}}" POINT-SIZE="{{style.node_label_size(item)}}">{{ style.node_label(item) }}</FONT></TD>
 {% if item.outputNames[0] is defined %}
-    <TD PORT="{{item.outputNames[0]}}"><FONT POINT-SIZE="9.0">{{item.outputNames[0]}}</FONT></TD>
+    <TD PORT="{{item.outputNames[0]}}"><FONT POINT-SIZE="{{style.port_font_size(item,0)}}" COLOR="{{style.port_font_color(item,0)}}">{{item.outputNames[0]}}</FONT></TD>
 {% else %}
     <TD></TD>
 {% endif %}
   </TR>
 {% for id in range(1,item.maxNbIOs) -%}
 <TR>
 {% if item.inputNames[id] -%}
 {% set input %}{{item.inputNames[id]}}{% endset %}
-<TD PORT="{{input}}"><FONT POINT-SIZE="9.0">{{input}}</FONT></TD>
+<TD PORT="{{input}}"><FONT POINT-SIZE="{{style.port_font_size(item,id,input=True)}}" COLOR="{{style.port_font_color(item,id,input=True)}}">{{input}}</FONT></TD>
 {% else %} 
 <TD></TD>
 {%- endif %}
 
 {% if item.outputNames[id] -%}
 {% set output %}{{item.outputNames[id]}}{% endset %}
-<TD PORT="{{output}}"><FONT POINT-SIZE="9.0">{{output}}</FONT></TD>
+<TD PORT="{{output}}"><FONT POINT-SIZE="{{style.port_font_size(item,id)}}" COLOR="{{style.port_font_color(item,id)}}">{{output}}</FONT></TD>
 {% else %} 
 <TD></TD>
 {%- endif %}
 </TR>
 {%- endfor %}
 
 
@@ -120,43 +120,43 @@
 {% endfor %}
 
 
 {% for id in range(nbFifos) %}
 {{delayBox(id)}}
 {% if fifos[id].hasDelay %}
 
-{{io(fifos[id].src.owner,fifos[id].src)}} -> {{delayBoxID(id)}}:i [label=""{{edgelabel(fifos[id].src,"taillabel")}}]
+{{io(fifos[id].src.owner,fifos[id].src)}} -> {{delayBoxID(id)}}:i [style="{{style.delay_edge_style(fifos[id].src,fifos[id].delay)}}",color="{{style.delay_edge_color(fifos[id].src,fifos[id].delay)}}",label=""{{edgelabel(fifos[id].src,"taillabel")}}]
 
 {% if config.displayFIFOBuf %}
-{{delayBoxID(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="buf{{fifos[id].bufferID}}"
+{{delayBoxID(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos[id])}}",label="buf{{fifos[id].bufferID}}"
 {{edgelabel(fifos[id].src,"headlabel")}}]
 {% else %}
-{{delayBoxID(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="{{fifos[id].theType.graphViztype}}({{fifos[id].length}})"
+{{delayBoxID(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos[id])}}",label=<{{style.edge_label(fifos[id],fifos[id].theType.graphViztype,fifos[id].length)}}>
 {{edgelabel(fifos[id].dst,"headlabel")}}]
 {% endif %}
 
 {% else %}
 {% if config.displayFIFOBuf %}
-{{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="buf{{fifos[id].bufferID}}"
+{{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos[id])}}",label="buf{{fifos[id].bufferID}}"
 {{edgelabel(fifos[id].dst,"headlabel")}}
 {{edgelabel(fifos[id].src,"taillabel")}}]
 {% else %}
-{{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="{{fifos[id].theType.graphViztype}}({{fifos[id].length}})"
+{{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos[id])}}",label=<{{style.edge_label(fifos[id],fifos[id].theType.graphViztype,fifos[id].length)}}>
 {{edgelabel(fifos[id].dst,"headlabel")}}
 {{edgelabel(fifos[id].src,"taillabel")}}]
 {% endif %}
 {% endif %}
 {% endfor %}
 
 {% for c in constObjs %}
 {{c.name}} [label=<
-<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+<TABLE color="{{style.const_boundary_color(c.name)}}" bgcolor="{{style.const_color(c.name)}}" BORDER="0" CELLBORDER="{{style.const_border(c.name)}}" CELLSPACING="0" CELLPADDING="4">
   <TR>
-    <TD ALIGN="CENTER" PORT="i">{{c.name}}</TD>
+    <TD ALIGN="CENTER" PORT="i"><FONT COLOR="{{style.const_label_color(c.name)}}" POINT-SIZE="{{style.const_label_size(c.name)}}">{{c.name}}</FONT></TD>
   </TR>
 </TABLE>>];
 {% endfor %}
 
 {% for edgeID in range(nbConstEdges) %}
-{{constEdges[edgeID][0].name}}:i -> {{constdst(edgeID)}}
+{{constEdges[edgeID][0].name}}:i -> {{constdst(edgeID)}} [style="{{style.const_edge_style(constEdges[edgeID][0].name,constEdges[edgeID][1])}}",color="{{style.const_edge_color(constEdges[edgeID][0].name,constEdges[edgeID][1])}}"]
 {% endfor %}
 }
```

### html2text {}

```diff
@@ -5,40 +5,60 @@
 {{ioport.nbSamples}}
 >{% endif %} {%- endmacro %} {% macro constdst(theID) -%} {{constEdges[theID]
 [1].owner.nodeID}}:{{constEdges[theID][1].name}} {% endmacro -%} {% macro
 delayBoxID(id) -%}{{fifos[id].src.owner.nodeID}}{{fifos
 [id].dst.owner.nodeID}}Delay{%- endmacro %} {% macro delayBox(edge) -%} {% if
 fifos[edge].hasDelay %} {{delayBoxID(edge)}} [label=<
 {{fifos[edge].delay}}
->]; {% endif %} {%- endmacro %} digraph structs { node [shape=plaintext] {% if
-config.horizontal %} rankdir=LR {% endif %} edge [arrowsize=0.5]
-fontname="times" {% for item in nodes %} {% if item.isDuplicateNode %} {
-{item.nodeID}} [shape=point,label={{item.nodeName}}] {% else %} {% if not
+>]; {% endif %} {%- endmacro %} digraph structs { bgcolor = "{{style
+['graph_background']}}" node [shape=plaintext,color="{{style
+['node_boundary_color']}}",fontcolor="{{style['node_label_color']}}",fontname="
+{{style['graph_font']}}"] {% if config.horizontal %} rankdir=LR {% endif %}
+edge [arrowsize="{{style['arrow_size']}}",color="{{style
+['edge_color']}}",fontcolor="{{style['edge_label_color']}}",fontname="{{style
+['graph_font']}}"] {% for item in nodes %} {% if item.isDuplicateNode %} {
+{item.nodeID}} [shape=point,label="{{item.nodeName}}"] {% else %} {% if not
 item.hasManyIOs %} {{item.nodeID}} [label=<
-{{item.graphvizName}}
+{{ style.node_label(item) }}
 >]; {% else %} {% if not config.horizontal %} {{item.nodeID}} [label=<
 {{input}}
-{{ item.graphvizName }}
+{{ style.node_label(item) }}
 {{output}}
 >]; {% else %} {{item.nodeID}} [label=<
-{{item.inputNames[0]}}  {{ item.graphvizName }} {{item.outputNames[0]}}
+{{item.inputNames[0]}}  {{ style.node_label(item) }} {{item.outputNames[0]}}
 {{input}}               {{output}}
 >]; {% endif %} {% endif %} {% endif %} {% endfor %} {% for id in range
 (nbFifos) %} {{delayBox(id)}} {% if fifos[id].hasDelay %} {{io(fifos
-[id].src.owner,fifos[id].src)}} -> {{delayBoxID(id)}}:i [label=""{{edgelabel
+[id].src.owner,fifos[id].src)}} -> {{delayBoxID(id)}}:i [style="{
+{style.delay_edge_style(fifos[id].src,fifos[id].delay)}}",color="{
+{style.delay_edge_color(fifos[id].src,fifos[id].delay)}}",label=""{{edgelabel
 (fifos[id].src,"taillabel")}}] {% if config.displayFIFOBuf %} {{delayBoxID
-(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="buf{{fifos
-[id].bufferID}}" {{edgelabel(fifos[id].src,"headlabel")}}] {% else %} {
-{delayBoxID(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [label="{
-{fifos[id].theType.graphViztype}}({{fifos[id].length}})" {{edgelabel(fifos
+(id)}}:i -> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{
+{style.edge_style(fifos[id])}}",color="{{style.edge_color(fifos
+[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{
+{style.edge_label_color(fifos[id])}}",label="buf{{fifos[id].bufferID}}" {
+{edgelabel(fifos[id].src,"headlabel")}}] {% else %} {{delayBoxID(id)}}:i -> {
+{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos
+[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{
+{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos
+[id])}}",label=<{{style.edge_label(fifos[id],fifos
+[id].theType.graphViztype,fifos[id].length)}}> {{edgelabel(fifos
 [id].dst,"headlabel")}}] {% endif %} {% else %} {% if config.displayFIFOBuf %}
 {{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos
-[id].dst)}} [label="buf{{fifos[id].bufferID}}" {{edgelabel(fifos
-[id].dst,"headlabel")}} {{edgelabel(fifos[id].src,"taillabel")}}] {% else %} {
-{io(fifos[id].src.owner,fifos[id].src)}} -> {{io(fifos[id].dst.owner,fifos
-[id].dst)}} [label="{{fifos[id].theType.graphViztype}}({{fifos[id].length}})" {
+[id].dst)}} [style="{{style.edge_style(fifos[id])}}",color="{{style.edge_color
+(fifos[id])}}",fontsize="{{style.edge_label_size(fifos[id])}}",fontcolor="{
+{style.edge_label_color(fifos[id])}}",label="buf{{fifos[id].bufferID}}" {
 {edgelabel(fifos[id].dst,"headlabel")}} {{edgelabel(fifos
-[id].src,"taillabel")}}] {% endif %} {% endif %} {% endfor %} {% for c in
-constObjs %} {{c.name}} [label=<
+[id].src,"taillabel")}}] {% else %} {{io(fifos[id].src.owner,fifos[id].src)}} -
+> {{io(fifos[id].dst.owner,fifos[id].dst)}} [style="{{style.edge_style(fifos
+[id])}}",color="{{style.edge_color(fifos[id])}}",fontsize="{
+{style.edge_label_size(fifos[id])}}",fontcolor="{{style.edge_label_color(fifos
+[id])}}",label=<{{style.edge_label(fifos[id],fifos
+[id].theType.graphViztype,fifos[id].length)}}> {{edgelabel(fifos
+[id].dst,"headlabel")}} {{edgelabel(fifos[id].src,"taillabel")}}] {% endif %}
+{% endif %} {% endfor %} {% for c in constObjs %} {{c.name}} [label=<
 {{c.name}}
 >]; {% endfor %} {% for edgeID in range(nbConstEdges) %} {{constEdges[edgeID]
-[0].name}}:i -> {{constdst(edgeID)}} {% endfor %} }
+[0].name}}:i -> {{constdst(edgeID)}} [style="{{style.const_edge_style
+(constEdges[edgeID][0].name,constEdges[edgeID][1])}}",color="{
+{style.const_edge_color(constEdges[edgeID][0].name,constEdges[edgeID][1])}}"]
+{% endfor %} }
```

## Comparing `cmsis_stream-1.3.0.dist-info/LICENSE.txt` & `cmsis_stream-1.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.3.0.dist-info/METADATA` & `cmsis_stream-1.4.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.3.0
+Version: 1.4.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -41,14 +41,21 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate a C scheduler to run the graph on your target
 
 # Change history
 
+## Version 1.4.0:
+
+* Possibility to customize the style of the graph pictures (colors, fonts ...)
+* Graph picture can now also be generated before schedule computation (useful to debug an incorrect graph before trying to compute a schedule)
+* Possibility to use more **pure** C functions in the graph. The `GenericFunction` node can now easily be used to plug more kind of C functions without having to write a C++ wrapper
+* `Dsp` node has been removed. Instead use the `Unary`, `Binary` or the more flexible `GenericFunction` node
+
 ## Version 1.3.0:
 
 * New nodes `GenericToMany`, `GenericFromMany`, `GenericManyToMany`
 * `Duplicate` node implementation now using `GenericToMany`
 * Possibility to change the name of IOs in `Binary`, `Unary` and `Dsp` nodes
 
 ## Version 1.2.1:
```

## Comparing `cmsis_stream-1.3.0.dist-info/RECORD` & `cmsis_stream-1.4.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=f57rHk2gtgkikywW_ZEkdXlibV4wnHbOQ5vi0fHRcME,3018
 cmsis_stream/cg/scheduler/config.py,sha256=J3W01wi-DO32EVKsgQ5ztUeNMBl0fDk2cXuOzySMM30,6665
-cmsis_stream/cg/scheduler/description.py,sha256=BJ0293P4bQL5iU1RxBJF_3mSJhGDIOjurS6eUTiBWCc,41606
-cmsis_stream/cg/scheduler/graphviz.py,sha256=wmbSzhIlOD9Z1E5NBsNklk4LvpaLQfs9Tmw-vAxwSPM,1784
-cmsis_stream/cg/scheduler/node.py,sha256=kMeAhr109SCg77tbP6iTZGBvuKz7y4Md9AQa2OOkKP0,36807
+cmsis_stream/cg/scheduler/description.py,sha256=FPLRFTxk3mGduq2_hLPxNiL5MNzpFDzl-Nk1ivyyBVk,41853
+cmsis_stream/cg/scheduler/graphviz.py,sha256=TwiDslHOJlek2otwA_5sspTWaf_trLV4QMthpv6fzM4,10849
+cmsis_stream/cg/scheduler/node.py,sha256=RqSxM0EHSUUkrBu9wEMByEGbGgW2QA_jMXm5kAT4d9A,37754
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=bDtCVYvgtLO_wpl33HlyyAEZtfyW6wHyANQsdPvdlBA,1796
 cmsis_stream/cg/scheduler/standard.py,sha256=VngMlAxV9n8HNPX50KDD_OLQvaTI4Q7iz_mxjRgHEWU,7523
 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
 cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
 cmsis_stream/cg/scheduler/example/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
 cmsis_stream/cg/scheduler/example/README.md,sha256=_o0nMzYUELDms9o9Gh__4fuOTYqUAwabijVBSHkqsiA,566
@@ -44,24 +44,24 @@
 cmsis_stream/cg/scheduler/example/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
 cmsis_stream/cg/scheduler/example/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
 cmsis_stream/cg/scheduler/example/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
 cmsis_stream/cg/scheduler/example/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
 cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
 cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=Xs7uGOL8YYvTaWc_L-07t029hiQiN5NqtV7g9V3s-gE,16526
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
-cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=yNiZSHN-riYPkzCenN6UUoZD9ZieCI8L9viXYkQCCz0,431
-cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=wbXrZ1fWz2YmD-yyvMshlaXvWXgTmfKokVEFu6SwAVk,279
-cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=bo05ISPFatzhi09c36ioA4HSJUtJc30k3T-z31oWN-8,674
-cmsis_stream/cg/scheduler/templates/cmsisNode.cpp,sha256=luXUXScO1ncXx1m2kI2e40DyjobwbwVucCY0QernoGc,297
+cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=Fw5MHQqCZt2srXAuJjvXSHS1m-78DGdT4sGHDEQgG28,434
+cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=iC5sSkuZ01iGT0dBfqNPUbMKE86y10-0Gj8fLOfbgi8,287
+cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=JMn_nIJiPYSnu7qVKHS8jKEtAjktGpWSyzxg-r2olgw,682
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
 cmsis_stream/cg/scheduler/templates/code.h,sha256=BULWyJn9FAU6laXpg6UjyP5TtHHMCW_3zTccu_EtjKU,1111
 cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
-cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=6fn_IVXZy77h8TQN2vSsuwMUVJFjyPtVzURjhnriAo0,3185
+cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=aL_bl4hTZ5dtNGKOoLxgqURt6rH6AJt3Sw-61qmFSJs,3305
 cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=nmlbxVoBiujXLYerA056T_GPRL-LZSo0IFcz6BHdTHc,4482
-cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=h9R25-RcgG_kDKg4-xsGih4yPnffdNbZwkZMe5UXmhA,1051
-cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=GJyuIQkdt3RZvq2SRSBYrmuWj7QW9T4wVO-1GRGB8B0,4848
-cmsis_stream-1.3.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.3.0.dist-info/METADATA,sha256=AoZOWEdgDMib_FLS4vv9CiikCpE60u-It-8Wt6RpJ_0,3506
-cmsis_stream-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.3.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.3.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.3.0.dist-info/RECORD,,
+cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=KoW0i45XF2-Ghcs-snyqlyysT0SfcKVJcStrBotO1gE,1427
+cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=_4a8oe0kvSDx-Hl1P0aIZMFAOYMpknhGkeOUI8Nqy6g,7826
+cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot,sha256=wLfhZpZS0VHm43dpaQYZBSd8ftd0KdUS_hSo2cSHwLU,7555
+cmsis_stream-1.4.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.4.0.dist-info/METADATA,sha256=UakFDEe3RXFSR9baQZ5IMDZ-3I0HbSmJhFQao94fBKM,4046
+cmsis_stream-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.4.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.4.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.4.0.dist-info/RECORD,,
```

