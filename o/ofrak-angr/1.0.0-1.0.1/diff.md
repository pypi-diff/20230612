# Comparing `tmp/ofrak_angr-1.0.0.tar.gz` & `tmp/ofrak_angr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofrak_angr-1.0.0.tar", last modified: Thu Jan 26 06:29:10 2023, max compression
+gzip compressed data, was "ofrak_angr-1.0.1.tar", last modified: Mon Jun 12 18:29:55 2023, max compression
```

## Comparing `ofrak_angr-1.0.0.tar` & `ofrak_angr-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-26 06:29:10.723410 ofrak_angr-1.0.0/
--rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/LICENSE
--rw-r--r--   0 edward     (501) staff       (20)     5104 2023-01-26 06:29:10.722796 ofrak_angr-1.0.0/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     4190 2023-01-26 06:28:46.000000 ofrak_angr-1.0.0/README.md
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-26 06:29:10.712988 ofrak_angr-1.0.0/ofrak_angr/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/ofrak_angr/__init__.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-26 06:29:10.720722 ofrak_angr-1.0.0/ofrak_angr/components/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/ofrak_angr/components/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)     4169 2023-01-18 23:40:02.000000 ofrak_angr-1.0.0/ofrak_angr/components/angr_analyzer.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-26 06:29:10.722216 ofrak_angr-1.0.0/ofrak_angr/components/blocks/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/ofrak_angr/components/blocks/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)     9836 2023-01-26 06:28:46.000000 ofrak_angr-1.0.0/ofrak_angr/components/blocks/unpackers.py
--rw-r--r--   0 edward     (501) staff       (20)      390 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/ofrak_angr/components/identifiers.py
--rw-r--r--   0 edward     (501) staff       (20)      336 2022-11-09 21:07:02.000000 ofrak_angr-1.0.0/ofrak_angr/model.py
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.0/ofrak_angr/py.typed
--rw-r--r--   0 edward     (501) staff       (20)      659 2022-10-20 20:17:11.000000 ofrak_angr-1.0.0/ofrak_angr/serializer.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-26 06:29:10.718658 ofrak_angr-1.0.0/ofrak_angr.egg-info/
--rw-r--r--   0 edward     (501) staff       (20)     5104 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)      513 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/SOURCES.txt
--rw-r--r--   0 edward     (501) staff       (20)        1 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/dependency_links.txt
--rw-r--r--   0 edward     (501) staff       (20)       45 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/entry_points.txt
--rw-r--r--   0 edward     (501) staff       (20)      120 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/requires.txt
--rw-r--r--   0 edward     (501) staff       (20)       11 2023-01-26 06:29:10.000000 ofrak_angr-1.0.0/ofrak_angr.egg-info/top_level.txt
--rw-r--r--   0 edward     (501) staff       (20)       38 2023-01-26 06:29:10.723557 ofrak_angr-1.0.0/setup.cfg
--rw-r--r--   0 edward     (501) staff       (20)     2138 2023-01-26 06:28:46.000000 ofrak_angr-1.0.0/setup.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:55.754578 ofrak_angr-1.0.1/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)       26 2023-04-27 21:00:41.000000 ofrak_angr-1.0.1/MANIFEST.in
+-rw-r--r--   0 edward     (501) staff       (20)     5104 2023-06-12 18:29:55.754157 ofrak_angr-1.0.1/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     4190 2023-02-02 23:02:31.000000 ofrak_angr-1.0.1/README.md
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:55.745472 ofrak_angr-1.0.1/ofrak_angr/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr/__init__.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:55.752174 ofrak_angr-1.0.1/ofrak_angr/components/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr/components/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)     4169 2023-02-02 23:02:31.000000 ofrak_angr-1.0.1/ofrak_angr/components/angr_analyzer.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:55.753235 ofrak_angr-1.0.1/ofrak_angr/components/blocks/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr/components/blocks/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)    12349 2023-06-12 14:38:38.000000 ofrak_angr-1.0.1/ofrak_angr/components/blocks/unpackers.py
+-rw-r--r--   0 edward     (501) staff       (20)      390 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr/components/identifiers.py
+-rw-r--r--   0 edward     (501) staff       (20)      336 2022-11-09 21:07:02.000000 ofrak_angr-1.0.1/ofrak_angr/model.py
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr/py.typed
+-rw-r--r--   0 edward     (501) staff       (20)      659 2022-10-20 20:17:11.000000 ofrak_angr-1.0.1/ofrak_angr/serializer.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:55.750445 ofrak_angr-1.0.1/ofrak_angr.egg-info/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:34.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)     5104 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)      570 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/SOURCES.txt
+-rw-r--r--   0 edward     (501) staff       (20)        1 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/dependency_links.txt
+-rw-r--r--   0 edward     (501) staff       (20)       45 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/entry_points.txt
+-rw-r--r--   0 edward     (501) staff       (20)      120 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/requires.txt
+-rw-r--r--   0 edward     (501) staff       (20)       11 2023-06-12 18:29:55.000000 ofrak_angr-1.0.1/ofrak_angr.egg-info/top_level.txt
+-rw-r--r--   0 edward     (501) staff       (20)       12 2023-02-16 21:44:17.000000 ofrak_angr-1.0.1/requirements.txt
+-rw-r--r--   0 edward     (501) staff       (20)       38 2023-06-12 18:29:55.754698 ofrak_angr-1.0.1/setup.cfg
+-rw-r--r--   0 edward     (501) staff       (20)     2465 2023-06-12 14:38:38.000000 ofrak_angr-1.0.1/setup.py
```

### Comparing `ofrak_angr-1.0.0/LICENSE` & `ofrak_angr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofrak_angr-1.0.0/PKG-INFO` & `ofrak_angr-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak_angr
-Version: 1.0.0
+Version: 1.0.1
 Summary: OFRAK angr Components
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_angr-1.0.0/README.md` & `ofrak_angr-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ofrak_angr-1.0.0/ofrak_angr/components/angr_analyzer.py` & `ofrak_angr-1.0.1/ofrak_angr/components/angr_analyzer.py`

 * *Files identical despite different names*

### Comparing `ofrak_angr-1.0.0/ofrak_angr/components/blocks/unpackers.py` & `ofrak_angr-1.0.1/ofrak_angr/components/blocks/unpackers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
-from typing import Iterable, Tuple
+from typing import Iterable, Tuple, List
 from typing import Optional
 from warnings import warn
 
 from angr.knowledge_plugins.functions.function import Function as AngrFunction
-from archinfo.arch_arm import get_real_address_if_arm
+from archinfo.arch_arm import get_real_address_if_arm, is_arm_arch
+
+from ofrak.component.unpacker import UnpackerError
 from ofrak_type.architecture import InstructionSetMode
 from ofrak_type.range import Range
 
 from ofrak.core.basic_block import BasicBlock
 from ofrak.core.code_region import CodeRegionUnpacker, CodeRegion
 from ofrak.core.complex_block import ComplexBlock, ComplexBlockUnpacker
 from ofrak.core.data import DataWord
@@ -19,29 +21,29 @@
 from ofrak_angr.model import AngrAnalysis
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AngrCodeRegionUnpacker(CodeRegionUnpacker):
     async def unpack(self, resource: Resource, config: Optional[AngrAnalyzerConfig] = None):
-        ## Prepare CR unpacker
+        # Prepare CR unpacker
         cr_view = await resource.view_as(CodeRegion)
 
-        ## Run AngrAnalyzer
+        # Run AngrAnalyzer
         root_resource = await resource.get_only_ancestor(
             ResourceFilter(tags=[AngrAnalysisResource], include_self=True)
         )
         angr_analysis = await root_resource.analyze(AngrAnalysis)
 
-        ## Fixup the CodeRegion's virtual address after analyzing with angr.
+        # Fixup the CodeRegion's virtual address after analyzing with angr.
         await resource.run(AngrCodeRegionModifier, None)
 
         cr_vaddr_range = cr_view.vaddr_range()
 
-        ## Fetch and create complex blocks to populate the CR with
+        # Fetch and create complex blocks to populate the CR with
         num_overlapping_cbs = 0
 
         for complex_block in self._angr_get_complex_blocks(angr_analysis, cr_vaddr_range):
             await cr_view.create_child_region(complex_block)
 
         if num_overlapping_cbs > 0:
             LOGGER.warning(
@@ -58,60 +60,65 @@
         :param angr_analysis: angr project state for the binary-under-analysis
         :param region_vaddr: Virtual address range of the code region to unpack complex blocks
 
         :return: Yield the next Complex Block (sorted by entrypoint address)
         """
         LOGGER.debug(f"Getting complex blocks from region {region_vaddr.start:#x}")
 
-        ## Filter for functions within the requested region
+        # Filter for functions within the requested region
         angr_funcs: Iterable[Tuple[int, AngrFunction]] = angr_analysis.project.kb.functions.items()
         funcs = [f[1] for f in angr_funcs if f[0] in region_vaddr]
 
-        ## Filter out non-returning functions, unless it's an entrypoint
+        # Filter out non-returning functions, unless it's an entrypoint
         # TODO: Re-visit this; this will likely filter HW interrupt funcs
         funcs = [f for f in funcs if (f.has_return) or (f.addr == angr_analysis.project.entry)]
 
-        ## Yield the next function via a generator
+        # Yield the next function via a generator
         for idx, func in enumerate(funcs):
             start_addr = func.addr
 
-            ## Adjust the upper bound of the CB to include DWORDS
-            ## The boundary of a CB extends up to min(region_end_vaddr, next_func_addr)
+            # Adjust the upper bound of the CB to include DWORDS
+            # The boundary of a CB extends up to min(region_end_vaddr, next_func_addr)
             next_idx = idx + 1
             if next_idx < len(funcs):
                 end_addr = min(region_vaddr.end, funcs[next_idx].addr)
             else:
                 end_addr = region_vaddr.end
 
-            ## OFRAK expects real addresses, so we need to convert the thumb-masked addresses angr returns
+            # OFRAK expects real addresses, so we need to convert the thumb-masked addresses angr returns
             start_addr = get_real_address_if_arm(angr_analysis.project.arch, start_addr)
             end_addr = get_real_address_if_arm(angr_analysis.project.arch, end_addr)
 
             yield ComplexBlock(start_addr, end_addr - start_addr, func.name)
 
 
 class AngrComplexBlockUnpacker(ComplexBlockUnpacker):
     async def unpack(self, resource: Resource, config: Optional[AngrAnalyzerConfig] = None):
-        ## Prepare CB unpacker
+        # Prepare CB unpacker
         cb_view = await resource.view_as(ComplexBlock)
         cb_vaddr_range = cb_view.vaddr_range()
         cb_data_range = await resource.get_data_range_within_root()
 
-        ## Run / fetch angr analyzer
+        # Run / fetch angr analyzer
         root_resource = await resource.get_only_ancestor(
             ResourceFilter(tags=[AngrAnalysisResource], include_self=True)
         )
         angr_analysis = await root_resource.analyze(AngrAnalysis)
 
-        ## Fetch and create Basic Blocks to populate the CB with
+        valid_data_xref_ranges = []
+        # Fetch and create Basic Blocks to populate the CB with
         for basic_block in self._angr_get_basic_blocks(angr_analysis, cb_vaddr_range):
             await cb_view.create_child_region(basic_block)
+            valid_data_xref_ranges.append(basic_block.vaddr_range())
 
-        ## Fetch and create Data Words to populate the CB with
-        for data_word in self._angr_get_dword_blocks(angr_analysis, cb_vaddr_range, cb_data_range):
+        valid_data_xref_ranges = Range.merge_ranges(valid_data_xref_ranges)
+        # Fetch and create Data Words to populate the CB with
+        for data_word in self._angr_get_dword_blocks(
+            angr_analysis, cb_vaddr_range, cb_data_range, valid_data_xref_ranges
+        ):
             await cb_view.create_child_region(data_word)
 
     @staticmethod
     def _angr_get_basic_blocks(
         angr_analysis: AngrAnalysis, cb_vaddr_range: Range
     ) -> Iterable[BasicBlock]:
         """
@@ -121,39 +128,40 @@
         :param cb_vaddr_range: Total virtual address range of the CB
 
         :return: Yield the next Basic Block (sorted by entrypoint address)
         """
         LOGGER.debug(f"Getting basic blocks from function {cb_vaddr_range.start:#x}")
 
         angr_complex_block = angr_analysis.project.kb.functions.function(addr=cb_vaddr_range.start)
+        if not angr_complex_block and is_arm_arch(angr_analysis.project.arch):
+            thumb_cb_vaddr = cb_vaddr_range.start | 0x1
+            angr_complex_block = angr_analysis.project.kb.functions.function(addr=thumb_cb_vaddr)
+
         if not angr_complex_block:
             LOGGER.error(f"Could not find complex block at {cb_vaddr_range.start:#x} in angr")
             return
 
         angr_cb_basic_blocks = sorted(list(angr_complex_block.blocks), key=lambda bb: bb.addr)
         for idx, bb in enumerate(angr_cb_basic_blocks):
             bb_addr = get_real_address_if_arm(angr_analysis.project.arch, bb.addr)
 
-            bb_mode = (
-                InstructionSetMode.THUMB if "thumb" in bb.arch.name else InstructionSetMode.NONE
-            )
-
-            ## Fetch the exit point addr (if it exists) and sanity check the selection
-            bb_is_exit_point = bb.codenode in angr_complex_block.endpoints
-            if bb_is_exit_point:
-                bb_exit_addr = None
-            else:
-                if idx == len(angr_cb_basic_blocks) - 1:
-                    LOGGER.error(
-                        f"Exit point defined for BB even though it is the last BB on the addr list"
-                    )
-                    return
-                bb_exit_addr = get_real_address_if_arm(
-                    angr_analysis.project.arch, angr_cb_basic_blocks[(idx + 1)].addr
+            bb_mode = InstructionSetMode.NONE
+            if is_arm_arch(bb.arch) and (bb.addr & 0x1):
+                bb_mode = InstructionSetMode.THUMB
+
+            try:
+                bb_is_exit_point, bb_exit_addr = _get_bb_exit_addr_info(
+                    angr_analysis,
+                    angr_complex_block,
+                    angr_cb_basic_blocks,
+                    bb,
+                    idx,
                 )
+            except UnpackerError:
+                return
 
             if (bb_addr + bb.size) > cb_vaddr_range.end or bb_addr < cb_vaddr_range.start:
                 warning_string = (
                     f"Basic block {bb_addr:#x} does not fall within "
                     f"complex block {cb_vaddr_range.start:#x} at "
                     f"addresses {cb_vaddr_range.start:#x}-{cb_vaddr_range.end:#x}"
                 )
@@ -169,14 +177,15 @@
             )
 
     @staticmethod
     def _angr_get_dword_blocks(
         angr_analysis: AngrAnalysis,
         cb_data_range: Range,
         cb_vaddr_range: Range,
+        valid_data_xref_ranges: List[Range],
     ) -> Iterable[DataWord]:
         """
         Iterator which yields Dword Blocks derived from the angr CFG within an address range
 
         :param angr_analysis: angr project state for the binary-under-analysis
         :param cb_data_range: Data range of the CB
         :param cb_vaddr_range: Total virtual address range of the CB
@@ -200,29 +209,82 @@
                 "This should have been populated by AngrAnalyzer, or "
                 "there may be an error in the provided post-analysis hook."
             )
             return
 
         # Filter xrefs within the requested address range & if known dword type
         cb_data_xrefs = [
-            d
-            for d in angr_cfg.insn_addr_to_memory_data.items()
-            if (d[1].addr in cb_data_range) and (d[1].sort in dword_types)
+            (xref, cb_data_xref)
+            for xref, cb_data_xref in angr_cfg.insn_addr_to_memory_data.items()
+            if (cb_data_xref.addr in cb_data_range) and (cb_data_xref.sort in dword_types)
         ]
 
         for xref, cb_data_xref in cb_data_xrefs:
             word_size = cb_data_xref.size
             cb_data_xref_addr = cb_data_xref.addr
 
             if word_size not in dword_size_map:
                 raise ValueError(f"Bad word size {word_size} at {cb_data_xref_addr:#x}")
 
+            if xref is None or not any(xref in bb_range for bb_range in valid_data_xref_ranges):
+                continue
+
             LOGGER.debug(f"Creating DataWord for {cb_data_xref.content} @ {cb_data_xref_addr:#x}")
 
             format_string = endian_flag + dword_size_map[word_size]
 
             cb_data_xref_addr = get_real_address_if_arm(
                 angr_analysis.project.arch, cb_data_xref_addr
             )
             xref = get_real_address_if_arm(angr_analysis.project.arch, xref) if xref else None
 
             yield DataWord(cb_data_xref_addr, word_size, format_string, (xref,))
+
+
+def _get_bb_exit_addr_info(
+    angr_analysis,
+    angr_complex_block,
+    angr_cb_basic_blocks,
+    current_angr_bb,
+    current_bb_idx,
+) -> Tuple[bool, Optional[int]]:
+    """
+    Get exit address info needed for BasicBlock creation:
+    BasicBlock.is_exit_point, BasicBlock.exit_addr.
+    """
+    # Fetch the exit point addr (if it exists) and sanity check the selection
+    if current_angr_bb.codenode in angr_complex_block.endpoints:
+        return True, None
+
+    if current_bb_idx == len(angr_cb_basic_blocks) - 1:
+        LOGGER.error(
+            f"Exit point defined for BB 0x{current_angr_bb.addr:x} even though it is the last BB on the addr list"
+        )
+        raise UnpackerError()
+
+    # If no conditional branches taken, execution "falls through" to next basic block
+    fallthrough_vaddr = get_real_address_if_arm(
+        angr_analysis.project.arch, angr_cb_basic_blocks[current_bb_idx + 1].addr
+    )
+    try:
+        successor_vaddrs = [
+            get_real_address_if_arm(angr_analysis.project.arch, succ_codenode.addr)
+            for succ_codenode, edge_info in angr_complex_block.graph.succ[
+                current_angr_bb.codenode
+            ].items()
+        ]
+    except KeyError:
+        LOGGER.warning(
+            f"Cannot find any successors in angr for BB 0x{current_angr_bb.addr:x}, but since it "
+            f"has a BB after it, assume that it still falls through to the next BB."
+        )
+        return True, fallthrough_vaddr
+
+    if fallthrough_vaddr in successor_vaddrs:
+        # Basic block can fall through to next block, so the next block should be the exit addr
+        return False, fallthrough_vaddr
+    else:
+        # Basic block can't fall through to next block, choose first succ as exit addr
+        # For example: basic block ends in unconditional one-way branch (not a call)
+        # If there are somehow multiple successors and the fallthrough block is not one of them,
+        # choosing the first succ as the exit addr is arbitrary, but better choice is unclear.
+        return False, successor_vaddrs[0]
```

### Comparing `ofrak_angr-1.0.0/ofrak_angr/serializer.py` & `ofrak_angr-1.0.1/ofrak_angr/serializer.py`

 * *Files identical despite different names*

### Comparing `ofrak_angr-1.0.0/ofrak_angr.egg-info/PKG-INFO` & `ofrak_angr-1.0.1/ofrak_angr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak-angr
-Version: 1.0.0
+Version: 1.0.1
 Summary: OFRAK angr Components
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_angr-1.0.0/ofrak_angr.egg-info/SOURCES.txt` & `ofrak_angr-1.0.1/ofrak_angr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 ofrak_angr/__init__.py
 ofrak_angr/model.py
 ofrak_angr/py.typed
 ofrak_angr/serializer.py
+ofrak_angr.egg-info/LICENSE
 ofrak_angr.egg-info/PKG-INFO
 ofrak_angr.egg-info/SOURCES.txt
 ofrak_angr.egg-info/dependency_links.txt
 ofrak_angr.egg-info/entry_points.txt
 ofrak_angr.egg-info/requires.txt
 ofrak_angr.egg-info/top_level.txt
 ofrak_angr/components/__init__.py
```

### Comparing `ofrak_angr-1.0.0/setup.py` & `ofrak_angr-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import setuptools
+import pkg_resources
 from setuptools.command.egg_info import egg_info
 
 
 class egg_info_ex(egg_info):
     """Includes license file into `.egg-info` folder."""
 
     def run(self):
@@ -14,24 +15,34 @@
 
         egg_info.run(self)
 
 
 with open("README.md") as f:
     long_description = f.read()
 
+
+# Should be the same as in build_image.py
+def read_requirements(requirements_path):
+    with open(requirements_path) as requirements_handle:
+        return [
+            str(requirement)
+            for requirement in pkg_resources.parse_requirements(requirements_handle)
+        ]
+
+
 setuptools.setup(
     name="ofrak_angr",
-    version="1.0.0",
+    version="1.0.1",
     description="OFRAK angr Components",
     packages=setuptools.find_packages(exclude=["ofrak_angr_test", "ofrak_angr_test.*"]),
     package_data={"ofrak_angr": ["py.typed"]},
     install_requires=[
-        "angr==9.2.6",
         "ofrak",
-    ],
+    ]
+    + read_requirements("requirements.txt"),
     extras_require={
         "test": [
             "fun-coverage==0.2.0",
             "pytest",
             "pytest-asyncio==0.19.0",
             "pytest-cov",
             "requests",
```

