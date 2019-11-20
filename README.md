# Optimization-LinearProgramming-Python

<html>
<head><meta charset="utf-8" />

<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="&gt;&gt;-Linear-programming:">&gt;&gt; Linear programming:<a class="anchor-link" href="#&gt;&gt;-Linear-programming:">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>One of the Optimization topics is Linear Programming. In this category of optimization problems, both the cost function and all the restrictions are linear.</p>
<p>Linear programming (LP) is one of the simplest ways to perform optimization. We can solve some very complex optimization problems by making a few simplifying assumptions. As an analyst one is bound to come across applications and problems to be solved by Linear Programming.</p>
<p>It is a simple technique where we depict complex relationships through linear functions and then find the optimum points. The real relationships might be much more complex – but we can simplify them to linear relationships.</p>
<p>It could be a breakthrough method while solving optimization problems. One can use it to find Minimum cost expenditure, maximum profit gained, shortest path to travel, etc.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Simple-Example:">Simple Example:<a class="anchor-link" href="#Simple-Example:">&#182;</a></h1><blockquote><p>Here I am providing a simple example to illustrate solving a simple LP optimization problem.</p>
<blockquote><p>Find the maximal and minimal value of <strong>z = 3x + 4y</strong> subject to the following <strong>constraints</strong>:</p>
<blockquote><p>x + 2y &lt;= 14,</p>
<p>3x - y &gt;= 0,</p>
<p>x - y &lt;= 2</p>
</blockquote>
<p>Here we need to find <strong>optimum (Max/Min)</strong> solution for the <strong>Objective Function: z = 3x + 4y</strong>. First of all, we will convert constraints equations into more simpler way:
<img src="eqn.png" alt="alt txt" title="Simplified equation"></p>
<p>Now we will plot graph for these constraint equations.</p>
</blockquote>
</blockquote>
<p><img src="graph.png" alt="alt txt" title="Graph system"></p>
<blockquote><blockquote><p>The soltuion lies in the bounded (feasible) region. And the optimal solution is  @ either of these corners.</p>
<p>Its tabular repsentation to find the corner points.</p>
</blockquote>
</blockquote>
<p><img src="Table.png" alt="alt txt" title="Table"></p>
<blockquote><blockquote><blockquote><p>Solution for these corner points:</p>
<blockquote><p>(2, 6):      z = 3(2)   + 4(6)   =   6 + 24 =   30</p>
<p>(6, 4):      z = 3(6)   + 4(4)   = 18 + 16 =   34</p>
<p>(–1, –3):  z = 3(–1) + 4(–3) = –3 – 12 = –15</p>
<blockquote><p>Then the maximum of <strong>z = 34</strong> occurs at (6, 4),</p>
<p>and the minimum of <strong>z = –15</strong> occurs at (–1, –3).</p>
</blockquote>
</blockquote>
</blockquote>
</blockquote>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="&gt;&gt;-Common-terminologies-used-in-Linear-Programming">&gt;&gt; Common terminologies used in Linear Programming<a class="anchor-link" href="#&gt;&gt;-Common-terminologies-used-in-Linear-Programming">&#182;</a></h1><blockquote><p><strong>Decision Variables</strong>: The decision variables are the variables which will decide my output. They represent my ultimate solution. To solve any problem, we first need to identify the decision variables. For the above example, the total number of units for A and B denoted by X &amp; Y respectively are my decision variables.</p>
<p><strong>Objective Function</strong>: It is defined as the objective of making decisions. In the above example, the company wishes to increase the total profit represented by Z. So, profit is my objective function.</p>
<p><strong>Constraints</strong>: The constraints are the restrictions or limitations on the decision variables. They usually limit the value of the decision variables. In the above example, the limit on the availability of resources Milk and Choco are my constraints.</p>
<p><strong>Non-negativity restriction</strong>: For all linear programs, the decision variables should always take non-negative values. Which means the values for decision variables should be greater than or equal to 0.</p>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="&gt;&gt;-Solving-LP-problems:">&gt;&gt; Solving LP problems:<a class="anchor-link" href="#&gt;&gt;-Solving-LP-problems:">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<blockquote><p>There are many ways to solve a LP problem; like:- solving it throgh converting it to Standard Form, Graphical Method.
Out of which, Graphical Method is most popular method.</p>
<p>Additionally, we have multiple libraries for python that can help us soving a LP problem.
viz.</p>
<blockquote><p>1.) scipy.optimize.minimize</p>
<p>2.) scipy.optimize.linprog</p>
<p>3.) PuLP</p>
<p>4.) Analyzing graphs through plotting with Matplotlib</p>
<p>..... And there must be few other methods also.</p>
</blockquote>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="&gt;&gt;-Circumstances-in-which-we-apply-LP-technique-to-solve-our-daily-analytics-operation">&gt;&gt; Circumstances in which we apply LP technique to solve our daily analytics operation<a class="anchor-link" href="#&gt;&gt;-Circumstances-in-which-we-apply-LP-technique-to-solve-our-daily-analytics-operation">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>we use LP technique to solve the optimiziation cases:</p>
<blockquote><blockquote><p>When we want to get best outcome (such as <strong>maximum profit</strong> or <strong>lowest cost</strong>) in a mathematical model; considering whose <strong>requirements are represented by "linear relationships" </strong>.</p>
<p>When its <strong>objective function</strong> can be represented through a <strong> <u>linear function </u></strong>.
    and subject to subject to <strong><u>linear equality</u></strong> and <strong><u>linear inequality</u> constraints</strong>.</p>
<p>-&gt;It can be applied in following application indaily analytics operations:</p>
<blockquote><ol>
<li><p>Manufacturing industries use linear programming for <u>analyzing their supply chain operations</u>. Their motive is to <strong>maximize efficiency</strong> with <strong>minimum operation cost</strong>.</p>
</li>
<li><p>Linear programming is also used in <strong>organized retail</strong> for <u>shelf space optimization</u>. Since the number of products in the market have increased in leaps and bounds, it is important to understand what does the customer want.</p>
</li>
<li><p>Optimization is also used for <u>optimizing Delivery Routes</u>. This is an extension of the popular traveling salesman problem.</p>
</li>
<li>Optimizations is also used in <u>Machine Learning</u>. <strong>Supervised Learning</strong> works on the fundamental of linear programming.</li>
<li>There are many more applications of linear programming in <strong>real-world</strong> like applied by <strong>Shareholders, Sports, Stock Markets</strong>, etc.  </li>
</ol>
</blockquote>
</blockquote>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Question:">Question:<a class="anchor-link" href="#Question:">&#182;</a></h1>
</div>
</div>
</div>> A car company produces 2 models, model A and model B. Long-term projections indicate an expected demand of at least 100 model A cars and 80 model B cars each day. Because of limitations on production capacity, no more than 200 model A cars and 170 model B cars can be made daily. To satisfy a shipping contract, a total of at least 200 cars much be shipped each day. If each model A car sold results in a $2000 loss, but each model B car produces a $5000 profit, how many of each type should be made daily to maximize net profits?
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<blockquote><p>car models - <strong>A</strong> &amp; <strong>B</strong></p>
<p>*demand: A &gt;= 100 ; B &gt;= 80</p>
<p>*produce: A &lt;= 200 ; B &lt;= 170</p>
<blockquote><p>So, we can conclude that: <strong>200 &gt;= A &gt;= 100</strong>   and  <strong>170 &gt;= B &gt;= 80</strong></p>
</blockquote>
<p>*Shipping: A + B &gt;= 200</p>
<p>*objective function: <strong>( z = 5000B - 2000A )</strong></p>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="visualization-of-the-problem:">visualization of the problem:<a class="anchor-link" href="#visualization-of-the-problem:">&#182;</a></h1><blockquote><h1 id="The-solution-lies-in-the-feasible-region(-green-region)-------">The solution lies in the feasible region( green region) ------<a class="anchor-link" href="#The-solution-lies-in-the-feasible-region(-green-region)-------">&#182;</a></h1>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> 
<span class="kn">from</span> <span class="nn">matplotlib.pyplot</span> <span class="k">import</span> <span class="o">*</span>
<span class="kn">import</span> <span class="nn">numpy</span>
<span class="kn">from</span> <span class="nn">numpy</span> <span class="k">import</span> <span class="n">arange</span>

<span class="n">figure</span><span class="p">()</span>
<span class="n">A</span> <span class="o">=</span> <span class="n">arange</span><span class="p">(</span><span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>
<span class="n">B</span> <span class="o">=</span> <span class="n">arange</span><span class="p">(</span><span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>

<span class="c1"># constraint equation</span>

<span class="n">B1</span> <span class="o">=</span> <span class="mf">200.0</span> <span class="o">-</span> <span class="n">A</span>



<span class="n">xlim</span> <span class="o">=</span> <span class="p">(</span><span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">)</span>
<span class="n">ylim</span><span class="o">=</span> <span class="p">(</span><span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">)</span>
<span class="n">hlines</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;k&#39;</span><span class="p">)</span>
<span class="n">vlines</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="o">-</span><span class="mi">100</span><span class="p">,</span> <span class="mi">220</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;k&#39;</span><span class="p">)</span>
<span class="n">grid</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>

<span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;X-axis&#39;</span><span class="p">)</span>
<span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Y-axis&#39;</span><span class="p">)</span>

<span class="c1">#Plotting graph</span>

<span class="n">plot</span><span class="p">(</span><span class="n">A</span><span class="p">,</span> <span class="n">B1</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;b&#39;</span><span class="p">)</span>
<span class="n">axhline</span><span class="p">(</span><span class="n">y</span> <span class="o">=</span> <span class="mi">80</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;r&#39;</span><span class="p">)</span>
<span class="n">axhline</span><span class="p">(</span><span class="n">y</span> <span class="o">=</span> <span class="mi">170</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;m&#39;</span><span class="p">)</span>
<span class="n">axvline</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="mi">200</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;b&#39;</span><span class="p">)</span>
<span class="n">axvline</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="mi">100</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;g&#39;</span><span class="p">)</span>

<span class="n">title</span><span class="p">(</span><span class="s1">&#39;objective function: z = 5000B - 2000A with following constarints&#39;</span><span class="p">)</span>
<span class="n">legend</span><span class="p">([</span><span class="s1">&#39;A+B&gt;=200&#39;</span><span class="p">,</span><span class="s1">&#39;200&gt;=A&gt;=100&#39;</span><span class="p">,</span><span class="s1">&#39;170&gt;=B&gt;=80&#39;</span><span class="p">])</span>

<span class="c1"># get the co-ordinates of intersection points by mere visualisation</span>
<span class="n">A</span> <span class="o">=</span> <span class="p">[</span><span class="mf">200.0</span><span class="p">,</span><span class="mf">100.0</span><span class="p">,</span> <span class="mf">100.0</span><span class="p">,</span> <span class="mf">120.0</span><span class="p">,</span><span class="mf">200.0</span><span class="p">]</span>
<span class="n">B</span> <span class="o">=</span> <span class="p">[</span><span class="mf">170.0</span><span class="p">,</span> <span class="mf">170.0</span><span class="p">,</span> <span class="mf">100.0</span><span class="p">,</span> <span class="mf">80.0</span><span class="p">,</span> <span class="mf">80.0</span><span class="p">]</span>
<span class="n">fill</span><span class="p">(</span><span class="n">A</span><span class="p">,</span><span class="n">B</span><span class="p">,</span><span class="s1">&#39;g+&#39;</span><span class="p">)</span>


<span class="n">show</span><span class="p">()</span>

<span class="c1">#Getting Solution</span>
<span class="n">checker</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">A</span><span class="p">,</span><span class="n">B</span><span class="p">):</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1"> calculating for point: A = </span><span class="si">{0:f}</span><span class="s1"> and B = </span><span class="si">{1:f}</span><span class="s1">&#39;</span> <span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">i</span><span class="p">,</span><span class="n">j</span><span class="p">))</span>
    <span class="nb">print</span><span class="p">(</span><span class="s1">&#39;solution for z = &#39;</span><span class="p">,</span> <span class="mi">5000</span><span class="o">*</span><span class="n">j</span><span class="o">-</span><span class="mi">2000</span><span class="o">*</span><span class="n">i</span><span class="p">)</span>
    <span class="k">if</span><span class="p">(</span><span class="n">checker</span> <span class="o">&lt;=</span> <span class="p">(</span><span class="mi">5000</span><span class="o">*</span><span class="n">j</span><span class="o">-</span><span class="mi">2000</span><span class="o">*</span><span class="n">i</span><span class="p">)):</span>
       <span class="n">checker</span> <span class="o">=</span> <span class="p">(</span><span class="mi">5000</span><span class="o">*</span><span class="n">j</span><span class="o">-</span><span class="mi">2000</span><span class="o">*</span><span class="n">i</span><span class="p">)</span>
       <span class="n">X</span><span class="p">,</span><span class="n">Y</span> <span class="o">=</span> <span class="n">i</span><span class="p">,</span><span class="n">j</span>
       
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1"> the maximum profit z = $</span><span class="si">{0:f}</span><span class="s1"> @ A = </span><span class="si">{1:f}</span><span class="s1"> and B = </span><span class="si">{2:f}</span><span class="s1">&#39;</span> <span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">checker</span><span class="p">,</span><span class="n">X</span><span class="p">,</span><span class="n">Y</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

### Output::::::::::::
![Output for Question](https://github.com/Atul-Anand-Jha/Optimization-LinearProgramming-Python/blob/master/output-graph.png "Output-graph")


</div>

</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Solving-using-library-PULP:">Solving using library PULP:<a class="anchor-link" href="#Solving-using-library-PULP:">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">from</span> <span class="nn">pulp</span> <span class="k">import</span> <span class="o">*</span>
<span class="c1"># declare your variables</span>
<span class="n">A</span> <span class="o">=</span> <span class="n">LpVariable</span><span class="p">(</span><span class="s2">&quot;A&quot;</span><span class="p">,</span> <span class="mi">100</span><span class="p">,</span> <span class="mi">200</span><span class="p">)</span>   <span class="c1"># 100 &lt;= A &lt;= 200</span>
<span class="n">B</span> <span class="o">=</span> <span class="n">LpVariable</span><span class="p">(</span><span class="s2">&quot;B&quot;</span><span class="p">,</span> <span class="mi">80</span><span class="p">,</span> <span class="mi">170</span><span class="p">)</span> <span class="c1"># 80 &lt;= B &lt;= 170</span>
 
<span class="c1"># defines the problem: optimization - Maximization</span>
<span class="n">prob</span> <span class="o">=</span> <span class="n">LpProblem</span><span class="p">(</span><span class="s2">&quot;problem&quot;</span><span class="p">,</span> <span class="n">LpMaximize</span><span class="p">)</span>
 
<span class="c1"># defines the constraints</span>
<span class="n">prob</span> <span class="o">+=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span> <span class="o">&gt;=</span><span class="mi">200</span> 
<span class="n">prob</span> <span class="o">+=</span> <span class="n">A</span><span class="o">&lt;=</span><span class="mi">200</span>
<span class="n">prob</span> <span class="o">+=</span> <span class="n">A</span><span class="o">&gt;=</span><span class="mi">100</span>
<span class="n">prob</span> <span class="o">+=</span> <span class="n">B</span><span class="o">&gt;=</span><span class="mi">80</span>
<span class="n">prob</span> <span class="o">+=</span> <span class="n">B</span><span class="o">&lt;=</span><span class="mi">170</span>
 
<span class="c1"># defines the objective function to maximize</span>
<span class="n">prob</span> <span class="o">+=</span> <span class="mi">5000</span><span class="o">*</span><span class="n">B</span><span class="o">-</span><span class="mi">2000</span><span class="o">*</span><span class="n">A</span>
 
<span class="c1"># solve the problem</span>
<span class="n">status</span> <span class="o">=</span> <span class="n">prob</span><span class="o">.</span><span class="n">solve</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;printing status of the LP problem: &#39;</span><span class="p">,</span> <span class="n">LpStatus</span><span class="p">[</span><span class="n">status</span><span class="p">])</span>
 
<span class="c1"># print the results A = 100, B = 170</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Value of model A car: &#39;</span><span class="p">,</span> <span class="n">value</span><span class="p">(</span><span class="n">A</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Value of model B car: &#39;</span><span class="p">,</span> <span class="n">value</span><span class="p">(</span><span class="n">B</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;the optimal solution or say maximum profit: $&#39;</span><span class="p">,</span> <span class="n">value</span><span class="p">(</span><span class="n">prob</span><span class="o">.</span><span class="n">objective</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>

### Output::::::::::::
<div class="output_subarea output_stream output_stdout output_text">
<pre>printing status of the LP problem:  Optimal
Value of model A car:  100.0
Value of model B car:  170.0
the optimal solution or say maximum profit: $ 650000.0
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Solving-using-Scipy-Library:">Solving using Scipy Library:<a class="anchor-link" href="#Solving-using-Scipy-Library:">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">from</span> <span class="nn">scipy.optimize</span> <span class="k">import</span> <span class="n">minimize</span>

<span class="c1">#defining our Objective function</span>
<span class="k">def</span> <span class="nf">objective</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="n">A</span> <span class="o">=</span> <span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
    <span class="n">B</span> <span class="o">=</span> <span class="n">x</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
    <span class="c1">#since we are finding Max result using Minimizer. So returned the negative value.</span>
    <span class="k">return</span> <span class="o">-</span><span class="p">(</span><span class="mi">5000</span><span class="o">*</span><span class="n">B</span><span class="o">-</span><span class="mi">2000</span><span class="o">*</span><span class="n">A</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">constraint</span><span class="p">(</span><span class="n">x</span><span class="p">):</span>
    <span class="k">return</span> <span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">+</span><span class="n">x</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">-</span><span class="mi">200</span>

<span class="c1">#boundations</span>

<span class="n">b1</span> <span class="o">=</span> <span class="p">[</span><span class="mi">100</span><span class="p">,</span> <span class="mi">200</span><span class="p">]</span>     <span class="c1">#bounds on A: 200 &gt;= A &gt;= 100</span>
<span class="n">b2</span> <span class="o">=</span> <span class="p">[</span><span class="mi">80</span><span class="p">,</span> <span class="mi">170</span><span class="p">]</span>      <span class="c1">#bounds on B: 170 &gt;= B &gt;= 80</span>

<span class="n">bnds</span> <span class="o">=</span> <span class="p">(</span><span class="n">b1</span><span class="p">,</span><span class="n">b2</span><span class="p">)</span>

<span class="c1">#defining Inequality type of constraint.</span>
<span class="n">con</span> <span class="o">=</span> <span class="p">{</span><span class="s1">&#39;type&#39;</span><span class="p">:</span> <span class="s1">&#39;ineq&#39;</span><span class="p">,</span> <span class="s1">&#39;fun&#39;</span><span class="p">:</span> <span class="n">constraint</span><span class="p">}</span>

<span class="c1"># passing any guess value for A and B into minimize fuinction.</span>
<span class="n">Xguess</span> <span class="o">=</span> <span class="p">[</span><span class="mi">100</span><span class="p">,</span><span class="mi">100</span><span class="p">]</span>

<span class="c1">#Predicting Maximization values for the objective function by seeding guess value Xguess; boundations included..</span>
<span class="n">sol</span> <span class="o">=</span> <span class="n">minimize</span><span class="p">(</span><span class="n">objective</span><span class="p">,</span> <span class="n">Xguess</span><span class="p">,</span> <span class="n">method</span> <span class="o">=</span> <span class="s1">&#39;SLSQP&#39;</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;disp&#39;</span><span class="p">:</span><span class="kc">True</span><span class="p">},</span> <span class="n">bounds</span> <span class="o">=</span> <span class="n">bnds</span><span class="p">,</span> <span class="n">constraints</span> <span class="o">=</span> <span class="n">con</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;About solution from Optimize.minnimize: </span><span class="se">\n</span><span class="s1">&#39;</span> <span class="p">,</span><span class="n">sol</span><span class="p">)</span>


<span class="c1">#assigning values to desired results.</span>
<span class="n">profit</span> <span class="o">=</span> <span class="o">-</span><span class="n">sol</span><span class="o">.</span><span class="n">fun</span>   <span class="c1">#converting back to positive answer</span>
<span class="n">CarA</span> <span class="o">=</span> <span class="n">sol</span><span class="o">.</span><span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>     <span class="c1"># number of car A models</span>
<span class="n">CarB</span> <span class="o">=</span> <span class="n">sol</span><span class="o">.</span><span class="n">x</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>     <span class="c1"># number of car B models</span>

<span class="c1">###################################################################</span>

<span class="nb">print</span> <span class="p">(</span><span class="s1">&#39;</span><span class="se">\n\n\n</span><span class="s1">Printing the Results: </span><span class="se">\n\n\n</span><span class="s1">&#39;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;maximum Profit Gained: $&#39;</span><span class="p">,</span> <span class="n">profit</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1"> Number of Model A Cars: &#39;</span><span class="p">,</span><span class="n">CarA</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1"> Number of Model B Cars: &#39;</span><span class="p">,</span><span class="n">CarB</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>

### Output::::::::::::
<div class="output_subarea output_stream output_stdout output_text">

<pre>Positive directional derivative for linesearch    (Exit mode 8)
            Current function value: -650000.0
            Iterations: 7
            Function evaluations: 12
            Gradient evaluations: 3
About solution from Optimize.minnimize: 
      fun: -650000.0
     jac: array([ 2000., -5000.])
 message: &#39;Positive directional derivative for linesearch&#39;
    nfev: 12
     nit: 7
    njev: 3
  status: 8
 success: False
       x: array([ 100.,  170.])



Printing the Results: 



maximum Profit Gained: $ 650000.0

 Number of Model A Cars:  100.0

 Number of Model B Cars:  170.0
</pre>
</div>
</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>
