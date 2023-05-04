Download Link: https://assignmentchef.com/product/solved-cs5007-homework-4
<br>
<h1>1             Archimedean spiral</h1>

Using Pyplot and Numpy, state a function arc that draws a green Archimedean spiral according to the following parameterized equation:

<ul>

 <li><em>x</em>(<em>t</em>) = <em>cos</em>(<em>t</em>)</li>

 <li><em>y</em>(<em>t</em>) = <em>sin</em>(<em>t</em>)</li>

</ul>

<em>t </em>should vary in [0<em>,</em>5<em>π</em>] (step 0.01) and the function should call plt.plot with arguments <em>x </em>and <em>y</em>, as well as plt.show() function at the end. Call the function.

<h1>2             Heart</h1>

Using Pyplot and Numpy, state a function heart that draws in dashed red the following parameterized equation:

<ul>

 <li><em>x</em>(<em>t</em>) = 16<em>sin</em><sup>3</sup>(<em>t</em>)</li>

 <li><em>y</em>(<em>t</em>) = 13<em>cos</em>(<em>t</em>) − 5<em>cos</em>(2<em>t</em>) − 2<em>.</em>5<em>cos</em>(3<em>t</em>) − <em>cos</em>(4<em>t</em>)</li>

</ul>

<em>t </em>should vary in [0<em>,</em>2<em>π</em>] (step 0.01) and the function should call plt.plot with arguments <em>x </em>and <em>y</em>, as well as plt.show() function at the end. Call the function.

To see the result you should first close the window of part 1 (Archimedean spiral).

<h1>3             Graphs</h1>

We wish to use graph theory in order to solve the following problem. A company should carry different chemical products <em>P</em><sub>1</sub>, <em>P</em><sub>2</sub>, <em>…</em>, <em>P<sub>k </sub></em>from the factory to a city. For security reasons, some products should not be carried in the same truck: ∀<em>i,</em>0 <em>&lt; i &lt; k,P<sub>i </sub></em>is not compatible with <em>P<sub>i</sub></em><sub>+1</sub>. Moreover <em>P<sub>k </sub></em>is not compatible with <em>P</em><sub>1</sub>.

<ul>

 <li>Write a comment: how can we state an undirected graph that visually represents this problem: 1. What are the vertices, what are the edges? 2. What is the specific property of this graph?</li>

 <li>Write an algorithm that, given an integer <em>k &gt; </em>1, returns the minimum number of trucks necessary to carry all the products.</li>

</ul>

<h1>4             Algorithm</h1>

In ancient times, Egyptians did not use multiplication tables. Instead, they transformed any calculation into multiplication by two, and additions. The principle of Egyptian multiplication is the following: (<em>x </em>∗ <em>y</em>) = 2 ∗ (<em>x </em>∗ (<em>y/</em>2)) if y is even, and

(<em>x </em>∗ <em>y</em>) = <em>x </em>+ (<em>x </em>∗ (<em>y </em>− 1)) if y is odd. For instance,

(7 ∗ 10) = (2 ∗ (7 ∗ 5)) = (2 ∗ (7 + (7 ∗ 4))) = (2 ∗ (7 + (2 ∗ (7 ∗ 2))))<em>.</em>

Write a recursive Python function that, given two strictly positive integers x and y (the arguments of the function), returns the result of <em>x </em>∗ <em>y </em>obtained using the Egyptian method. Of course, directly multiplying <em>x </em>by <em>y </em>is allowed in your code if and only if <em>x </em>≤ 2 or <em>y </em>≤ 2.