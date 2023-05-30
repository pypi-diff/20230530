# Comparing `tmp/dupechecker-0.0.0.tar.gz` & `tmp/dupechecker-0.1.0.tar.gz`

## Comparing `dupechecker-0.0.0.tar` & `dupechecker-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.0.0/docs/dupechecker.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.0.0/docs/index.html
--rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 dupechecker-0.0.0/docs/search.js
--rw-r--r--   0        0        0    97002 2020-02-02 00:00:00.000000 dupechecker-0.0.0/docs/dupechecker/dupechecker.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.0.0/src/dupechecker/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 dupechecker-0.0.0/src/dupechecker/dupechecker.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.0.0/README.md
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dupechecker-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 dupechecker-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/dupechecker.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/index.html
+-rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/search.js
+-rw-r--r--   0        0        0    99179 2020-02-02 00:00:00.000000 dupechecker-0.1.0/docs/dupechecker/dupechecker.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.1.0/src/dupechecker/__init__.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 dupechecker-0.1.0/src/dupechecker/dupechecker.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.1.0/README.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dupechecker-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 dupechecker-0.1.0/PKG-INFO
```

### Comparing `dupechecker-0.0.0/docs/dupechecker.html` & `dupechecker-0.1.0/docs/dupechecker.html`

 * *Files identical despite different names*

### Comparing `dupechecker-0.0.0/docs/search.js` & `dupechecker-0.1.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `dupechecker-0.0.0/docs/dupechecker/dupechecker.html` & `dupechecker-0.1.0/docs/dupechecker/dupechecker.html`

 * *Files 2% similar despite different names*

```diff
@@ -138,64 +138,68 @@
 </span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
 </span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
 </span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>
 </span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="p">)</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot; | &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">)&lt;-&gt;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">prompt</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="p">)</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="p">]</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="p">)</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="p">]</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_duplicates">
                             <input id="get_duplicates-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -303,24 +307,27 @@
 
                 <label class="view-source-button" for="delete_wizard-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_wizard"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-76"><a href="#delete_wizard-76"><span class="linenos">76</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
 </span><span id="delete_wizard-77"><a href="#delete_wizard-77"><span class="linenos">77</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="delete_wizard-78"><a href="#delete_wizard-78"><span class="linenos">78</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-79"><a href="#delete_wizard-79"><span class="linenos">79</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="delete_wizard-80"><a href="#delete_wizard-80"><span class="linenos">80</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="delete_wizard-81"><a href="#delete_wizard-81"><span class="linenos">81</span></a>    <span class="p">)</span>
-</span><span id="delete_wizard-82"><a href="#delete_wizard-82"><span class="linenos">82</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="delete_wizard-83"><a href="#delete_wizard-83"><span class="linenos">83</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="delete_wizard-84"><a href="#delete_wizard-84"><span class="linenos">84</span></a>        <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot; | &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">)&lt;-&gt;</span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span>
-</span><span id="delete_wizard-85"><a href="#delete_wizard-85"><span class="linenos">85</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">prompt</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-86"><a href="#delete_wizard-86"><span class="linenos">86</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="delete_wizard-87"><a href="#delete_wizard-87"><span class="linenos">87</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="delete_wizard-78"><a href="#delete_wizard-78"><span class="linenos">78</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-79"><a href="#delete_wizard-79"><span class="linenos">79</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-80"><a href="#delete_wizard-80"><span class="linenos">80</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="delete_wizard-81"><a href="#delete_wizard-81"><span class="linenos">81</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="delete_wizard-82"><a href="#delete_wizard-82"><span class="linenos">82</span></a>    <span class="p">)</span>
+</span><span id="delete_wizard-83"><a href="#delete_wizard-83"><span class="linenos">83</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-84"><a href="#delete_wizard-84"><span class="linenos">84</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="delete_wizard-85"><a href="#delete_wizard-85"><span class="linenos">85</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="delete_wizard-86"><a href="#delete_wizard-86"><span class="linenos">86</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="delete_wizard-87"><a href="#delete_wizard-87"><span class="linenos">87</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="delete_wizard-88"><a href="#delete_wizard-88"><span class="linenos">88</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-89"><a href="#delete_wizard-89"><span class="linenos">89</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="delete_wizard-90"><a href="#delete_wizard-90"><span class="linenos">90</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Ask which file to keep for each set.</p>
 </div>
 
 
@@ -332,19 +339,19 @@
         <span class="def">def</span>
         <span class="name">autodelete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="autodelete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#autodelete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-90"><a href="#autodelete-90"><span class="linenos">90</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="autodelete-91"><a href="#autodelete-91"><span class="linenos">91</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="autodelete-92"><a href="#autodelete-92"><span class="linenos">92</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="autodelete-93"><a href="#autodelete-93"><span class="linenos">93</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="autodelete-94"><a href="#autodelete-94"><span class="linenos">94</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-93"><a href="#autodelete-93"><span class="linenos">93</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="autodelete-94"><a href="#autodelete-94"><span class="linenos">94</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="autodelete-95"><a href="#autodelete-95"><span class="linenos">95</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="autodelete-96"><a href="#autodelete-96"><span class="linenos">96</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="autodelete-97"><a href="#autodelete-97"><span class="linenos">97</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Keep one of each set in <code>matches</code> and delete the others.</p>
 </div>
 
 
@@ -356,41 +363,42 @@
         <span class="def">def</span>
         <span class="name">dupechecker</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="dupechecker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#dupechecker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-97"><a href="#dupechecker-97"><span class="linenos"> 97</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="dupechecker-98"><a href="#dupechecker-98"><span class="linenos"> 98</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="dupechecker-99"><a href="#dupechecker-99"><span class="linenos"> 99</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="dupechecker-100"><a href="#dupechecker-100"><span class="linenos">100</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="dupechecker-101"><a href="#dupechecker-101"><span class="linenos">101</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="dupechecker-102"><a href="#dupechecker-102"><span class="linenos">102</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="dupechecker-103"><a href="#dupechecker-103"><span class="linenos">103</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="dupechecker-104"><a href="#dupechecker-104"><span class="linenos">104</span></a>    <span class="p">]</span>
-</span><span id="dupechecker-105"><a href="#dupechecker-105"><span class="linenos">105</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="dupechecker-106"><a href="#dupechecker-106"><span class="linenos">106</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="dupechecker-107"><a href="#dupechecker-107"><span class="linenos">107</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="dupechecker-108"><a href="#dupechecker-108"><span class="linenos">108</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
-</span><span id="dupechecker-109"><a href="#dupechecker-109"><span class="linenos">109</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="dupechecker-110"><a href="#dupechecker-110"><span class="linenos">110</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="dupechecker-111"><a href="#dupechecker-111"><span class="linenos">111</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="dupechecker-112"><a href="#dupechecker-112"><span class="linenos">112</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="dupechecker-113"><a href="#dupechecker-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="dupechecker-114"><a href="#dupechecker-114"><span class="linenos">114</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-115"><a href="#dupechecker-115"><span class="linenos">115</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="dupechecker-116"><a href="#dupechecker-116"><span class="linenos">116</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
-</span><span id="dupechecker-117"><a href="#dupechecker-117"><span class="linenos">117</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="dupechecker-118"><a href="#dupechecker-118"><span class="linenos">118</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-119"><a href="#dupechecker-119"><span class="linenos">119</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="dupechecker-120"><a href="#dupechecker-120"><span class="linenos">120</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-121"><a href="#dupechecker-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-122"><a href="#dupechecker-122"><span class="linenos">122</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-100"><a href="#dupechecker-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="dupechecker-101"><a href="#dupechecker-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="dupechecker-102"><a href="#dupechecker-102"><span class="linenos">102</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="dupechecker-103"><a href="#dupechecker-103"><span class="linenos">103</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="dupechecker-104"><a href="#dupechecker-104"><span class="linenos">104</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="dupechecker-105"><a href="#dupechecker-105"><span class="linenos">105</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="dupechecker-106"><a href="#dupechecker-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
+</span><span id="dupechecker-107"><a href="#dupechecker-107"><span class="linenos">107</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
+</span><span id="dupechecker-108"><a href="#dupechecker-108"><span class="linenos">108</span></a>    <span class="p">]</span>
+</span><span id="dupechecker-109"><a href="#dupechecker-109"><span class="linenos">109</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="dupechecker-110"><a href="#dupechecker-110"><span class="linenos">110</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="dupechecker-111"><a href="#dupechecker-111"><span class="linenos">111</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="dupechecker-112"><a href="#dupechecker-112"><span class="linenos">112</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span><span class="p">)</span>
+</span><span id="dupechecker-113"><a href="#dupechecker-113"><span class="linenos">113</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
+</span><span id="dupechecker-114"><a href="#dupechecker-114"><span class="linenos">114</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="dupechecker-115"><a href="#dupechecker-115"><span class="linenos">115</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="dupechecker-116"><a href="#dupechecker-116"><span class="linenos">116</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
+</span><span id="dupechecker-117"><a href="#dupechecker-117"><span class="linenos">117</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="dupechecker-118"><a href="#dupechecker-118"><span class="linenos">118</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-119"><a href="#dupechecker-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="dupechecker-120"><a href="#dupechecker-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">matches</span><span class="p">))</span>
+</span><span id="dupechecker-121"><a href="#dupechecker-121"><span class="linenos">121</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="dupechecker-122"><a href="#dupechecker-122"><span class="linenos">122</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">size</span> <span class="o">-</span> <span class="n">args</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -91,66 +91,72 @@
 _70        args.path = Pathier(args.path)
 _71
 _72    return args
 _73
 _74
 _75def delete_wizard(matches: list[list[Pathier]]):
 _76    """Ask which file to keep for each set."""
-_77    print("Enter the corresponding number of the file to keep.")
-_78    print(
-_79        "Press 'Enter' without giving a number to skip deleting any files
+_77    print()
+_78    print("Enter the corresponding number of the file to keep.")
+_79    print(
+_80        "Press 'Enter' without giving a number to skip deleting any files
 for the given set."
-_80    )
-_81    for match in matches:
-_82        map_ = {str(i): file for i, file in enumerate(match, 1)}
-_83        prompt = " | ".join(f"({i})<->{file}" for i, file in map_.items())
-_84        keeper = input(prompt + " ")
-_85        if keeper:
-_86            [map_[num].delete() for num in map_ if num != keeper]
-_87
-_88
-_89def autodelete(matches: list[list[Pathier]]):
-_90    """Keep one of each set in `matches` and delete the others."""
-_91    for match in matches:
-_92        match.pop()
-_93        [file.delete() for file in match]
-_94
-_95
-_96def dupechecker(args: argparse.Namespace | None = None):
-_97    if not args:
-_98        args = get_args()
-_99    s = [
-100        ch.rjust(i + j)
-101        for i in range(1, 25, 3)
-102        for j, ch in enumerate(["/", "-", "\\"])
-103    ]
-104    s += s[::-1]
-105    with Spinner(s) as spinner:
-106        with ThreadPoolExecutor() as exc:
-107            thread = exc.submit(get_duplicates, args.path, args.recursive)
-108            while not thread.done():
-109                spinner.display()
-110                time.sleep(0.025)
-111            matches = thread.result()
-112    if matches:
-113        print(f"Found {len(matches)} duplicate sets of files.")
-114        if not args.no_show:
-115            print(griddy(matches))
-116        if args.delete_dupes or args.autodelete:
-117            size = args.path.size()
-118            delete_wizard(matches) if args.delete_dupes else autodelete
+_81    )
+_82    print()
+_83    for match in matches:
+_84        map_ = {str(i): file for i, file in enumerate(match, 1)}
+_85        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+"\n"
+_86        print(options)
+_87        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+())}): ")
+_88        if keeper:
+_89            [map_[num].delete() for num in map_ if num != keeper]
+_90
+_91
+_92def autodelete(matches: list[list[Pathier]]):
+_93    """Keep one of each set in `matches` and delete the others."""
+_94    for match in matches:
+_95        match.pop()
+_96        [file.delete() for file in match]
+_97
+_98
+_99def dupechecker(args: argparse.Namespace | None = None):
+100    print()
+101    if not args:
+102        args = get_args()
+103    s = [
+104        ch.rjust(i + j)
+105        for i in range(1, 25, 3)
+106        for j, ch in enumerate(["/", "-", "\\"])
+107    ]
+108    s += s[::-1]
+109    with Spinner(s) as spinner:
+110        with ThreadPoolExecutor() as exc:
+111            thread = exc.submit(get_duplicates, args.path, args.recursive)
+112            while not thread.done():
+113                spinner.display()
+114                time.sleep(0.025)
+115            matches = thread.result()
+116    if matches:
+117        print(f"Found {len(matches)} duplicate sets of files.")
+118        if not args.no_show:
+119            print(griddy(matches))
+120        if args.delete_dupes or args.autodelete:
+121            size = args.path.size()
+122            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-119            deleted_size = size - args.path.size()
-120            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-121    else:
-122        print("No duplicates detected.")
-123
-124
-125if __name__ == "__main__":
-126    dupechecker(get_args())
+123            deleted_size = size - args.path.size()
+124            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+125    else:
+126        print("No duplicates detected.")
+127
+128
+129if __name__ == "__main__":
+130    dupechecker(get_args())
   ⁰
 def get_duplicates(
 path: pathier.pathier.Pathier,
 recursive: bool = False) -> list[list[pathier.pathier.Pathier]]: View Source
 12def get_duplicates(path: Pathier, recursive: bool = False) -> list[list
 [Pathier]]:
 13    """Return a list of lists for duplicate files in `path`.
@@ -223,58 +229,64 @@
 71        args.path = Pathier(args.path)
 72
 73    return args
   ⁰
 def delete_wizard(matches: list[list[pathier.pathier.Pathier]]): View Source
 76def delete_wizard(matches: list[list[Pathier]]):
 77    """Ask which file to keep for each set."""
-78    print("Enter the corresponding number of the file to keep.")
-79    print(
-80        "Press 'Enter' without giving a number to skip deleting any files for
+78    print()
+79    print("Enter the corresponding number of the file to keep.")
+80    print(
+81        "Press 'Enter' without giving a number to skip deleting any files for
 the given set."
-81    )
-82    for match in matches:
-83        map_ = {str(i): file for i, file in enumerate(match, 1)}
-84        prompt = " | ".join(f"({i})<->{file}" for i, file in map_.items())
-85        keeper = input(prompt + " ")
-86        if keeper:
-87            [map_[num].delete() for num in map_ if num != keeper]
+82    )
+83    print()
+84    for match in matches:
+85        map_ = {str(i): file for i, file in enumerate(match, 1)}
+86        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+"\n"
+87        print(options)
+88        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+())}): ")
+89        if keeper:
+90            [map_[num].delete() for num in map_ if num != keeper]
 Ask which file to keep for each set.
   ⁰
 def autodelete(matches: list[list[pathier.pathier.Pathier]]): View Source
-90def autodelete(matches: list[list[Pathier]]):
-91    """Keep one of each set in `matches` and delete the others."""
-92    for match in matches:
-93        match.pop()
-94        [file.delete() for file in match]
+93def autodelete(matches: list[list[Pathier]]):
+94    """Keep one of each set in `matches` and delete the others."""
+95    for match in matches:
+96        match.pop()
+97        [file.delete() for file in match]
 Keep one of each set in matches and delete the others.
   ⁰
 def dupechecker(args: argparse.Namespace | None = None): View Source
-_97def dupechecker(args: argparse.Namespace | None = None):
-_98    if not args:
-_99        args = get_args()
-100    s = [
-101        ch.rjust(i + j)
-102        for i in range(1, 25, 3)
-103        for j, ch in enumerate(["/", "-", "\\"])
-104    ]
-105    s += s[::-1]
-106    with Spinner(s) as spinner:
-107        with ThreadPoolExecutor() as exc:
-108            thread = exc.submit(get_duplicates, args.path, args.recursive)
-109            while not thread.done():
-110                spinner.display()
-111                time.sleep(0.025)
-112            matches = thread.result()
-113    if matches:
-114        print(f"Found {len(matches)} duplicate sets of files.")
-115        if not args.no_show:
-116            print(griddy(matches))
-117        if args.delete_dupes or args.autodelete:
-118            size = args.path.size()
-119            delete_wizard(matches) if args.delete_dupes else autodelete
+100def dupechecker(args: argparse.Namespace | None = None):
+101    print()
+102    if not args:
+103        args = get_args()
+104    s = [
+105        ch.rjust(i + j)
+106        for i in range(1, 25, 3)
+107        for j, ch in enumerate(["/", "-", "\\"])
+108    ]
+109    s += s[::-1]
+110    with Spinner(s) as spinner:
+111        with ThreadPoolExecutor() as exc:
+112            thread = exc.submit(get_duplicates, args.path, args.recursive)
+113            while not thread.done():
+114                spinner.display()
+115                time.sleep(0.025)
+116            matches = thread.result()
+117    if matches:
+118        print(f"Found {len(matches)} duplicate sets of files.")
+119        if not args.no_show:
+120            print(griddy(matches))
+121        if args.delete_dupes or args.autodelete:
+122            size = args.path.size()
+123            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-120            deleted_size = size - args.path.size()
-121            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-122    else:
-123        print("No duplicates detected.")
+124            deleted_size = size - args.path.size()
+125            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+126    else:
+127        print("No duplicates detected.")
```

### Comparing `dupechecker-0.0.0/src/dupechecker/dupechecker.py` & `dupechecker-0.1.0/src/dupechecker/dupechecker.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,34 +70,38 @@
         args.path = Pathier(args.path)
 
     return args
 
 
 def delete_wizard(matches: list[list[Pathier]]):
     """Ask which file to keep for each set."""
+    print()
     print("Enter the corresponding number of the file to keep.")
     print(
         "Press 'Enter' without giving a number to skip deleting any files for the given set."
     )
+    print()
     for match in matches:
         map_ = {str(i): file for i, file in enumerate(match, 1)}
-        prompt = " | ".join(f"({i})<->{file}" for i, file in map_.items())
-        keeper = input(prompt + " ")
+        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) + "\n"
+        print(options)
+        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys())}): ")
         if keeper:
             [map_[num].delete() for num in map_ if num != keeper]
 
 
 def autodelete(matches: list[list[Pathier]]):
     """Keep one of each set in `matches` and delete the others."""
     for match in matches:
         match.pop()
         [file.delete() for file in match]
 
 
 def dupechecker(args: argparse.Namespace | None = None):
+    print()
     if not args:
         args = get_args()
     s = [
         ch.rjust(i + j)
         for i in range(1, 25, 3)
         for j, ch in enumerate(["/", "-", "\\"])
     ]
```

### Comparing `dupechecker-0.0.0/LICENSE.txt` & `dupechecker-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dupechecker-0.0.0/README.md` & `dupechecker-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dupechecker-0.0.0/pyproject.toml` & `dupechecker-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,71 +2,72 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6475 7065 6368 6563 6b65 7222 0d0a   "dupechecker"..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
-00000080: 6865 636b 2062 696e 6172 7920 636f 6e74  heck binary cont
-00000090: 656e 7420 6f66 2066 696c 6573 2061 6e64  ent of files and
-000000a0: 2063 6f6d 7061 7265 2066 6f72 2073 696d   compare for sim
-000000b0: 696c 6172 6974 7922 0d0a 7665 7273 696f  ilarity"..versio
-000000c0: 6e20 3d20 2230 2e30 2e30 220d 0a72 6571  n = "0.0.0"..req
-000000d0: 7569 7265 732d 7079 7468 6f6e 203d 2022  uires-python = "
-000000e0: 3e3d 332e 3130 220d 0a64 6570 656e 6465  >=3.10"..depende
-000000f0: 6e63 6965 7320 3d20 5b22 6772 6964 646c  ncies = ["griddl
-00000100: 6522 2c20 2270 6174 6869 6572 222c 2022  e", "pathier", "
-00000110: 7072 696e 7462 7564 6469 6573 222c 2022  printbuddies", "
-00000120: 7079 7465 7374 225d 0d0a 7265 6164 6d65  pytest"]..readme
-00000130: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
-00000140: 6b65 7977 6f72 6473 203d 205b 2264 6966  keywords = ["dif
-00000150: 666c 6962 222c 2022 636c 6922 2c20 2266  flib", "cli", "f
-00000160: 696c 6573 7973 7465 6d22 5d0d 0a63 6c61  ilesystem"]..cla
-00000170: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
-00000180: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001a0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
-000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001d0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
-000001e0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001f0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000200: 222c 0d0a 2020 2020 5d0d 0a0d 0a5b 5b70  ",..    ]....[[p
-00000210: 726f 6a65 6374 2e61 7574 686f 7273 5d5d  roject.authors]]
-00000220: 0d0a 6e61 6d65 203d 2022 4d61 7474 204d  ..name = "Matt M
-00000230: 616e 6573 220d 0a65 6d61 696c 203d 2022  anes"..email = "
-00000240: 6d61 7474 6d61 6e65 7340 706d 2e6d 6522  mattmanes@pm.me"
-00000250: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
-00000260: 735d 0d0a 2248 6f6d 6570 6167 6522 203d  s].."Homepage" =
-00000270: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000280: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
-00000290: 6475 7065 6368 6563 6b65 7222 0d0a 2244  dupechecker".."D
-000002a0: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
-000002b0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002c0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f64  com/matt-manes/d
-000002d0: 7570 6563 6865 636b 6572 2f74 7265 652f  upechecker/tree/
-000002e0: 6d61 696e 2f64 6f63 7322 0d0a 2253 6f75  main/docs".."Sou
-000002f0: 7263 6520 636f 6465 2220 3d20 2268 7474  rce code" = "htt
-00000300: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000310: 6d61 7474 2d6d 616e 6573 2f64 7570 6563  matt-manes/dupec
-00000320: 6865 636b 6572 2f74 7265 652f 6d61 696e  hecker/tree/main
-00000330: 2f73 7263 2f64 7570 6563 6865 636b 6572  /src/dupechecker
-00000340: 220d 0a0d 0a5b 746f 6f6c 2e70 7974 6573  "....[tool.pytes
-00000350: 742e 696e 695f 6f70 7469 6f6e 735d 0d0a  t.ini_options]..
-00000360: 6164 646f 7074 7320 3d20 5b0d 0a20 2020  addopts = [..   
-00000370: 2022 2d2d 696d 706f 7274 2d6d 6f64 653d   "--import-mode=
-00000380: 696d 706f 7274 6c69 6222 2c0d 0a20 2020  importlib",..   
-00000390: 205d 0d0a 7079 7468 6f6e 7061 7468 203d   ]..pythonpath =
-000003a0: 2022 7372 6322 0d0a 0d0a 5b74 6f6f 6c2e   "src"....[tool.
-000003b0: 6861 7463 682e 6275 696c 642e 7461 7267  hatch.build.targ
-000003c0: 6574 732e 7364 6973 745d 0d0a 6578 636c  ets.sdist]..excl
-000003d0: 7564 6520 3d20 5b0d 0a20 2020 2022 2e63  ude = [..    ".c
-000003e0: 6f76 6572 6167 6522 2c0d 0a20 2020 2022  overage",..    "
-000003f0: 2e70 7974 6573 745f 6361 6368 6522 2c0d  .pytest_cache",.
-00000400: 0a20 2020 2022 2e76 7363 6f64 6522 2c0d  .    ".vscode",.
-00000410: 0a20 2020 2022 7465 7374 7322 2c0d 0a20  .    "tests",.. 
-00000420: 2020 2022 2e67 6974 6967 6e6f 7265 220d     ".gitignore".
-00000430: 0a20 2020 205d 0d0a 5b70 726f 6a65 6374  .    ]..[project
-00000440: 2e73 6372 6970 7473 5d0d 0a64 7570 6563  .scripts]..dupec
-00000450: 6865 636b 6572 203d 2022 6475 7065 6368  hecker = "dupech
-00000460: 6563 6b65 722e 6475 7065 6368 6563 6b65  ecker.dupechecke
-00000470: 723a 6475 7065 6368 6563 6b65 7222 0d0a  r:dupechecker"..
+00000080: 6865 636b 2066 6f72 2061 6e64 2064 656c  heck for and del
+00000090: 6574 6520 6475 706c 6963 6174 6520 6669  ete duplicate fi
+000000a0: 6c65 7320 6672 6f6d 2074 6865 2063 6f6d  les from the com
+000000b0: 6d61 6e64 206c 696e 652e 220d 0a76 6572  mand line."..ver
+000000c0: 7369 6f6e 203d 2022 302e 312e 3022 0d0a  sion = "0.1.0"..
+000000d0: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
+000000e0: 3d20 223e 3d33 2e31 3022 0d0a 6465 7065  = ">=3.10"..depe
+000000f0: 6e64 656e 6369 6573 203d 205b 2267 7269  ndencies = ["gri
+00000100: 6464 6c65 222c 2022 7061 7468 6965 7222  ddle", "pathier"
+00000110: 2c20 2270 7269 6e74 6275 6464 6965 7322  , "printbuddies"
+00000120: 2c20 2270 7974 6573 7422 5d0d 0a72 6561  , "pytest"]..rea
+00000130: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
+00000140: 220d 0a6b 6579 776f 7264 7320 3d20 5b22  "..keywords = ["
+00000150: 6669 6c65 636d 7022 2c20 2263 6c69 222c  filecmp", "cli",
+00000160: 2022 6669 6c65 7379 7374 656d 225d 0d0a   "filesystem"]..
+00000170: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
+00000180: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
+00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001a0: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
+000001b0: 2022 4c69 6365 6e73 6520 3a3a 204f 5349   "License :: OSI
+000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001d0: 204c 6963 656e 7365 222c 0d0a 2020 2020   License",..    
+000001e0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
+000001f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000200: 656e 7422 2c0d 0a20 2020 205d 0d0a 0d0a  ent",..    ]....
+00000210: 5b5b 7072 6f6a 6563 742e 6175 7468 6f72  [[project.author
+00000220: 735d 5d0d 0a6e 616d 6520 3d20 224d 6174  s]]..name = "Mat
+00000230: 7420 4d61 6e65 7322 0d0a 656d 6169 6c20  t Manes"..email 
+00000240: 3d20 226d 6174 746d 616e 6573 4070 6d2e  = "mattmanes@pm.
+00000250: 6d65 220d 0a0d 0a5b 7072 6f6a 6563 742e  me"....[project.
+00000260: 7572 6c73 5d0d 0a22 486f 6d65 7061 6765  urls].."Homepage
+00000270: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
+00000280: 6875 622e 636f 6d2f 6d61 7474 2d6d 616e  hub.com/matt-man
+00000290: 6573 2f64 7570 6563 6865 636b 6572 220d  es/dupechecker".
+000002a0: 0a22 446f 6375 6d65 6e74 6174 696f 6e22  ."Documentation"
+000002b0: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+000002c0: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
+000002d0: 732f 6475 7065 6368 6563 6b65 722f 7472  s/dupechecker/tr
+000002e0: 6565 2f6d 6169 6e2f 646f 6373 220d 0a22  ee/main/docs".."
+000002f0: 536f 7572 6365 2063 6f64 6522 203d 2022  Source code" = "
+00000300: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000310: 6f6d 2f6d 6174 742d 6d61 6e65 732f 6475  om/matt-manes/du
+00000320: 7065 6368 6563 6b65 722f 7472 6565 2f6d  pechecker/tree/m
+00000330: 6169 6e2f 7372 632f 6475 7065 6368 6563  ain/src/dupechec
+00000340: 6b65 7222 0d0a 0d0a 5b74 6f6f 6c2e 7079  ker"....[tool.py
+00000350: 7465 7374 2e69 6e69 5f6f 7074 696f 6e73  test.ini_options
+00000360: 5d0d 0a61 6464 6f70 7473 203d 205b 0d0a  ]..addopts = [..
+00000370: 2020 2020 222d 2d69 6d70 6f72 742d 6d6f      "--import-mo
+00000380: 6465 3d69 6d70 6f72 746c 6962 222c 0d0a  de=importlib",..
+00000390: 2020 2020 5d0d 0a70 7974 686f 6e70 6174      ]..pythonpat
+000003a0: 6820 3d20 2273 7263 220d 0a0d 0a5b 746f  h = "src"....[to
+000003b0: 6f6c 2e68 6174 6368 2e62 7569 6c64 2e74  ol.hatch.build.t
+000003c0: 6172 6765 7473 2e73 6469 7374 5d0d 0a65  argets.sdist]..e
+000003d0: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
+000003e0: 222e 636f 7665 7261 6765 222c 0d0a 2020  ".coverage",..  
+000003f0: 2020 222e 7079 7465 7374 5f63 6163 6865    ".pytest_cache
+00000400: 222c 0d0a 2020 2020 222e 7673 636f 6465  ",..    ".vscode
+00000410: 222c 0d0a 2020 2020 2274 6573 7473 222c  ",..    "tests",
+00000420: 0d0a 2020 2020 222e 6769 7469 676e 6f72  ..    ".gitignor
+00000430: 6522 0d0a 2020 2020 5d0d 0a5b 7072 6f6a  e"..    ]..[proj
+00000440: 6563 742e 7363 7269 7074 735d 0d0a 6475  ect.scripts]..du
+00000450: 7065 6368 6563 6b65 7220 3d20 2264 7570  pechecker = "dup
+00000460: 6563 6865 636b 6572 2e64 7570 6563 6865  echecker.dupeche
+00000470: 636b 6572 3a64 7570 6563 6865 636b 6572  cker:dupechecker
+00000480: 220d 0a                                  "..
```

### Comparing `dupechecker-0.0.0/PKG-INFO` & `dupechecker-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dupechecker
-Version: 0.0.0
-Summary: Check binary content of files and compare for similarity
+Version: 0.1.0
+Summary: Check for and delete duplicate files from the command line.
 Project-URL: Homepage, https://github.com/matt-manes/dupechecker
 Project-URL: Documentation, https://github.com/matt-manes/dupechecker/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/dupechecker/tree/main/src/dupechecker
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
-Keywords: cli,difflib,filesystem
+Keywords: cli,filecmp,filesystem
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: griddle
 Requires-Dist: pathier
 Requires-Dist: printbuddies
```

