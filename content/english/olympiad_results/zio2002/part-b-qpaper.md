---
draft: false
title: "ZIO 2002"
job_nature: ""
category: ""
---

<div id="cont">
<h5 align="left">Zonal Informatics Olympiad 2002, Part B</h5>
<p style="font-weight: bold">Question Paper</p>

<p style="font-weight: bold">Instructions:</p>

<ol>

<li> <p>The test consists of two problems.  You have three hours
to work out and submit the solutions.</p>

<li> <p>Solutions must be in Pascal, C or C++.  Use only standard
features of language.  For evaluation, you will submit source
code that we will compile to test for correctness.</p>

<li> <p>Save the source code of your solution to the two problems
in separate files.  When you submit your solutions, you will be
asked to supply the file names of the source files.</p>

</ol>


<p style="font-weight: bold">Questions:</p>

<ol>

<li> <p>Write a program that reads an integer <em>n</em> as input
and prints out the decimal representation of <em>1/n</em>.  If
<em>1/n</em> is a recurring decimal, print out <em>two</em>
copies of the recurring portion.  You may assume that <em>n</em>
is between 1 and 10000.</p>

<p> Here are some sample inputs and outputs for this problem:</p>

<ul>

<li> <p><em>Input</em>: 2<br> 
<em>Output</em>: 0.50 or 0.5</p>

<li> <p><em>Input</em>: 3<br> 
<em>Output</em>: 0.33</p>

<li> <p><em>Input</em>: 5<br> 
<em>Output</em>: 0.20 or 0.2</p>

<li> <p><em>Input</em>: 7<br> 
<em>Output</em>: 0.142857142857</p>

<li> <p><em>Input</em>: 11<br> 
<em>Output</em>: 0.0909</p>

</ul>

<li> <p>Write a program that reads the following sequence of inputs:</p>

<ul>

<li> <p> An integer <em>n</em> between 1 and 10000</p>

<li> <p> <em>n</em> values of type real/float, to be stored in an
array <code><b>a</b></code> with index values in the range <code><b>[0..n-1]</b></code></p>

<li> <p> <em>n</em> integer values, to be stored in an array
<code><b>p</b></code></p>

</ul>

The <em>n</em> integer values stored in <tt>p</tt> represent a
rearrangement (permutation) of the integers from 0 to
<em>n-1</em>.  In other words, <code><b>p</b></code> contains
each integer from 0 to <em>n-1</em> exactly once, but not in any
particular order.</p>

The problem is to rearrange the elements of <code><b>a</b></code>
according to the rearrangement specified in
<code><b>p</b></code>.  For instance if <code><b>n =
3</b></code>, <code><b>a = [2.1, 3.5, 7.6]</b></code> and
<code><b>p = [2,1,0]</b></code>, then <code><b>a</b></code>
should be rearranged as <code><b>[7.6, 3.5, 2.1]</b></code>.  In
other words, <code><b>a[0]</b></code> is replaced by
<code><b>a[2]</b></code> because <code><b>p[0]=2</b></code>,
<code><b>a[1]</b></code> remains <code><b>a[1]</b></code> because
<code><b>p[1]=1</b></code> and <code><b>a[2]</b></code> is
replaced by <code><b>a[0]</b></code> because
<code><b>p[2]=0</b></code>.</p>

After rearranging the elements in <code><b>a</b></code> according
to <code><b>p</b></code>, your program should print out the
contents of <code><b>a</b></code> from <code><b>a[0]</b></code>
to <code><b>a[n-1]</b></code>.</p>

<p><strong>Important restriction</strong>: Your program should
not use any arrays other than <code><b>a</b></code> and
<code><b>p</b></code>.</p>

<p><strong>Note:</strong> You <em>must</em> store the rearranged
values in <code><b>a</b></code>.  It is not sufficient to just
print out the rearrangement.  The output should be printed using
a simple loop that runs through the rearranged version of
<code><b>a</b></code> from position 0 to position
<em>n-1</em>.</p>


Here are some sample inputs and outputs for this problem:</p>

<ul>

<li> <p><em>Input</em>:</p>

3 </p>
2.0<br>
3.5<br>
7.0</p>
2<br>
0<br>
1</p>

<em>Output</em></p>

7.0, 2.0, 3.5</p>


<li> <p><em>Input</em>:</p>

5</p>
2.0<br>
3.5<br>
7.0<br>
10.5<br>
13.0</p>
2<br>
4<br>
3<br>
1<br>
0</p>

<em>Output</em></p>

7.0, 13.0, 10.5, 3.5, 2.0</p>

</ul>


</ol>


