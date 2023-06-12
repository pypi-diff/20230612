# Comparing `tmp/pipen_board-0.5.1.tar.gz` & `tmp/pipen_board-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.5.1.tar", max compression
+gzip compressed data, was "pipen_board-0.5.2.tar", max compression
```

## Comparing `pipen_board-0.5.1.tar` & `pipen_board-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6281 2023-06-11 08:14:30.402279 pipen_board-0.5.1/README.md
--rw-r--r--   0        0        0      268 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/__init__.py
--rw-r--r--   0        0        0     8985 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/apis.py
--rw-r--r--   0        0        0     4367 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/cli.py
--rw-r--r--   0        0        0    26842 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/data_manager.py
--rw-r--r--   0        0        0     6243 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-06-11 08:14:30.402279 pipen_board-0.5.1/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   625559 2023-06-11 08:14:30.406279 pipen_board-0.5.1/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   752853 2023-06-11 08:14:30.414279 pipen_board-0.5.1/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-06-11 08:14:30.414279 pipen_board-0.5.1/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-06-11 08:14:30.414279 pipen_board-0.5.1/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7562 2023-06-11 08:14:30.418279 pipen_board-0.5.1/pipen_board/plugin.py
--rw-r--r--   0        0        0     3974 2023-06-11 08:14:30.418279 pipen_board-0.5.1/pipen_board/quart_app.py
--rw-r--r--   0        0        0       22 2023-06-11 08:14:30.418279 pipen_board-0.5.1/pipen_board/version.py
--rw-r--r--   0        0        0      732 2023-06-11 08:14:30.418279 pipen_board-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 pipen_board-0.5.1/setup.py
--rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 pipen_board-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6281 2023-06-12 20:30:22.676940 pipen_board-0.5.2/README.md
+-rw-r--r--   0        0        0      268 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/__init__.py
+-rw-r--r--   0        0        0     8985 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/apis.py
+-rw-r--r--   0        0        0     4367 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/cli.py
+-rw-r--r--   0        0        0    28609 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     6243 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-06-12 20:30:22.676940 pipen_board-0.5.2/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   625559 2023-06-12 20:30:22.680940 pipen_board-0.5.2/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   753061 2023-06-12 20:30:22.684940 pipen_board-0.5.2/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-06-12 20:30:22.684940 pipen_board-0.5.2/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-06-12 20:30:22.684940 pipen_board-0.5.2/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7562 2023-06-12 20:30:22.688940 pipen_board-0.5.2/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3974 2023-06-12 20:30:22.688940 pipen_board-0.5.2/pipen_board/quart_app.py
+-rw-r--r--   0        0        0       22 2023-06-12 20:30:22.688940 pipen_board-0.5.2/pipen_board/version.py
+-rw-r--r--   0        0        0      732 2023-06-12 20:30:22.688940 pipen_board-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 pipen_board-0.5.2/setup.py
+-rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 pipen_board-0.5.2/PKG-INFO
```

### Comparing `pipen_board-0.5.1/README.md` & `pipen_board-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/apis.py` & `pipen_board-0.5.2/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/cli.py` & `pipen_board-0.5.2/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/data_manager.py` & `pipen_board-0.5.2/pipen_board/data_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,29 +148,29 @@
         else:
             argspec[arg]["type"] = argspec[arg].pop("btype")
 
         t = argspec[arg].get("type")
         if t == "ns":
             argspec[arg]["value"] = _anno_to_argspec(arginfo.terms)
         elif t in ("choice", "mchoice"):
-            argspec[arg]["value"] = argspec[arg].pop("default", [])
+            argspec[arg]["value"] = argspec[arg].get("default", [])
             argspec[arg]["choices"] = list(arginfo.terms)
             argspec[arg]["choices_desc"] = [
                 term.help
                 if not term.help
                 else term.help.splitlines()[0]
                 for term in arginfo.terms.values()
             ]
             argspec[arg]["desc"] += "\n"
             # Add the choices to the description
             for termname, term in arginfo.terms.items():
                 h = re.sub(r"([\.\?!:])\s*\n", "\\1<br />\n", term.help)
                 argspec[arg]["desc"] += f"- `{termname}`: {h}\n"
         else:
-            argspec[arg]["value"] = argspec[arg].pop("default", None)
+            argspec[arg]["value"] = argspec[arg].get("default", None)
 
         # determine the itype for list elements
         if t == "list":
             if argspec[arg]["value"] is not None and not isinstance(
                 argspec[arg]["value"], list
             ):
                 argspec[arg]["value"] = [argspec[arg]["value"]]
@@ -182,17 +182,48 @@
                 and not isinstance(argspec[arg]["value"][0], str)
             ):
                 argspec[arg]["itype"] = type(argspec[arg]["value"][0]).__name__
 
             if "bitype" in argspec[arg]:
                 argspec[arg]["itype"] = argspec[arg].pop("bitype")
 
+    # argspec.setdefault("default", argspec.get("value", None))
     return argspec
 
 
+def _get_default(argspec: Mapping[str, Any], force_ns: bool = False) -> Any:
+    """Set the default using the value for the argspec
+
+    This can be used to omit the argument in final config in frontend
+    in case the value is the same as the default
+    """
+    value = argspec.get("value", None)
+    if not force_ns and argspec.get("type") not in ("ns", "namespace"):
+        argspec.setdefault("default", value)
+        return argspec["default"]
+
+    # flatten the namespace
+    if value is None:
+        argspec.setdefault("default", {})
+        return argspec["default"]
+
+    default = {}
+    for arg, arginfo in value.items():
+        # placeholder
+        if arg.startswith("<") and arg.endswith(">"):
+            continue
+
+        # Set the default for sub-item
+        dlt = _get_default(arginfo)
+        default[arg] = dlt
+
+    argspec.setdefault("default", default)
+    return default
+
+
 def _proc_to_argspec(
     proc: Proc | Type[Proc],
     is_start: bool,
     hidden: bool = False,
     order: int = 0,
 ) -> Mapping[str, Any]:
     """Convert the proc to the argument spec"""
@@ -219,28 +250,47 @@
             "required": True,
             "value": _anno_to_argspec(anno.get("Input", {})),
         }
     argspec["value"]["envs"] = {
         "desc": "Environment variables for the process, used across jobs",
         "value": _anno_to_argspec(anno.get("Envs", {})),
     }
+    _get_default(argspec["value"]["envs"], force_ns=True)
+
     argspec["value"]["plugin_opts"] = PIPELINE_OPTIONS["plugin_opts"]
+    _get_default(argspec["value"]["plugin_opts"], force_ns=True)
+
     argspec["value"]["scheduler_opts"] = PIPELINE_OPTIONS["scheduler_opts"]
+    _get_default(argspec["value"]["scheduler_opts"], force_ns=True)
+
     argspec["value"]["forks"] = PIPELINE_OPTIONS["forks"]
+    _get_default(argspec["value"]["forks"])
+
     argspec["value"]["cache"] = PIPELINE_OPTIONS["cache"]
+    _get_default(argspec["value"]["cache"])
+
     argspec["value"]["scheduler"] = PIPELINE_OPTIONS["scheduler"]
+    _get_default(argspec["value"]["scheduler"])
+
     argspec["value"]["dirsig"] = PIPELINE_OPTIONS["dirsig"]
+    _get_default(argspec["value"]["dirsig"])
+
     argspec["value"]["error_strategy"] = PIPELINE_OPTIONS["error_strategy"]
+    _get_default(argspec["value"]["error_strategy"])
+
     argspec["value"]["num_retries"] = PIPELINE_OPTIONS["num_retries"]
+    _get_default(argspec["value"]["num_retries"])
+
     argspec["value"]["lang"] = {
         "desc": "The interpreter to run the script",
         "hidden": True,
         "placeholder": proc.lang,
         # Don't include it in the config file if not specified
         "value": None,
+        "default": None,
     }
 
     return argspec
 
 
 def _load_additional(additional: str, **kwargs) -> Mapping[str, Any]:
     """Load additional config files"""
@@ -285,15 +335,21 @@
     # kwargs passed, treat the file as a template
     additional = Path(additional)
     tpl = Liquid(additional, mode="wild", from_file=True)
     configfile = cache_dir.joinpath(
         f"{slugify(str(additional.resolve()))}.rendered{additional.suffix}"
     )
     configfile.write_text(tpl.render(**kwargs))
-    return Config.load(configfile)
+
+    out = Config.load(configfile)
+    if "ADDITIONAL_OPTIONS" in out:
+        for val in out["ADDITIONAL_OPTIONS"].values():
+            _get_default(val)
+
+    return out
 
 
 async def _get_config_data(args: Namespace) -> Mapping[str, Any]:
     """Get the pipeline data"""
     old_argv = sys.argv
     sys.argv = ["@pipen-board"] + args.pipeline_args
     logger.info(
@@ -345,14 +401,17 @@
     }
     data[SECTION_PIPELINE_OPTIONS]["outdir"] = {
         "desc": "The output directory of your pipeline",
         "placeholder": "./<name>-output",
         "type": "str",
         "value": None,
     }
+    for key, val in data[SECTION_PIPELINE_OPTIONS].items():
+        _get_default(val, key in ("plugin_opts", "scheduler_opts"))
+
     data[SECTION_PROCESSES] = {}
 
     if pipeline.config.plugin_opts.get("args_flatten") is True or (
         "args_flatten" not in pipeline.config.plugin_opts
         and len(pipeline.procs) == 1
     ):
         data[SECTION_PIPELINE_OPTIONS]["plugin_opts"]["value"][
@@ -361,14 +420,15 @@
             "desc": (
                 "Flatten the arguments of the pipeline. "
                 "For example, [envs] will ba treated as [<Process>.envs]. "
                 "Only works for single-process pipeline"
             ),
             "type": "bool",
             "value": True,
+            "default": True,
             "readonly": True,
         }
 
     pg_sec = {}
     for i, proc in enumerate(pipeline.procs):
         logger.info(
             "[bold][yellow]DBG[/yellow][/bold] Parsing process: %s ...",
```

### Comparing `pipen_board-0.5.1/pipen_board/defaults.py` & `pipen_board-0.5.2/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.5.2/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.5.2/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.5.2/pipen_board/frontend/build/assets/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4586,18 +4586,21 @@
 
 function updateConfig(t, e, n, r = !1, l = null) {
     if (n = n || {}, moreLikeOption(e)) return {
         ...t,
         ...Object.fromEntries(n.value ? n.value.filter(a => a[0] !== void 0 && a[0] !== null && a[0] !== "").map(a => [a[0], applyAtomicType(a[1], "auto")]) : [])
     };
     if ((n.type === "ns" || n.type === "namespace") && (r = !0), r) {
-        for (let a in n.value) t[e] = updateConfig(t[e] || {}, a, n.value[a], !1, l);
+        for (let a in n.value) {
+            const o = updateConfig(t[e] || {}, a, n.value[a], !1, l);
+            Object.keys(o).length !== 0 && (t[e] = o)
+        }
         return t
     }
-    return l && n.pgarg && get_pgvalue(l, n.pgarg === !0 ? e : n.pgarg) == n.value || n.value === void 0 || n.value === null ? t : {
+    return l && n.pgarg && get_pgvalue(l, n.pgarg === !0 ? e : n.pgarg) == n.value || n.value === void 0 || n.value === null || _equal(n.value, n.default) ? t : {
         ...t,
         [e]: n.value
     }
 }
 
 function finalizeConfig(t) {
     let e = {};
@@ -4609,15 +4612,18 @@
         for (let [o, u] of Object.entries(l.value || {})) a = updateConfig(a, o, u, o.endsWith("_opts") || o === "envs"), _equal(a[o], e[o]) && delete a[o];
         Object.keys(a).length > 0 && (n ? e = {
             ...e,
             ...a
         } : e[r] = a)
     }
     for (let [r, l] of Object.entries(t[SECTION_PROCGROUPS] || {})) {
-        for (let a in l.ARGUMENTS) e[r] = updateConfig(e[r] || {}, a, l.ARGUMENTS[a]);
+        for (let a in l.ARGUMENTS) {
+            const o = updateConfig(e[r] || {}, a, l.ARGUMENTS[a]);
+            Object.keys(o).length > 0 && (e[r] = o)
+        }
         for (let [a, o] of Object.entries(l.PROCESSES)) {
             let u = {};
             for (let [s, c] of Object.entries(o.value || {})) u = updateConfig(u, s, c, s.endsWith("_opts") || s === "envs", l.ARGUMENTS), _equal(u[s], e[s]) && delete u[s];
             Object.keys(u).length > 0 && (e[a] = u)
         }
     }
     return e
@@ -17923,15 +17929,15 @@
         b = "",
         y = a,
         E = a,
         S = [u];
     s && (S = ["required", ...S]);
     const T = C => {
         if (E == null && (C === "" || C === null || C === void 0) && !s) {
-            n(9, a = E), n(6, v = !1);
+            n(9, a = E), n(6, v = !1), g(`${c} / ${l}`);
             return
         }
         const W = validateData(C, S);
         n(6, v = W !== null), n(7, b = W), v ? d(`${c} / ${l}`, b) : g(`${c} / ${l}`)
     };
     onMount(() => {
         _ || T(y)
@@ -18858,15 +18864,15 @@
         v = !1,
         b = "",
         y = a,
         E = null;
     u && (m = ["required", ...m]);
     const S = C => {
         if (y == null && (C === "" || C === null || C === void 0) && !u) {
-            n(1, a = y), n(6, v = !1);
+            n(1, a = y), n(6, v = !1), d(`${s} / ${l}`);
             return
         }
         const W = validateData(C, m);
         n(6, v = W !== null), n(7, b = W), v ? _(`${s} / ${l}`, b) : d(`${s} / ${l}`), autoHeight(E)
     };
     onMount(() => {
         c || S(a)
@@ -20280,42 +20286,42 @@
     }
 }
 
 function create_field_slot$5(t) {
     let e, n, r, l, a;
 
     function o(c) {
-        t[18](c)
+        t[19](c)
     }
 
     function u(c) {
-        t[19](c)
+        t[20](c)
     }
     let s = {
         itemToString: t[10],
         size: "sm",
         titleText: t[1],
         hideLabel: !0,
         invalid: t[7],
         invalidText: t[8],
         label: "Select an option",
-        items: t[2].map(t[17])
+        items: t[2].map(t[18])
     };
     return t[5] !== void 0 && (s.selectedId = t[5]), t[6] !== void 0 && (s.ref = t[6]), n = new Dropdown$1({
         props: s
-    }), binding_callbacks.push(() => bind(n, "selectedId", o)), binding_callbacks.push(() => bind(n, "ref", u)), n.$on("select", t[20]), {
+    }), binding_callbacks.push(() => bind(n, "selectedId", o)), binding_callbacks.push(() => bind(n, "ref", u)), n.$on("select", t[21]), {
         c() {
             e = element("div"), create_component(n.$$.fragment), attr(e, "slot", "field")
         },
         m(c, _) {
             insert(c, e, _), mount_component(n, e, null), a = !0
         },
         p(c, _) {
             const d = {};
-            _ & 2 && (d.titleText = c[1]), _ & 128 && (d.invalid = c[7]), _ & 256 && (d.invalidText = c[8]), _ & 4 && (d.items = c[2].map(c[17])), !r && _ & 32 && (r = !0, d.selectedId = c[5], add_flush_callback(() => r = !1)), !l && _ & 64 && (l = !0, d.ref = c[6], add_flush_callback(() => l = !1)), n.$set(d)
+            _ & 2 && (d.titleText = c[1]), _ & 128 && (d.invalid = c[7]), _ & 256 && (d.invalidText = c[8]), _ & 4 && (d.items = c[2].map(c[18])), !r && _ & 32 && (r = !0, d.selectedId = c[5], add_flush_callback(() => r = !1)), !l && _ & 64 && (l = !0, d.ref = c[6], add_flush_callback(() => l = !1)), n.$set(d)
         },
         i(c) {
             a || (transition_in(n.$$.fragment, c), a = !0)
         },
         o(c) {
             transition_out(n.$$.fragment, c), a = !1
         },
@@ -20333,15 +20339,15 @@
                 field: [create_field_slot$5],
                 label: [create_label_slot$5]
             },
             $$scope: {
                 ctx: t
             }
         }
-    }), e.$on("mouseenter", t[21]), e.$on("mouseleave", t[22]), {
+    }), e.$on("mouseenter", t[22]), e.$on("mouseleave", t[23]), {
         c() {
             create_component(e.$$.fragment)
         },
         m(r, l) {
             mount_component(e, r, l), n = !0
         },
         p(r, [l]) {
@@ -20402,15 +20408,15 @@
         E = createEventDispatcher();
     const S = C => {
             const W = u ? u[C.id] : null;
             return W ? `${C.text}: ${W}` : C.text
         },
         T = C => {
             if (C !== -1 || !c) {
-                n(7, b = !1);
+                n(7, b = !1), removeError(`${s} / ${l}`);
                 return
             }
             const W = validateData(void 0, ["required"]);
             n(7, b = W !== null), n(8, y = W), b ? setError(`${s} / ${l}`, y) : removeError(`${s} / ${l}`)
         };
     onMount(() => {
         n(6, p.onfocus = () => {
@@ -20421,48 +20427,48 @@
     });
     const A = C => ({
         id: o.indexOf(C),
         text: C
     });
 
     function q(C) {
-        m = C, n(5, m), n(16, r), n(0, h), n(2, o), n(15, d), n(4, g), n(1, l)
+        m = C, n(5, m), n(17, r), n(0, h), n(2, o), n(16, d), n(4, g), n(1, l)
     }
 
     function P(C) {
         p = C, n(6, p)
     }
     const M = C => {
-        n(0, h = !0), _ && n(5, m = v)
+        n(0, h = !0), _ && n(5, m = v), T(m)
     };
 
     function D(C) {
         bubble.call(this, t, C)
     }
 
     function G(C) {
         bubble.call(this, t, C)
     }
     return t.$$set = C => {
-        "key" in C && n(1, l = C.key), "value" in C && n(11, a = C.value), "choices" in C && n(2, o = C.choices), "choicesDesc" in C && n(12, u = C.choicesDesc), "activeNavItem" in C && n(13, s = C.activeNavItem), "required" in C && n(14, c = C.required), "readonly" in C && n(3, _ = C.readonly), "pgargs" in C && n(15, d = C.pgargs), "pgargkey" in C && n(4, g = C.pgargkey), "changed" in C && n(0, h = C.changed)
+        "key" in C && n(1, l = C.key), "value" in C && n(12, a = C.value), "choices" in C && n(2, o = C.choices), "choicesDesc" in C && n(13, u = C.choicesDesc), "activeNavItem" in C && n(14, s = C.activeNavItem), "required" in C && n(15, c = C.required), "readonly" in C && n(3, _ = C.readonly), "pgargs" in C && n(16, d = C.pgargs), "pgargkey" in C && n(4, g = C.pgargkey), "changed" in C && n(0, h = C.changed)
     }, t.$$.update = () => {
-        t.$$.dirty & 32786 && n(16, r = get_pgvalue(d, g === !0 ? l : g)), t.$$.dirty & 65541 && r !== void 0 && !h && n(5, m = o.indexOf(r)), t.$$.dirty & 36 && n(11, a = o[m])
-    }, [h, l, o, _, g, m, p, b, y, v, S, a, u, s, c, d, r, A, q, P, M, D, G]
+        t.$$.dirty & 65554 && n(17, r = get_pgvalue(d, g === !0 ? l : g)), t.$$.dirty & 131077 && r !== void 0 && !h && n(5, m = o.indexOf(r)), t.$$.dirty & 36 && n(12, a = o[m])
+    }, [h, l, o, _, g, m, p, b, y, v, S, T, a, u, s, c, d, r, A, q, P, M, D, G]
 }
 class ChoiceOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$B, create_fragment$B, safe_not_equal, {
             key: 1,
-            value: 11,
+            value: 12,
             choices: 2,
-            choicesDesc: 12,
-            activeNavItem: 13,
-            required: 14,
+            choicesDesc: 13,
+            activeNavItem: 14,
+            required: 15,
             readonly: 3,
-            pgargs: 15,
+            pgargs: 16,
             pgargkey: 4,
             changed: 0
         })
     }
 }
 
 function create_fragment$A(t) {
@@ -23111,15 +23117,15 @@
         y = a,
         E = a,
         S = null;
     const T = j => j == null ? "" : typeof j == "string" ? j : JSON.stringify(j, null, 2);
     a && typeof a == "object" && (y = T(a)), u && (m = ["required", ...m]);
     const A = (j, U = !1) => {
         if (E == null && (j === "" || j === null || j === void 0) && !u) {
-            n(10, a = E), n(6, v = !1);
+            n(10, a = E), n(6, v = !1), d(`${c} / ${l}`);
             return
         }
         const Q = validateData(j, m);
         n(6, v = Q !== null), n(7, b = Q), v ? (_(`${c} / ${l}`, b), n(10, a = j)) : (d(`${c} / ${l}`), U || n(10, a = applyAtomicType(j, "auto"))), autoHeight(S)
     };
     onMount(() => {
         s || A(y, !0)
@@ -23639,15 +23645,15 @@
         b = "",
         y = a,
         E = a,
         S = null;
     a && typeof a == "object" && (y = JSON.stringify(a, null, 2)), u && (m = ["required", ...m]);
     const T = (W, j = !1) => {
         if (E == null && (W === "" || W === null || W === void 0) && !u) {
-            n(10, a = E), n(6, v = !1);
+            n(10, a = E), n(6, v = !1), d(`${s} / ${l}`);
             return
         }
         const U = validateData(W, m);
         n(6, v = U !== null), n(7, b = U), v ? (_(`${s} / ${l}`, b), n(10, a = W)) : (d(`${s} / ${l}`), j || n(10, a = JSON.parse(W))), autoHeight(S)
     };
     onMount(() => {
         c || T(y, !0)
```

### Comparing `pipen_board-0.5.1/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.5.2/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/plugin.py` & `pipen_board-0.5.2/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pipen_board/quart_app.py` & `pipen_board-0.5.2/pipen_board/quart_app.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.5.1/pyproject.toml` & `pipen_board-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.5.1"
+version = "0.5.2"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
```

### Comparing `pipen_board-0.5.1/setup.py` & `pipen_board-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': '# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        \'__main__\'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n## Describing arguments in docstring\n\n### Docstring schema\n\n```python\nclass ProcessOrProcessGroup:\n    """Short summary\n\n    Long description\n    Long description\n\n    Args:\n        arg1 (<metadata>): description\n            - subarg1 (<metadata>): description\n            - subarg2 (<metadata>): description\n        arg2 (<metadata>): description\n\n    <Other Sections>:\n        <content>\n    """\n```\n\nThe metadata can have multiple attributes, separated by semicolon (`;`). For example:\n\n```\narg1 (action=ns;required): description\n```\n\n### Marks\n\nYou can mark a process using `pipen.utils.mark(<mark>=<value>)` as a decorator to decorate a process. For example:\n\n```python\nfrom pipen import Proc\nfrom pipen.utils import mark\n\n@mark(board_config_no_input=True)\nclass MyProc(Proc):\n    pass\n```\n\nAvailable marks:\n\n- `board_config_no_input`: Whether to show the input section for the process in configuation page. Only affects the start processes. Default to `False`.\n- `board_config_hidden`: Whether to hide the process options in the configuration page. Note that the process is still visible in the process list. Default to `False`.\n\n### Metadata for arguments\n\n\n| Name     | Description | Allowed values |\n| -------- | ----------- | -------------- |\n| `action` | Like the `action` argument in [`argx`][2]*. | `store_true`, `store_false`, `ns`, `namespace`, `append`, `extend`, `clear_append`, `clear_extend` (other values are allowed but ignore, they may be effective for CLI use) |\n| `btype`  | Board type (option type specified directly). If specified, `action` will be ignored | `ns`, `choice`, `mchoice`, `array`, `list`, `json`, `int`, `float`, `bool`, `str`, `text`, `auto`* |\n| `type` | Fallback for `action` and `btype` | Same as `btype` |\n| `flag` | Fallback for `action=store_true` | No values needed |\n| `text`/`mline`/`mlines` | Shortcut for `btype=text` | No values needed |\n| `ns`/`namespace` | Shortcut for `btype=ns` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `array`/`list` | Shortcut for `btype=array`/`btype=list` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `order` | The order of the argument in the UI. | Any integer |\n| `readonly` | Whether the argument is readonly. | No values needed (True if specified, otherwise False) |\n| `required` | Whether the argument is required. | No values needed (True if specified, otherwise False) |\n| `placeholder` | The placeholder in the UI for the argument. | Any string |\n| `bitype` | The type of the elements in an array or list. | `int`, `float`, `bool`, `str`, `json`, `auto`* |\n| `itype` | Fallback for `bitype` | Same as `bitype` |\n\n- `argx*`: An argument parser for Python, compatible with `argparse`.\n- `auto*`: Automatically infer the type from a string value.\n  - Any of `True`, `TRUE`, `true`, `False`, `FALSE`, `false` will be inferred as a `bool` value.\n  - Any of `None`, `NONE`, `none`, `null`, `NULL` will be inferred as `None`.\n  - Any integers will be inferred as `int`.\n  - Any floats will be inferred as `float`.\n  - Try to parse the value as JSON. If succeed, the value will be inferred as `json`.\n  - Otherwise, the value will be inferred as `str`.\n\n### Types of options in the UI\n\nThe type of an option in the UI is determined by the `btype`, `action` or `type` metadata. If neither is specified, a `PlainText` will be used.\n\n- `BoolOption`: Shown as a switch\n- `TextOption`: Shown as a textarea (allow multiple lines)\n- `ChoiceOption`: Shown as a dropdown list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `MChoiceOption`: Shown as a multiple choice list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `JsonOption`: Shown as a textarea, but the value will be validated and parsed as JSON\n- `ArrayOption`: Shown as a tag input. Items can be added or removed.\n- `AutoOption`: Shown as a 1-row textarea, and the value will be parsed automatically\n- `PlainText`: Shown as a plain text. No validation or parsing will be performed.\n- `MoreLikeOption`: Show as a box with buttons to add or remove sub-options. It\'s usally used together with `ns` type. If there is a sub-option under the option in the docstring wrapped by `<...>`, it indicates that we may have more sub-options.\n\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://github.com/pwwang/argx\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.5.1/PKG-INFO` & `pipen_board-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.5.1
+Version: 0.5.2
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

