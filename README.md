<h1><a id="Big_O_Notation_0"></a>Big O Notation</h1>
<h2><a id="What_is_The_Big_O_Notation_1"></a>What is The Big O Notation?</h2>
<p>The Big O Notation, is a method of calculating the rate of growth of an algorithm. This allows programmers to assess the potential performance or complexity of an algorithm. The results of  the Big O Notation are based on the worst possible scenario of an algorithms result.</p>
<h2><a id="Why_is_the_worst_result_documented_4"></a>Why is the worst result documented?</h2>
<p>The Big O Notation has its focus on the worst possible scenario because of probability. An algorithm is more likely to break than to compile first time. An algorithm is less likely to compile on average, than break.<br>
Average Results are therefore unreliable data.The likelihood of code compilation breaking is higher, therefore the results are more reliable. If we have a program with a.search() algorithm which takes linear time to execute: The worst case is O(N), This may occur if the query is at the end of the list. This will likely happen. The best case is O(1), This may occur if the query is at the front of the list. This will become more unlikely as the code continues to run, showing more search items in the list.</p>
<h2><a id="How_is_The_Big_O_Notation_utilised_8"></a>How is The Big O Notation utilised?</h2>
<p>The Big O Notation describes the rate of growth of an algorithm over time. This is written out in as the equation O(). There are different types of the Big O Notation.</p>
<h3><a id="Constant_Time__O1_11"></a>Constant Time - O(1):</h3>
<p>O(1) is known as a Constant Time O <a href="http://Notation.It">Notation.It</a> describes an algorithms rate of growth over a constant time period. It is commonly associated with basic statements such as inserting / retrieving items into lists, assigning variables with values and so forth. Other simple statements include obtaining data from hashmaps using keys and determining boolean values in Binary.<br>
A Code Example of O(1) would be:</p>
<pre><code class="language-java">    <span class="hljs-keyword">long</span> dataValue = <span class="hljs-number">1</span>;
</code></pre>
<h3><a id="Linear_Time__ON_18"></a>Linear Time - O(N):</h3>
<p>O(N) is known as a Linear Time O Notation. It describes an algorithm rate of growth over a linear time period.<br>
It is commonly associated with algorithms within loops. The algorithm look executes N times. If the algorithm within the look is O(1), the operation time of the loop is NO(1). This is represented as O(N).</p>
<p>Common uses of Linear Algorithms include:</p>
<ul>
<li>Finding data within an unordered List.</li>
<li>Sorting data within arrays and lists.</li>
</ul>
<p>A Code Example of O(N) would be:</p>
<pre><code class="language-java">   <span class="hljs-keyword">for</span> (<span class="hljs-keyword">int</span> i = <span class="hljs-number">0</span>; i &lt; N; i++) {
       <span class="hljs-comment">// Do something</span>
   }
</code></pre>
<h3><a id="Quadratic_Time__ON2_33"></a>Quadratic Time - O(N^2)</h3>
<p>O(N^2) is known as a Quadratic Time O Notation. It describes an algorithm rate of growth over a Quadratic time period. It is commonly associated with algorithms within Nested loops. The algorithm look executes N times.<br>
For every outer loop, the nested loop recurses N times. The nested loop executes a total of N  N times.<br>
This is represented as O(NN) which equals O(N2). Quadratic Time Algorithms should be avoided as the complexity grows in quadratic time. The longer a Quadratic Algorithm is active, the longer it takes to perform operations.</p>
<p>Common uses of Quadratic Algorithm include:</p>
<ul>
<li>Finding data within a Matrix (A Two Dimensional Array).</li>
<li>Insertion sort algorithms.</li>
</ul>
<p>A Code Example of O(N^2) would be:</p>
<pre><code class="language-Java">    <span class="hljs-keyword">for</span> (<span class="hljs-keyword">int</span> i = <span class="hljs-number">0</span>; i &lt; N; i++) {
        <span class="hljs-keyword">for</span> (<span class="hljs-keyword">int</span> j = <span class="hljs-number">0</span>; j &lt; N; j++) {
            <span class="hljs-comment">// Do something</span>
        }
    }
</code></pre>
<h3><a id="Logarithmic_Time__OLog_N_51"></a>Logarithmic Time - O(Log N)</h3>
<p>O(Log N) is known as a Logarithmic Time O Notation. It describes an algorithm rate of growth over a Logarithmic time period. Unlike the Linear Time O Notation which is written similarly, Logarithmic Time gets slower as  N grows. A quick way to check if a Loop is in Log N would be to check whether the counting variable doubles, instead of increments of 1. The algorithm look executes N times. For every loop, the counting variable doubles with each loop. The loop executes in log(N) time. This is represented as O(Log N).<br>
Common uses of Quadratic Algorithm include:</p>
<ul>
<li>Binary Data Searches.</li>
<li>Insertion and Deleting data within Heap Data Structures…</li>
</ul>
<p>A Code Example of O(Log N) would be:</p>
<pre><code class="language-Java">    <span class="hljs-keyword">for</span>(<span class="hljs-keyword">int</span> i = <span class="hljs-number">0</span>; i &lt; n; i = <span class="hljs-number">2</span>) {
        <span class="hljs-comment">// Do Something</span>
    }
</code></pre>
<p>Logarithms can be seen as strange, intimidating and confusing. Logarithms are inverse operations of exponentiating input values. In simple terms, Logarithms are an opposite method of increasing input value powers. Logarithms are often used with input values are constantly halved or doubled. This makes Logarithms excellent for operation in large datasets.</p>
<h3><a id="Linearithmic_Time__ONLog_N_66"></a>Linearithmic Time - O(N*Log N)</h3>
<p>O(NLog N) is known as a Linearithmic Time period. It describes an algorithm rate of growth over a nested Logarithmic time period. Similar to Quadratic Time, Linearithmic is based on a nested loop algorithm. For every outer loop, the nested loop recurses log(N) times. The nested loop executes a total of N  Log(N) times. This is represented as O(NLog N).</p>
<p>Examples of Linearithmic Algorithms include:</p>
<ul>
<li>Heap Sort Algorithms.</li>
<li>Merge Sort Algorithms.</li>
<li>Quick Sort Algorithms.</li>
</ul>
<p>A Code Example of O(N*Log N)</p>
<pre><code class="language-Java">    <span class="hljs-keyword">for</span>(<span class="hljs-keyword">int</span> i = <span class="hljs-number">0</span>; i &lt; n; i++) {
        <span class="hljs-keyword">for</span>(<span class="hljs-keyword">int</span> j = <span class="hljs-number">1</span>; j &lt; n; j = <span class="hljs-number">2</span>){
            <span class="hljs-comment">// Do Something</span>
        }
    }
</code></pre>
