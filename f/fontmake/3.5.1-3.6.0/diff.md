# Comparing `tmp/fontmake-3.5.1.zip` & `tmp/fontmake-3.6.0.zip`

## zipinfo {}

```diff
@@ -1,724 +1,727 @@
-Zip file size: 463050 bytes, number of entries: 722
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/Lib/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/.github/
--rw-r--r--  2.0 unx      485 b- defN 22-Dec-08 19:32 fontmake-3.5.1/requirements.txt
--rw-r--r--  2.0 unx      191 b- defN 22-Dec-08 19:32 fontmake-3.5.1/test_requirements.txt
--rw-r--r--  2.0 unx     2924 b- defN 22-Dec-08 19:32 fontmake-3.5.1/setup.py
--rw-r--r--  2.0 unx      792 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.coveragerc
--rw-r--r--  2.0 unx      226 b- defN 22-Dec-08 19:32 fontmake-3.5.1/setup.cfg
--rw-r--r--  2.0 unx      322 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.gitattributes
--rwxr-xr-x  2.0 unx     1673 b- defN 22-Dec-08 19:32 fontmake-3.5.1/build_pyz.sh
--rw-r--r--  2.0 unx     7231 b- defN 22-Dec-08 19:32 fontmake-3.5.1/PKG-INFO
--rw-r--r--  2.0 unx      802 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tox.ini
--rw-r--r--  2.0 unx     1450 b- defN 22-Dec-08 19:32 fontmake-3.5.1/CONTRIBUTING.md
--rw-r--r--  2.0 unx    19601 b- defN 22-Dec-08 19:32 fontmake-3.5.1/USAGE.md
--rw-r--r--  2.0 unx       77 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.codecov.yml
--rw-r--r--  2.0 unx      227 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.editorconfig
--rw-r--r--  2.0 unx     3193 b- defN 22-Dec-08 19:32 fontmake-3.5.1/TROUBLESHOOTING.md
--rw-r--r--  2.0 unx      168 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.pyup.yml
--rw-r--r--  2.0 unx    11357 b- defN 22-Dec-08 19:32 fontmake-3.5.1/LICENSE
--rw-r--r--  2.0 unx     6215 b- defN 22-Dec-08 19:32 fontmake-3.5.1/README.md
--rw-r--r--  2.0 unx      163 b- defN 22-Dec-08 19:32 fontmake-3.5.1/pyproject.toml
--rw-r--r--  2.0 unx     1453 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.gitignore
--rw-r--r--  2.0 unx      142 b- defN 22-Dec-08 19:32 fontmake-3.5.1/MANIFEST.in
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/
--rw-r--r--  2.0 unx      108 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/__init__.py
--rw-r--r--  2.0 unx    25138 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/__main__.py
--rw-r--r--  2.0 unx     3049 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/compatibility.py
--rw-r--r--  2.0 unx     3288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/ttfautohint.py
--rw-r--r--  2.0 unx    57364 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/font_project.py
--rw-r--r--  2.0 unx    31075 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/instantiator.py
--rw-r--r--  2.0 unx      176 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/_version.py
--rw-r--r--  2.0 unx     1439 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake/errors.py
--rw-r--r--  2.0 unx        1 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       52 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/top_level.txt
--rw-r--r--  2.0 unx     7231 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      402 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/requires.txt
--rw-r--r--  2.0 unx    42087 b- defN 22-Dec-08 19:32 fontmake-3.5.1/Lib/fontmake.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/
--rw-r--r--  2.0 unx    25200 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/test_instantiator.py
--rw-r--r--  2.0 unx    32827 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/test_main.py
--rw-r--r--  2.0 unx      133 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/conftest.py
--rw-r--r--  2.0 unx     1668 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/test_compatibility.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/AutohintingTest/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/
--rw-r--r--  2.0 unx     6386 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/TestSubset.glyphs
--rw-r--r--  2.0 unx     6381 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/TestSubset2.glyphs
--rw-r--r--  2.0 unx    30579 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx     1135 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
--rw-r--r--  2.0 unx      983 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      303 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      887 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      479 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
--rw-r--r--  2.0 unx      288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      343 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      303 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx      886 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      425 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
--rw-r--r--  2.0 unx      288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      345 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
--rw-r--r--  2.0 unx     2611 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
--rw-r--r--  2.0 unx     7111 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans.designspace
--rw-r--r--  2.0 unx     1394 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
--rw-r--r--  2.0 unx     8462 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_missing.designspace
--rw-r--r--  2.0 unx     1074 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/LICENSE
--rw-r--r--  2.0 unx     7834 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
--rw-r--r--  2.0 unx     1412 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
--rw-r--r--  2.0 unx    16617 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1386 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      615 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx      344 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
--rw-r--r--  2.0 unx     1938 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2307 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      422 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2646 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      923 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx      983 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx     1806 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      341 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx      268 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
--rw-r--r--  2.0 unx     3181 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
--rw-r--r--  2.0 unx      950 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
--rw-r--r--  2.0 unx      343 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
--rw-r--r--  2.0 unx    18792 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1888 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      491 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx      811 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx      517 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx     2825 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx      238 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx     1176 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx      247 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
--rw-r--r--  2.0 unx     3543 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3534 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx     1402 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1966 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      193 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      264 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      929 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      627 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx      538 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      929 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx     1120 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      377 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      739 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      853 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      701 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx     1728 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     2687 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      914 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      737 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx      369 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      628 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx      233 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx     2453 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      350 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      743 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx      235 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      626 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      975 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      546 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1462 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1136 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      352 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx     1105 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      325 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      798 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      870 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      230 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      690 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      739 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      349 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx     1372 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx      736 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      515 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx      942 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1146 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      358 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      797 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      741 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     1799 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      244 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     3998 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     3358 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      247 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx      422 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
--rw-r--r--  2.0 unx     2452 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
--rw-r--r--  2.0 unx      482 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3498 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      751 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
--rw-r--r--  2.0 unx     1471 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
--rw-r--r--  2.0 unx     2111 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx      853 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
--rw-r--r--  2.0 unx      330 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx     2706 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      828 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
--rw-r--r--  2.0 unx    12341 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1870 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      366 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       36 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx      301 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1418 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2369 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      205 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      264 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx     1037 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      495 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx      545 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      940 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      750 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      380 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      750 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      861 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      701 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx     1747 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     2687 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      919 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      742 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx      370 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      491 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx      245 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx     2376 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      350 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      750 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx      259 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      492 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      988 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      549 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1495 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1150 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      354 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx     1154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      325 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      803 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      875 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      242 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      493 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      742 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      351 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx     1387 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx      745 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      522 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx      947 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1140 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      360 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      806 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      748 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2203 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1986 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2005 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
--rw-r--r--  2.0 unx    18291 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1873 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      366 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       37 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx     4852 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
--rw-r--r--  2.0 unx      236 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      341 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      237 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx     1416 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1970 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      193 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      264 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      943 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      518 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx      542 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx     1056 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      747 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      378 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      752 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      857 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      703 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx     1751 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     2687 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      924 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      740 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx      370 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      514 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx      233 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx     2358 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      352 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      954 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx      235 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      517 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx     1357 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      549 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1459 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1134 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      354 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx     1158 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      325 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      801 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      875 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      230 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      518 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      743 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      349 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx     1388 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx      749 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      521 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     1320 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1130 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      360 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      802 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      750 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     1785 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1965 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      344 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
--rw-r--r--  2.0 unx    16223 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1384 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx     5462 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2148 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      376 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      911 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1162 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx     1824 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      343 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2396 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
--rw-r--r--  2.0 unx     7840 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1885 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      366 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       42 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx     4580 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx     1785 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      371 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2285 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      566 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      264 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      936 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      491 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx      542 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      936 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      748 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      379 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      744 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      858 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      701 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx     1774 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     2687 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      915 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      740 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx      384 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      491 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx      245 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx     2367 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      350 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      747 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx      608 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      490 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx     1382 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      546 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1829 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1128 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      340 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx     1137 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      325 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      800 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      872 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      242 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      490 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      741 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      351 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx     1359 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx      741 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      521 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     1319 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1204 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      346 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      825 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      743 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     1799 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1988 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx   125360 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/AutohintingTest/Padyakke.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
--rw-r--r--  2.0 unx      830 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
--rw-r--r--  2.0 unx     1030 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
--rw-r--r--  2.0 unx      900 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      283 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
--rw-r--r--  2.0 unx      247 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      243 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      786 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
--rw-r--r--  2.0 unx     1030 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
--rw-r--r--  2.0 unx      897 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      283 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
--rw-r--r--  2.0 unx      247 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      243 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      770 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
--rw-r--r--  2.0 unx      762 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx     2113 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx     1158 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      101 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      215 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      429 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      694 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx     1196 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      560 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx     2107 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
--rw-r--r--  2.0 unx     1160 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx      217 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      429 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      652 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      154 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      893 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      652 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
--rw-r--r--  2.0 unx        7 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/family.fea
--rw-r--r--  2.0 unx     1059 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      897 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx      899 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx       20 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx      745 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
--rw-r--r--  2.0 unx     1340 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
--rw-r--r--  2.0 unx      983 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
--rw-r--r--  2.0 unx      614 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
--rw-r--r--  2.0 unx      916 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
--rw-r--r--  2.0 unx      621 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
--rw-r--r--  2.0 unx      852 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      240 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      878 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      357 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      237 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      343 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      548 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      237 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      345 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx     6904 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
--rw-r--r--  2.0 unx      249 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
--rw-r--r--  2.0 unx      716 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
--rw-r--r--  2.0 unx       73 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
--rw-r--r--  2.0 unx     2035 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
--rw-r--r--  2.0 unx      360 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
--rw-r--r--  2.0 unx      887 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      275 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1659 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      412 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1455 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx     1261 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1265 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
--rw-r--r--  2.0 unx      360 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
--rw-r--r--  2.0 unx      890 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      275 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1642 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      412 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1439 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx     1263 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1263 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
--rw-r--r--  2.0 unx       83 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
--rw-r--r--  2.0 unx    22772 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
--rw-r--r--  2.0 unx      454 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--  2.0 unx     1889 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
--rw-r--r--  2.0 unx     5010 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
--rw-r--r--  2.0 unx     1580 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
--rw-r--r--  2.0 unx     1308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
--rw-r--r--  2.0 unx      764 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
--rw-r--r--  2.0 unx      445 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--  2.0 unx      902 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
--rw-r--r--  2.0 unx     1026 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--  2.0 unx     2295 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
--rw-r--r--  2.0 unx     6165 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
--rw-r--r--  2.0 unx     5180 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
--rw-r--r--  2.0 unx     7158 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
--rw-r--r--  2.0 unx     5741 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
--rw-r--r--  2.0 unx     5197 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
--rw-r--r--  2.0 unx     1074 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/LICENSE
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
--rw-r--r--  2.0 unx    16556 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1844 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      749 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx      240 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx     2492 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx      238 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx     1176 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx      241 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
--rw-r--r--  2.0 unx     3060 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3051 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1827 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      473 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2247 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx     1028 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      687 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      874 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      238 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     3539 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2617 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      241 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx      232 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3007 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx      274 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx     2474 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      732 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx    16556 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1849 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      271 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       68 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx      232 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
--rw-r--r--  2.0 unx    10710 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1826 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      361 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       36 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2192 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      473 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2206 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx     1062 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      690 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      879 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      240 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1847 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     1865 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
--rw-r--r--  2.0 unx    16116 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1829 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      361 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       37 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx      236 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      341 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      237 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1831 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      654 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      473 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2188 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx     1065 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      691 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1222 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      240 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1818 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      344 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
--rw-r--r--  2.0 unx    16116 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1834 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      271 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx       37 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx      232 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1578 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
--rw-r--r--  2.0 unx     6839 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1841 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      361 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx       42 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      308 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx      353 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     2099 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      473 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2197 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx     1057 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      689 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1221 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      240 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     1849 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
--rw-r--r--  2.0 unx      443 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
--rw-r--r--  2.0 unx      790 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      471 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
--rw-r--r--  2.0 unx      714 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
--rw-r--r--  2.0 unx      382 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
--rw-r--r--  2.0 unx      522 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
--rw-r--r--  2.0 unx      543 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      436 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      393 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
--rw-r--r--  2.0 unx      581 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
--rw-r--r--  2.0 unx      156 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      646 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
--rw-r--r--  2.0 unx      410 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
--rw-r--r--  2.0 unx      790 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      287 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
--rw-r--r--  2.0 unx      318 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
--rw-r--r--  2.0 unx      205 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
--rw-r--r--  2.0 unx      784 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
--rw-r--r--  2.0 unx      487 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      898 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      539 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
--rw-r--r--  2.0 unx      221 b- defN 22-Dec-08 19:32 fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-08 19:32 fontmake-3.5.1/.github/workflows/
--rw-r--r--  2.0 unx     4276 b- defN 22-Dec-08 19:32 fontmake-3.5.1/.github/workflows/ci.yml
-722 files, 1194982 bytes uncompressed, 292024 bytes compressed:  75.6%
+Zip file size: 468242 bytes, number of entries: 725
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/Lib/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/.github/
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-12 16:08 fontmake-3.6.0/setup.cfg
+-rw-r--r--  2.0 unx      322 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.gitattributes
+-rw-r--r--  2.0 unx     1453 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.gitignore
+-rw-r--r--  2.0 unx      806 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tox.ini
+-rw-r--r--  2.0 unx      227 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.editorconfig
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-12 16:07 fontmake-3.6.0/test_requirements.txt
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-12 16:07 fontmake-3.6.0/MANIFEST.in
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-12 16:07 fontmake-3.6.0/pyproject.toml
+-rw-r--r--  2.0 unx     1450 b- defN 23-Jun-12 16:07 fontmake-3.6.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-12 16:07 fontmake-3.6.0/LICENSE
+-rw-r--r--  2.0 unx    19601 b- defN 23-Jun-12 16:07 fontmake-3.6.0/USAGE.md
+-rw-r--r--  2.0 unx      466 b- defN 23-Jun-12 16:07 fontmake-3.6.0/requirements.txt
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-12 16:08 fontmake-3.6.0/PKG-INFO
+-rw-r--r--  2.0 unx     3193 b- defN 23-Jun-12 16:07 fontmake-3.6.0/TROUBLESHOOTING.md
+-rwxr-xr-x  2.0 unx     1673 b- defN 23-Jun-12 16:07 fontmake-3.6.0/build_pyz.sh
+-rw-r--r--  2.0 unx     2924 b- defN 23-Jun-12 16:07 fontmake-3.6.0/setup.py
+-rw-r--r--  2.0 unx     6285 b- defN 23-Jun-12 16:07 fontmake-3.6.0/README.md
+-rw-r--r--  2.0 unx      792 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.coveragerc
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.pyup.yml
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.codecov.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/
+-rw-r--r--  2.0 unx     1668 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/test_compatibility.py
+-rw-r--r--  2.0 unx    25699 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/test_instantiator.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/conftest.py
+-rw-r--r--  2.0 unx    33198 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/test_main.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/SwapGlyphNames/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/AutohintingTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InterpolateLayoutTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/IncompatibleSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/
+-rw-r--r--  2.0 unx     6386 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/TestSubset.glyphs
+-rw-r--r--  2.0 unx    30579 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans.glyphs
+-rw-r--r--  2.0 unx     6381 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/TestSubset2.glyphs
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+-rw-r--r--  2.0 unx    22772 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+-rw-r--r--  2.0 unx      454 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--  2.0 unx     5010 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+-rw-r--r--  2.0 unx     1580 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--  2.0 unx     6165 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+-rw-r--r--  2.0 unx      764 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+-rw-r--r--  2.0 unx      902 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+-rw-r--r--  2.0 unx     1889 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/
+-rw-r--r--  2.0 unx      410 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      221 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+-rw-r--r--  2.0 unx      539 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+-rw-r--r--  2.0 unx      487 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+-rw-r--r--  2.0 unx      898 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/
+-rw-r--r--  2.0 unx      443 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/lib.plist
+-rw-r--r--  2.0 unx      471 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/groups.plist
+-rw-r--r--  2.0 unx      714 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      382 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+-rw-r--r--  2.0 unx      581 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+-rw-r--r--  2.0 unx      543 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      393 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      436 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx      852 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+-rw-r--r--  2.0 unx     2253 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+-rw-r--r--  2.0 unx      621 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest.designspace
+-rw-r--r--  2.0 unx      745 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+-rw-r--r--  2.0 unx     1340 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+-rw-r--r--  2.0 unx      614 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+-rw-r--r--  2.0 unx     3057 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufoz
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      878 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      548 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx   125360 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/AutohintingTest/Padyakke.glyphs
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+-rw-r--r--  2.0 unx     5180 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+-rw-r--r--  2.0 unx     5741 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+-rw-r--r--  2.0 unx     7158 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+-rw-r--r--  2.0 unx     5197 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/LICENSE
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    16116 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1829 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2188 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1222 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2537 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+-rw-r--r--  2.0 unx     1818 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    16556 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1844 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx     3060 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+-rw-r--r--  2.0 unx     3051 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      687 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1827 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2247 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx     1028 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      874 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     2492 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+-rw-r--r--  2.0 unx     2474 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      732 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx     3007 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     3539 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2617 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+-rw-r--r--  2.0 unx     6839 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1841 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     2099 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2197 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx     1057 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1221 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1849 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    10710 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1826 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      690 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2206 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      879 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1847 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+-rw-r--r--  2.0 unx    16116 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1834 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1578 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx    16556 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1849 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+-rw-r--r--  2.0 unx      249 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+-rw-r--r--  2.0 unx      716 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+-rw-r--r--  2.0 unx     6904 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+-rw-r--r--  2.0 unx      762 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx     2113 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1158 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      429 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx     2107 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1160 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      429 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      217 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      893 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+-rw-r--r--  2.0 unx     2035 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx     1455 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx     1659 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1261 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--  2.0 unx     1265 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      890 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx     1439 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx     1642 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+-rw-r--r--  2.0 unx     1135 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      479 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      886 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      425 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/family.fea
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      899 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+-rw-r--r--  2.0 unx     7111 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans.designspace
+-rw-r--r--  2.0 unx     8462 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_missing.designspace
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+-rw-r--r--  2.0 unx     1394 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-width-only.designspace
+-rw-r--r--  2.0 unx     2611 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/LICENSE
+-rw-r--r--  2.0 unx     1412 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+-rw-r--r--  2.0 unx     7834 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_no_default.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    18291 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+-rw-r--r--  2.0 unx     4852 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1873 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      740 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1751 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      514 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      802 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx     1459 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx     1970 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      752 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      378 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1357 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      857 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      875 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1130 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      747 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx     2358 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx     1158 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      954 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      801 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      703 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      370 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      943 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2537 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+-rw-r--r--  2.0 unx     1965 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    18792 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx     3543 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+-rw-r--r--  2.0 unx     3534 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      737 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1728 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      515 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      628 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      797 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx     1462 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      538 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      690 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx     1966 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      377 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      975 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      853 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      870 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     1120 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx     2453 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx     1105 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      626 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      736 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      914 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      798 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      369 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx     1402 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      942 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      358 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx     1372 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     2825 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx      853 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+-rw-r--r--  2.0 unx     2706 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      828 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx     2452 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+-rw-r--r--  2.0 unx     1471 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+-rw-r--r--  2.0 unx      482 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx     3498 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx      751 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+-rw-r--r--  2.0 unx     2111 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     3998 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      244 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     3358 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+-rw-r--r--  2.0 unx     7840 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx     4580 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1885 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      740 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1774 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      608 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      825 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx     1829 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      340 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      744 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      379 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1382 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      858 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      872 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1204 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      566 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      748 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx     2367 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx     1137 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      747 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      915 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      800 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1128 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      384 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx     1319 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx     1359 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1988 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    12341 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+-rw-r--r--  2.0 unx      301 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1870 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1747 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      259 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      806 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx     1495 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      545 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      940 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      493 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx     2369 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      748 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      380 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      988 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      861 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      875 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      750 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx     2376 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx     1154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      492 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      745 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      919 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     2203 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      803 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      495 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      370 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx     1418 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      947 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1037 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx     1387 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1986 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2005 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    16617 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      615 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1386 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+-rw-r--r--  2.0 unx      268 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+-rw-r--r--  2.0 unx     3181 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+-rw-r--r--  2.0 unx     1938 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+-rw-r--r--  2.0 unx     2307 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2646 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      923 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1806 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2353 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+-rw-r--r--  2.0 unx    16223 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+-rw-r--r--  2.0 unx     5462 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1384 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx     2148 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx     1162 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      376 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      911 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1824 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2396 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+-rw-r--r--  2.0 unx      830 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+-rw-r--r--  2.0 unx     1030 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      786 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+-rw-r--r--  2.0 unx     1030 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      770 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 16:07 fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake/
+-rw-r--r--  2.0 unx      402 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx    42241 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1439 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/errors.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/__init__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-12 16:08 fontmake-3.6.0/Lib/fontmake/_version.py
+-rw-r--r--  2.0 unx    32133 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/instantiator.py
+-rw-r--r--  2.0 unx    58334 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/font_project.py
+-rw-r--r--  2.0 unx    25640 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/__main__.py
+-rw-r--r--  2.0 unx     3049 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/compatibility.py
+-rw-r--r--  2.0 unx     3288 b- defN 23-Jun-12 16:07 fontmake-3.6.0/Lib/fontmake/ttfautohint.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-12 16:08 fontmake-3.6.0/.github/workflows/
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jun-12 16:07 fontmake-3.6.0/.github/workflows/ci.yml
+725 files, 1205095 bytes uncompressed, 296596 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,2167 +1,2176 @@
-Filename: fontmake-3.5.1/
+Filename: fontmake-3.6.0/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/
+Filename: fontmake-3.6.0/tests/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/
+Filename: fontmake-3.6.0/Lib/
 Comment: 
 
-Filename: fontmake-3.5.1/.github/
+Filename: fontmake-3.6.0/.github/
 Comment: 
 
-Filename: fontmake-3.5.1/requirements.txt
+Filename: fontmake-3.6.0/setup.cfg
 Comment: 
 
-Filename: fontmake-3.5.1/test_requirements.txt
+Filename: fontmake-3.6.0/.gitattributes
 Comment: 
 
-Filename: fontmake-3.5.1/setup.py
+Filename: fontmake-3.6.0/.gitignore
 Comment: 
 
-Filename: fontmake-3.5.1/.coveragerc
+Filename: fontmake-3.6.0/tox.ini
 Comment: 
 
-Filename: fontmake-3.5.1/setup.cfg
+Filename: fontmake-3.6.0/.editorconfig
 Comment: 
 
-Filename: fontmake-3.5.1/.gitattributes
+Filename: fontmake-3.6.0/test_requirements.txt
 Comment: 
 
-Filename: fontmake-3.5.1/build_pyz.sh
+Filename: fontmake-3.6.0/MANIFEST.in
 Comment: 
 
-Filename: fontmake-3.5.1/PKG-INFO
+Filename: fontmake-3.6.0/pyproject.toml
 Comment: 
 
-Filename: fontmake-3.5.1/tox.ini
+Filename: fontmake-3.6.0/CONTRIBUTING.md
 Comment: 
 
-Filename: fontmake-3.5.1/CONTRIBUTING.md
+Filename: fontmake-3.6.0/LICENSE
 Comment: 
 
-Filename: fontmake-3.5.1/USAGE.md
+Filename: fontmake-3.6.0/USAGE.md
 Comment: 
 
-Filename: fontmake-3.5.1/.codecov.yml
+Filename: fontmake-3.6.0/requirements.txt
 Comment: 
 
-Filename: fontmake-3.5.1/.editorconfig
+Filename: fontmake-3.6.0/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.5.1/TROUBLESHOOTING.md
+Filename: fontmake-3.6.0/TROUBLESHOOTING.md
 Comment: 
 
-Filename: fontmake-3.5.1/.pyup.yml
+Filename: fontmake-3.6.0/build_pyz.sh
 Comment: 
 
-Filename: fontmake-3.5.1/LICENSE
+Filename: fontmake-3.6.0/setup.py
 Comment: 
 
-Filename: fontmake-3.5.1/README.md
+Filename: fontmake-3.6.0/README.md
 Comment: 
 
-Filename: fontmake-3.5.1/pyproject.toml
+Filename: fontmake-3.6.0/.coveragerc
 Comment: 
 
-Filename: fontmake-3.5.1/.gitignore
+Filename: fontmake-3.6.0/.pyup.yml
 Comment: 
 
-Filename: fontmake-3.5.1/MANIFEST.in
+Filename: fontmake-3.6.0/.codecov.yml
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/
+Filename: fontmake-3.6.0/tests/data/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/
+Filename: fontmake-3.6.0/tests/test_compatibility.py
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/__init__.py
+Filename: fontmake-3.6.0/tests/test_instantiator.py
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/__main__.py
+Filename: fontmake-3.6.0/tests/conftest.py
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/compatibility.py
+Filename: fontmake-3.6.0/tests/test_main.py
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/ttfautohint.py
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/font_project.py
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/instantiator.py
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/_version.py
+Filename: fontmake-3.6.0/tests/data/AutohintingTest/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake/errors.py
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/dependency_links.txt
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/entry_points.txt
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/top_level.txt
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/PKG-INFO
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/requires.txt
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/
 Comment: 
 
-Filename: fontmake-3.5.1/Lib/fontmake.egg-info/SOURCES.txt
+Filename: fontmake-3.6.0/tests/data/MutatorSans/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/test_instantiator.py
+Filename: fontmake-3.6.0/tests/data/TestSubset.glyphs
 Comment: 
 
-Filename: fontmake-3.5.1/tests/test_main.py
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans.glyphs
 Comment: 
 
-Filename: fontmake-3.5.1/tests/conftest.py
+Filename: fontmake-3.6.0/tests/data/TestSubset2.glyphs
 Comment: 
 
-Filename: fontmake-3.5.1/tests/test_compatibility.py
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/AutohintingTest/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/TestSubset.glyphs
+Filename: fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/TestSubset2.glyphs
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans.glyphs
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_missing.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufoz
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/LICENSE
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufoz
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/AutohintingTest/Padyakke.glyphs
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/LICENSE
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/family.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_missing.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-width-only.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/LICENSE
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-weight-only.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_no_default.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/AutohintingTest/Padyakke.glyphs
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/family.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/LICENSE
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+Filename: fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+Filename: fontmake-3.6.0/Lib/fontmake/
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/requires.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/dependency_links.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/SOURCES.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/entry_points.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+Filename: fontmake-3.6.0/Lib/fontmake.egg-info/top_level.txt
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+Filename: fontmake-3.6.0/Lib/fontmake/errors.py
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+Filename: fontmake-3.6.0/Lib/fontmake/__init__.py
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+Filename: fontmake-3.6.0/Lib/fontmake/_version.py
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+Filename: fontmake-3.6.0/Lib/fontmake/instantiator.py
 Comment: 
 
-Filename: fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+Filename: fontmake-3.6.0/Lib/fontmake/font_project.py
 Comment: 
 
-Filename: fontmake-3.5.1/.github/workflows/
+Filename: fontmake-3.6.0/Lib/fontmake/__main__.py
 Comment: 
 
-Filename: fontmake-3.5.1/.github/workflows/ci.yml
+Filename: fontmake-3.6.0/Lib/fontmake/compatibility.py
+Comment: 
+
+Filename: fontmake-3.6.0/Lib/fontmake/ttfautohint.py
+Comment: 
+
+Filename: fontmake-3.6.0/.github/workflows/
+Comment: 
+
+Filename: fontmake-3.6.0/.github/workflows/ci.yml
 Comment: 
 
 Zip file comment:
```

## Comparing `fontmake-3.5.1/setup.py` & `fontmake-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,22 @@
     long_description_content_type="text/markdown",
     url="https://github.com/googlei18n/fontmake",
     license="Apache Software License 2.0",
     packages=find_packages("Lib"),
     package_dir={"": "Lib"},
     entry_points={"console_scripts": ["fontmake = fontmake.__main__:main"]},
     setup_requires=wheel + ["setuptools_scm"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "fonttools[ufo,lxml,unicode]>=4.38.0 ; implementation_name == 'cpython'",
-        "fonttools[ufo,unicode]>=4.38.0 ; implementation_name != 'cpython'",
-        "glyphsLib>=6.1.0",
-        "ufo2ft[compreffor]>=2.29.0",
+        "fonttools[ufo,lxml,unicode]>=4.40.0 ; implementation_name == 'cpython'",
+        "fonttools[ufo,unicode]>=4.40.0 ; implementation_name != 'cpython'",
+        "glyphsLib>=6.2.1",
+        "ufo2ft[compreffor]>=2.32.0",
         "fontMath>=0.9.3",
-        "ufoLib2>=0.13.0",
+        "ufoLib2>=0.14.0",
         "attrs>=19",
     ],
     extras_require=extras_require,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

## Comparing `fontmake-3.5.1/.coveragerc` & `fontmake-3.6.0/.coveragerc`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/build_pyz.sh` & `fontmake-3.6.0/build_pyz.sh`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/PKG-INFO` & `fontmake-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.5.1
+Version: 3.6.0
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Text Processing :: Fonts
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathops
 Provides-Extra: lxml
 Provides-Extra: mutatormath
 Provides-Extra: autohint
 Provides-Extra: all
 License-File: LICENSE
@@ -30,15 +30,15 @@
 
 # fontmake
 
 `fontmake` compiles fonts from various sources (`.glyphs`, `.ufo`, `designspace`) into binaries (`.otf`, `.ttf`). You can use it to create static instances and variable fonts.
 
 ## Installation
 
-Fontmake requires Python 3.7 or later.
+Fontmake requires Python 3.8 or later.
 
 Releases are available on [PyPI][] and can be installed with [pip][].
 
 ``` bash
 pip3 install fontmake
 ```
 
@@ -63,15 +63,15 @@
 
 ### Source file format options
 
 There are two ways to specify the source file or files:
 
 One can either use the following, mutually exclusive, flags:
 * `-g filename.glyphs`: Converts a Glyphs source file to binary.
-* `-u filename.ufo ...`: Converts one or more UFO files to binary.
+* `-u filename.ufo ...`: Converts one or more UFO(Z) files to binary.
 * `-m filename.designspace`: Converts a Designspace file to binary. (The `-m` is for `mutatormath`, an old Python library for handling designspaces.)
 
 Alternatively, one can specify the input(s) as positional arguments without the flag, letting fontmake infer the source format from the file extension: e.g. ``fontmake MyFont.designspace``, etc.
 
 Note: if the positional arguments are preceded by an option that takes one or more arguments, you need to use the special `--` separator to mark all following
 arguments as positional (non-options), otherwise the parser gets confused. E.g., the `-i` option takes zero or one arguments (see futher below for details); without `--`, argparse thinks you didn't provide any inputs:
 
@@ -93,15 +93,15 @@
 * `variable`: A TrueType variable font. Placed in the `variable_ttf/` directory.
 * `variable-cff2`: A variable font with CFF2 outlines. Placed in the `variable_otf/` directory.
 
 The following output file formats are also available, but are generally used internally by fontmake as an intermediate step to one of the above outputs:
 
 * `otf-interpolatable`: OTF binaries suitable for merging into a variable font. Placed in the `master_otf_interpolatable/` directory. (These differ from `otf` in that the outlines are unoptimized.)
 * `ttf-interpolatable`: TTF binaries suitable for merging into a variable font. Placed in the `master_ttf_interpolatable/` directory. (The outlines are converted to quadratic curves in an interpolation-compatible way.)
-* `ufo`: Glyphs sources can be converted to UFO. Placed in the `master_ufo/` directory.
+* `ufo`: Glyphs sources can be converted to UFO, or to UFO zip (`.ufoz`) format with the flag `--save-ufo-as-zip`. Placed in the `master_ufo/` directory. 
 
 If no format option is specified, the default is `-o otf ttf`.
 
 ### Other important command line options
 
 * `-i` (Interpolate instances): Having per-master binaries is not always what you expect; if you have defined instances ("exports") in your Glyphs file, they will *not* be generated by default. To generate them, pass the `-i` flag, which interpolates static instances, and places them in the `instance_ttf/` or `instance_otf/` directory as appropriate.
```

## Comparing `fontmake-3.5.1/tox.ini` & `fontmake-3.6.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = lint, py3{7,8,9}, pypy3, coverage-report
+envlist = lint, py3{8,9,10,11}, pypy3, coverage-report
 skip_missing_interpreters = true
 
 [testenv]
 deps =
     -r requirements.txt
     -r test_requirements.txt
 ; download the latest pip, setuptools and wheel when creating the venv
```

## Comparing `fontmake-3.5.1/CONTRIBUTING.md` & `fontmake-3.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/USAGE.md` & `fontmake-3.6.0/USAGE.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/TROUBLESHOOTING.md` & `fontmake-3.6.0/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/LICENSE` & `fontmake-3.6.0/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/README.md` & `fontmake-3.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # fontmake
 
 `fontmake` compiles fonts from various sources (`.glyphs`, `.ufo`, `designspace`) into binaries (`.otf`, `.ttf`). You can use it to create static instances and variable fonts.
 
 ## Installation
 
-Fontmake requires Python 3.7 or later.
+Fontmake requires Python 3.8 or later.
 
 Releases are available on [PyPI][] and can be installed with [pip][].
 
 ``` bash
 pip3 install fontmake
 ```
 
@@ -36,15 +36,15 @@
 
 ### Source file format options
 
 There are two ways to specify the source file or files:
 
 One can either use the following, mutually exclusive, flags:
 * `-g filename.glyphs`: Converts a Glyphs source file to binary.
-* `-u filename.ufo ...`: Converts one or more UFO files to binary.
+* `-u filename.ufo ...`: Converts one or more UFO(Z) files to binary.
 * `-m filename.designspace`: Converts a Designspace file to binary. (The `-m` is for `mutatormath`, an old Python library for handling designspaces.)
 
 Alternatively, one can specify the input(s) as positional arguments without the flag, letting fontmake infer the source format from the file extension: e.g. ``fontmake MyFont.designspace``, etc.
 
 Note: if the positional arguments are preceded by an option that takes one or more arguments, you need to use the special `--` separator to mark all following
 arguments as positional (non-options), otherwise the parser gets confused. E.g., the `-i` option takes zero or one arguments (see futher below for details); without `--`, argparse thinks you didn't provide any inputs:
 
@@ -66,15 +66,15 @@
 * `variable`: A TrueType variable font. Placed in the `variable_ttf/` directory.
 * `variable-cff2`: A variable font with CFF2 outlines. Placed in the `variable_otf/` directory.
 
 The following output file formats are also available, but are generally used internally by fontmake as an intermediate step to one of the above outputs:
 
 * `otf-interpolatable`: OTF binaries suitable for merging into a variable font. Placed in the `master_otf_interpolatable/` directory. (These differ from `otf` in that the outlines are unoptimized.)
 * `ttf-interpolatable`: TTF binaries suitable for merging into a variable font. Placed in the `master_ttf_interpolatable/` directory. (The outlines are converted to quadratic curves in an interpolation-compatible way.)
-* `ufo`: Glyphs sources can be converted to UFO. Placed in the `master_ufo/` directory.
+* `ufo`: Glyphs sources can be converted to UFO, or to UFO zip (`.ufoz`) format with the flag `--save-ufo-as-zip`. Placed in the `master_ufo/` directory. 
 
 If no format option is specified, the default is `-o otf ttf`.
 
 ### Other important command line options
 
 * `-i` (Interpolate instances): Having per-master binaries is not always what you expect; if you have defined instances ("exports") in your Glyphs file, they will *not* be generated by default. To generate them, pass the `-i` flag, which interpolates static instances, and places them in the `instance_ttf/` or `instance_otf/` directory as appropriate.
```

## Comparing `fontmake-3.5.1/.gitignore` & `fontmake-3.6.0/.gitignore`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/Lib/fontmake/__main__.py` & `fontmake-3.6.0/Lib/fontmake/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,20 +128,20 @@
             if glyphs_path:
                 parser.error("Only one *.glyphs source file is allowed")
             glyphs_path = filename
         elif filename.endswith(".designspace"):
             if designspace_path:
                 parser.error("Only one *.designspace source file is allowed")
             designspace_path = filename
-        elif (filename.endswith(".ufo") and os.path.isdir(filename)) or (
-            filename.endswith(".ufoz") and os.path.isfile(filename)
-        ):
+        elif (
+            os.path.normpath(filename).endswith(".ufo") and os.path.isdir(filename)
+        ) or (filename.endswith(".ufoz") and os.path.isfile(filename)):
             ufo_paths.append(filename)
         else:
-            parser.error(f"Unknown input file extension: '{filename}'")
+            parser.error(f"Unknown input file extension: {filename!r}")
 
     count = sum(bool(p) for p in (glyphs_path, ufo_paths, designspace_path))
     if count == 0:
         parser.error("No input files specified")
     elif count > 1:
         parser.error(f"Expected 1, got {count} different types of inputs files")
 
@@ -500,14 +500,26 @@
         "built-in or from an external module, optionally initialized with "
         "the given keyword arguments. The class and module names are "
         "separated by '::'. The option can be repeated multiple times "
         "for each filter class. The option overrides the filters specified "
         "in the UFO lib. You can use an ellipsis --filter='...' to keep the "
         "latter and insert additional --filter(s), either before or after it.",
     )
+    contourGroup.add_argument(
+        "--no-auto-use-my-metrics",
+        dest="auto_use_my_metrics",
+        action="store_false",
+        help="Don't automatically set USE_MY_METRICS glyf component flags (0x0200).",
+    )
+    contourGroup.add_argument(
+        "--drop-implied-oncurves",
+        action="store_true",
+        help="drop on-curve points that can be implied when exactly in the middle of "
+        "two off-curve points (TrueType only; default: %(default)s).",
+    )
 
     layoutGroup = parser.add_argument_group(title="Handling of OpenType Layout")
     layoutGroup.add_argument(
         "--interpolate-binary-layout",
         nargs="?",
         default=False,
         const=True,
```

## Comparing `fontmake-3.5.1/Lib/fontmake/compatibility.py` & `fontmake-3.6.0/Lib/fontmake/compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/Lib/fontmake/ttfautohint.py` & `fontmake-3.6.0/Lib/fontmake/ttfautohint.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/Lib/fontmake/font_project.py` & `fontmake-3.6.0/Lib/fontmake/font_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,27 +308,29 @@
         conversion_error=None,
         feature_writers=None,
         cff_round_tolerance=None,
         debug_feature_file=None,
         fea_include_dir=None,
         flatten_components=False,
         filters=None,
+        auto_use_my_metrics=True,
         **kwargs,
     ):
         if ttf:
             return ufo2ft.compileInterpolatableTTFsFromDS(
                 designspace,
                 useProductionNames=use_production_names,
                 reverseDirection=reverse_direction,
                 cubicConversionError=conversion_error,
                 featureWriters=feature_writers,
                 debugFeatureFile=debug_feature_file,
                 feaIncludeDir=fea_include_dir,
                 filters=filters,
                 flattenComponents=flatten_components,
+                autoUseMyMetrics=auto_use_my_metrics,
                 inplace=True,
             )
         else:
             return ufo2ft.compileInterpolatableOTFsFromDS(
                 designspace,
                 useProductionNames=use_production_names,
                 roundTolerance=cff_round_tolerance,
@@ -365,14 +367,16 @@
         conversion_error=None,
         feature_writers=None,
         cff_round_tolerance=None,
         debug_feature_file=None,
         fea_include_dir=None,
         flatten_components=False,
         filters=None,
+        auto_use_my_metrics=True,
+        drop_implied_oncurves=False,
         **kwargs,
     ):
         """Build OpenType variable fonts from masters in a designspace."""
         assert not (output_path and output_dir), "mutually exclusive args"
 
         vfs_in_document = designspace.getVariableFonts()
         if not vfs_in_document:
@@ -426,14 +430,16 @@
                 optimizeGvar=optimize_gvar,
                 flattenComponents=flatten_components,
                 debugFeatureFile=debug_feature_file,
                 feaIncludeDir=fea_include_dir,
                 filters=filters,
                 inplace=True,
                 variableFontNames=list(vf_name_to_output_path),
+                autoUseMyMetrics=auto_use_my_metrics,
+                dropImpliedOnCurves=drop_implied_oncurves,
             )
         else:
             fonts = ufo2ft.compileVariableCFF2s(
                 designspace,
                 featureWriters=feature_writers,
                 useProductionNames=use_production_names,
                 roundTolerance=cff_round_tolerance,
@@ -457,14 +463,16 @@
                 options.pop(key, None)
             compile_func, fmt = ufo2ft.compileTTF, "TTF"
         else:
             for key in (
                 "cubicConversionError",
                 "reverseDirection",
                 "flattenComponents",
+                "autoUseMyMetrics",
+                "dropImpliedOnCurves",
             ):
                 options.pop(key, None)
             compile_func, fmt = ufo2ft.compileOTF, "OTF"
 
         writeFontName = len(ufos) > 1
         for ufo in ufos:
             name = self._font_name(ufo)
@@ -503,14 +511,16 @@
         inplace=True,
         cff_version=1,
         subroutinizer=None,
         flatten_components=False,
         filters=None,
         generate_GDEF=True,
         fea_include_dir=None,
+        auto_use_my_metrics=True,
+        drop_implied_oncurves=False,
     ):
         """Build OpenType binaries from UFOs.
 
         Args:
             ufos: Font objects to compile.
             ttf: If True, build fonts with TrueType outlines and .ttf extension.
             is_instance: If output fonts are instances, for generating paths.
@@ -558,26 +568,31 @@
                 level.
             filters: list of ufo2ft-compatible filter classes or
                 pre-initialized objects that are passed on to ufo2ft
                 pre-processor to modify the glyph set. The filters are either
                 pre-filters or post-filters, called before or after the default
                 filters. The default filters are format specific and some can
                 be disabled with other arguments.
+            auto_use_my_metrics: whether to automatically set USE_MY_METRICS glyf
+                component flags (0x0200). Not needed unless the font has hinted metrics.
+            drop_implied_oncurves: drop on-curve points that can be implied when exactly
+                in the middle of two off-curve points (TrueType only; default: False).
         """  # noqa: B950
         assert not (output_path and output_dir), "mutually exclusive args"
 
         if output_path is not None and len(ufos) > 1:
             raise ValueError("output_path requires a single input")
 
         if subroutinize is not None:
             import warnings
 
             warnings.warn(
                 "the 'subroutinize' argument is deprecated, use 'optimize_cff'",
                 UserWarning,
+                stacklevel=2,
             )
             if subroutinize:
                 optimize_cff = CFFOptimization.SUBROUTINIZE
             else:
                 # for b/w compatibility, we still run the charstring specializer
                 # even when --no-subroutinize is used. Use the new --optimize-cff
                 # option to disable both specilization and subroutinization
@@ -610,14 +625,16 @@
             featureWriters=feature_writers,
             debugFeatureFile=debug_feature_file,
             feaIncludeDir=fea_include_dir,
             cffVersion=cff_version,
             subroutinizer=subroutinizer,
             flattenComponents=flatten_components,
             filters=filters,
+            autoUseMyMetrics=auto_use_my_metrics,
+            dropImpliedOnCurves=drop_implied_oncurves,
             inplace=True,  # avoid extra copy
         )
 
         for font, ufo in zip(fonts, ufos):
             if interpolate_layout_from is not None:
                 master_locations, instance_locations = self._designspace_locations(
                     interpolate_layout_from
@@ -905,21 +922,23 @@
                 if not instance.lib.get("com.schriftgestaltung.export", True):
                     continue
 
                 # Skip instances that do not match the user's inclusion regex if given.
                 if include is not None and not fullmatch(include, instance.name):
                     continue
 
-                logger.info(f'Generating instance UFO for "{instance.name}"')
+                logger.info("Generating instance UFO for {!r}".format(instance.name))
 
                 try:
                     instance.font = generator.generate_instance(instance)
                 except instantiator.InstantiatorError as e:
                     raise FontmakeError(
-                        f"Interpolating instance '{instance.styleName}' failed.",
+                        "Interpolating instance {!r} failed.".format(
+                            instance.styleName
+                        ),
                         designspace.path,
                     ) from e
 
                 apply_instance_data_to_ufo(instance.font, instance, subDoc)
 
                 # TODO: Making filenames up on the spot is complicated, ideally don't save
                 # anything if filename is not set, but make something up when "ufo" is in
```

## Comparing `fontmake-3.5.1/Lib/fontmake/instantiator.py` & `fontmake-3.6.0/Lib/fontmake/instantiator.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,28 +220,49 @@
 
         designspace.loadSourceFonts(ufoLib2.Font.open)
 
         # The default font (default layer) determines which glyphs are interpolated,
         # because the math behind varLib and MutatorMath uses the default font as the
         # point of reference for all data.
         default_font = designspace.default.font
+        non_default_layer_name = designspace.default.layerName
+
         glyph_names: Set[str] = set(default_font.keys())
 
+        if non_default_layer_name is not None:
+            try:
+                layer = default_font.layers[non_default_layer_name]
+            except KeyError as e:
+                raise InstantiatorError(
+                    f"Layer {non_default_layer_name!r} not found "
+                    f"in {designspace.default.filename}"
+                ) from e
+            layer = default_font.layers[non_default_layer_name]
+            glyph_names = layer.keys()
+            logger.info(f"Building from layer {layer.name}")
+
         for source in designspace.sources:
             other_names = set(source.font.keys())
             diff_names = other_names - glyph_names
             if diff_names:
+                max_diff_glyphs = 10
                 logger.warning(
-                    "The source %s (%s) contains glyphs that are missing from the "
-                    "default source, which will be ignored: %s. If this is unintended, "
+                    "The source %s (%s)%s contains glyphs that are missing from the "
+                    "default source, which will be ignored: %s%s; if this is unintended, "
                     "check that these glyphs have the exact same name as the "
                     "corresponding glyphs in the default source.",
                     source.name,
                     source.filename,
-                    ", ".join(sorted(diff_names)),
+                    f" [layer: {source.layerName}]"
+                    if non_default_layer_name is not None
+                    else "",
+                    ", ".join(sorted(diff_names)[0:max_diff_glyphs]),
+                    f"... ({len(diff_names)} total)"
+                    if len(diff_names) > max_diff_glyphs
+                    else "",
                 )
 
         # Construct Variators
         axis_bounds: AxisBounds = {}  # Design space!
         axis_order: List[str] = []
         special_axes = {}
         for axis in designspace.axes:
@@ -275,15 +296,15 @@
         glyph_name_to_unicodes: Dict[str, List[int]] = {}
         for glyph_name in glyph_names:
             items = collect_glyph_masters(designspace, glyph_name, axis_bounds)
             try:
                 glyph_mutators[glyph_name] = Variator.from_masters(items, axis_order)
             except varLib.errors.VarLibError as e:
                 raise InstantiatorError(
-                    f"Cannot set up glyph '{glyph_name}' for interpolation: {e}'"
+                    f"Cannot set up glyph {glyph_name} for interpolation: {e}'"
                 ) from e
             glyph_name_to_unicodes[glyph_name] = default_font[glyph_name].unicodes
 
         # Construct defaults to copy over
         copy_feature_text: str = default_font.features.text
         copy_nonkerning_groups: Mapping[str, List[str]] = {
             key: glyph_names
@@ -378,15 +399,15 @@
                 glyph_instance.extractGlyph(glyph, onlyGeometry=True)
             except Exception as e:
                 # TODO: Figure out what exceptions fontMath/varLib can throw.
                 # By default, explode if we cannot generate a glyph instance for
                 # whatever reason (usually outline incompatibility)...
                 if glyph_name not in self.skip_export_glyphs:
                     raise InstantiatorError(
-                        f"Failed to generate instance of glyph '{glyph_name}': "
+                        f"Failed to generate instance of glyph {glyph_name!r}: "
                         f"{str(e)}. (Note: the most common cause for an error here is "
                         "that the glyph outlines are not point-for-point compatible or "
                         "have the same starting point or are in the same order in all "
                         "masters.)"
                     ) from e
 
                 # ...except if the glyph is in public.skipExportGlyphs and would
@@ -490,17 +511,17 @@
 
     default_location = ", ".join(
         f"{k}: {v}" for k, v in designspace.newDefaultLocation().items()
     )
 
     return (
         "Can't generate UFOs from this Designspace because there is no default "
-        f"master source at location '{default_location}'. Check that all 'default' "
+        "master source at location {!r}. Check that all 'default' "
         "values of all axes together point to a single actual master source. "
-        f"{bonus_msg}"
+        "{!s}".format(default_location, bonus_msg)
     )
 
 
 def location_to_key(location: Location) -> LocationKey:
     """Converts a Location into a sorted tuple so it can be used as a dict
     key."""
     return tuple(sorted(location.items()))
@@ -513,17 +534,18 @@
 
 
 def collect_info_masters(
     designspace: designspaceLib.DesignSpaceDocument, axis_bounds: AxisBounds
 ) -> List[Tuple[Location, FontMathObject]]:
     """Return master Info objects wrapped by MathInfo."""
     locations_and_masters = []
+
     for source in designspace.sources:
-        if source.layerName is not None:
-            continue  # No font info in source layers.
+        if source.layerName is not None and source is not designspace.default:
+            continue  # No font info in non-default source layers.
 
         normalized_location = varLib.models.normalizeLocation(
             source.location, axis_bounds
         )
         locations_and_masters.append(
             (normalized_location, fontMath.MathInfo(source.font.info))
         )
@@ -537,17 +559,18 @@
     """Return master kerning objects wrapped by MathKerning."""
 
     # Always take the groups from the default source. This also avoids fontMath
     # making a union of all groups it is given.
     groups = designspace.default.font.groups
 
     locations_and_masters = []
+
     for source in designspace.sources:
-        if source.layerName is not None:
-            continue  # No kerning in source layers.
+        if source.layerName is not None and source is not designspace.default:
+            continue  # No kerning in non-default source layers.
 
         # If a source has groups, they should match the default's.
         if source.font.groups and source.font.groups != groups:
             logger.warning(
                 "The source %s (%s) contains different groups than the default source. "
                 "The default source's groups will be used for the instances.",
                 source.name,
@@ -661,16 +684,17 @@
 
     The .unicodes are not swapped. The rules mechanism is supposed to swap
     glyphs, not characters.
     """
 
     if name_old not in font or name_new not in font:
         raise InstantiatorError(
-            f"Cannot swap glyphs '{name_old}' and '{name_new}', as either or both are "
-            "missing."
+            "Cannot swap glyphs {!r} and {!r}, as either or both are missing".format(
+                name_old, name_new
+            )
         )
 
     # 1. Swap outlines and glyph width. Ignore lib content and other properties.
     glyph_swap = ufoLib2.objects.Glyph(name="temporary_swap_glyph")
     glyph_old = font[name_old]
     glyph_new = font[name_new]
```

## Comparing `fontmake-3.5.1/Lib/fontmake/errors.py` & `fontmake-3.6.0/Lib/fontmake/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __init__(self, msg, source_file):
         self.msg = msg
         self.source_trail = [source_file]
 
     def __str__(self):
         trail = " -> ".join(
-            f"'{str(_try_relative_path(s))}'"
+            f"{str(_try_relative_path(s))!r}"
             for s in reversed(self.source_trail)
             if s is not None
         )
         cause = str(self.__cause__) if self.__cause__ is not None else None
 
         message = ""
         if trail:
```

## Comparing `fontmake-3.5.1/Lib/fontmake.egg-info/PKG-INFO` & `fontmake-3.6.0/Lib/fontmake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.5.1
+Version: 3.6.0
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Text Processing :: Fonts
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathops
 Provides-Extra: lxml
 Provides-Extra: mutatormath
 Provides-Extra: autohint
 Provides-Extra: all
 License-File: LICENSE
@@ -30,15 +30,15 @@
 
 # fontmake
 
 `fontmake` compiles fonts from various sources (`.glyphs`, `.ufo`, `designspace`) into binaries (`.otf`, `.ttf`). You can use it to create static instances and variable fonts.
 
 ## Installation
 
-Fontmake requires Python 3.7 or later.
+Fontmake requires Python 3.8 or later.
 
 Releases are available on [PyPI][] and can be installed with [pip][].
 
 ``` bash
 pip3 install fontmake
 ```
 
@@ -63,15 +63,15 @@
 
 ### Source file format options
 
 There are two ways to specify the source file or files:
 
 One can either use the following, mutually exclusive, flags:
 * `-g filename.glyphs`: Converts a Glyphs source file to binary.
-* `-u filename.ufo ...`: Converts one or more UFO files to binary.
+* `-u filename.ufo ...`: Converts one or more UFO(Z) files to binary.
 * `-m filename.designspace`: Converts a Designspace file to binary. (The `-m` is for `mutatormath`, an old Python library for handling designspaces.)
 
 Alternatively, one can specify the input(s) as positional arguments without the flag, letting fontmake infer the source format from the file extension: e.g. ``fontmake MyFont.designspace``, etc.
 
 Note: if the positional arguments are preceded by an option that takes one or more arguments, you need to use the special `--` separator to mark all following
 arguments as positional (non-options), otherwise the parser gets confused. E.g., the `-i` option takes zero or one arguments (see futher below for details); without `--`, argparse thinks you didn't provide any inputs:
 
@@ -93,15 +93,15 @@
 * `variable`: A TrueType variable font. Placed in the `variable_ttf/` directory.
 * `variable-cff2`: A variable font with CFF2 outlines. Placed in the `variable_otf/` directory.
 
 The following output file formats are also available, but are generally used internally by fontmake as an intermediate step to one of the above outputs:
 
 * `otf-interpolatable`: OTF binaries suitable for merging into a variable font. Placed in the `master_otf_interpolatable/` directory. (These differ from `otf` in that the outlines are unoptimized.)
 * `ttf-interpolatable`: TTF binaries suitable for merging into a variable font. Placed in the `master_ttf_interpolatable/` directory. (The outlines are converted to quadratic curves in an interpolation-compatible way.)
-* `ufo`: Glyphs sources can be converted to UFO. Placed in the `master_ufo/` directory.
+* `ufo`: Glyphs sources can be converted to UFO, or to UFO zip (`.ufoz`) format with the flag `--save-ufo-as-zip`. Placed in the `master_ufo/` directory. 
 
 If no format option is specified, the default is `-o otf ttf`.
 
 ### Other important command line options
 
 * `-i` (Interpolate instances): Having per-master binaries is not always what you expect; if you have defined instances ("exports") in your Glyphs file, they will *not* be generated by default. To generate them, pass the `-i` flag, which interpolates static instances, and places them in the `instance_ttf/` or `instance_otf/` directory as appropriate.
```

## Comparing `fontmake-3.5.1/Lib/fontmake.egg-info/SOURCES.txt` & `fontmake-3.6.0/Lib/fontmake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
 tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
 tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
 tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
 tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
 tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
 tests/data/DesignspaceTest/DesignspaceTest.designspace
+tests/data/DesignspaceTest/MyFont-Bold.ufoz
+tests/data/DesignspaceTest/MyFont-Light.ufoz
 tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
 tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
 tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
 tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
 tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
 tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
 tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
@@ -158,14 +160,15 @@
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
 tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
 tests/data/MutatorSans/LICENSE
+tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
 tests/data/MutatorSans/MutatorSans-weight-only.designspace
 tests/data/MutatorSans/MutatorSans-width-only.designspace
 tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
 tests/data/MutatorSans/MutatorSans.designspace
 tests/data/MutatorSans/MutatorSans_missing.designspace
 tests/data/MutatorSans/MutatorSans_no_default.designspace
 tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
```

## Comparing `fontmake-3.5.1/tests/test_instantiator.py` & `fontmake-3.6.0/tests/test_instantiator.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,14 +416,26 @@
     assert instance_font.info.styleName == "Light ASDF"
     assert instance_font["l"].width == 160
     instance_font = generator.generate_instance(designspace.instances[1])
     assert instance_font.info.styleName == "Bold ASDF"
     assert instance_font["l"].width == 280
 
 
+def test_non_default_layer(data_dir, caplog):
+    designspace = designspaceLib.DesignSpaceDocument.fromfile(
+        data_dir / "MutatorSans" / "MutatorSans-non-default-layer.designspace"
+    )
+    designspace.loadSourceFonts(ufoLib2.Font.open)
+    generator = fontmake.instantiator.Instantiator.from_designspace(
+        designspace, round_geometry=True
+    )
+    instance_font = generator.generate_instance(designspace.instances[0])
+    assert {g.name for g in instance_font} == {"A", "S", "W"}
+
+
 def test_instance_attributes(data_dir):
     designspace = designspaceLib.DesignSpaceDocument.fromfile(
         data_dir / "DesignspaceTest" / "DesignspaceTest-instance-attrs.designspace"
     )
     generator = fontmake.instantiator.Instantiator.from_designspace(
         designspace, round_geometry=True
     )
```

## Comparing `fontmake-3.5.1/tests/test_main.py` & `fontmake-3.6.0/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,14 +705,29 @@
             str(tmp_path),
         ]
     )
 
     assert {p.name for p in tmp_path.glob("*.otf")} == {"MyFont-Light.otf"}
 
 
+def test_ufoz_to_static_otf_cff2(data_dir, tmp_path):
+    fontmake.__main__.main(
+        [
+            "-u",
+            str(data_dir / "DesignspaceTest" / "MyFont-Light.ufoz"),
+            "-o",
+            "otf-cff2",
+            "--output-dir",
+            str(tmp_path),
+        ]
+    )
+
+    assert {p.name for p in tmp_path.glob("*.otf")} == {"MyFont-Light.otf"}
+
+
 def test_static_otf_cffsubr_subroutinizer(data_dir, tmp_path):
     fontmake.__main__.main(
         [
             "-u",
             str(data_dir / "DesignspaceTest" / "MyFont-Light.ufo"),
             "-o",
             "otf",
```

## Comparing `fontmake-3.5.1/tests/test_compatibility.py` & `fontmake-3.6.0/tests/test_compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/TestSubset.glyphs` & `fontmake-3.6.0/tests/data/TestSubset.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/TestSubset2.glyphs` & `fontmake-3.6.0/tests/data/TestSubset2.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans.glyphs` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace` & `fontmake-3.6.0/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-width-only.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-width-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_missing.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_missing.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/LICENSE` & `fontmake-3.6.0/tests/data/MutatorSansLite/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans_no_default.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans_no_default.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSans-weight-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/AutohintingTest/Padyakke.glyphs` & `fontmake-3.6.0/tests/data/AutohintingTest/Padyakke.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif` & `fontmake-3.6.0/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans.designspace` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif` & `fontmake-3.6.0/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest.designspace` & `fontmake-3.6.0/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace` & `fontmake-3.6.0/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs` & `fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist` & `fontmake-3.6.0/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont.designspace` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.6.0/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph` & `fontmake-3.6.0/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/LICENSE` & `fontmake-3.6.0/tests/data/MutatorSans/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.6.0/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist` & `fontmake-3.6.0/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif` & `fontmake-3.6.0/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.5.1/.github/workflows/ci.yml` & `fontmake-3.6.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     # https://github.community/t/github-actions-does-not-respect-skip-ci/17325/8
     if: "! contains(toJSON(github.event.commits.*.message), '[skip ci]')"
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.x"
     - name: Install dependencies
       run: pip install tox
     - name: Run style and static checks
       run: tox -e lint
   test:
     runs-on: ${{ matrix.platform }}
     if: "! contains(toJSON(github.event.commits.*.message), '[skip ci]')"
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, "3.10", "pypy-3.7"]
+        python-version: [3.8, 3.9, "3.10", "3.11", "pypy-3.9"]
         platform: [ubuntu-latest, windows-latest]
         exclude:
           - platform: windows-latest
-            python-version: "pypy-3.7"
+            python-version: "pypy-3.9"
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: pip install tox
     - name: Test with tox
       run: tox -e py
     - name: Produce coverage files
@@ -58,20 +58,20 @@
     if: startsWith(github.ref, 'refs/tags/v')
     # ... and both the lint and test jobs completed successfully
     needs:
       - lint
       - test
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         # setuptools_scm requires the git clone to not be 'shallow'
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.x"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Extract release notes from annotated tag message
```

