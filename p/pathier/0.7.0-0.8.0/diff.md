# Comparing `tmp/pathier-0.7.0.tar.gz` & `tmp/pathier-0.8.0.tar.gz`

## Comparing `pathier-0.7.0.tar` & `pathier-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pathier-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-0.7.0/docs/index.html
--rw-r--r--   0        0        0   225776 2020-02-02 00:00:00.000000 pathier-0.7.0/docs/pathier.html
--rw-r--r--   0        0        0    45759 2020-02-02 00:00:00.000000 pathier-0.7.0/docs/search.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pathier-0.7.0/src/pathier/__init__.py
--rw-r--r--   0        0        0    12933 2020-02-02 00:00:00.000000 pathier-0.7.0/src/pathier/pathier.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-0.7.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pathier-0.7.0/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pathier-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 pathier-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 pathier-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-0.8.0/docs/index.html
+-rw-r--r--   0        0        0   225780 2020-02-02 00:00:00.000000 pathier-0.8.0/docs/pathier.html
+-rw-r--r--   0        0        0    45759 2020-02-02 00:00:00.000000 pathier-0.8.0/docs/search.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pathier-0.8.0/src/pathier/__init__.py
+-rw-r--r--   0        0        0    12963 2020-02-02 00:00:00.000000 pathier-0.8.0/src/pathier/pathier.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pathier-0.8.0/README.md
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pathier-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pathier-0.8.0/PKG-INFO
```

### Comparing `pathier-0.7.0/CHANGELOG.md` & `pathier-0.8.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 # Changelog
 
-## 0.6.0 (2023-04-02)
+## 0.7.0 (2023-04-11)
+
+#### New Features
+
+* add remove_from_PATH and make in_PATH a property
+* add functions to add path to sys.path
+* add 'PathLike' reference for annotating types that can be Pathier, pathlib.Path, or str
+#### Others
+
+* update readme
+
+
+## v0.6.0 (2023-04-02)
 
 #### New Features
 
 * add mkcwd() method
 #### Others
 
+* build v0.6.0
+* update changelog
 * update readme
 
 
 ## v0.5.0 (2023-04-01)
 
 #### New Features
```

### Comparing `pathier-0.7.0/docs/pathier.html` & `pathier-0.8.0/docs/pathier.html`

 * *Files 0% similar despite different names*

```diff
@@ -154,355 +154,355 @@
     <span class="def">class</span>
     <span class="name">Pathier</span><wbr>(<span class="base">pathlib.Path</span>):
 
                 <label class="view-source-button" for="Pathier-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier-14"><a href="#Pathier-14"><span class="linenos"> 14</span></a><span class="k">class</span> <span class="nc">Pathier</span><span class="p">(</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
-</span><span id="Pathier-15"><a href="#Pathier-15"><span class="linenos"> 15</span></a>    <span class="sd">&quot;&quot;&quot;Subclasses the standard library pathlib.Path class.&quot;&quot;&quot;</span>
-</span><span id="Pathier-16"><a href="#Pathier-16"><span class="linenos"> 16</span></a>
-</span><span id="Pathier-17"><a href="#Pathier-17"><span class="linenos"> 17</span></a>    <span class="k">def</span> <span class="fm">__new__</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="Pathier-18"><a href="#Pathier-18"><span class="linenos"> 18</span></a>        <span class="k">if</span> <span class="bp">cls</span> <span class="ow">is</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="Pathier-19"><a href="#Pathier-19"><span class="linenos"> 19</span></a>            <span class="bp">cls</span> <span class="o">=</span> <span class="n">WindowsPath</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;nt&quot;</span> <span class="k">else</span> <span class="n">PosixPath</span>
-</span><span id="Pathier-20"><a href="#Pathier-20"><span class="linenos"> 20</span></a>        <span class="bp">self</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_from_parts</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Pathier-21"><a href="#Pathier-21"><span class="linenos"> 21</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_flavour</span><span class="o">.</span><span class="n">is_supported</span><span class="p">:</span>
-</span><span id="Pathier-22"><a href="#Pathier-22"><span class="linenos"> 22</span></a>            <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">(</span>
-</span><span id="Pathier-23"><a href="#Pathier-23"><span class="linenos"> 23</span></a>                <span class="s2">&quot;cannot instantiate </span><span class="si">%r</span><span class="s2"> on your system&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,)</span>
-</span><span id="Pathier-24"><a href="#Pathier-24"><span class="linenos"> 24</span></a>            <span class="p">)</span>
-</span><span id="Pathier-25"><a href="#Pathier-25"><span class="linenos"> 25</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="Pathier-26"><a href="#Pathier-26"><span class="linenos"> 26</span></a>
-</span><span id="Pathier-27"><a href="#Pathier-27"><span class="linenos"> 27</span></a>    <span class="c1"># ===============================================stats===============================================</span>
-</span><span id="Pathier-28"><a href="#Pathier-28"><span class="linenos"> 28</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-29"><a href="#Pathier-29"><span class="linenos"> 29</span></a>    <span class="k">def</span> <span class="nf">dob</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-30"><a href="#Pathier-30"><span class="linenos"> 30</span></a>        <span class="sd">&quot;&quot;&quot;Returns the creation date of this file</span>
-</span><span id="Pathier-31"><a href="#Pathier-31"><span class="linenos"> 31</span></a><span class="sd">        or directory as a dateime.datetime object.&quot;&quot;&quot;</span>
-</span><span id="Pathier-32"><a href="#Pathier-32"><span class="linenos"> 32</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-33"><a href="#Pathier-33"><span class="linenos"> 33</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_ctime</span><span class="p">)</span>
-</span><span id="Pathier-34"><a href="#Pathier-34"><span class="linenos"> 34</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-35"><a href="#Pathier-35"><span class="linenos"> 35</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-36"><a href="#Pathier-36"><span class="linenos"> 36</span></a>
-</span><span id="Pathier-37"><a href="#Pathier-37"><span class="linenos"> 37</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-38"><a href="#Pathier-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="nf">age</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-39"><a href="#Pathier-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;Returns the age in seconds of this file or directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-40"><a href="#Pathier-40"><span class="linenos"> 40</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-41"><a href="#Pathier-41"><span class="linenos"> 41</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Pathier-42"><a href="#Pathier-42"><span class="linenos"> 42</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-43"><a href="#Pathier-43"><span class="linenos"> 43</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-44"><a href="#Pathier-44"><span class="linenos"> 44</span></a>
-</span><span id="Pathier-45"><a href="#Pathier-45"><span class="linenos"> 45</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-46"><a href="#Pathier-46"><span class="linenos"> 46</span></a>    <span class="k">def</span> <span class="nf">mod_date</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-47"><a href="#Pathier-47"><span class="linenos"> 47</span></a>        <span class="sd">&quot;&quot;&quot;Returns the modification date of this file</span>
-</span><span id="Pathier-48"><a href="#Pathier-48"><span class="linenos"> 48</span></a><span class="sd">        or directory as a datetime.datetime object.&quot;&quot;&quot;</span>
-</span><span id="Pathier-49"><a href="#Pathier-49"><span class="linenos"> 49</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-50"><a href="#Pathier-50"><span class="linenos"> 50</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_mtime</span><span class="p">)</span>
-</span><span id="Pathier-51"><a href="#Pathier-51"><span class="linenos"> 51</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-52"><a href="#Pathier-52"><span class="linenos"> 52</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-53"><a href="#Pathier-53"><span class="linenos"> 53</span></a>
-</span><span id="Pathier-54"><a href="#Pathier-54"><span class="linenos"> 54</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-55"><a href="#Pathier-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">mod_delta</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-56"><a href="#Pathier-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Returns how long ago in seconds this file</span>
-</span><span id="Pathier-57"><a href="#Pathier-57"><span class="linenos"> 57</span></a><span class="sd">        or directory was modified.&quot;&quot;&quot;</span>
-</span><span id="Pathier-58"><a href="#Pathier-58"><span class="linenos"> 58</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-59"><a href="#Pathier-59"><span class="linenos"> 59</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Pathier-60"><a href="#Pathier-60"><span class="linenos"> 60</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-61"><a href="#Pathier-61"><span class="linenos"> 61</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-62"><a href="#Pathier-62"><span class="linenos"> 62</span></a>
-</span><span id="Pathier-63"><a href="#Pathier-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-64"><a href="#Pathier-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
-</span><span id="Pathier-65"><a href="#Pathier-65"><span class="linenos"> 65</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
-</span><span id="Pathier-66"><a href="#Pathier-66"><span class="linenos"> 66</span></a>
-</span><span id="Pathier-67"><a href="#Pathier-67"><span class="linenos"> 67</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Pathier-68"><a href="#Pathier-68"><span class="linenos"> 68</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-69"><a href="#Pathier-69"><span class="linenos"> 69</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-70"><a href="#Pathier-70"><span class="linenos"> 70</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-71"><a href="#Pathier-71"><span class="linenos"> 71</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
-</span><span id="Pathier-72"><a href="#Pathier-72"><span class="linenos"> 72</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-73"><a href="#Pathier-73"><span class="linenos"> 73</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="Pathier-74"><a href="#Pathier-74"><span class="linenos"> 74</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Pathier-75"><a href="#Pathier-75"><span class="linenos"> 75</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
-</span><span id="Pathier-76"><a href="#Pathier-76"><span class="linenos"> 76</span></a>        <span class="k">return</span> <span class="n">size</span>
-</span><span id="Pathier-77"><a href="#Pathier-77"><span class="linenos"> 77</span></a>
-</span><span id="Pathier-78"><a href="#Pathier-78"><span class="linenos"> 78</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier-79"><a href="#Pathier-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier-80"><a href="#Pathier-80"><span class="linenos"> 80</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
-</span><span id="Pathier-81"><a href="#Pathier-81"><span class="linenos"> 81</span></a><span class="sd">        and rounded to two decimal places.</span>
-</span><span id="Pathier-82"><a href="#Pathier-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-83"><a href="#Pathier-83"><span class="linenos"> 83</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier-84"><a href="#Pathier-84"><span class="linenos"> 84</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier-85"><a href="#Pathier-85"><span class="linenos"> 85</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier-86"><a href="#Pathier-86"><span class="linenos"> 86</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier-87"><a href="#Pathier-87"><span class="linenos"> 87</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier-88"><a href="#Pathier-88"><span class="linenos"> 88</span></a>
-</span><span id="Pathier-89"><a href="#Pathier-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-90"><a href="#Pathier-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
-</span><span id="Pathier-91"><a href="#Pathier-91"><span class="linenos"> 91</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-92"><a href="#Pathier-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="Pathier-93"><a href="#Pathier-93"><span class="linenos"> 93</span></a>
-</span><span id="Pathier-94"><a href="#Pathier-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-95"><a href="#Pathier-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
-</span><span id="Pathier-96"><a href="#Pathier-96"><span class="linenos"> 96</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-97"><a href="#Pathier-97"><span class="linenos"> 97</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
-</span><span id="Pathier-98"><a href="#Pathier-98"><span class="linenos"> 98</span></a>
-</span><span id="Pathier-99"><a href="#Pathier-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-100"><a href="#Pathier-100"><span class="linenos">100</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
-</span><span id="Pathier-101"><a href="#Pathier-101"><span class="linenos">101</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
-</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a>
-</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
-</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>
-</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>        <span class="sd">&quot;&quot;&quot;Return True if this</span>
-</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a><span class="sd">        path is in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
-</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a>
-</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
-</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a><span class="sd">        if it isn&#39;t already there.</span>
-</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a>
-</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a><span class="sd">        :param index: The index of sys.path</span>
-</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
-</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>
-</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
-</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier-128"><a href="#Pathier-128"><span class="linenos">128</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>
-</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-133"><a href="#Pathier-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
-</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
-</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a>
-</span><span id="Pathier-138"><a href="#Pathier-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
-</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier-143"><a href="#Pathier-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
-</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>
-</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object moved up &#39;levels&#39; number of parents from the current path.</span>
-</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
-</span><span id="Pathier-154"><a href="#Pathier-154"><span class="linenos">154</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
-</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
-</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
-</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a>        <span class="k">return</span> <span class="n">path</span>
-</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a>
-</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
-</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
-</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
-</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a>
-</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
-</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
-</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a>
-</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
-</span><span id="Pathier-178"><a href="#Pathier-178"><span class="linenos">178</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
-</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a>
-</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a>    <span class="c1"># ============================================write and read============================================</span>
-</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a><span class="sd">        Same as Path().mkdir() except</span>
-</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
-</span><span id="Pathier-194"><a href="#Pathier-194"><span class="linenos">194</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
-</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
-</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a>
-</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
-</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
-</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a>
-</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>    <span class="p">):</span>
-</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
-</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
-</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
-</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>        <span class="p">)</span>
-</span><span id="Pathier-220"><a href="#Pathier-220"><span class="linenos">220</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>
-</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>
-</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
-</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
-</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>
-</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
-</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>
-</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-268"><a href="#Pathier-268"><span class="linenos">268</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>        <span class="p">)</span>
-</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a>
-</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
-</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>
-</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-286"><a href="#Pathier-286"><span class="linenos">286</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a>    <span class="p">):</span>
-</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>        <span class="p">)</span>
-</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a>
-</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-294"><a href="#Pathier-294"><span class="linenos">294</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>
-</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier-302"><a href="#Pathier-302"><span class="linenos">302</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-307"><a href="#Pathier-307"><span class="linenos">307</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-309"><a href="#Pathier-309"><span class="linenos">309</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a>    <span class="p">):</span>
-</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a>                <span class="p">)</span>
-</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
-</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a>
-</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-325"><a href="#Pathier-325"><span class="linenos">325</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a>
-</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-332"><a href="#Pathier-332"><span class="linenos">332</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
-</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
-</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a>
-</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a><span class="sd">        :param new_path: The copy destination.</span>
-</span><span id="Pathier-337"><a href="#Pathier-337"><span class="linenos">337</span></a>
-</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
-</span><span id="Pathier-339"><a href="#Pathier-339"><span class="linenos">339</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
-</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-344"><a href="#Pathier-344"><span class="linenos">344</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>        <span class="k">return</span> <span class="n">new_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier-15"><a href="#Pathier-15"><span class="linenos"> 15</span></a><span class="k">class</span> <span class="nc">Pathier</span><span class="p">(</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">):</span>
+</span><span id="Pathier-16"><a href="#Pathier-16"><span class="linenos"> 16</span></a>    <span class="sd">&quot;&quot;&quot;Subclasses the standard library pathlib.Path class.&quot;&quot;&quot;</span>
+</span><span id="Pathier-17"><a href="#Pathier-17"><span class="linenos"> 17</span></a>
+</span><span id="Pathier-18"><a href="#Pathier-18"><span class="linenos"> 18</span></a>    <span class="k">def</span> <span class="fm">__new__</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="Pathier-19"><a href="#Pathier-19"><span class="linenos"> 19</span></a>        <span class="k">if</span> <span class="bp">cls</span> <span class="ow">is</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="Pathier-20"><a href="#Pathier-20"><span class="linenos"> 20</span></a>            <span class="bp">cls</span> <span class="o">=</span> <span class="n">WindowsPath</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;nt&quot;</span> <span class="k">else</span> <span class="n">PosixPath</span>
+</span><span id="Pathier-21"><a href="#Pathier-21"><span class="linenos"> 21</span></a>        <span class="bp">self</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">_from_parts</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Pathier-22"><a href="#Pathier-22"><span class="linenos"> 22</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_flavour</span><span class="o">.</span><span class="n">is_supported</span><span class="p">:</span>
+</span><span id="Pathier-23"><a href="#Pathier-23"><span class="linenos"> 23</span></a>            <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">(</span>
+</span><span id="Pathier-24"><a href="#Pathier-24"><span class="linenos"> 24</span></a>                <span class="s2">&quot;cannot instantiate </span><span class="si">%r</span><span class="s2"> on your system&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,)</span>
+</span><span id="Pathier-25"><a href="#Pathier-25"><span class="linenos"> 25</span></a>            <span class="p">)</span>
+</span><span id="Pathier-26"><a href="#Pathier-26"><span class="linenos"> 26</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Pathier-27"><a href="#Pathier-27"><span class="linenos"> 27</span></a>
+</span><span id="Pathier-28"><a href="#Pathier-28"><span class="linenos"> 28</span></a>    <span class="c1"># ===============================================stats===============================================</span>
+</span><span id="Pathier-29"><a href="#Pathier-29"><span class="linenos"> 29</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-30"><a href="#Pathier-30"><span class="linenos"> 30</span></a>    <span class="k">def</span> <span class="nf">dob</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-31"><a href="#Pathier-31"><span class="linenos"> 31</span></a>        <span class="sd">&quot;&quot;&quot;Returns the creation date of this file</span>
+</span><span id="Pathier-32"><a href="#Pathier-32"><span class="linenos"> 32</span></a><span class="sd">        or directory as a dateime.datetime object.&quot;&quot;&quot;</span>
+</span><span id="Pathier-33"><a href="#Pathier-33"><span class="linenos"> 33</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-34"><a href="#Pathier-34"><span class="linenos"> 34</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_ctime</span><span class="p">)</span>
+</span><span id="Pathier-35"><a href="#Pathier-35"><span class="linenos"> 35</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-36"><a href="#Pathier-36"><span class="linenos"> 36</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-37"><a href="#Pathier-37"><span class="linenos"> 37</span></a>
+</span><span id="Pathier-38"><a href="#Pathier-38"><span class="linenos"> 38</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-39"><a href="#Pathier-39"><span class="linenos"> 39</span></a>    <span class="k">def</span> <span class="nf">age</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-40"><a href="#Pathier-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;Returns the age in seconds of this file or directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-41"><a href="#Pathier-41"><span class="linenos"> 41</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-42"><a href="#Pathier-42"><span class="linenos"> 42</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
+</span><span id="Pathier-43"><a href="#Pathier-43"><span class="linenos"> 43</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-44"><a href="#Pathier-44"><span class="linenos"> 44</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-45"><a href="#Pathier-45"><span class="linenos"> 45</span></a>
+</span><span id="Pathier-46"><a href="#Pathier-46"><span class="linenos"> 46</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-47"><a href="#Pathier-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">mod_date</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-48"><a href="#Pathier-48"><span class="linenos"> 48</span></a>        <span class="sd">&quot;&quot;&quot;Returns the modification date of this file</span>
+</span><span id="Pathier-49"><a href="#Pathier-49"><span class="linenos"> 49</span></a><span class="sd">        or directory as a datetime.datetime object.&quot;&quot;&quot;</span>
+</span><span id="Pathier-50"><a href="#Pathier-50"><span class="linenos"> 50</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-51"><a href="#Pathier-51"><span class="linenos"> 51</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_mtime</span><span class="p">)</span>
+</span><span id="Pathier-52"><a href="#Pathier-52"><span class="linenos"> 52</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-53"><a href="#Pathier-53"><span class="linenos"> 53</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-54"><a href="#Pathier-54"><span class="linenos"> 54</span></a>
+</span><span id="Pathier-55"><a href="#Pathier-55"><span class="linenos"> 55</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-56"><a href="#Pathier-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="nf">mod_delta</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-57"><a href="#Pathier-57"><span class="linenos"> 57</span></a>        <span class="sd">&quot;&quot;&quot;Returns how long ago in seconds this file</span>
+</span><span id="Pathier-58"><a href="#Pathier-58"><span class="linenos"> 58</span></a><span class="sd">        or directory was modified.&quot;&quot;&quot;</span>
+</span><span id="Pathier-59"><a href="#Pathier-59"><span class="linenos"> 59</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-60"><a href="#Pathier-60"><span class="linenos"> 60</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
+</span><span id="Pathier-61"><a href="#Pathier-61"><span class="linenos"> 61</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-62"><a href="#Pathier-62"><span class="linenos"> 62</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-63"><a href="#Pathier-63"><span class="linenos"> 63</span></a>
+</span><span id="Pathier-64"><a href="#Pathier-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-65"><a href="#Pathier-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
+</span><span id="Pathier-66"><a href="#Pathier-66"><span class="linenos"> 66</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
+</span><span id="Pathier-67"><a href="#Pathier-67"><span class="linenos"> 67</span></a>
+</span><span id="Pathier-68"><a href="#Pathier-68"><span class="linenos"> 68</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="Pathier-69"><a href="#Pathier-69"><span class="linenos"> 69</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-70"><a href="#Pathier-70"><span class="linenos"> 70</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-71"><a href="#Pathier-71"><span class="linenos"> 71</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-72"><a href="#Pathier-72"><span class="linenos"> 72</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
+</span><span id="Pathier-73"><a href="#Pathier-73"><span class="linenos"> 73</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-74"><a href="#Pathier-74"><span class="linenos"> 74</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="Pathier-75"><a href="#Pathier-75"><span class="linenos"> 75</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
+</span><span id="Pathier-76"><a href="#Pathier-76"><span class="linenos"> 76</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
+</span><span id="Pathier-77"><a href="#Pathier-77"><span class="linenos"> 77</span></a>        <span class="k">return</span> <span class="n">size</span>
+</span><span id="Pathier-78"><a href="#Pathier-78"><span class="linenos"> 78</span></a>
+</span><span id="Pathier-79"><a href="#Pathier-79"><span class="linenos"> 79</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier-80"><a href="#Pathier-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier-81"><a href="#Pathier-81"><span class="linenos"> 81</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
+</span><span id="Pathier-82"><a href="#Pathier-82"><span class="linenos"> 82</span></a><span class="sd">        and rounded to two decimal places.</span>
+</span><span id="Pathier-83"><a href="#Pathier-83"><span class="linenos"> 83</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-84"><a href="#Pathier-84"><span class="linenos"> 84</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier-85"><a href="#Pathier-85"><span class="linenos"> 85</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier-86"><a href="#Pathier-86"><span class="linenos"> 86</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier-87"><a href="#Pathier-87"><span class="linenos"> 87</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier-88"><a href="#Pathier-88"><span class="linenos"> 88</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier-89"><a href="#Pathier-89"><span class="linenos"> 89</span></a>
+</span><span id="Pathier-90"><a href="#Pathier-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-91"><a href="#Pathier-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
+</span><span id="Pathier-92"><a href="#Pathier-92"><span class="linenos"> 92</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier-93"><a href="#Pathier-93"><span class="linenos"> 93</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="Pathier-94"><a href="#Pathier-94"><span class="linenos"> 94</span></a>
+</span><span id="Pathier-95"><a href="#Pathier-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-96"><a href="#Pathier-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
+</span><span id="Pathier-97"><a href="#Pathier-97"><span class="linenos"> 97</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier-98"><a href="#Pathier-98"><span class="linenos"> 98</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+</span><span id="Pathier-99"><a href="#Pathier-99"><span class="linenos"> 99</span></a>
+</span><span id="Pathier-100"><a href="#Pathier-100"><span class="linenos">100</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-101"><a href="#Pathier-101"><span class="linenos">101</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
+</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
+</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>
+</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
+</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>
+</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Return True if this</span>
+</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a><span class="sd">        path is in sys.path.&quot;&quot;&quot;</span>
+</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
+</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>
+</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
+</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a><span class="sd">        if it isn&#39;t already there.</span>
+</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a>
+</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a><span class="sd">        :param index: The index of sys.path</span>
+</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>
+</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
+</span><span id="Pathier-128"><a href="#Pathier-128"><span class="linenos">128</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>
+</span><span id="Pathier-133"><a href="#Pathier-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
+</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
+</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+</span><span id="Pathier-138"><a href="#Pathier-138"><span class="linenos">138</span></a>
+</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
+</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-143"><a href="#Pathier-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>
+</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object moved up &#39;levels&#39; number of parents from the current path.</span>
+</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-154"><a href="#Pathier-154"><span class="linenos">154</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
+</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
+</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
+</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
+</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="n">path</span>
+</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a>
+</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
+</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
+</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
+</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a>
+</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
+</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
+</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a>
+</span><span id="Pathier-178"><a href="#Pathier-178"><span class="linenos">178</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
+</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a>
+</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a>    <span class="c1"># ============================================write and read============================================</span>
+</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a><span class="sd">        Same as Path().mkdir() except</span>
+</span><span id="Pathier-194"><a href="#Pathier-194"><span class="linenos">194</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
+</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
+</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
+</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a>
+</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
+</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a>
+</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>    <span class="p">):</span>
+</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
+</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
+</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
+</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-220"><a href="#Pathier-220"><span class="linenos">220</span></a>        <span class="p">)</span>
+</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>            <span class="k">raise</span>
+</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>
+</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a>
+</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
+</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
+</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>            <span class="k">raise</span>
+</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>
+</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>
+</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-268"><a href="#Pathier-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a>        <span class="p">)</span>
+</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a>
+</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>
+</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-286"><a href="#Pathier-286"><span class="linenos">286</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>    <span class="p">):</span>
+</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a>        <span class="p">)</span>
+</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>
+</span><span id="Pathier-294"><a href="#Pathier-294"><span class="linenos">294</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>
+</span><span id="Pathier-302"><a href="#Pathier-302"><span class="linenos">302</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-307"><a href="#Pathier-307"><span class="linenos">307</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-309"><a href="#Pathier-309"><span class="linenos">309</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a>    <span class="p">):</span>
+</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a>                <span class="p">)</span>
+</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>
+</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-325"><a href="#Pathier-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a>
+</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier-332"><a href="#Pathier-332"><span class="linenos">332</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
+</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
+</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a>
+</span><span id="Pathier-337"><a href="#Pathier-337"><span class="linenos">337</span></a><span class="sd">        :param new_path: The copy destination.</span>
+</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a>
+</span><span id="Pathier-339"><a href="#Pathier-339"><span class="linenos">339</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
+</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
+</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-344"><a href="#Pathier-344"><span class="linenos">344</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>        <span class="k">return</span> <span class="n">new_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclasses the standard library pathlib.Path class.</p>
 </div>
 
 
@@ -580,28 +580,28 @@
         <span class="def">def</span>
         <span class="name">size</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.size-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.size"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.size-63"><a href="#Pathier.size-63"><span class="linenos">63</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier.size-64"><a href="#Pathier.size-64"><span class="linenos">64</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
-</span><span id="Pathier.size-65"><a href="#Pathier.size-65"><span class="linenos">65</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
-</span><span id="Pathier.size-66"><a href="#Pathier.size-66"><span class="linenos">66</span></a>
-</span><span id="Pathier.size-67"><a href="#Pathier.size-67"><span class="linenos">67</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Pathier.size-68"><a href="#Pathier.size-68"><span class="linenos">68</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.size-69"><a href="#Pathier.size-69"><span class="linenos">69</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier.size-70"><a href="#Pathier.size-70"><span class="linenos">70</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.size-71"><a href="#Pathier.size-71"><span class="linenos">71</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
-</span><span id="Pathier.size-72"><a href="#Pathier.size-72"><span class="linenos">72</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.size-73"><a href="#Pathier.size-73"><span class="linenos">73</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="Pathier.size-74"><a href="#Pathier.size-74"><span class="linenos">74</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Pathier.size-75"><a href="#Pathier.size-75"><span class="linenos">75</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
-</span><span id="Pathier.size-76"><a href="#Pathier.size-76"><span class="linenos">76</span></a>        <span class="k">return</span> <span class="n">size</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.size-64"><a href="#Pathier.size-64"><span class="linenos">64</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier.size-65"><a href="#Pathier.size-65"><span class="linenos">65</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
+</span><span id="Pathier.size-66"><a href="#Pathier.size-66"><span class="linenos">66</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
+</span><span id="Pathier.size-67"><a href="#Pathier.size-67"><span class="linenos">67</span></a>
+</span><span id="Pathier.size-68"><a href="#Pathier.size-68"><span class="linenos">68</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="Pathier.size-69"><a href="#Pathier.size-69"><span class="linenos">69</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.size-70"><a href="#Pathier.size-70"><span class="linenos">70</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier.size-71"><a href="#Pathier.size-71"><span class="linenos">71</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.size-72"><a href="#Pathier.size-72"><span class="linenos">72</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
+</span><span id="Pathier.size-73"><a href="#Pathier.size-73"><span class="linenos">73</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.size-74"><a href="#Pathier.size-74"><span class="linenos">74</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="Pathier.size-75"><a href="#Pathier.size-75"><span class="linenos">75</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
+</span><span id="Pathier.size-76"><a href="#Pathier.size-76"><span class="linenos">76</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
+</span><span id="Pathier.size-77"><a href="#Pathier.size-77"><span class="linenos">77</span></a>        <span class="k">return</span> <span class="n">size</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns the size in bytes of this file or directory.
 Returns None if this path doesn't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -621,24 +621,24 @@
         <span class="def">def</span>
         <span class="name">format_size</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">size</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.format_size-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.format_size"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_size-78"><a href="#Pathier.format_size-78"><span class="linenos">78</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier.format_size-79"><a href="#Pathier.format_size-79"><span class="linenos">79</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier.format_size-80"><a href="#Pathier.format_size-80"><span class="linenos">80</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
-</span><span id="Pathier.format_size-81"><a href="#Pathier.format_size-81"><span class="linenos">81</span></a><span class="sd">        and rounded to two decimal places.</span>
-</span><span id="Pathier.format_size-82"><a href="#Pathier.format_size-82"><span class="linenos">82</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.format_size-83"><a href="#Pathier.format_size-83"><span class="linenos">83</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier.format_size-84"><a href="#Pathier.format_size-84"><span class="linenos">84</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_size-85"><a href="#Pathier.format_size-85"><span class="linenos">85</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier.format_size-86"><a href="#Pathier.format_size-86"><span class="linenos">86</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_size-87"><a href="#Pathier.format_size-87"><span class="linenos">87</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_size-79"><a href="#Pathier.format_size-79"><span class="linenos">79</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier.format_size-80"><a href="#Pathier.format_size-80"><span class="linenos">80</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier.format_size-81"><a href="#Pathier.format_size-81"><span class="linenos">81</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
+</span><span id="Pathier.format_size-82"><a href="#Pathier.format_size-82"><span class="linenos">82</span></a><span class="sd">        and rounded to two decimal places.</span>
+</span><span id="Pathier.format_size-83"><a href="#Pathier.format_size-83"><span class="linenos">83</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.format_size-84"><a href="#Pathier.format_size-84"><span class="linenos">84</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier.format_size-85"><a href="#Pathier.format_size-85"><span class="linenos">85</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_size-86"><a href="#Pathier.format_size-86"><span class="linenos">86</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier.format_size-87"><a href="#Pathier.format_size-87"><span class="linenos">87</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_size-88"><a href="#Pathier.format_size-88"><span class="linenos">88</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Format 'size' with common file size abbreviations
 and rounded to two decimal places.</p>
 
 <div class="pdoc-code codehilite">
@@ -656,18 +656,18 @@
         <span class="def">def</span>
         <span class="name">is_larger</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_larger-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_larger"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-89"><a href="#Pathier.is_larger-89"><span class="linenos">89</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_larger-90"><a href="#Pathier.is_larger-90"><span class="linenos">90</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
-</span><span id="Pathier.is_larger-91"><a href="#Pathier.is_larger-91"><span class="linenos">91</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_larger-92"><a href="#Pathier.is_larger-92"><span class="linenos">92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-90"><a href="#Pathier.is_larger-90"><span class="linenos">90</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_larger-91"><a href="#Pathier.is_larger-91"><span class="linenos">91</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
+</span><span id="Pathier.is_larger-92"><a href="#Pathier.is_larger-92"><span class="linenos">92</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_larger-93"><a href="#Pathier.is_larger-93"><span class="linenos">93</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder is larger than
 the one pointed to by 'path'.</p>
 </div>
 
@@ -680,18 +680,18 @@
         <span class="def">def</span>
         <span class="name">is_older</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_older-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_older"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-94"><a href="#Pathier.is_older-94"><span class="linenos">94</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_older-95"><a href="#Pathier.is_older-95"><span class="linenos">95</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
-</span><span id="Pathier.is_older-96"><a href="#Pathier.is_older-96"><span class="linenos">96</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_older-97"><a href="#Pathier.is_older-97"><span class="linenos">97</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-95"><a href="#Pathier.is_older-95"><span class="linenos">95</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_older-96"><a href="#Pathier.is_older-96"><span class="linenos">96</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
+</span><span id="Pathier.is_older-97"><a href="#Pathier.is_older-97"><span class="linenos">97</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_older-98"><a href="#Pathier.is_older-98"><span class="linenos">98</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder is older than
 the one pointed to by 'path'.</p>
 </div>
 
@@ -704,18 +704,18 @@
         <span class="def">def</span>
         <span class="name">modified_more_recently</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.modified_more_recently-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.modified_more_recently"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-99"><a href="#Pathier.modified_more_recently-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.modified_more_recently-100"><a href="#Pathier.modified_more_recently-100"><span class="linenos">100</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
-</span><span id="Pathier.modified_more_recently-101"><a href="#Pathier.modified_more_recently-101"><span class="linenos">101</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.modified_more_recently-102"><a href="#Pathier.modified_more_recently-102"><span class="linenos">102</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-100"><a href="#Pathier.modified_more_recently-100"><span class="linenos">100</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.modified_more_recently-101"><a href="#Pathier.modified_more_recently-101"><span class="linenos">101</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
+</span><span id="Pathier.modified_more_recently-102"><a href="#Pathier.modified_more_recently-102"><span class="linenos">102</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
+</span><span id="Pathier.modified_more_recently-103"><a href="#Pathier.modified_more_recently-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder was modified
 more recently than the one pointed to by 'path'.</p>
 </div>
 
@@ -728,17 +728,17 @@
         <span class="def">def</span>
         <span class="name">mkcwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkcwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkcwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-105"><a href="#Pathier.mkcwd-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.mkcwd-106"><a href="#Pathier.mkcwd-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkcwd-107"><a href="#Pathier.mkcwd-107"><span class="linenos">107</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-106"><a href="#Pathier.mkcwd-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.mkcwd-107"><a href="#Pathier.mkcwd-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkcwd-108"><a href="#Pathier.mkcwd-108"><span class="linenos">108</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make this path your current working directory.</p>
 </div>
 
 
@@ -764,23 +764,23 @@
         <span class="def">def</span>
         <span class="name">add_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.add_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.add_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-115"><a href="#Pathier.add_to_PATH-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier.add_to_PATH-116"><a href="#Pathier.add_to_PATH-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
-</span><span id="Pathier.add_to_PATH-117"><a href="#Pathier.add_to_PATH-117"><span class="linenos">117</span></a><span class="sd">        if it isn&#39;t already there.</span>
-</span><span id="Pathier.add_to_PATH-118"><a href="#Pathier.add_to_PATH-118"><span class="linenos">118</span></a>
-</span><span id="Pathier.add_to_PATH-119"><a href="#Pathier.add_to_PATH-119"><span class="linenos">119</span></a><span class="sd">        :param index: The index of sys.path</span>
-</span><span id="Pathier.add_to_PATH-120"><a href="#Pathier.add_to_PATH-120"><span class="linenos">120</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier.add_to_PATH-121"><a href="#Pathier.add_to_PATH-121"><span class="linenos">121</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.add_to_PATH-122"><a href="#Pathier.add_to_PATH-122"><span class="linenos">122</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.add_to_PATH-123"><a href="#Pathier.add_to_PATH-123"><span class="linenos">123</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-116"><a href="#Pathier.add_to_PATH-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier.add_to_PATH-117"><a href="#Pathier.add_to_PATH-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
+</span><span id="Pathier.add_to_PATH-118"><a href="#Pathier.add_to_PATH-118"><span class="linenos">118</span></a><span class="sd">        if it isn&#39;t already there.</span>
+</span><span id="Pathier.add_to_PATH-119"><a href="#Pathier.add_to_PATH-119"><span class="linenos">119</span></a>
+</span><span id="Pathier.add_to_PATH-120"><a href="#Pathier.add_to_PATH-120"><span class="linenos">120</span></a><span class="sd">        :param index: The index of sys.path</span>
+</span><span id="Pathier.add_to_PATH-121"><a href="#Pathier.add_to_PATH-121"><span class="linenos">121</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier.add_to_PATH-122"><a href="#Pathier.add_to_PATH-122"><span class="linenos">122</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.add_to_PATH-123"><a href="#Pathier.add_to_PATH-123"><span class="linenos">123</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.add_to_PATH-124"><a href="#Pathier.add_to_PATH-124"><span class="linenos">124</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Insert this path into sys.path
 if it isn't already there.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -800,20 +800,20 @@
         <span class="def">def</span>
         <span class="name">append_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.append_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.append_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-125"><a href="#Pathier.append_to_PATH-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.append_to_PATH-126"><a href="#Pathier.append_to_PATH-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
-</span><span id="Pathier.append_to_PATH-127"><a href="#Pathier.append_to_PATH-127"><span class="linenos">127</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier.append_to_PATH-128"><a href="#Pathier.append_to_PATH-128"><span class="linenos">128</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.append_to_PATH-129"><a href="#Pathier.append_to_PATH-129"><span class="linenos">129</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.append_to_PATH-130"><a href="#Pathier.append_to_PATH-130"><span class="linenos">130</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-126"><a href="#Pathier.append_to_PATH-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.append_to_PATH-127"><a href="#Pathier.append_to_PATH-127"><span class="linenos">127</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
+</span><span id="Pathier.append_to_PATH-128"><a href="#Pathier.append_to_PATH-128"><span class="linenos">128</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier.append_to_PATH-129"><a href="#Pathier.append_to_PATH-129"><span class="linenos">129</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.append_to_PATH-130"><a href="#Pathier.append_to_PATH-130"><span class="linenos">130</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.append_to_PATH-131"><a href="#Pathier.append_to_PATH-131"><span class="linenos">131</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Append this path to sys.path
 if it isn't already there.</p>
 </div>
 
@@ -826,19 +826,19 @@
         <span class="def">def</span>
         <span class="name">remove_from_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.remove_from_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.remove_from_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-132"><a href="#Pathier.remove_from_PATH-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.remove_from_PATH-133"><a href="#Pathier.remove_from_PATH-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
-</span><span id="Pathier.remove_from_PATH-134"><a href="#Pathier.remove_from_PATH-134"><span class="linenos">134</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier.remove_from_PATH-135"><a href="#Pathier.remove_from_PATH-135"><span class="linenos">135</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.remove_from_PATH-136"><a href="#Pathier.remove_from_PATH-136"><span class="linenos">136</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-133"><a href="#Pathier.remove_from_PATH-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.remove_from_PATH-134"><a href="#Pathier.remove_from_PATH-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
+</span><span id="Pathier.remove_from_PATH-135"><a href="#Pathier.remove_from_PATH-135"><span class="linenos">135</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
+</span><span id="Pathier.remove_from_PATH-136"><a href="#Pathier.remove_from_PATH-136"><span class="linenos">136</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.remove_from_PATH-137"><a href="#Pathier.remove_from_PATH-137"><span class="linenos">137</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Remove this path from sys.path
 if it's in sys.path.</p>
 </div>
 
@@ -851,25 +851,25 @@
         <span class="def">def</span>
         <span class="name">moveup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.moveup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.moveup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-138"><a href="#Pathier.moveup-138"><span class="linenos">138</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.moveup-139"><a href="#Pathier.moveup-139"><span class="linenos">139</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
-</span><span id="Pathier.moveup-140"><a href="#Pathier.moveup-140"><span class="linenos">140</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.moveup-141"><a href="#Pathier.moveup-141"><span class="linenos">141</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier.moveup-142"><a href="#Pathier.moveup-142"><span class="linenos">142</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier.moveup-143"><a href="#Pathier.moveup-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier.moveup-144"><a href="#Pathier.moveup-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier.moveup-145"><a href="#Pathier.moveup-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.moveup-146"><a href="#Pathier.moveup-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.moveup-147"><a href="#Pathier.moveup-147"><span class="linenos">147</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.moveup-148"><a href="#Pathier.moveup-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-139"><a href="#Pathier.moveup-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.moveup-140"><a href="#Pathier.moveup-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
+</span><span id="Pathier.moveup-141"><a href="#Pathier.moveup-141"><span class="linenos">141</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier.moveup-142"><a href="#Pathier.moveup-142"><span class="linenos">142</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier.moveup-143"><a href="#Pathier.moveup-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier.moveup-144"><a href="#Pathier.moveup-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier.moveup-145"><a href="#Pathier.moveup-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier.moveup-146"><a href="#Pathier.moveup-146"><span class="linenos">146</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.moveup-147"><a href="#Pathier.moveup-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.moveup-148"><a href="#Pathier.moveup-148"><span class="linenos">148</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.moveup-149"><a href="#Pathier.moveup-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new Pathier object that is a parent of this instance.
 'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
 
 <div class="pdoc-code codehilite">
@@ -891,24 +891,24 @@
         <span class="def">def</span>
         <span class="name">move_under</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.move_under-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.move_under"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-161"><a href="#Pathier.move_under-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.move_under-162"><a href="#Pathier.move_under-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
-</span><span id="Pathier.move_under-163"><a href="#Pathier.move_under-163"><span class="linenos">163</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
-</span><span id="Pathier.move_under-164"><a href="#Pathier.move_under-164"><span class="linenos">164</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.move_under-165"><a href="#Pathier.move_under-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.move_under-166"><a href="#Pathier.move_under-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier.move_under-167"><a href="#Pathier.move_under-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.move_under-168"><a href="#Pathier.move_under-168"><span class="linenos">168</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.move_under-169"><a href="#Pathier.move_under-169"><span class="linenos">169</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.move_under-170"><a href="#Pathier.move_under-170"><span class="linenos">170</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-162"><a href="#Pathier.move_under-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.move_under-163"><a href="#Pathier.move_under-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
+</span><span id="Pathier.move_under-164"><a href="#Pathier.move_under-164"><span class="linenos">164</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
+</span><span id="Pathier.move_under-165"><a href="#Pathier.move_under-165"><span class="linenos">165</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier.move_under-166"><a href="#Pathier.move_under-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.move_under-167"><a href="#Pathier.move_under-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier.move_under-168"><a href="#Pathier.move_under-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.move_under-169"><a href="#Pathier.move_under-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.move_under-170"><a href="#Pathier.move_under-170"><span class="linenos">170</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.move_under-171"><a href="#Pathier.move_under-171"><span class="linenos">171</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new Pathier object such that the stem
 is one level below the folder 'name'.
 'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
 
@@ -929,30 +929,30 @@
         <span class="def">def</span>
         <span class="name">separate</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.separate-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.separate"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-172"><a href="#Pathier.separate-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.separate-173"><a href="#Pathier.separate-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
-</span><span id="Pathier.separate-174"><a href="#Pathier.separate-174"><span class="linenos">174</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
-</span><span id="Pathier.separate-175"><a href="#Pathier.separate-175"><span class="linenos">175</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.separate-176"><a href="#Pathier.separate-176"><span class="linenos">176</span></a>
-</span><span id="Pathier.separate-177"><a href="#Pathier.separate-177"><span class="linenos">177</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
-</span><span id="Pathier.separate-178"><a href="#Pathier.separate-178"><span class="linenos">178</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.separate-179"><a href="#Pathier.separate-179"><span class="linenos">179</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier.separate-180"><a href="#Pathier.separate-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier.separate-181"><a href="#Pathier.separate-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier.separate-182"><a href="#Pathier.separate-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.separate-183"><a href="#Pathier.separate-183"><span class="linenos">183</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.separate-184"><a href="#Pathier.separate-184"><span class="linenos">184</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.separate-185"><a href="#Pathier.separate-185"><span class="linenos">185</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier.separate-186"><a href="#Pathier.separate-186"><span class="linenos">186</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier.separate-187"><a href="#Pathier.separate-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-173"><a href="#Pathier.separate-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.separate-174"><a href="#Pathier.separate-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
+</span><span id="Pathier.separate-175"><a href="#Pathier.separate-175"><span class="linenos">175</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
+</span><span id="Pathier.separate-176"><a href="#Pathier.separate-176"><span class="linenos">176</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier.separate-177"><a href="#Pathier.separate-177"><span class="linenos">177</span></a>
+</span><span id="Pathier.separate-178"><a href="#Pathier.separate-178"><span class="linenos">178</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
+</span><span id="Pathier.separate-179"><a href="#Pathier.separate-179"><span class="linenos">179</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.separate-180"><a href="#Pathier.separate-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier.separate-181"><a href="#Pathier.separate-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier.separate-182"><a href="#Pathier.separate-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier.separate-183"><a href="#Pathier.separate-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.separate-184"><a href="#Pathier.separate-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.separate-185"><a href="#Pathier.separate-185"><span class="linenos">185</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.separate-186"><a href="#Pathier.separate-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier.separate-187"><a href="#Pathier.separate-187"><span class="linenos">187</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier.separate-188"><a href="#Pathier.separate-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new Pathier object that is the
 relative child path after 'name'.
 'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
 
@@ -977,20 +977,20 @@
         <span class="def">def</span>
         <span class="name">mkdir</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>, </span><span class="param"><span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkdir-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkdir"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-190"><a href="#Pathier.mkdir-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.mkdir-191"><a href="#Pathier.mkdir-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier.mkdir-192"><a href="#Pathier.mkdir-192"><span class="linenos">192</span></a><span class="sd">        Same as Path().mkdir() except</span>
-</span><span id="Pathier.mkdir-193"><a href="#Pathier.mkdir-193"><span class="linenos">193</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
-</span><span id="Pathier.mkdir-194"><a href="#Pathier.mkdir-194"><span class="linenos">194</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkdir-195"><a href="#Pathier.mkdir-195"><span class="linenos">195</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-191"><a href="#Pathier.mkdir-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.mkdir-192"><a href="#Pathier.mkdir-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier.mkdir-193"><a href="#Pathier.mkdir-193"><span class="linenos">193</span></a><span class="sd">        Same as Path().mkdir() except</span>
+</span><span id="Pathier.mkdir-194"><a href="#Pathier.mkdir-194"><span class="linenos">194</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
+</span><span id="Pathier.mkdir-195"><a href="#Pathier.mkdir-195"><span class="linenos">195</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkdir-196"><a href="#Pathier.mkdir-196"><span class="linenos">196</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create this directory.
 Same as Path().mkdir() except
 'parents' and 'exist_ok' default
 to True instead of False.</p>
@@ -1005,18 +1005,18 @@
         <span class="def">def</span>
         <span class="name">touch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.touch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.touch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-197"><a href="#Pathier.touch-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.touch-198"><a href="#Pathier.touch-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
-</span><span id="Pathier.touch-199"><a href="#Pathier.touch-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier.touch-200"><a href="#Pathier.touch-200"><span class="linenos">200</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-198"><a href="#Pathier.touch-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.touch-199"><a href="#Pathier.touch-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
+</span><span id="Pathier.touch-200"><a href="#Pathier.touch-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier.touch-201"><a href="#Pathier.touch-201"><span class="linenos">201</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create file and parents if necessary.</p>
 </div>
 
 
@@ -1028,45 +1028,45 @@
         <span class="def">def</span>
         <span class="name">write_text</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_text-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_text"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-202"><a href="#Pathier.write_text-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier.write_text-203"><a href="#Pathier.write_text-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.write_text-204"><a href="#Pathier.write_text-204"><span class="linenos">204</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.write_text-205"><a href="#Pathier.write_text-205"><span class="linenos">205</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-206"><a href="#Pathier.write_text-206"><span class="linenos">206</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-207"><a href="#Pathier.write_text-207"><span class="linenos">207</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-208"><a href="#Pathier.write_text-208"><span class="linenos">208</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.write_text-209"><a href="#Pathier.write_text-209"><span class="linenos">209</span></a>    <span class="p">):</span>
-</span><span id="Pathier.write_text-210"><a href="#Pathier.write_text-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
-</span><span id="Pathier.write_text-211"><a href="#Pathier.write_text-211"><span class="linenos">211</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
-</span><span id="Pathier.write_text-212"><a href="#Pathier.write_text-212"><span class="linenos">212</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
-</span><span id="Pathier.write_text-213"><a href="#Pathier.write_text-213"><span class="linenos">213</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_text-214"><a href="#Pathier.write_text-214"><span class="linenos">214</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier.write_text-215"><a href="#Pathier.write_text-215"><span class="linenos">215</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier.write_text-216"><a href="#Pathier.write_text-216"><span class="linenos">216</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.write_text-217"><a href="#Pathier.write_text-217"><span class="linenos">217</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.write_text-218"><a href="#Pathier.write_text-218"><span class="linenos">218</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.write_text-219"><a href="#Pathier.write_text-219"><span class="linenos">219</span></a>        <span class="p">)</span>
-</span><span id="Pathier.write_text-220"><a href="#Pathier.write_text-220"><span class="linenos">220</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_text-221"><a href="#Pathier.write_text-221"><span class="linenos">221</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-222"><a href="#Pathier.write_text-222"><span class="linenos">222</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-223"><a href="#Pathier.write_text-223"><span class="linenos">223</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-224"><a href="#Pathier.write_text-224"><span class="linenos">224</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-225"><a href="#Pathier.write_text-225"><span class="linenos">225</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-226"><a href="#Pathier.write_text-226"><span class="linenos">226</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_text-227"><a href="#Pathier.write_text-227"><span class="linenos">227</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_text-228"><a href="#Pathier.write_text-228"><span class="linenos">228</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-229"><a href="#Pathier.write_text-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_text-230"><a href="#Pathier.write_text-230"><span class="linenos">230</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_text-231"><a href="#Pathier.write_text-231"><span class="linenos">231</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_text-232"><a href="#Pathier.write_text-232"><span class="linenos">232</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-203"><a href="#Pathier.write_text-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier.write_text-204"><a href="#Pathier.write_text-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.write_text-205"><a href="#Pathier.write_text-205"><span class="linenos">205</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.write_text-206"><a href="#Pathier.write_text-206"><span class="linenos">206</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-207"><a href="#Pathier.write_text-207"><span class="linenos">207</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-208"><a href="#Pathier.write_text-208"><span class="linenos">208</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-209"><a href="#Pathier.write_text-209"><span class="linenos">209</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.write_text-210"><a href="#Pathier.write_text-210"><span class="linenos">210</span></a>    <span class="p">):</span>
+</span><span id="Pathier.write_text-211"><a href="#Pathier.write_text-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
+</span><span id="Pathier.write_text-212"><a href="#Pathier.write_text-212"><span class="linenos">212</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
+</span><span id="Pathier.write_text-213"><a href="#Pathier.write_text-213"><span class="linenos">213</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
+</span><span id="Pathier.write_text-214"><a href="#Pathier.write_text-214"><span class="linenos">214</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_text-215"><a href="#Pathier.write_text-215"><span class="linenos">215</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier.write_text-216"><a href="#Pathier.write_text-216"><span class="linenos">216</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier.write_text-217"><a href="#Pathier.write_text-217"><span class="linenos">217</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.write_text-218"><a href="#Pathier.write_text-218"><span class="linenos">218</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.write_text-219"><a href="#Pathier.write_text-219"><span class="linenos">219</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.write_text-220"><a href="#Pathier.write_text-220"><span class="linenos">220</span></a>        <span class="p">)</span>
+</span><span id="Pathier.write_text-221"><a href="#Pathier.write_text-221"><span class="linenos">221</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_text-222"><a href="#Pathier.write_text-222"><span class="linenos">222</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-223"><a href="#Pathier.write_text-223"><span class="linenos">223</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-224"><a href="#Pathier.write_text-224"><span class="linenos">224</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-225"><a href="#Pathier.write_text-225"><span class="linenos">225</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-226"><a href="#Pathier.write_text-226"><span class="linenos">226</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-227"><a href="#Pathier.write_text-227"><span class="linenos">227</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_text-228"><a href="#Pathier.write_text-228"><span class="linenos">228</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_text-229"><a href="#Pathier.write_text-229"><span class="linenos">229</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-230"><a href="#Pathier.write_text-230"><span class="linenos">230</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_text-231"><a href="#Pathier.write_text-231"><span class="linenos">231</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_text-232"><a href="#Pathier.write_text-232"><span class="linenos">232</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_text-233"><a href="#Pathier.write_text-233"><span class="linenos">233</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write data to file. If a TypeError is raised, the function
 will attempt to case data to a str and try the write again.
 If a FileNotFoundError is raised and parents = True,
 self.parent will be created.</p>
@@ -1081,30 +1081,30 @@
         <span class="def">def</span>
         <span class="name">write_bytes</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_bytes-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_bytes"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-234"><a href="#Pathier.write_bytes-234"><span class="linenos">234</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.write_bytes-235"><a href="#Pathier.write_bytes-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier.write_bytes-236"><a href="#Pathier.write_bytes-236"><span class="linenos">236</span></a>
-</span><span id="Pathier.write_bytes-237"><a href="#Pathier.write_bytes-237"><span class="linenos">237</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
-</span><span id="Pathier.write_bytes-238"><a href="#Pathier.write_bytes-238"><span class="linenos">238</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
-</span><span id="Pathier.write_bytes-239"><a href="#Pathier.write_bytes-239"><span class="linenos">239</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_bytes-240"><a href="#Pathier.write_bytes-240"><span class="linenos">240</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-241"><a href="#Pathier.write_bytes-241"><span class="linenos">241</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-242"><a href="#Pathier.write_bytes-242"><span class="linenos">242</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-243"><a href="#Pathier.write_bytes-243"><span class="linenos">243</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-244"><a href="#Pathier.write_bytes-244"><span class="linenos">244</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-245"><a href="#Pathier.write_bytes-245"><span class="linenos">245</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-246"><a href="#Pathier.write_bytes-246"><span class="linenos">246</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-247"><a href="#Pathier.write_bytes-247"><span class="linenos">247</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_bytes-248"><a href="#Pathier.write_bytes-248"><span class="linenos">248</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-249"><a href="#Pathier.write_bytes-249"><span class="linenos">249</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-235"><a href="#Pathier.write_bytes-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.write_bytes-236"><a href="#Pathier.write_bytes-236"><span class="linenos">236</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier.write_bytes-237"><a href="#Pathier.write_bytes-237"><span class="linenos">237</span></a>
+</span><span id="Pathier.write_bytes-238"><a href="#Pathier.write_bytes-238"><span class="linenos">238</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
+</span><span id="Pathier.write_bytes-239"><a href="#Pathier.write_bytes-239"><span class="linenos">239</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
+</span><span id="Pathier.write_bytes-240"><a href="#Pathier.write_bytes-240"><span class="linenos">240</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_bytes-241"><a href="#Pathier.write_bytes-241"><span class="linenos">241</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-242"><a href="#Pathier.write_bytes-242"><span class="linenos">242</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-243"><a href="#Pathier.write_bytes-243"><span class="linenos">243</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-244"><a href="#Pathier.write_bytes-244"><span class="linenos">244</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-245"><a href="#Pathier.write_bytes-245"><span class="linenos">245</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-246"><a href="#Pathier.write_bytes-246"><span class="linenos">246</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-247"><a href="#Pathier.write_bytes-247"><span class="linenos">247</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-248"><a href="#Pathier.write_bytes-248"><span class="linenos">248</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_bytes-249"><a href="#Pathier.write_bytes-249"><span class="linenos">249</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-250"><a href="#Pathier.write_bytes-250"><span class="linenos">250</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write bytes to file.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1124,17 +1124,17 @@
         <span class="def">def</span>
         <span class="name">json_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-251"><a href="#Pathier.json_loads-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_loads-252"><a href="#Pathier.json_loads-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_loads-253"><a href="#Pathier.json_loads-253"><span class="linenos">253</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-252"><a href="#Pathier.json_loads-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_loads-253"><a href="#Pathier.json_loads-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_loads-254"><a href="#Pathier.json_loads-254"><span class="linenos">254</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load json file.</p>
 </div>
 
 
@@ -1146,33 +1146,33 @@
         <span class="def">def</span>
         <span class="name">json_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-255"><a href="#Pathier.json_dumps-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-256"><a href="#Pathier.json_dumps-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-257"><a href="#Pathier.json_dumps-257"><span class="linenos">257</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-258"><a href="#Pathier.json_dumps-258"><span class="linenos">258</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-259"><a href="#Pathier.json_dumps-259"><span class="linenos">259</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-260"><a href="#Pathier.json_dumps-260"><span class="linenos">260</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-261"><a href="#Pathier.json_dumps-261"><span class="linenos">261</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-262"><a href="#Pathier.json_dumps-262"><span class="linenos">262</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-263"><a href="#Pathier.json_dumps-263"><span class="linenos">263</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-264"><a href="#Pathier.json_dumps-264"><span class="linenos">264</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-265"><a href="#Pathier.json_dumps-265"><span class="linenos">265</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_dumps-266"><a href="#Pathier.json_dumps-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_dumps-267"><a href="#Pathier.json_dumps-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-268"><a href="#Pathier.json_dumps-268"><span class="linenos">268</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier.json_dumps-269"><a href="#Pathier.json_dumps-269"><span class="linenos">269</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-270"><a href="#Pathier.json_dumps-270"><span class="linenos">270</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-271"><a href="#Pathier.json_dumps-271"><span class="linenos">271</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-272"><a href="#Pathier.json_dumps-272"><span class="linenos">272</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-273"><a href="#Pathier.json_dumps-273"><span class="linenos">273</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-256"><a href="#Pathier.json_dumps-256"><span class="linenos">256</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-257"><a href="#Pathier.json_dumps-257"><span class="linenos">257</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-258"><a href="#Pathier.json_dumps-258"><span class="linenos">258</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-259"><a href="#Pathier.json_dumps-259"><span class="linenos">259</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-260"><a href="#Pathier.json_dumps-260"><span class="linenos">260</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-261"><a href="#Pathier.json_dumps-261"><span class="linenos">261</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-262"><a href="#Pathier.json_dumps-262"><span class="linenos">262</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-263"><a href="#Pathier.json_dumps-263"><span class="linenos">263</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-264"><a href="#Pathier.json_dumps-264"><span class="linenos">264</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-265"><a href="#Pathier.json_dumps-265"><span class="linenos">265</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-266"><a href="#Pathier.json_dumps-266"><span class="linenos">266</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_dumps-267"><a href="#Pathier.json_dumps-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_dumps-268"><a href="#Pathier.json_dumps-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-269"><a href="#Pathier.json_dumps-269"><span class="linenos">269</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier.json_dumps-270"><a href="#Pathier.json_dumps-270"><span class="linenos">270</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-271"><a href="#Pathier.json_dumps-271"><span class="linenos">271</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-272"><a href="#Pathier.json_dumps-272"><span class="linenos">272</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-273"><a href="#Pathier.json_dumps-273"><span class="linenos">273</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-274"><a href="#Pathier.json_dumps-274"><span class="linenos">274</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump data to json file.</p>
 </div>
 
 
@@ -1184,17 +1184,17 @@
         <span class="def">def</span>
         <span class="name">toml_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-275"><a href="#Pathier.toml_loads-275"><span class="linenos">275</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.toml_loads-276"><a href="#Pathier.toml_loads-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_loads-277"><a href="#Pathier.toml_loads-277"><span class="linenos">277</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-276"><a href="#Pathier.toml_loads-276"><span class="linenos">276</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.toml_loads-277"><a href="#Pathier.toml_loads-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_loads-278"><a href="#Pathier.toml_loads-278"><span class="linenos">278</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load toml file.</p>
 </div>
 
 
@@ -1206,27 +1206,27 @@
         <span class="def">def</span>
         <span class="name">toml_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-279"><a href="#Pathier.toml_dumps-279"><span class="linenos">279</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-280"><a href="#Pathier.toml_dumps-280"><span class="linenos">280</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-281"><a href="#Pathier.toml_dumps-281"><span class="linenos">281</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-282"><a href="#Pathier.toml_dumps-282"><span class="linenos">282</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-283"><a href="#Pathier.toml_dumps-283"><span class="linenos">283</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-284"><a href="#Pathier.toml_dumps-284"><span class="linenos">284</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-285"><a href="#Pathier.toml_dumps-285"><span class="linenos">285</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-286"><a href="#Pathier.toml_dumps-286"><span class="linenos">286</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-287"><a href="#Pathier.toml_dumps-287"><span class="linenos">287</span></a>    <span class="p">):</span>
-</span><span id="Pathier.toml_dumps-288"><a href="#Pathier.toml_dumps-288"><span class="linenos">288</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_dumps-289"><a href="#Pathier.toml_dumps-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-290"><a href="#Pathier.toml_dumps-290"><span class="linenos">290</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.toml_dumps-291"><a href="#Pathier.toml_dumps-291"><span class="linenos">291</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-280"><a href="#Pathier.toml_dumps-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-281"><a href="#Pathier.toml_dumps-281"><span class="linenos">281</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-282"><a href="#Pathier.toml_dumps-282"><span class="linenos">282</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-283"><a href="#Pathier.toml_dumps-283"><span class="linenos">283</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-284"><a href="#Pathier.toml_dumps-284"><span class="linenos">284</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-285"><a href="#Pathier.toml_dumps-285"><span class="linenos">285</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-286"><a href="#Pathier.toml_dumps-286"><span class="linenos">286</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-287"><a href="#Pathier.toml_dumps-287"><span class="linenos">287</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-288"><a href="#Pathier.toml_dumps-288"><span class="linenos">288</span></a>    <span class="p">):</span>
+</span><span id="Pathier.toml_dumps-289"><a href="#Pathier.toml_dumps-289"><span class="linenos">289</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_dumps-290"><a href="#Pathier.toml_dumps-290"><span class="linenos">290</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-291"><a href="#Pathier.toml_dumps-291"><span class="linenos">291</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.toml_dumps-292"><a href="#Pathier.toml_dumps-292"><span class="linenos">292</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump data to toml file.</p>
 </div>
 
 
@@ -1238,21 +1238,21 @@
         <span class="def">def</span>
         <span class="name">loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-293"><a href="#Pathier.loads-293"><span class="linenos">293</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.loads-294"><a href="#Pathier.loads-294"><span class="linenos">294</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.loads-295"><a href="#Pathier.loads-295"><span class="linenos">295</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.loads-296"><a href="#Pathier.loads-296"><span class="linenos">296</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-297"><a href="#Pathier.loads-297"><span class="linenos">297</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier.loads-298"><a href="#Pathier.loads-298"><span class="linenos">298</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-299"><a href="#Pathier.loads-299"><span class="linenos">299</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-294"><a href="#Pathier.loads-294"><span class="linenos">294</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.loads-295"><a href="#Pathier.loads-295"><span class="linenos">295</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.loads-296"><a href="#Pathier.loads-296"><span class="linenos">296</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.loads-297"><a href="#Pathier.loads-297"><span class="linenos">297</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-298"><a href="#Pathier.loads-298"><span class="linenos">298</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier.loads-299"><a href="#Pathier.loads-299"><span class="linenos">299</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-300"><a href="#Pathier.loads-300"><span class="linenos">300</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load a json or toml file based off this instance's suffix.</p>
 </div>
 
 
@@ -1264,33 +1264,33 @@
         <span class="def">def</span>
         <span class="name">dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-301"><a href="#Pathier.dumps-301"><span class="linenos">301</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-302"><a href="#Pathier.dumps-302"><span class="linenos">302</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.dumps-303"><a href="#Pathier.dumps-303"><span class="linenos">303</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.dumps-304"><a href="#Pathier.dumps-304"><span class="linenos">304</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-305"><a href="#Pathier.dumps-305"><span class="linenos">305</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-306"><a href="#Pathier.dumps-306"><span class="linenos">306</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-307"><a href="#Pathier.dumps-307"><span class="linenos">307</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.dumps-308"><a href="#Pathier.dumps-308"><span class="linenos">308</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-309"><a href="#Pathier.dumps-309"><span class="linenos">309</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-310"><a href="#Pathier.dumps-310"><span class="linenos">310</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.dumps-311"><a href="#Pathier.dumps-311"><span class="linenos">311</span></a>    <span class="p">):</span>
-</span><span id="Pathier.dumps-312"><a href="#Pathier.dumps-312"><span class="linenos">312</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.dumps-313"><a href="#Pathier.dumps-313"><span class="linenos">313</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.dumps-314"><a href="#Pathier.dumps-314"><span class="linenos">314</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-315"><a href="#Pathier.dumps-315"><span class="linenos">315</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-316"><a href="#Pathier.dumps-316"><span class="linenos">316</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.dumps-317"><a href="#Pathier.dumps-317"><span class="linenos">317</span></a>                <span class="p">)</span>
-</span><span id="Pathier.dumps-318"><a href="#Pathier.dumps-318"><span class="linenos">318</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-319"><a href="#Pathier.dumps-319"><span class="linenos">319</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-302"><a href="#Pathier.dumps-302"><span class="linenos">302</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-303"><a href="#Pathier.dumps-303"><span class="linenos">303</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.dumps-304"><a href="#Pathier.dumps-304"><span class="linenos">304</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.dumps-305"><a href="#Pathier.dumps-305"><span class="linenos">305</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-306"><a href="#Pathier.dumps-306"><span class="linenos">306</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-307"><a href="#Pathier.dumps-307"><span class="linenos">307</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-308"><a href="#Pathier.dumps-308"><span class="linenos">308</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.dumps-309"><a href="#Pathier.dumps-309"><span class="linenos">309</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-310"><a href="#Pathier.dumps-310"><span class="linenos">310</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-311"><a href="#Pathier.dumps-311"><span class="linenos">311</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.dumps-312"><a href="#Pathier.dumps-312"><span class="linenos">312</span></a>    <span class="p">):</span>
+</span><span id="Pathier.dumps-313"><a href="#Pathier.dumps-313"><span class="linenos">313</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.dumps-314"><a href="#Pathier.dumps-314"><span class="linenos">314</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.dumps-315"><a href="#Pathier.dumps-315"><span class="linenos">315</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-316"><a href="#Pathier.dumps-316"><span class="linenos">316</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-317"><a href="#Pathier.dumps-317"><span class="linenos">317</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.dumps-318"><a href="#Pathier.dumps-318"><span class="linenos">318</span></a>                <span class="p">)</span>
+</span><span id="Pathier.dumps-319"><a href="#Pathier.dumps-319"><span class="linenos">319</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-320"><a href="#Pathier.dumps-320"><span class="linenos">320</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump data to a json or toml file based off this instance's suffix.</p>
 </div>
 
 
@@ -1302,21 +1302,21 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-321"><a href="#Pathier.delete-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.delete-322"><a href="#Pathier.delete-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier.delete-323"><a href="#Pathier.delete-323"><span class="linenos">323</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.delete-324"><a href="#Pathier.delete-324"><span class="linenos">324</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.delete-325"><a href="#Pathier.delete-325"><span class="linenos">325</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier.delete-326"><a href="#Pathier.delete-326"><span class="linenos">326</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.delete-327"><a href="#Pathier.delete-327"><span class="linenos">327</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-322"><a href="#Pathier.delete-322"><span class="linenos">322</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.delete-323"><a href="#Pathier.delete-323"><span class="linenos">323</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier.delete-324"><a href="#Pathier.delete-324"><span class="linenos">324</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.delete-325"><a href="#Pathier.delete-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.delete-326"><a href="#Pathier.delete-326"><span class="linenos">326</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier.delete-327"><a href="#Pathier.delete-327"><span class="linenos">327</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.delete-328"><a href="#Pathier.delete-328"><span class="linenos">328</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete the file or folder pointed to by this instance.
 Uses self.unlink() if a file and uses shutil.rmtree() if a directory.</p>
 </div>
 
@@ -1329,40 +1329,40 @@
         <span class="def">def</span>
         <span class="name">copy</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">new_path</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">Self</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.copy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.copy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-329"><a href="#Pathier.copy-329"><span class="linenos">329</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier.copy-330"><a href="#Pathier.copy-330"><span class="linenos">330</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier.copy-331"><a href="#Pathier.copy-331"><span class="linenos">331</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.copy-332"><a href="#Pathier.copy-332"><span class="linenos">332</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier.copy-333"><a href="#Pathier.copy-333"><span class="linenos">333</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
-</span><span id="Pathier.copy-334"><a href="#Pathier.copy-334"><span class="linenos">334</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
-</span><span id="Pathier.copy-335"><a href="#Pathier.copy-335"><span class="linenos">335</span></a>
-</span><span id="Pathier.copy-336"><a href="#Pathier.copy-336"><span class="linenos">336</span></a><span class="sd">        :param new_path: The copy destination.</span>
-</span><span id="Pathier.copy-337"><a href="#Pathier.copy-337"><span class="linenos">337</span></a>
-</span><span id="Pathier.copy-338"><a href="#Pathier.copy-338"><span class="linenos">338</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
-</span><span id="Pathier.copy-339"><a href="#Pathier.copy-339"><span class="linenos">339</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
-</span><span id="Pathier.copy-340"><a href="#Pathier.copy-340"><span class="linenos">340</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier.copy-341"><a href="#Pathier.copy-341"><span class="linenos">341</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-342"><a href="#Pathier.copy-342"><span class="linenos">342</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.copy-343"><a href="#Pathier.copy-343"><span class="linenos">343</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-344"><a href="#Pathier.copy-344"><span class="linenos">344</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.copy-345"><a href="#Pathier.copy-345"><span class="linenos">345</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.copy-346"><a href="#Pathier.copy-346"><span class="linenos">346</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier.copy-347"><a href="#Pathier.copy-347"><span class="linenos">347</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier.copy-348"><a href="#Pathier.copy-348"><span class="linenos">348</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier.copy-349"><a href="#Pathier.copy-349"><span class="linenos">349</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-350"><a href="#Pathier.copy-350"><span class="linenos">350</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier.copy-351"><a href="#Pathier.copy-351"><span class="linenos">351</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.copy-352"><a href="#Pathier.copy-352"><span class="linenos">352</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-353"><a href="#Pathier.copy-353"><span class="linenos">353</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-354"><a href="#Pathier.copy-354"><span class="linenos">354</span></a>        <span class="k">return</span> <span class="n">new_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-330"><a href="#Pathier.copy-330"><span class="linenos">330</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier.copy-331"><a href="#Pathier.copy-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier.copy-332"><a href="#Pathier.copy-332"><span class="linenos">332</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.copy-333"><a href="#Pathier.copy-333"><span class="linenos">333</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier.copy-334"><a href="#Pathier.copy-334"><span class="linenos">334</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
+</span><span id="Pathier.copy-335"><a href="#Pathier.copy-335"><span class="linenos">335</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
+</span><span id="Pathier.copy-336"><a href="#Pathier.copy-336"><span class="linenos">336</span></a>
+</span><span id="Pathier.copy-337"><a href="#Pathier.copy-337"><span class="linenos">337</span></a><span class="sd">        :param new_path: The copy destination.</span>
+</span><span id="Pathier.copy-338"><a href="#Pathier.copy-338"><span class="linenos">338</span></a>
+</span><span id="Pathier.copy-339"><a href="#Pathier.copy-339"><span class="linenos">339</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
+</span><span id="Pathier.copy-340"><a href="#Pathier.copy-340"><span class="linenos">340</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
+</span><span id="Pathier.copy-341"><a href="#Pathier.copy-341"><span class="linenos">341</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier.copy-342"><a href="#Pathier.copy-342"><span class="linenos">342</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-343"><a href="#Pathier.copy-343"><span class="linenos">343</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.copy-344"><a href="#Pathier.copy-344"><span class="linenos">344</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-345"><a href="#Pathier.copy-345"><span class="linenos">345</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.copy-346"><a href="#Pathier.copy-346"><span class="linenos">346</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.copy-347"><a href="#Pathier.copy-347"><span class="linenos">347</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier.copy-348"><a href="#Pathier.copy-348"><span class="linenos">348</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier.copy-349"><a href="#Pathier.copy-349"><span class="linenos">349</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier.copy-350"><a href="#Pathier.copy-350"><span class="linenos">350</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-351"><a href="#Pathier.copy-351"><span class="linenos">351</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier.copy-352"><a href="#Pathier.copy-352"><span class="linenos">352</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.copy-353"><a href="#Pathier.copy-353"><span class="linenos">353</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-354"><a href="#Pathier.copy-354"><span class="linenos">354</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-355"><a href="#Pathier.copy-355"><span class="linenos">355</span></a>        <span class="k">return</span> <span class="n">new_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Copy the path pointed to by this instance
 to the instance pointed to by new_path using shutil.copyfile
 or shutil.copytree. Returns the new path.</p>
```

#### html2text {}

```diff
@@ -38,801 +38,801 @@
 ****** pathier ******
 ⁰ View Source
 1from .pathier import Pathier
 2
 3__all__ = ["Pathier"]
   ⁰
 class Pathier(pathlib.Path): View Source
-_14class Pathier(pathlib.Path):
-_15    """Subclasses the standard library pathlib.Path class."""
-_16
-_17    def __new__(cls, *args, **kwargs):
-_18        if cls is Pathier:
-_19            cls = WindowsPath if os.name == "nt" else PosixPath
-_20        self = cls._from_parts(args)
-_21        if not self._flavour.is_supported:
-_22            raise NotImplementedError(
-_23                "cannot instantiate %r on your system" % (cls.__name__,)
-_24            )
-_25        return self
-_26
-_27    #
+_15class Pathier(pathlib.Path):
+_16    """Subclasses the standard library pathlib.Path class."""
+_17
+_18    def __new__(cls, *args, **kwargs):
+_19        if cls is Pathier:
+_20            cls = WindowsPath if os.name == "nt" else PosixPath
+_21        self = cls._from_parts(args)
+_22        if not self._flavour.is_supported:
+_23            raise NotImplementedError(
+_24                "cannot instantiate %r on your system" % (cls.__name__,)
+_25            )
+_26        return self
+_27
+_28    #
 ===============================================stats===============================================
-_28    @property
-_29    def dob(self) -> datetime.datetime | None:
-_30        """Returns the creation date of this file
-_31        or directory as a dateime.datetime object."""
-_32        if self.exists():
-_33            return datetime.datetime.fromtimestamp(self.stat().st_ctime)
-_34        else:
-_35            return None
-_36
-_37    @property
-_38    def age(self) -> float | None:
-_39        """Returns the age in seconds of this file or directory."""
-_40        if self.exists():
-_41            return (datetime.datetime.now() - self.dob).total_seconds()
-_42        else:
-_43            return None
-_44
-_45    @property
-_46    def mod_date(self) -> datetime.datetime | None:
-_47        """Returns the modification date of this file
-_48        or directory as a datetime.datetime object."""
-_49        if self.exists():
-_50            return datetime.datetime.fromtimestamp(self.stat().st_mtime)
-_51        else:
-_52            return None
-_53
-_54    @property
-_55    def mod_delta(self) -> float | None:
-_56        """Returns how long ago in seconds this file
-_57        or directory was modified."""
-_58        if self.exists():
-_59            return (datetime.datetime.now() - self.mod_date).total_seconds()
-_60        else:
-_61            return None
-_62
-_63    def size(self, format: bool = False) -> int | str | None:
-_64        """Returns the size in bytes of this file or directory.
-_65        Returns None if this path doesn't exist.
-_66
-_67        :param format: If True, return value as a formatted string."""
-_68        if not self.exists():
-_69            return None
-_70        if self.is_file():
-_71            size = self.stat().st_size
-_72        if self.is_dir():
-_73            size = sum(file.stat().st_size for file in self.rglob("*.*"))
-_74        if format:
-_75            return self.format_size(size)
-_76        return size
-_77
-_78    @staticmethod
-_79    def format_size(size: int) -> str:
-_80        """Format 'size' with common file size abbreviations
-_81        and rounded to two decimal places.
-_82        >>> 1234 -> "1.23 kb" """
-_83        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-_84            if unit != "bytes":
-_85                size *= 0.001
-_86            if size < 1000 or unit == "pb":
-_87                return f"{round(size, 2)} {unit}"
-_88
-_89    def is_larger(self, path: Self) -> bool:
-_90        """Returns whether this file or folder is larger than
-_91        the one pointed to by 'path'."""
-_92        return self.size() > path.size()
-_93
-_94    def is_older(self, path: Self) -> bool:
-_95        """Returns whether this file or folder is older than
-_96        the one pointed to by 'path'."""
-_97        return self.dob < path.dob
-_98
-_99    def modified_more_recently(self, path: Self) -> bool:
-100        """Returns whether this file or folder was modified
-101        more recently than the one pointed to by 'path'."""
-102        return self.mod_date > path.mod_date
-103
-104    #
+_29    @property
+_30    def dob(self) -> datetime.datetime | None:
+_31        """Returns the creation date of this file
+_32        or directory as a dateime.datetime object."""
+_33        if self.exists():
+_34            return datetime.datetime.fromtimestamp(self.stat().st_ctime)
+_35        else:
+_36            return None
+_37
+_38    @property
+_39    def age(self) -> float | None:
+_40        """Returns the age in seconds of this file or directory."""
+_41        if self.exists():
+_42            return (datetime.datetime.now() - self.dob).total_seconds()
+_43        else:
+_44            return None
+_45
+_46    @property
+_47    def mod_date(self) -> datetime.datetime | None:
+_48        """Returns the modification date of this file
+_49        or directory as a datetime.datetime object."""
+_50        if self.exists():
+_51            return datetime.datetime.fromtimestamp(self.stat().st_mtime)
+_52        else:
+_53            return None
+_54
+_55    @property
+_56    def mod_delta(self) -> float | None:
+_57        """Returns how long ago in seconds this file
+_58        or directory was modified."""
+_59        if self.exists():
+_60            return (datetime.datetime.now() - self.mod_date).total_seconds()
+_61        else:
+_62            return None
+_63
+_64    def size(self, format: bool = False) -> int | str | None:
+_65        """Returns the size in bytes of this file or directory.
+_66        Returns None if this path doesn't exist.
+_67
+_68        :param format: If True, return value as a formatted string."""
+_69        if not self.exists():
+_70            return None
+_71        if self.is_file():
+_72            size = self.stat().st_size
+_73        if self.is_dir():
+_74            size = sum(file.stat().st_size for file in self.rglob("*.*"))
+_75        if format:
+_76            return self.format_size(size)
+_77        return size
+_78
+_79    @staticmethod
+_80    def format_size(size: int) -> str:
+_81        """Format 'size' with common file size abbreviations
+_82        and rounded to two decimal places.
+_83        >>> 1234 -> "1.23 kb" """
+_84        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+_85            if unit != "bytes":
+_86                size *= 0.001
+_87            if size < 1000 or unit == "pb":
+_88                return f"{round(size, 2)} {unit}"
+_89
+_90    def is_larger(self, path: Self) -> bool:
+_91        """Returns whether this file or folder is larger than
+_92        the one pointed to by 'path'."""
+_93        return self.size() > path.size()
+_94
+_95    def is_older(self, path: Self) -> bool:
+_96        """Returns whether this file or folder is older than
+_97        the one pointed to by 'path'."""
+_98        return self.dob < path.dob
+_99
+100    def modified_more_recently(self, path: Self) -> bool:
+101        """Returns whether this file or folder was modified
+102        more recently than the one pointed to by 'path'."""
+103        return self.mod_date > path.mod_date
+104
+105    #
 ===============================================navigation===============================================
-105    def mkcwd(self):
-106        """Make this path your current working directory."""
-107        os.chdir(self)
-108
-109    @property
-110    def in_PATH(self) -> bool:
-111        """Return True if this
-112        path is in sys.path."""
-113        return str(self) in sys.path
-114
-115    def add_to_PATH(self, index: int = 0):
-116        """Insert this path into sys.path
-117        if it isn't already there.
-118
-119        :param index: The index of sys.path
-120        to insert this path at."""
-121        path = str(self)
-122        if not self.in_PATH:
-123            sys.path.insert(index, path)
-124
-125    def append_to_PATH(self):
-126        """Append this path to sys.path
-127        if it isn't already there."""
-128        path = str(self)
-129        if not self.in_PATH:
-130            sys.path.append(path)
-131
-132    def remove_from_PATH(self):
-133        """Remove this path from sys.path
-134        if it's in sys.path."""
-135        if self.in_PATH:
-136            sys.path.remove(str(self))
-137
-138    def moveup(self, name: str) -> Self:
-139        """Return a new Pathier object that is a parent of this instance.
-140        'name' is case-sensitive and raises an exception if it isn't in
+106    def mkcwd(self):
+107        """Make this path your current working directory."""
+108        os.chdir(self)
+109
+110    @property
+111    def in_PATH(self) -> bool:
+112        """Return True if this
+113        path is in sys.path."""
+114        return str(self) in sys.path
+115
+116    def add_to_PATH(self, index: int = 0):
+117        """Insert this path into sys.path
+118        if it isn't already there.
+119
+120        :param index: The index of sys.path
+121        to insert this path at."""
+122        path = str(self)
+123        if not self.in_PATH:
+124            sys.path.insert(index, path)
+125
+126    def append_to_PATH(self):
+127        """Append this path to sys.path
+128        if it isn't already there."""
+129        path = str(self)
+130        if not self.in_PATH:
+131            sys.path.append(path)
+132
+133    def remove_from_PATH(self):
+134        """Remove this path from sys.path
+135        if it's in sys.path."""
+136        if self.in_PATH:
+137            sys.path.remove(str(self))
+138
+139    def moveup(self, name: str) -> Self:
+140        """Return a new Pathier object that is a parent of this instance.
+141        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-141        >>> p = Pathier("C:\some\directory\in\your\system")
-142        >>> print(p.moveup("directory"))
-143        >>> "C:\some\directory"
-144        >>> print(p.moveup("yeet"))
-145        >>> "Exception: yeet is not a parent of C:
+142        >>> p = Pathier("C:\some\directory\in\your\system")
+143        >>> print(p.moveup("directory"))
+144        >>> "C:\some\directory"
+145        >>> print(p.moveup("yeet"))
+146        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-146        if name not in self.parts:
-147            raise Exception(f"{name} is not a parent of {self}")
-148        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
-149
-150    def __sub__(self, levels: int) -> Self:
-151        """Return a new Pathier object moved up 'levels' number of parents
+147        if name not in self.parts:
+148            raise Exception(f"{name} is not a parent of {self}")
+149        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+150
+151    def __sub__(self, levels: int) -> Self:
+152        """Return a new Pathier object moved up 'levels' number of parents
 from the current path.
-152        >>> p = Pathier("C:\some\directory\in\your\system")
-153        >>> new_p = p - 3
-154        >>> print(new_p)
-155        >>> "C:\some\directory" """
-156        path = self
-157        for _ in range(levels):
-158            path = path.parent
-159        return path
-160
-161    def move_under(self, name: str) -> Self:
-162        """Return a new Pathier object such that the stem
-163        is one level below the folder 'name'.
-164        'name' is case-sensitive and raises an exception if it isn't in
+153        >>> p = Pathier("C:\some\directory\in\your\system")
+154        >>> new_p = p - 3
+155        >>> print(new_p)
+156        >>> "C:\some\directory" """
+157        path = self
+158        for _ in range(levels):
+159            path = path.parent
+160        return path
+161
+162    def move_under(self, name: str) -> Self:
+163        """Return a new Pathier object such that the stem
+164        is one level below the folder 'name'.
+165        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-165        >>> p = Pathier("a/b/c/d/e/f/g")
-166        >>> print(p.move_under("c"))
-167        >>> 'a/b/c/d'"""
-168        if name not in self.parts:
-169            raise Exception(f"{name} is not a parent of {self}")
-170        return self - (len(self.parts) - self.parts.index(name) - 2)
-171
-172    def separate(self, name: str, keep_name: bool = False) -> Self:
-173        """Return a new Pathier object that is the
-174        relative child path after 'name'.
-175        'name' is case-sensitive and raises an exception if it isn't in
+166        >>> p = Pathier("a/b/c/d/e/f/g")
+167        >>> print(p.move_under("c"))
+168        >>> 'a/b/c/d'"""
+169        if name not in self.parts:
+170            raise Exception(f"{name} is not a parent of {self}")
+171        return self - (len(self.parts) - self.parts.index(name) - 2)
+172
+173    def separate(self, name: str, keep_name: bool = False) -> Self:
+174        """Return a new Pathier object that is the
+175        relative child path after 'name'.
+176        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-176
-177        :param keep_name: If True, the returned path will start with 'name'.
-178        >>> p = Pathier("a/b/c/d/e/f/g")
-179        >>> print(p.separate("c"))
-180        >>> 'd/e/f/g'
-181        >>> print(p.separate("c", True))
-182        >>> 'c/d/e/f/g'"""
-183        if name not in self.parts:
-184            raise Exception(f"{name} is not a parent of {self}")
-185        if keep_name:
-186            return Pathier(*self.parts[self.parts.index(name) :])
-187        return Pathier(*self.parts[self.parts.index(name) + 1 :])
-188
-189    # ============================================write and
+177
+178        :param keep_name: If True, the returned path will start with 'name'.
+179        >>> p = Pathier("a/b/c/d/e/f/g")
+180        >>> print(p.separate("c"))
+181        >>> 'd/e/f/g'
+182        >>> print(p.separate("c", True))
+183        >>> 'c/d/e/f/g'"""
+184        if name not in self.parts:
+185            raise Exception(f"{name} is not a parent of {self}")
+186        if keep_name:
+187            return Pathier(*self.parts[self.parts.index(name) :])
+188        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+189
+190    # ============================================write and
 read============================================
-190    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+191    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-191        """Create this directory.
-192        Same as Path().mkdir() except
-193        'parents' and 'exist_ok' default
-194        to True instead of False."""
-195        super().mkdir(mode, parents, exist_ok)
-196
-197    def touch(self):
-198        """Create file and parents if necessary."""
-199        self.parent.mkdir()
-200        super().touch()
-201
-202    def write_text(
-203        self,
-204        data: Any,
-205        encoding: Any | None = None,
-206        errors: Any | None = None,
-207        newline: Any | None = None,
-208        parents: bool = True,
-209    ):
-210        """Write data to file. If a TypeError is raised, the function
-211        will attempt to case data to a str and try the write again.
-212        If a FileNotFoundError is raised and parents = True,
-213        self.parent will be created."""
-214        write = functools.partial(
-215            super().write_text,
-216            encoding=encoding,
-217            errors=errors,
-218            newline=newline,
-219        )
-220        try:
-221            write(data)
-222        except TypeError:
-223            data = str(data)
-224            write(data)
-225        except FileNotFoundError:
-226            if parents:
-227                self.parent.mkdir(parents=True)
-228                write(data)
-229            else:
-230                raise
-231        except Exception as e:
-232            raise
-233
-234    def write_bytes(self, data: bytes, parents: bool = True):
-235        """Write bytes to file.
-236
-237        :param parents: If True and the write operation fails
-238        with a FileNotFoundError, make the parent directory
-239        and retry the write."""
-240        try:
-241            super().write_bytes(data)
-242        except FileNotFoundError:
-243            if parents:
-244                self.parent.mkdir(parents=True)
-245                super().write_bytes(data)
-246            else:
-247                raise
-248        except Exception as e:
-249            raise
-250
-251    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+192        """Create this directory.
+193        Same as Path().mkdir() except
+194        'parents' and 'exist_ok' default
+195        to True instead of False."""
+196        super().mkdir(mode, parents, exist_ok)
+197
+198    def touch(self):
+199        """Create file and parents if necessary."""
+200        self.parent.mkdir()
+201        super().touch()
+202
+203    def write_text(
+204        self,
+205        data: Any,
+206        encoding: Any | None = None,
+207        errors: Any | None = None,
+208        newline: Any | None = None,
+209        parents: bool = True,
+210    ):
+211        """Write data to file. If a TypeError is raised, the function
+212        will attempt to case data to a str and try the write again.
+213        If a FileNotFoundError is raised and parents = True,
+214        self.parent will be created."""
+215        write = functools.partial(
+216            super().write_text,
+217            encoding=encoding,
+218            errors=errors,
+219            newline=newline,
+220        )
+221        try:
+222            write(data)
+223        except TypeError:
+224            data = str(data)
+225            write(data)
+226        except FileNotFoundError:
+227            if parents:
+228                self.parent.mkdir(parents=True)
+229                write(data)
+230            else:
+231                raise
+232        except Exception as e:
+233            raise
+234
+235    def write_bytes(self, data: bytes, parents: bool = True):
+236        """Write bytes to file.
+237
+238        :param parents: If True and the write operation fails
+239        with a FileNotFoundError, make the parent directory
+240        and retry the write."""
+241        try:
+242            super().write_bytes(data)
+243        except FileNotFoundError:
+244            if parents:
+245                self.parent.mkdir(parents=True)
+246                super().write_bytes(data)
+247            else:
+248                raise
+249        except Exception as e:
+250            raise
+251
+252    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-252        """Load json file."""
-253        return json.loads(self.read_text(encoding, errors))
-254
-255    def json_dumps(
-256        self,
-257        data: Any,
-258        encoding: Any | None = None,
-259        errors: Any | None = None,
-260        newline: Any | None = None,
-261        sort_keys: bool = False,
-262        indent: Any | None = None,
-263        default: Any | None = None,
-264        parents: bool = True,
-265    ) -> Any:
-266        """Dump data to json file."""
-267        self.write_text(
-268            json.dumps(data, indent=indent, default=default,
+253        """Load json file."""
+254        return json.loads(self.read_text(encoding, errors))
+255
+256    def json_dumps(
+257        self,
+258        data: Any,
+259        encoding: Any | None = None,
+260        errors: Any | None = None,
+261        newline: Any | None = None,
+262        sort_keys: bool = False,
+263        indent: Any | None = None,
+264        default: Any | None = None,
+265        parents: bool = True,
+266    ) -> Any:
+267        """Dump data to json file."""
+268        self.write_text(
+269            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-269            encoding,
-270            errors,
-271            newline,
-272            parents,
-273        )
-274
-275    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+270            encoding,
+271            errors,
+272            newline,
+273            parents,
+274        )
+275
+276    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-276        """Load toml file."""
-277        return tomlkit.loads(self.read_text(encoding, errors))
-278
-279    def toml_dumps(
-280        self,
-281        data: Any,
-282        encoding: Any | None = None,
-283        errors: Any | None = None,
-284        newline: Any | None = None,
-285        sort_keys: bool = False,
-286        parents: bool = True,
-287    ):
-288        """Dump data to toml file."""
-289        self.write_text(
-290            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+277        """Load toml file."""
+278        return tomlkit.loads(self.read_text(encoding, errors))
+279
+280    def toml_dumps(
+281        self,
+282        data: Any,
+283        encoding: Any | None = None,
+284        errors: Any | None = None,
+285        newline: Any | None = None,
+286        sort_keys: bool = False,
+287        parents: bool = True,
+288    ):
+289        """Dump data to toml file."""
+290        self.write_text(
+291            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-291        )
-292
-293    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+292        )
+293
+294    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-294        """Load a json or toml file based off this instance's suffix."""
-295        match self.suffix:
-296            case ".json":
-297                return self.json_loads(encoding, errors)
-298            case ".toml":
-299                return self.toml_loads(encoding, errors)
-300
-301    def dumps(
-302        self,
-303        data: Any,
-304        encoding: Any | None = None,
-305        errors: Any | None = None,
-306        newline: Any | None = None,
-307        sort_keys: bool = False,
-308        indent: Any | None = None,
-309        default: Any | None = None,
-310        parents: bool = True,
-311    ):
-312        """Dump data to a json or toml file based off this instance's
+295        """Load a json or toml file based off this instance's suffix."""
+296        match self.suffix:
+297            case ".json":
+298                return self.json_loads(encoding, errors)
+299            case ".toml":
+300                return self.toml_loads(encoding, errors)
+301
+302    def dumps(
+303        self,
+304        data: Any,
+305        encoding: Any | None = None,
+306        errors: Any | None = None,
+307        newline: Any | None = None,
+308        sort_keys: bool = False,
+309        indent: Any | None = None,
+310        default: Any | None = None,
+311        parents: bool = True,
+312    ):
+313        """Dump data to a json or toml file based off this instance's
 suffix."""
-313        match self.suffix:
-314            case ".json":
-315                self.json_dumps(
-316                    data, encoding, errors, newline, sort_keys, indent,
+314        match self.suffix:
+315            case ".json":
+316                self.json_dumps(
+317                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-317                )
-318            case ".toml":
-319                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+318                )
+319            case ".toml":
+320                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
-320
-321    def delete(self, missing_ok: bool = True):
-322        """Delete the file or folder pointed to by this instance.
-323        Uses self.unlink() if a file and uses shutil.rmtree() if a
+321
+322    def delete(self, missing_ok: bool = True):
+323        """Delete the file or folder pointed to by this instance.
+324        Uses self.unlink() if a file and uses shutil.rmtree() if a
 directory."""
-324        if self.is_file():
-325            self.unlink(missing_ok)
-326        elif self.is_dir():
-327            shutil.rmtree(self)
-328
-329    def copy(
-330        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-331    ) -> Self:
-332        """Copy the path pointed to by this instance
-333        to the instance pointed to by new_path using shutil.copyfile
-334        or shutil.copytree. Returns the new path.
-335
-336        :param new_path: The copy destination.
-337
-338        :param overwrite: If True, files already existing in new_path
-339        will be overwritten. If False, only files that don't exist in
+325        if self.is_file():
+326            self.unlink(missing_ok)
+327        elif self.is_dir():
+328            shutil.rmtree(self)
+329
+330    def copy(
+331        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+332    ) -> Self:
+333        """Copy the path pointed to by this instance
+334        to the instance pointed to by new_path using shutil.copyfile
+335        or shutil.copytree. Returns the new path.
+336
+337        :param new_path: The copy destination.
+338
+339        :param overwrite: If True, files already existing in new_path
+340        will be overwritten. If False, only files that don't exist in
 new_path
-340        will be copied."""
-341        new_path = Pathier(new_path)
-342        if self.is_dir():
-343            if overwrite or not new_path.exists():
-344                shutil.copytree(self, new_path, dirs_exist_ok=True)
-345            else:
-346                files = self.rglob("*.*")
-347                for file in files:
-348                    dst = new_path.with_name(file.name)
-349                    if not dst.exists():
-350                        shutil.copyfile(file, dst)
-351        elif self.is_file():
-352            if overwrite or not new_path.exists():
-353                shutil.copyfile(self, new_path)
-354        return new_path
+341        will be copied."""
+342        new_path = Pathier(new_path)
+343        if self.is_dir():
+344            if overwrite or not new_path.exists():
+345                shutil.copytree(self, new_path, dirs_exist_ok=True)
+346            else:
+347                files = self.rglob("*.*")
+348                for file in files:
+349                    dst = new_path.with_name(file.name)
+350                    if not dst.exists():
+351                        shutil.copyfile(file, dst)
+352        elif self.is_file():
+353            if overwrite or not new_path.exists():
+354                shutil.copyfile(self, new_path)
+355        return new_path
 Subclasses the standard library pathlib.Path class.
 Pathier()
 dob: datetime.datetime | None
 Returns the creation date of this file or directory as a dateime.datetime
 object.
 age: float | None
 Returns the age in seconds of this file or directory.
 mod_date: datetime.datetime | None
 Returns the modification date of this file or directory as a datetime.datetime
 object.
 mod_delta: float | None
 Returns how long ago in seconds this file or directory was modified.
 ⁰
 def size(self, format: bool = False) -> int | str | None: View Source
-63    def size(self, format: bool = False) -> int | str | None:
-64        """Returns the size in bytes of this file or directory.
-65        Returns None if this path doesn't exist.
-66
-67        :param format: If True, return value as a formatted string."""
-68        if not self.exists():
-69            return None
-70        if self.is_file():
-71            size = self.stat().st_size
-72        if self.is_dir():
-73            size = sum(file.stat().st_size for file in self.rglob("*.*"))
-74        if format:
-75            return self.format_size(size)
-76        return size
+64    def size(self, format: bool = False) -> int | str | None:
+65        """Returns the size in bytes of this file or directory.
+66        Returns None if this path doesn't exist.
+67
+68        :param format: If True, return value as a formatted string."""
+69        if not self.exists():
+70            return None
+71        if self.is_file():
+72            size = self.stat().st_size
+73        if self.is_dir():
+74            size = sum(file.stat().st_size for file in self.rglob("*.*"))
+75        if format:
+76            return self.format_size(size)
+77        return size
 Returns the size in bytes of this file or directory. Returns None if this path
 doesn't exist.
 * Parameters *
     * format: If True, return value as a formatted string.
 ⁰
 @staticmethod
 def format_size(size: int) -> str: View Source
-78    @staticmethod
-79    def format_size(size: int) -> str:
-80        """Format 'size' with common file size abbreviations
-81        and rounded to two decimal places.
-82        >>> 1234 -> "1.23 kb" """
-83        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-84            if unit != "bytes":
-85                size *= 0.001
-86            if size < 1000 or unit == "pb":
-87                return f"{round(size, 2)} {unit}"
+79    @staticmethod
+80    def format_size(size: int) -> str:
+81        """Format 'size' with common file size abbreviations
+82        and rounded to two decimal places.
+83        >>> 1234 -> "1.23 kb" """
+84        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+85            if unit != "bytes":
+86                size *= 0.001
+87            if size < 1000 or unit == "pb":
+88                return f"{round(size, 2)} {unit}"
 Format 'size' with common file size abbreviations and rounded to two decimal
 places.
 >>> 1234 -> "1.23 kb"
 ⁰
 def is_larger(self, path: Self) -> bool: View Source
-89    def is_larger(self, path: Self) -> bool:
-90        """Returns whether this file or folder is larger than
-91        the one pointed to by 'path'."""
-92        return self.size() > path.size()
+90    def is_larger(self, path: Self) -> bool:
+91        """Returns whether this file or folder is larger than
+92        the one pointed to by 'path'."""
+93        return self.size() > path.size()
 Returns whether this file or folder is larger than the one pointed to by
 'path'.
 ⁰
 def is_older(self, path: Self) -> bool: View Source
-94    def is_older(self, path: Self) -> bool:
-95        """Returns whether this file or folder is older than
-96        the one pointed to by 'path'."""
-97        return self.dob < path.dob
+95    def is_older(self, path: Self) -> bool:
+96        """Returns whether this file or folder is older than
+97        the one pointed to by 'path'."""
+98        return self.dob < path.dob
 Returns whether this file or folder is older than the one pointed to by 'path'.
 ⁰
 def modified_more_recently(self, path: Self) -> bool: View Source
-_99    def modified_more_recently(self, path: Self) -> bool:
-100        """Returns whether this file or folder was modified
-101        more recently than the one pointed to by 'path'."""
-102        return self.mod_date > path.mod_date
+100    def modified_more_recently(self, path: Self) -> bool:
+101        """Returns whether this file or folder was modified
+102        more recently than the one pointed to by 'path'."""
+103        return self.mod_date > path.mod_date
 Returns whether this file or folder was modified more recently than the one
 pointed to by 'path'.
 ⁰
 def mkcwd(self): View Source
-105    def mkcwd(self):
-106        """Make this path your current working directory."""
-107        os.chdir(self)
+106    def mkcwd(self):
+107        """Make this path your current working directory."""
+108        os.chdir(self)
 Make this path your current working directory.
 in_PATH: bool
 Return True if this path is in sys.path.
 ⁰
 def add_to_PATH(self, index: int = 0): View Source
-115    def add_to_PATH(self, index: int = 0):
-116        """Insert this path into sys.path
-117        if it isn't already there.
-118
-119        :param index: The index of sys.path
-120        to insert this path at."""
-121        path = str(self)
-122        if not self.in_PATH:
-123            sys.path.insert(index, path)
+116    def add_to_PATH(self, index: int = 0):
+117        """Insert this path into sys.path
+118        if it isn't already there.
+119
+120        :param index: The index of sys.path
+121        to insert this path at."""
+122        path = str(self)
+123        if not self.in_PATH:
+124            sys.path.insert(index, path)
 Insert this path into sys.path if it isn't already there.
 * Parameters *
     * index: The index of sys.path to insert this path at.
 ⁰
 def append_to_PATH(self): View Source
-125    def append_to_PATH(self):
-126        """Append this path to sys.path
-127        if it isn't already there."""
-128        path = str(self)
-129        if not self.in_PATH:
-130            sys.path.append(path)
+126    def append_to_PATH(self):
+127        """Append this path to sys.path
+128        if it isn't already there."""
+129        path = str(self)
+130        if not self.in_PATH:
+131            sys.path.append(path)
 Append this path to sys.path if it isn't already there.
 ⁰
 def remove_from_PATH(self): View Source
-132    def remove_from_PATH(self):
-133        """Remove this path from sys.path
-134        if it's in sys.path."""
-135        if self.in_PATH:
-136            sys.path.remove(str(self))
+133    def remove_from_PATH(self):
+134        """Remove this path from sys.path
+135        if it's in sys.path."""
+136        if self.in_PATH:
+137            sys.path.remove(str(self))
 Remove this path from sys.path if it's in sys.path.
 ⁰
 def moveup(self, name: str) -> Self: View Source
-138    def moveup(self, name: str) -> Self:
-139        """Return a new Pathier object that is a parent of this instance.
-140        'name' is case-sensitive and raises an exception if it isn't in
+139    def moveup(self, name: str) -> Self:
+140        """Return a new Pathier object that is a parent of this instance.
+141        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-141        >>> p = Pathier("C:\some\directory\in\your\system")
-142        >>> print(p.moveup("directory"))
-143        >>> "C:\some\directory"
-144        >>> print(p.moveup("yeet"))
-145        >>> "Exception: yeet is not a parent of C:
+142        >>> p = Pathier("C:\some\directory\in\your\system")
+143        >>> print(p.moveup("directory"))
+144        >>> "C:\some\directory"
+145        >>> print(p.moveup("yeet"))
+146        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-146        if name not in self.parts:
-147            raise Exception(f"{name} is not a parent of {self}")
-148        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+147        if name not in self.parts:
+148            raise Exception(f"{name} is not a parent of {self}")
+149        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
 Return a new Pathier object that is a parent of this instance. 'name' is case-
 sensitive and raises an exception if it isn't in self.parts.
 >>> p = Pathier("C:\some\directory\in\your\system")
 >>> print(p.moveup("directory"))
 >>> "C:\some\directory"
 >>> print(p.moveup("yeet"))
 >>> "Exception: yeet is not a parent of C:\some\directory\in\your\system"
 ⁰
 def move_under(self, name: str) -> Self: View Source
-161    def move_under(self, name: str) -> Self:
-162        """Return a new Pathier object such that the stem
-163        is one level below the folder 'name'.
-164        'name' is case-sensitive and raises an exception if it isn't in
+162    def move_under(self, name: str) -> Self:
+163        """Return a new Pathier object such that the stem
+164        is one level below the folder 'name'.
+165        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-165        >>> p = Pathier("a/b/c/d/e/f/g")
-166        >>> print(p.move_under("c"))
-167        >>> 'a/b/c/d'"""
-168        if name not in self.parts:
-169            raise Exception(f"{name} is not a parent of {self}")
-170        return self - (len(self.parts) - self.parts.index(name) - 2)
+166        >>> p = Pathier("a/b/c/d/e/f/g")
+167        >>> print(p.move_under("c"))
+168        >>> 'a/b/c/d'"""
+169        if name not in self.parts:
+170            raise Exception(f"{name} is not a parent of {self}")
+171        return self - (len(self.parts) - self.parts.index(name) - 2)
 Return a new Pathier object such that the stem is one level below the folder
 'name'. 'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
 >>> p = Pathier("a/b/c/d/e/f/g")
 >>> print(p.move_under("c"))
 >>> 'a/b/c/d'
 ⁰
 def separate(self, name: str, keep_name: bool = False) -> Self: View Source
-172    def separate(self, name: str, keep_name: bool = False) -> Self:
-173        """Return a new Pathier object that is the
-174        relative child path after 'name'.
-175        'name' is case-sensitive and raises an exception if it isn't in
+173    def separate(self, name: str, keep_name: bool = False) -> Self:
+174        """Return a new Pathier object that is the
+175        relative child path after 'name'.
+176        'name' is case-sensitive and raises an exception if it isn't in
 self.parts.
-176
-177        :param keep_name: If True, the returned path will start with 'name'.
-178        >>> p = Pathier("a/b/c/d/e/f/g")
-179        >>> print(p.separate("c"))
-180        >>> 'd/e/f/g'
-181        >>> print(p.separate("c", True))
-182        >>> 'c/d/e/f/g'"""
-183        if name not in self.parts:
-184            raise Exception(f"{name} is not a parent of {self}")
-185        if keep_name:
-186            return Pathier(*self.parts[self.parts.index(name) :])
-187        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+177
+178        :param keep_name: If True, the returned path will start with 'name'.
+179        >>> p = Pathier("a/b/c/d/e/f/g")
+180        >>> print(p.separate("c"))
+181        >>> 'd/e/f/g'
+182        >>> print(p.separate("c", True))
+183        >>> 'c/d/e/f/g'"""
+184        if name not in self.parts:
+185            raise Exception(f"{name} is not a parent of {self}")
+186        if keep_name:
+187            return Pathier(*self.parts[self.parts.index(name) :])
+188        return Pathier(*self.parts[self.parts.index(name) + 1 :])
 Return a new Pathier object that is the relative child path after 'name'.
 'name' is case-sensitive and raises an exception if it isn't in self.parts.
 * Parameters *
     * keep_name: If True, the returned path will start with 'name'. >>> p =
       Pathier("a/b/c/d/e/f/g") >>> print(p.separate("c")) >>> 'd/e/f/g' >>>
       print(p.separate("c", True)) >>> 'c/d/e/f/g'
 ⁰
 def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool = True):
 View Source
-190    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+191    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-191        """Create this directory.
-192        Same as Path().mkdir() except
-193        'parents' and 'exist_ok' default
-194        to True instead of False."""
-195        super().mkdir(mode, parents, exist_ok)
+192        """Create this directory.
+193        Same as Path().mkdir() except
+194        'parents' and 'exist_ok' default
+195        to True instead of False."""
+196        super().mkdir(mode, parents, exist_ok)
 Create this directory. Same as Path().mkdir() except 'parents' and 'exist_ok'
 default to True instead of False.
 ⁰
 def touch(self): View Source
-197    def touch(self):
-198        """Create file and parents if necessary."""
-199        self.parent.mkdir()
-200        super().touch()
+198    def touch(self):
+199        """Create file and parents if necessary."""
+200        self.parent.mkdir()
+201        super().touch()
 Create file and parents if necessary.
 ⁰
 def write_text(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 parents: bool = True): View Source
-202    def write_text(
-203        self,
-204        data: Any,
-205        encoding: Any | None = None,
-206        errors: Any | None = None,
-207        newline: Any | None = None,
-208        parents: bool = True,
-209    ):
-210        """Write data to file. If a TypeError is raised, the function
-211        will attempt to case data to a str and try the write again.
-212        If a FileNotFoundError is raised and parents = True,
-213        self.parent will be created."""
-214        write = functools.partial(
-215            super().write_text,
-216            encoding=encoding,
-217            errors=errors,
-218            newline=newline,
-219        )
-220        try:
-221            write(data)
-222        except TypeError:
-223            data = str(data)
-224            write(data)
-225        except FileNotFoundError:
-226            if parents:
-227                self.parent.mkdir(parents=True)
-228                write(data)
-229            else:
-230                raise
-231        except Exception as e:
-232            raise
+203    def write_text(
+204        self,
+205        data: Any,
+206        encoding: Any | None = None,
+207        errors: Any | None = None,
+208        newline: Any | None = None,
+209        parents: bool = True,
+210    ):
+211        """Write data to file. If a TypeError is raised, the function
+212        will attempt to case data to a str and try the write again.
+213        If a FileNotFoundError is raised and parents = True,
+214        self.parent will be created."""
+215        write = functools.partial(
+216            super().write_text,
+217            encoding=encoding,
+218            errors=errors,
+219            newline=newline,
+220        )
+221        try:
+222            write(data)
+223        except TypeError:
+224            data = str(data)
+225            write(data)
+226        except FileNotFoundError:
+227            if parents:
+228                self.parent.mkdir(parents=True)
+229                write(data)
+230            else:
+231                raise
+232        except Exception as e:
+233            raise
 Write data to file. If a TypeError is raised, the function will attempt to case
 data to a str and try the write again. If a FileNotFoundError is raised and
 parents = True, self.parent will be created.
 ⁰
 def write_bytes(self, data: bytes, parents: bool = True): View Source
-234    def write_bytes(self, data: bytes, parents: bool = True):
-235        """Write bytes to file.
-236
-237        :param parents: If True and the write operation fails
-238        with a FileNotFoundError, make the parent directory
-239        and retry the write."""
-240        try:
-241            super().write_bytes(data)
-242        except FileNotFoundError:
-243            if parents:
-244                self.parent.mkdir(parents=True)
-245                super().write_bytes(data)
-246            else:
-247                raise
-248        except Exception as e:
-249            raise
+235    def write_bytes(self, data: bytes, parents: bool = True):
+236        """Write bytes to file.
+237
+238        :param parents: If True and the write operation fails
+239        with a FileNotFoundError, make the parent directory
+240        and retry the write."""
+241        try:
+242            super().write_bytes(data)
+243        except FileNotFoundError:
+244            if parents:
+245                self.parent.mkdir(parents=True)
+246                super().write_bytes(data)
+247            else:
+248                raise
+249        except Exception as e:
+250            raise
 Write bytes to file.
 * Parameters *
     * parents: If True and the write operation fails with a FileNotFoundError,
       make the parent directory and retry the write.
 ⁰
 def json_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-251    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+252    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-252        """Load json file."""
-253        return json.loads(self.read_text(encoding, errors))
+253        """Load json file."""
+254        return json.loads(self.read_text(encoding, errors))
 Load json file.
 ⁰
 def json_dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 indent: typing.Any | None = None,
 default: typing.Any | None = None,
 parents: bool = True) -> Any: View Source
-255    def json_dumps(
-256        self,
-257        data: Any,
-258        encoding: Any | None = None,
-259        errors: Any | None = None,
-260        newline: Any | None = None,
-261        sort_keys: bool = False,
-262        indent: Any | None = None,
-263        default: Any | None = None,
-264        parents: bool = True,
-265    ) -> Any:
-266        """Dump data to json file."""
-267        self.write_text(
-268            json.dumps(data, indent=indent, default=default,
+256    def json_dumps(
+257        self,
+258        data: Any,
+259        encoding: Any | None = None,
+260        errors: Any | None = None,
+261        newline: Any | None = None,
+262        sort_keys: bool = False,
+263        indent: Any | None = None,
+264        default: Any | None = None,
+265        parents: bool = True,
+266    ) -> Any:
+267        """Dump data to json file."""
+268        self.write_text(
+269            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-269            encoding,
-270            errors,
-271            newline,
-272            parents,
-273        )
+270            encoding,
+271            errors,
+272            newline,
+273            parents,
+274        )
 Dump data to json file.
 ⁰
 def toml_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-275    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+276    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-276        """Load toml file."""
-277        return tomlkit.loads(self.read_text(encoding, errors))
+277        """Load toml file."""
+278        return tomlkit.loads(self.read_text(encoding, errors))
 Load toml file.
 ⁰
 def toml_dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 parents: bool = True): View Source
-279    def toml_dumps(
-280        self,
-281        data: Any,
-282        encoding: Any | None = None,
-283        errors: Any | None = None,
-284        newline: Any | None = None,
-285        sort_keys: bool = False,
-286        parents: bool = True,
-287    ):
-288        """Dump data to toml file."""
-289        self.write_text(
-290            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+280    def toml_dumps(
+281        self,
+282        data: Any,
+283        encoding: Any | None = None,
+284        errors: Any | None = None,
+285        newline: Any | None = None,
+286        sort_keys: bool = False,
+287        parents: bool = True,
+288    ):
+289        """Dump data to toml file."""
+290        self.write_text(
+291            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-291        )
+292        )
 Dump data to toml file.
 ⁰
 def loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-293    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+294    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-294        """Load a json or toml file based off this instance's suffix."""
-295        match self.suffix:
-296            case ".json":
-297                return self.json_loads(encoding, errors)
-298            case ".toml":
-299                return self.toml_loads(encoding, errors)
+295        """Load a json or toml file based off this instance's suffix."""
+296        match self.suffix:
+297            case ".json":
+298                return self.json_loads(encoding, errors)
+299            case ".toml":
+300                return self.toml_loads(encoding, errors)
 Load a json or toml file based off this instance's suffix.
 ⁰
 def dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 indent: typing.Any | None = None,
 default: typing.Any | None = None,
 parents: bool = True): View Source
-301    def dumps(
-302        self,
-303        data: Any,
-304        encoding: Any | None = None,
-305        errors: Any | None = None,
-306        newline: Any | None = None,
-307        sort_keys: bool = False,
-308        indent: Any | None = None,
-309        default: Any | None = None,
-310        parents: bool = True,
-311    ):
-312        """Dump data to a json or toml file based off this instance's
+302    def dumps(
+303        self,
+304        data: Any,
+305        encoding: Any | None = None,
+306        errors: Any | None = None,
+307        newline: Any | None = None,
+308        sort_keys: bool = False,
+309        indent: Any | None = None,
+310        default: Any | None = None,
+311        parents: bool = True,
+312    ):
+313        """Dump data to a json or toml file based off this instance's
 suffix."""
-313        match self.suffix:
-314            case ".json":
-315                self.json_dumps(
-316                    data, encoding, errors, newline, sort_keys, indent,
+314        match self.suffix:
+315            case ".json":
+316                self.json_dumps(
+317                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-317                )
-318            case ".toml":
-319                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+318                )
+319            case ".toml":
+320                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
 Dump data to a json or toml file based off this instance's suffix.
 ⁰
 def delete(self, missing_ok: bool = True): View Source
-321    def delete(self, missing_ok: bool = True):
-322        """Delete the file or folder pointed to by this instance.
-323        Uses self.unlink() if a file and uses shutil.rmtree() if a
+322    def delete(self, missing_ok: bool = True):
+323        """Delete the file or folder pointed to by this instance.
+324        Uses self.unlink() if a file and uses shutil.rmtree() if a
 directory."""
-324        if self.is_file():
-325            self.unlink(missing_ok)
-326        elif self.is_dir():
-327            shutil.rmtree(self)
+325        if self.is_file():
+326            self.unlink(missing_ok)
+327        elif self.is_dir():
+328            shutil.rmtree(self)
 Delete the file or folder pointed to by this instance. Uses self.unlink() if a
 file and uses shutil.rmtree() if a directory.
 ⁰
 def copy(
 self,
 new_path: Union[Self, pathlib.Path, str],
 overwrite: bool = False) -> Self: View Source
-329    def copy(
-330        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-331    ) -> Self:
-332        """Copy the path pointed to by this instance
-333        to the instance pointed to by new_path using shutil.copyfile
-334        or shutil.copytree. Returns the new path.
-335
-336        :param new_path: The copy destination.
-337
-338        :param overwrite: If True, files already existing in new_path
-339        will be overwritten. If False, only files that don't exist in
+330    def copy(
+331        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+332    ) -> Self:
+333        """Copy the path pointed to by this instance
+334        to the instance pointed to by new_path using shutil.copyfile
+335        or shutil.copytree. Returns the new path.
+336
+337        :param new_path: The copy destination.
+338
+339        :param overwrite: If True, files already existing in new_path
+340        will be overwritten. If False, only files that don't exist in
 new_path
-340        will be copied."""
-341        new_path = Pathier(new_path)
-342        if self.is_dir():
-343            if overwrite or not new_path.exists():
-344                shutil.copytree(self, new_path, dirs_exist_ok=True)
-345            else:
-346                files = self.rglob("*.*")
-347                for file in files:
-348                    dst = new_path.with_name(file.name)
-349                    if not dst.exists():
-350                        shutil.copyfile(file, dst)
-351        elif self.is_file():
-352            if overwrite or not new_path.exists():
-353                shutil.copyfile(self, new_path)
-354        return new_path
+341        will be copied."""
+342        new_path = Pathier(new_path)
+343        if self.is_dir():
+344            if overwrite or not new_path.exists():
+345                shutil.copytree(self, new_path, dirs_exist_ok=True)
+346            else:
+347                files = self.rglob("*.*")
+348                for file in files:
+349                    dst = new_path.with_name(file.name)
+350                    if not dst.exists():
+351                        shutil.copyfile(file, dst)
+352        elif self.is_file():
+353            if overwrite or not new_path.exists():
+354                shutil.copyfile(self, new_path)
+355        return new_path
 Copy the path pointed to by this instance to the instance pointed to by
 new_path using shutil.copyfile or shutil.copytree. Returns the new path.
 * Parameters *
     * new_path: The copy destination.
     * overwrite: If True, files already existing in new_path will be
       overwritten. If False, only files that don't exist in new_path will be
       copied.
```

### Comparing `pathier-0.7.0/docs/search.js` & `pathier-0.8.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `pathier-0.7.0/src/pathier/pathier.py` & `pathier-0.8.0/src/pathier/pathier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import functools
 import json
 import os
 import pathlib
 import shutil
 import sys
-from typing import Any, Self
+from typing import Any
 
 import tomlkit
+from typing_extensions import Self
 
 
 class Pathier(pathlib.Path):
     """Subclasses the standard library pathlib.Path class."""
 
     def __new__(cls, *args, **kwargs):
         if cls is Pathier:
```

### Comparing `pathier-0.7.0/LICENSE.txt` & `pathier-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathier-0.7.0/README.md` & `pathier-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pathier-0.7.0/pyproject.toml` & `pathier-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,65 +5,65 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7061 7468 6965 7222 0d0a 6465 7363   "pathier"..desc
 00000070: 7269 7074 696f 6e20 3d20 2245 7874 656e  ription = "Exten
 00000080: 6473 2074 6865 2073 7461 6e64 6172 6420  ds the standard 
 00000090: 6c69 6272 6172 7920 7061 7468 6c69 622e  library pathlib.
 000000a0: 5061 7468 2063 6c61 7373 2e22 0d0a 7665  Path class."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e37 2e30 220d  rsion = "0.7.0".
+000000b0: 7273 696f 6e20 3d20 2230 2e38 2e30 220d  rsion = "0.8.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
-000000d0: 203d 2022 3e3d 332e 3131 220d 0a64 6570   = ">=3.11"..dep
+000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 746f  endencies = ["to
 000000f0: 6d6c 6b69 7422 2c20 2270 7974 6573 7422  mlkit", "pytest"
-00000100: 2c20 2264 6174 6162 6173 6564 225d 0d0a  , "databased"]..
-00000110: 7265 6164 6d65 203d 2022 5245 4144 4d45  readme = "README
-00000120: 2e6d 6422 0d0a 6b65 7977 6f72 6473 203d  .md"..keywords =
-00000130: 205b 2270 6174 686c 6962 222c 2022 7061   ["pathlib", "pa
-00000140: 7468 222c 2022 6a73 6f6e 222c 2022 746f  th", "json", "to
-00000150: 6d6c 222c 2022 7368 7574 696c 222c 2022  ml", "shutil", "
-00000160: 6578 7465 6e64 6572 222c 2022 6578 7465  extender", "exte
-00000170: 6e73 696f 6e22 5d0d 0a63 6c61 7373 6966  nsion"]..classif
-00000180: 6965 7273 203d 205b 0d0a 2020 2020 2250  iers = [..    "P
-00000190: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001b0: 2033 222c 0d0a 2020 2020 224c 6963 656e   3",..    "Licen
-000001c0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000001d0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000001e0: 6522 2c0d 0a20 2020 2022 4f70 6572 6174  e",..    "Operat
-000001f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000200: 2049 6e64 6570 656e 6465 6e74 222c 0d0a   Independent",..
-00000210: 2020 2020 5d0d 0a0d 0a5b 5b70 726f 6a65      ]....[[proje
-00000220: 6374 2e61 7574 686f 7273 5d5d 0d0a 6e61  ct.authors]]..na
-00000230: 6d65 203d 2022 4d61 7474 204d 616e 6573  me = "Matt Manes
-00000240: 220d 0a65 6d61 696c 203d 2022 6d61 7474  "..email = "matt
-00000250: 6d61 6e65 7340 706d 2e6d 6522 0d0a 0d0a  manes@pm.me"....
-00000260: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
-00000270: 2248 6f6d 6570 6167 6522 203d 2022 6874  "Homepage" = "ht
-00000280: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000290: 2f6d 6174 742d 6d61 6e65 732f 7061 7468  /matt-manes/path
-000002a0: 6965 7222 0d0a 2244 6f63 756d 656e 7461  ier".."Documenta
-000002b0: 7469 6f6e 2220 3d20 2268 7474 7073 3a2f  tion" = "https:/
-000002c0: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
-000002d0: 2d6d 616e 6573 2f70 6174 6869 6572 2f74  -manes/pathier/t
-000002e0: 7265 652f 6d61 696e 2f64 6f63 7322 0d0a  ree/main/docs"..
-000002f0: 2253 6f75 7263 6520 636f 6465 2220 3d20  "Source code" = 
-00000300: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000310: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f70  com/matt-manes/p
-00000320: 6174 6869 6572 2f74 7265 652f 6d61 696e  athier/tree/main
-00000330: 2f73 7263 2f70 6174 6869 6572 220d 0a0d  /src/pathier"...
-00000340: 0a5b 746f 6f6c 2e70 7974 6573 742e 696e  .[tool.pytest.in
-00000350: 695f 6f70 7469 6f6e 735d 0d0a 6164 646f  i_options]..addo
-00000360: 7074 7320 3d20 5b0d 0a20 2020 2022 2d2d  pts = [..    "--
-00000370: 696d 706f 7274 2d6d 6f64 653d 696d 706f  import-mode=impo
-00000380: 7274 6c69 6222 2c0d 0a20 2020 205d 0d0a  rtlib",..    ]..
-00000390: 7079 7468 6f6e 7061 7468 203d 2022 7372  pythonpath = "sr
-000003a0: 6322 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463  c"....[tool.hatc
-000003b0: 682e 6275 696c 642e 7461 7267 6574 732e  h.build.targets.
-000003c0: 7364 6973 745d 0d0a 6578 636c 7564 6520  sdist]..exclude 
-000003d0: 3d20 5b0d 0a20 2020 2022 2e63 6f76 6572  = [..    ".cover
-000003e0: 6167 6522 2c0d 0a20 2020 2022 2e70 7974  age",..    ".pyt
-000003f0: 6573 745f 6361 6368 6522 2c0d 0a20 2020  est_cache",..   
-00000400: 2022 2e76 7363 6f64 6522 2c0d 0a20 2020   ".vscode",..   
-00000410: 2022 7465 7374 7322 2c0d 0a20 2020 2022   "tests",..    "
-00000420: 2e67 6974 6967 6e6f 7265 220d 0a20 2020  .gitignore"..   
-00000430: 205d 0d0a 5b70 726f 6a65 6374 2e73 6372   ]..[project.scr
-00000440: 6970 7473 5d                             ipts]
+00000100: 2c20 2274 7970 696e 675f 6578 7465 6e73  , "typing_extens
+00000110: 696f 6e73 225d 0d0a 7265 6164 6d65 203d  ions"]..readme =
+00000120: 2022 5245 4144 4d45 2e6d 6422 0d0a 6b65   "README.md"..ke
+00000130: 7977 6f72 6473 203d 205b 2270 6174 686c  ywords = ["pathl
+00000140: 6962 222c 2022 7061 7468 222c 2022 6a73  ib", "path", "js
+00000150: 6f6e 222c 2022 746f 6d6c 222c 2022 7368  on", "toml", "sh
+00000160: 7574 696c 222c 2022 6578 7465 6e64 6572  util", "extender
+00000170: 222c 2022 6578 7465 6e73 696f 6e22 5d0d  ", "extension"].
+00000180: 0a63 6c61 7373 6966 6965 7273 203d 205b  .classifiers = [
+00000190: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
+000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001b0: 7974 686f 6e20 3a3a 2033 222c 0d0a 2020  ython :: 3",..  
+000001c0: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
+000001d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000001e0: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
+000001f0: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
+00000200: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000210: 6465 6e74 222c 0d0a 2020 2020 5d0d 0a0d  dent",..    ]...
+00000220: 0a5b 5b70 726f 6a65 6374 2e61 7574 686f  .[[project.autho
+00000230: 7273 5d5d 0d0a 6e61 6d65 203d 2022 4d61  rs]]..name = "Ma
+00000240: 7474 204d 616e 6573 220d 0a65 6d61 696c  tt Manes"..email
+00000250: 203d 2022 6d61 7474 6d61 6e65 7340 706d   = "mattmanes@pm
+00000260: 2e6d 6522 0d0a 0d0a 5b70 726f 6a65 6374  .me"....[project
+00000270: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
+00000280: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
+00000290: 7468 7562 2e63 6f6d 2f6d 6174 742d 6d61  thub.com/matt-ma
+000002a0: 6e65 732f 7061 7468 6965 7222 0d0a 2244  nes/pathier".."D
+000002b0: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
+000002c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002d0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f70  com/matt-manes/p
+000002e0: 6174 6869 6572 2f74 7265 652f 6d61 696e  athier/tree/main
+000002f0: 2f64 6f63 7322 0d0a 2253 6f75 7263 6520  /docs".."Source 
+00000300: 636f 6465 2220 3d20 2268 7474 7073 3a2f  code" = "https:/
+00000310: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
+00000320: 2d6d 616e 6573 2f70 6174 6869 6572 2f74  -manes/pathier/t
+00000330: 7265 652f 6d61 696e 2f73 7263 2f70 6174  ree/main/src/pat
+00000340: 6869 6572 220d 0a0d 0a5b 746f 6f6c 2e70  hier"....[tool.p
+00000350: 7974 6573 742e 696e 695f 6f70 7469 6f6e  ytest.ini_option
+00000360: 735d 0d0a 6164 646f 7074 7320 3d20 5b0d  s]..addopts = [.
+00000370: 0a20 2020 2022 2d2d 696d 706f 7274 2d6d  .    "--import-m
+00000380: 6f64 653d 696d 706f 7274 6c69 6222 2c0d  ode=importlib",.
+00000390: 0a20 2020 205d 0d0a 7079 7468 6f6e 7061  .    ]..pythonpa
+000003a0: 7468 203d 2022 7372 6322 0d0a 0d0a 5b74  th = "src"....[t
+000003b0: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
+000003c0: 7461 7267 6574 732e 7364 6973 745d 0d0a  targets.sdist]..
+000003d0: 6578 636c 7564 6520 3d20 5b0d 0a20 2020  exclude = [..   
+000003e0: 2022 2e63 6f76 6572 6167 6522 2c0d 0a20   ".coverage",.. 
+000003f0: 2020 2022 2e70 7974 6573 745f 6361 6368     ".pytest_cach
+00000400: 6522 2c0d 0a20 2020 2022 2e76 7363 6f64  e",..    ".vscod
+00000410: 6522 2c0d 0a20 2020 2022 7465 7374 7322  e",..    "tests"
+00000420: 2c0d 0a20 2020 2022 2e67 6974 6967 6e6f  ,..    ".gitigno
+00000430: 7265 220d 0a20 2020 205d 0d0a 5b70 726f  re"..    ]..[pro
+00000440: 6a65 6374 2e73 6372 6970 7473 5d         ject.scripts]
```

### Comparing `pathier-0.7.0/PKG-INFO` & `pathier-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pathier
-Version: 0.7.0
+Version: 0.8.0
 Summary: Extends the standard library pathlib.Path class.
 Project-URL: Homepage, https://github.com/matt-manes/pathier
 Project-URL: Documentation, https://github.com/matt-manes/pathier/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/pathier/tree/main/src/pathier
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: extender,extension,json,path,pathlib,shutil,toml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Requires-Dist: databased
+Requires-Python: >=3.10
 Requires-Dist: pytest
 Requires-Dist: tomlkit
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # pathier
 
 Extends the standard library pathlib.Path class.
 
 ## Installation
```

