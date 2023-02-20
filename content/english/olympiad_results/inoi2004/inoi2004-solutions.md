---
draft: false
title: "Solutions INOI 2004"
job_nature: ""
category: ""
---

<div id="cont">
<h3 align="left">INOI 2004, Solutions</h3>
  


<h5 style="font-weight:bold">Question 1</h5>

<p> Finding whether a path exists is straightforward.  Start from
    the top left corner and, for each square, recursively explore
    all neighbours that are at most one unit higher or lower than
    the current square.  A path exists provided this recursive
    exploration reaches the bottom right corner.</p>

<p> To identify a path, enhance the recursive search by recording
    the direction from which you came.  For example, if your
    search takes you one square down, store the character
    <code>'u'</code> at the new position to say that you reached
    this square from the <em>up</em> direction.  In the end, you
    can follow the directions back from the bottom right square
    to reach the top left square.</p>

<p> Unfortunately, this provides the path that we wish to display
    in <em>reverse</em>.  Rather than reversing the path, we can
    reverse the direction of exploration!  Starting from the
    bottom right corner, we recursively explore all neighbours
    and see if we can reach the top left corner.  Now, the
    directions that we accumulate along the way provide a path
    from the top left corner to the bottom right corner</p>

<ul>

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr.c">C program for this solution</a>.

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahrcheck.c">C program to check that a solution is
     valid</a>.<br>

This program takes an input file name and output file name
as command line arguments and verifies if the solution
recorded in the output file is valid for this input.  For
instance:

<pre>
tahrcheck 1.in 1.out
</pre>

checks that the data in <code>1.out</code> correctly solves
the input instance <code>1.in</code>

<li> Test inputs and outputs:

<ul>

<li> 4x4 grid: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-1.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-1.out">Output</a>.

<li> 30x30 grid: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-2.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-2.out">Output</a>.

<li> 50x50 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-3.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-3.out">Output</a>.

<li> 60x60 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-4.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-4.out">Output</a>.

<li> 100x100 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-5.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-5.out">Output</a>.

<li> 200x200 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-6.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-6.out">Output</a>.

<li> 300x300 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-7.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-7.out">Output</a>.

<li> 600x600 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-8.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-8.out">Output</a>.

<li> 1000x1000 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-9.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-9.out">Output</a>.

<li> 1000x1000 grid:  <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-10.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-10.out">Output</a>.

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/tahr-data.zip">All test cases, zipped</a>.

</ul>


</ul>

<h5 style="font-weight:bold">Question 2</h5>

<p> From the problem statement, it is clear that wrestlers who
    win more matches should be ahead in the queue to meet the
    Rajah.  Thus, for <em>N</em> wrestlers, we can compute the
    outcome of all <em>N(N-1)</em> matches and record the number
    of matches won by each wrestler.  If we sort this list in
    descending order based on the number of wins, we are
    done.</p>

<p> What if a group of wrestlers have the same number of wins?
    How should we arrange such a group in the queue?  A little
    analysis shows that this cannot happen.  If wrestler
    <em>A</em> beats wrestler <em>B</em> and wrestler <em>B</em>
    beats wrestler <em>C</em>, then <em>A</em> also beats
    <em>C</em>!</p>

<p> To see this, let <em>sA</em>, <em>sB</em> and <em>sC</em>
    denote the strengths of <em>A</em>, <em>B</em> and <em>C</em>
    and let <em>rA</em>, <em>rB</em> and <em>rC</em> denote the
    power of their rings, respectively.   If <em>A</em> beat
    <em>B</em>, we know that <em>sA + rA*sB &gt; sB +
    rB*sA</em>.  If we collect the <em>sA</em> terms on the left
    and the <em>sB</em> terms on the right, we have <em>sA(1-rB)
    &gt; sB(1-rA)</em>, or <em>sA/(1-rA) &gt; sB/(1-rB)</em>.</p>

<p> Thus if <em>A</em> beats <em>B</em> and <em>B</em> beats
    <em>C</em>, we have <em>sA/(1-rA) &gt; sB/(1-rB)</em> and
    <em>sB/(1-rB) &gt; sC/(1-rC)</em>.  It is immediate that
    <em>sA/(1-rA) &gt; sC/(1-rC)</em>, so <em>A</em> beats
    <em>C</em>.</p>


<p> From this it follows that we can directly sort the wrestlers
    in descending order
    by  the value <em>s/(1-r)</em>, without computing the
    outcomes of all <em>N(N-1)</em> matches.</p>

<ul>

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-bsort.c">C program for this solution that
     uses bubble sort</a>.

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-qsort.c">C program for this solution that
     uses quicksort</a>.


<li> Test inputs and outputs:

<ul>


<li> 10 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-1.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-1.out">Output</a>.

<li> 20 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-2.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-2.out">Output</a>.

<li> 50 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-3.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-3.out">Output</a>.

<li> 100 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-4.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-3.out">Output</a>.

<li> 100 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-5.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-4.out">Output</a>.

<li> 200 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-6.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-5.out">Output</a>.

<li> 500 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-7.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-5.out">Output</a>.

<li> 1000 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-8.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-6.out">Output</a>.

<li> 5000 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-9.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-6.out">Output</a>.

<li> 10000 wrestlers: <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-10.in">Input</a>, <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-6.out">Output</a>.

<li> <a href="https://www.iarcs.org.in/inoi/2004/inoi2004/wrestler-data.zip">All test cases, zipped</a>.

</ul>


</ul>

<br />

</div>
