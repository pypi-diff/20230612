# Comparing `tmp/google_i18n_address-3.0.0.tar.gz` & `tmp/google_i18n_address-3.1.0.tar.gz`

## Comparing `google_i18n_address-3.0.0.tar` & `google_i18n_address-3.1.0.tar`

### file list

```diff
@@ -1,262 +1,262 @@
--rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/__init__.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/downloader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/scripts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ac.json
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ad.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ae.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/af.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ag.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ai.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/al.json
--rw-r--r--   0        0        0  1978328 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/all.json
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/am.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ao.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/aq.json
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ar.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/as.json
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/at.json
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/au.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/aw.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ax.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/az.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ba.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bb.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bd.json
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/be.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bf.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bg.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bh.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bi.json
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bj.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bl.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bm.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bn.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bo.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bq.json
--rw-r--r--   0        0        0   604459 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/br.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bs.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bt.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bv.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bw.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/by.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bz.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ca.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cc.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cd.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cf.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cg.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ch.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ci.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ck.json
--rw-r--r--   0        0        0    42698 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cl.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cm.json
--rw-r--r--   0        0        0   870883 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cn.json
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/co.json
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cr.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cu.json
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cv.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cw.json
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cx.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cy.json
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cz.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/de.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dj.json
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dk.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dm.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/do.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dz.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ec.json
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ee.json
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/eg.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/eh.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/er.json
--rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/es.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/et.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fi.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fj.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fk.json
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fm.json
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fo.json
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fr.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ga.json
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gb.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gd.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ge.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gf.json
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gg.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gh.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gi.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gl.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gm.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gn.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gp.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gq.json
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gr.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gs.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gt.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gu.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gw.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gy.json
--rw-r--r--   0        0        0    44334 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hk.json
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hm.json
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hn.json
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hr.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ht.json
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hu.json
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/id.json
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ie.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/il.json
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/im.json
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/in.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/io.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/iq.json
--rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ir.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/is.json
--rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/it.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/je.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jm.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jo.json
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jp.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ke.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kg.json
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kh.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ki.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/km.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kn.json
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kp.json
--rw-r--r--   0        0        0    56280 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kr.json
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kw.json
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ky.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kz.json
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/la.json
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lb.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lc.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/li.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lk.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lr.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ls.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lt.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lu.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lv.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ly.json
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ma.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mc.json
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/md.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/me.json
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mf.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mg.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mh.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mk.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ml.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mm.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mn.json
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mo.json
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mp.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mq.json
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mr.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ms.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mt.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mu.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mv.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mw.json
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mx.json
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/my.json
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mz.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/na.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nc.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ne.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nf.json
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ng.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ni.json
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nl.json
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/no.json
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/np.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nr.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nu.json
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nz.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/om.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pa.json
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pe.json
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pf.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pg.json
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ph.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pk.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pl.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pm.json
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pn.json
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pr.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ps.json
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pt.json
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pw.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/py.json
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/qa.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/re.json
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ro.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/rs.json
--rw-r--r--   0        0        0    33040 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ru.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/rw.json
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sa.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sb.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sc.json
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sd.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/se.json
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sg.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sh.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/si.json
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sj.json
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sk.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sl.json
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sm.json
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sn.json
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/so.json
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sr.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ss.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/st.json
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sv.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sx.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sy.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sz.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ta.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tc.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/td.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tf.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tg.json
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/th.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tj.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tk.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tl.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tm.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tn.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/to.json
--rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tr.json
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tt.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tv.json
--rw-r--r--   0        0        0    71130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tw.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tz.json
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ua.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ug.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/um.json
--rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/us.json
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/uy.json
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/uz.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/va.json
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vc.json
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ve.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vg.json
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vi.json
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vn.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vu.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/wf.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ws.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/xk.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ye.json
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/yt.json
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/za.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zm.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zw.json
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zz.json
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/.gitignore
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/LICENSE
--rw-r--r--   0        0        0    13625 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/README.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/__init__.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/downloader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/scripts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ac.json
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ad.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ae.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/af.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ag.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ai.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/al.json
+-rw-r--r--   0        0        0  1978328 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/all.json
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/am.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ao.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/aq.json
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ar.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/as.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/at.json
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/au.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/aw.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ax.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/az.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ba.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bb.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bd.json
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/be.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bf.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bg.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bh.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bi.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bj.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bl.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bm.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bn.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bo.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bq.json
+-rw-r--r--   0        0        0   604459 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/br.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bs.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bt.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bv.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bw.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/by.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/bz.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ca.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cc.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cd.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cf.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cg.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ch.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ci.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ck.json
+-rw-r--r--   0        0        0    42698 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cl.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cm.json
+-rw-r--r--   0        0        0   870883 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cn.json
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/co.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cr.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cu.json
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cv.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cw.json
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cx.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cy.json
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/cz.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/de.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/dj.json
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/dk.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/dm.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/do.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/dz.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ec.json
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ee.json
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/eg.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/eh.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/er.json
+-rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/es.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/et.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fi.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fj.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fk.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fm.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fo.json
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/fr.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ga.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gb.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gd.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ge.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gf.json
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gg.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gh.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gi.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gl.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gm.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gn.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gp.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gq.json
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gr.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gs.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gt.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gu.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gw.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/gy.json
+-rw-r--r--   0        0        0    44334 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/hk.json
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/hm.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/hn.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/hr.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ht.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/hu.json
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/id.json
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ie.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/il.json
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/im.json
+-rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/in.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/io.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/iq.json
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ir.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/is.json
+-rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/it.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/je.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/jm.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/jo.json
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/jp.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ke.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kg.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kh.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ki.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/km.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kn.json
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kp.json
+-rw-r--r--   0        0        0    56280 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kr.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kw.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ky.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/kz.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/la.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lb.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lc.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/li.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lk.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lr.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ls.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lt.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lu.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/lv.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ly.json
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ma.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mc.json
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/md.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/me.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mf.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mg.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mh.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mk.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ml.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mm.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mn.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mo.json
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mp.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mq.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mr.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ms.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mt.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mu.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mv.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mw.json
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mx.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/my.json
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/mz.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/na.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nc.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ne.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nf.json
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ng.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ni.json
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nl.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/no.json
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/np.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nr.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nu.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/nz.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/om.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pa.json
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pe.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pf.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pg.json
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ph.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pk.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pl.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pm.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pn.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pr.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ps.json
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pt.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/pw.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/py.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/qa.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/re.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ro.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/rs.json
+-rw-r--r--   0        0        0    33040 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ru.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/rw.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sa.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sb.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sc.json
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sd.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/se.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sg.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sh.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/si.json
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sj.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sk.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sl.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sm.json
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sn.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/so.json
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sr.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ss.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/st.json
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sv.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sx.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sy.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/sz.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ta.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tc.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/td.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tf.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tg.json
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/th.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tj.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tk.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tl.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tm.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tn.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/to.json
+-rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tr.json
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tt.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tv.json
+-rw-r--r--   0        0        0    71130 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tw.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/tz.json
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ua.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ug.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/um.json
+-rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/us.json
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/uy.json
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/uz.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/va.json
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/vc.json
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ve.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/vg.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/vi.json
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/vn.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/vu.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/wf.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ws.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/xk.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/ye.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/yt.json
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/za.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/zm.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/zw.json
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/i18naddress/data/zz.json
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/.gitignore
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/LICENSE
+-rw-r--r--   0        0        0    13625 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/README.rst
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 google_i18n_address-3.1.0/PKG-INFO
```

### Comparing `google_i18n_address-3.0.0/i18naddress/__init__.py` & `google_i18n_address-3.1.0/i18naddress/__init__.py`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/downloader.py` & `google_i18n_address-3.1.0/i18naddress/downloader.py`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/scripts.py` & `google_i18n_address-3.1.0/i18naddress/scripts.py`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ad.json` & `google_i18n_address-3.1.0/i18naddress/data/ad.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ae.json` & `google_i18n_address-3.1.0/i18naddress/data/ae.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/all.json` & `google_i18n_address-3.1.0/i18naddress/data/all.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/am.json` & `google_i18n_address-3.1.0/i18naddress/data/am.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ar.json` & `google_i18n_address-3.1.0/i18naddress/data/ar.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/au.json` & `google_i18n_address-3.1.0/i18naddress/data/au.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/br.json` & `google_i18n_address-3.1.0/i18naddress/data/br.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/bs.json` & `google_i18n_address-3.1.0/i18naddress/data/bs.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ca.json` & `google_i18n_address-3.1.0/i18naddress/data/ca.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/cl.json` & `google_i18n_address-3.1.0/i18naddress/data/cl.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/cn.json` & `google_i18n_address-3.1.0/i18naddress/data/cn.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/co.json` & `google_i18n_address-3.1.0/i18naddress/data/co.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/cu.json` & `google_i18n_address-3.1.0/i18naddress/data/cu.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/cv.json` & `google_i18n_address-3.1.0/i18naddress/data/cv.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/eg.json` & `google_i18n_address-3.1.0/i18naddress/data/eg.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/es.json` & `google_i18n_address-3.1.0/i18naddress/data/es.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/gb.json` & `google_i18n_address-3.1.0/i18naddress/data/gb.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/hk.json` & `google_i18n_address-3.1.0/i18naddress/data/hk.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/id.json` & `google_i18n_address-3.1.0/i18naddress/data/id.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ie.json` & `google_i18n_address-3.1.0/i18naddress/data/ie.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/in.json` & `google_i18n_address-3.1.0/i18naddress/data/in.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ir.json` & `google_i18n_address-3.1.0/i18naddress/data/ir.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/it.json` & `google_i18n_address-3.1.0/i18naddress/data/it.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/jm.json` & `google_i18n_address-3.1.0/i18naddress/data/jm.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/jp.json` & `google_i18n_address-3.1.0/i18naddress/data/jp.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/kp.json` & `google_i18n_address-3.1.0/i18naddress/data/kp.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/kr.json` & `google_i18n_address-3.1.0/i18naddress/data/kr.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ky.json` & `google_i18n_address-3.1.0/i18naddress/data/ky.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/mx.json` & `google_i18n_address-3.1.0/i18naddress/data/mx.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/my.json` & `google_i18n_address-3.1.0/i18naddress/data/my.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/mz.json` & `google_i18n_address-3.1.0/i18naddress/data/mz.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ng.json` & `google_i18n_address-3.1.0/i18naddress/data/ng.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ni.json` & `google_i18n_address-3.1.0/i18naddress/data/ni.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/nr.json` & `google_i18n_address-3.1.0/i18naddress/data/nr.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/pe.json` & `google_i18n_address-3.1.0/i18naddress/data/pe.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ph.json` & `google_i18n_address-3.1.0/i18naddress/data/ph.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ru.json` & `google_i18n_address-3.1.0/i18naddress/data/ru.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/so.json` & `google_i18n_address-3.1.0/i18naddress/data/so.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/sr.json` & `google_i18n_address-3.1.0/i18naddress/data/sr.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/sv.json` & `google_i18n_address-3.1.0/i18naddress/data/sv.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/th.json` & `google_i18n_address-3.1.0/i18naddress/data/th.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/tr.json` & `google_i18n_address-3.1.0/i18naddress/data/tr.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/tv.json` & `google_i18n_address-3.1.0/i18naddress/data/tv.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/tw.json` & `google_i18n_address-3.1.0/i18naddress/data/tw.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ua.json` & `google_i18n_address-3.1.0/i18naddress/data/ua.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/us.json` & `google_i18n_address-3.1.0/i18naddress/data/us.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/uy.json` & `google_i18n_address-3.1.0/i18naddress/data/uy.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/ve.json` & `google_i18n_address-3.1.0/i18naddress/data/ve.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/i18naddress/data/vn.json` & `google_i18n_address-3.1.0/i18naddress/data/vn.json`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/.gitignore` & `google_i18n_address-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/LICENSE` & `google_i18n_address-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/README.rst` & `google_i18n_address-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `google_i18n_address-3.0.0/pyproject.toml` & `google_i18n_address-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "google-i18n-address"
-version = "3.0.0"
+version = "3.1.0"
 readme = "README.rst"
 description = "Address validation helpers for Google's i18n address database"
 authors = [{ name = "Mirumee Software", email = "hello@mirumee.com" }]
 license = "BSD-3-Clause"
 dependencies = ["requests>=2.7.0"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -32,17 +32,14 @@
 update-validation-files = "i18naddress.scripts:download_json_files"
 
 [tool.hatch.build]
 exclude = ["tests"]
 include = [
   "i18naddress/**/*.py",
   "i18naddress/**/*.json",
-  "LICENSE",
-  "README.rst",
-  "pyproject.toml",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mirumee/google-i18n-address"
 "Repository" = "https://github.com/mirumee/google-i18n-address"
 "Bug Tracker" = "https://github.com/mirumee/google-i18n-address/issues"
```

### Comparing `google_i18n_address-3.0.0/PKG-INFO` & `google_i18n_address-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-i18n-address
-Version: 3.0.0
+Version: 3.1.0
 Summary: Address validation helpers for Google's i18n address database
 Project-URL: Homepage, https://github.com/mirumee/google-i18n-address
 Project-URL: Repository, https://github.com/mirumee/google-i18n-address
 Project-URL: Bug Tracker, https://github.com/mirumee/google-i18n-address/issues
 Author-email: Mirumee Software <hello@mirumee.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

