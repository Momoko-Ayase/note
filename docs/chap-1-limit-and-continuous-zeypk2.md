<h1>Chap 1. 极限与连续</h1>
<h2>1.1 函数</h2>
<h3>1. 集合</h3>
<p>定义：具有某种特定性质事物的总体</p>
<p>元素：组成集合的事物</p>
<p>（属于：<span class="language-math">a\in M</span>     不属于：<span class="language-math">a\notin M</span>）</p>
<p>表示方法：	(1) 列举法：<span class="language-math">A={\{a_1,a_2,...,a_n\}}=\{a_i\}^n_{i=1}</span></p>
<pre><code>	(2) 描述法：$M=\{x|x所具有的特征\}$
</code></pre>
<p>常见集合：<span class="language-math">\empty</span>, <span class="language-math">\mathbb{N}</span>, <span class="language-math">\mathbb{Z}</span>, <span class="language-math">\mathbb{Q}</span>, <span class="language-math">\mathbb{R}</span>, <span class="language-math">\mathbb{C}</span></p>
<blockquote>
<div class="language-math">M\text{为数集}\begin{cases}
	M^*\,\,\text{排除}0\\
	M^+\,\,\text{排除}0\text{和负数}\\
\end{cases}</div>
</blockquote>
<p><span class="language-math">(a,b)</span> <span class="language-math">[a,b]</span> <span class="language-math">(a,b]</span> <span class="language-math">[a,b)</span>						有限区间</p>
<p><span class="language-math">(-\infty ,\infty )</span> <span class="language-math">(-\infty ,b)</span> <span class="language-math">(-\infty ,b]</span> <span class="language-math">(a,\infty )</span> <span class="language-math">[a,\infty )</span>		无限区间</p>
<p>邻域：设<span class="language-math">a\in R</span>，<span class="language-math">\delta</span>为任一正数，则<span class="language-math">a</span>的<span class="language-math">\delta</span>邻域<span class="language-math">U(a,\delta )=\{x|a-\delta &lt;x&lt;a+\delta \}=\{x\in \mathbb{R}||x-a|&lt;\delta \}</span>，其中<span class="language-math">a</span>为邻域中心，<span class="language-math">\delta</span>为邻域半径</p>
<p><span class="language-math">a</span>的去心邻域<span class="language-math">\mathring{U}( a,\delta ) =\{ x\in \mathbb{R} |0&lt;|x-x_0|&lt;\delta \}</span>​</p>
<p>包含，相等     e.g. <span class="language-math">\mathbb{N} \subsetneqq \mathbb{Z} \subsetneqq \mathbb{Q} \subsetneqq \mathbb{R} \subsetneqq \mathbb{C}</span></p>
<p>两个集合间 并<span class="language-math">A\cup B</span>   交<span class="language-math">A\cap B</span>   差<span class="language-math">A\backslash B</span>（<span class="language-math">A</span>中的元素减去其中<span class="language-math">B</span>拥有的元素）   余(补)<span class="language-math">A^c</span>（即全集<span class="language-math">E\backslash A</span>)</p>
<p>直积（笛卡尔积）	<span class="language-math">A\times B=\{(x,y)|x\in A,y\in B\}</span></p>
<p><img src="assets/Untitled1-20230925123918-xczxps4.png" alt="Untitled1" /></p>
<pre><code>		$R\times R=\{(x,y)|x\in R,y\in R\}\xlongequal{\text{记作}}R^2$
</code></pre>
<h3>2. 映射（算子）</h3>
<p>对映射<span class="language-math">f:X\rightarrow Y</span>，若<span class="language-math">f(X)=Y</span>，则<span class="language-math">f</span>为<strong>满射</strong></p>
<blockquote>
<p><span class="language-math">f:X\rightarrow Y</span>   <span class="language-math">\forall x\in X\rightarrow y</span>(唯一确定), <span class="language-math">y\in Y</span>   <span class="language-math">f(x)=\{f(x)|\forall x\in X\}\subseteq Y</span></p>
</blockquote>
<p>若<span class="language-math">\forall x_1 , x_2 \in X</span>, <span class="language-math">x_1\ne x_2</span>，有<span class="language-math">f(x_1)\ne f(x_2)</span>，则<span class="language-math">f</span>为<strong>单射</strong>​</p>
<p>若<span class="language-math">f</span>既为满射又为单射，则<span class="language-math">f</span>为<strong>双射</strong>或<strong>一一映射</strong>​</p>
<p>e.g. 	<span class="language-math">X(\ne 0)\xrightarrow{f}Y</span>(数集)		<span class="language-math">f</span>称为<span class="language-math">X</span>上的<strong>泛函</strong></p>
<pre><code>$X(\ne 0)\xrightarrow{f}X$			$f$称为$X$上的**变换**

$X$(数集或点集)$\xrightarrow{f}\mathbb{R}$		$f$称为定义在$X$上的**函数**
</code></pre>
<p>对于<strong>双射</strong>：对于<span class="language-math">f:X\rightarrow Y</span>，<span class="language-math">f':Y\rightarrow X</span>为其<strong>逆映射</strong>​</p>
<h3>3. 函数：特殊的映射</h3>
<p>定义：设数集<span class="language-math">D\subset \mathbb{R}</span>，则称映射<span class="language-math">f:D\rightarrow \mathbb{R}</span>为定义在<span class="language-math">D</span>上的函数，记为<span class="language-math">y=f(x),x\in D</span>（自变量<span class="language-math">x</span>，因变量<span class="language-math">y</span>，定义域<span class="language-math">D</span>，值域<span class="language-math">f(D)</span>）</p>
<p>函数图形：<span class="language-math">C=\{(x,y)|y=f(x),x\in D\}\subset D\times f(D)</span>​</p>
<p>函数的表示方法：解析法、图像法、列表法</p>
<p>求函数定义域的几种方法：</p>
<ol>
<li>负数不开偶次方</li>
<li>分母不为零</li>
<li>对数的真数部分大于零</li>
<li><span class="language-math">\tan{x}</span>中<span class="language-math">x\ne k\pi +\frac{\pi}{2}</span>，<span class="language-math">\cot{x}</span>中<span class="language-math">x\ne k\pi</span>​</li>
<li><span class="language-math">\arcsin{x}</span>与<span class="language-math">\arccos{x}</span>中<span class="language-math">|x|\leqslant1</span>​</li>
<li>有限个函数之和的定义域为其中各函数定义域之交集</li>
</ol>
<p>如果自变量在定义域内任取一个数值时，对应的函数值总是只有一个，这种函数称为<strong>单值函数</strong>，否则称为<strong>多值函数</strong>​</p>
<p>特殊函数：</p>
<ol>
<li>
<p>符号函数：</p>
<div class="language-math">y=\text{sgn} \,x=\begin{cases}
	1, \quad\text{当}x&gt;0\\
	0, \quad\text{当}x=0\\
	-1, \quad\text{当}x&lt;0\\
\end{cases}</div>
<p><img src="assets/Untitled-20230925194918-5kbv7te.png" alt="Untitled-20230925194918-5kbv7te.png" /></p>
</li>
<li>
<p>取整函数：<span class="language-math">y=[x], x\in \mathbb{R}</span>（<span class="language-math">[x]</span>表示不超过<span class="language-math">x</span>的最大整数）</p>
<p><img src="assets/Untitled2-20230925200710-9n1r8kf.png" alt="Untitled2" /></p>
</li>
<li>
<p>狄利克雷函数：</p>
<div class="language-math">y=D\left( x \right) =\begin{cases}
	1, \text{当}x\text{为有理数}\\
	0, \text{当}x\text{为无理数}\\
\end{cases}</div>
</li>
<li>
<p>取最值函数：<span class="language-math">y=\max\{f(x),g(x)\}</span>，<span class="language-math">y=\min\{f(x),g(x)\}</span></p>
</li>
</ol>
<p>函数的特性：（设函数<span class="language-math">y=f(x), x\in D</span>，且有区间<span class="language-math">I\subset D</span>）</p>
<ol>
<li>
<p>有界性：</p>
<p><span class="language-math">\forall x\in D, \exists M&gt;0, s.t. |f(x)|\leqslant M</span>，称<span class="language-math">f(x)</span>为有界函数</p>
<p><span class="language-math">\forall x\in I, \exists M&gt;0, s.t. |f(x)|\leqslant M</span>，称<span class="language-math">f(x)</span>在<span class="language-math">I</span>上有界</p>
<p><img src="assets/Untitled3-20230925202538-oknvk74.png" alt="Untitled3" /></p>
<p>若<span class="language-math">M</span>不存在，则称<span class="language-math">f(x)</span>为无界函数或在<span class="language-math">I</span>上无界（仅有上界/下界也称无界）</p>
</li>
<li>
<p>单调性：<span class="language-math">\uparrow : x_1&gt;x_2\Rightarrow f(x_1)&gt;f(x_2)</span>     <span class="language-math">\downarrow : x_1&gt;x_2\Rightarrow f(x_1)&lt;f(x_2)</span>​</p>
</li>
<li>
<p>奇偶性：定义域<span class="language-math">D</span>关于原点对称<span class="language-math">\Rightarrow x\in D</span>，则<span class="language-math">-x\in D</span>     <span class="language-math">f(x)=f(-x)</span>偶   <span class="language-math">f(x)=-f(-x)</span>奇</p>
</li>
<li>
<p>周期性：<span class="language-math">x\in D\Rightarrow x+T\in D</span>，<span class="language-math">f(x+T)=f(x), \forall x\in D</span>，<span class="language-math">f(x)</span>以<span class="language-math">T</span>为周期</p>
<p>周期函数不一定存在最小正周期   任一有理数均为狄利克雷的周期，无最小正周期</p>
</li>
</ol>
<p>基本初等函数：</p>
<ol>
<li>
<p>幂函数</p>
<p><span class="language-math">y=x^\alpha</span>（<span class="language-math">\alpha</span>取定实数）</p>
<p><span class="language-math">y=x^3</span>，<span class="language-math">D=\mathbb{R}</span>，值域为<span class="language-math">\mathbb{R}</span>，奇函数，↑，无周期无界</p>
<p><span class="language-math">y=x^2</span>，偶函数，值域<span class="language-math">[0,+\infty)</span></p>
<p><span class="language-math">y=\sqrt{x}</span>，<span class="language-math">D=[0,+\infty)</span>，值域<span class="language-math">[0,+\infty)</span>，↑</p>
<p><span class="language-math">y=\frac{1}{x}</span>，<span class="language-math">D=\mathbb{R}^*</span>，值域<span class="language-math">\mathbb{R}^*</span>，奇函数，在<span class="language-math">(-\infty,0)</span>和<span class="language-math">(0,+\infty)</span>↓</p>
</li>
<li>
<p>指数</p>
<p><span class="language-math">y=a^x</span>（<span class="language-math">a&gt;0, a\ne1</span>)          <span class="language-math">a=\text{e}\Rightarrow y=\text{e}^x</span></p>
<p>case 1: <span class="language-math">a&gt;1</span>，↑，<span class="language-math">D=\mathbb{R}</span>，值域<span class="language-math">(0,+\infty)</span>​</p>
<p>case 2: $0&lt;a&lt;1<span class="language-math">，↓，</span>D=\mathbb{R}<span class="language-math">，值域</span>(0,+\infty)$</p>
</li>
<li>
<p>对数</p>
<p><span class="language-math">y=\log_ax</span>（<span class="language-math">a&gt;0,a\ne1)</span>   <span class="language-math">D=(0,+\infty)</span>          <span class="language-math">a=e\Rightarrow y=\log_ex=\ln x</span>​</p>
<p>case 1: <span class="language-math">a&gt;1</span>，↑</p>
<p>case 2: $0&lt;a&lt;1$，↓</p>
<blockquote>
<ol start="2">
<li>
<ol start="3">
<li>互为反函数</li>
</ol>
</li>
</ol>
</blockquote>
</li>
<li>
<p>三角函数</p>
</li>
</ol>
<p>‍</p>
