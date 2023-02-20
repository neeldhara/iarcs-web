---
draft: false
title: "Question Paper ZCO 2010"
job_nature: ""
category: ""
---

<div id="cont">
<h6 align="left">Zonal Computing Olympiad, 2010</h6>
  

  <p>The Zonal Computing Olympiad, 2010 was held in two sessions on Saturday, December 12, 2009.  Students could take part in either session.  The questions for the two sessions were as follows.</p>

<h5 style="font-weight: bold;"> Session 1, 10:00 am&ndash;1:00 pm IST</h5> <hr>

<h5>Sequence Game</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2010, 12 Dec 2009</h6>
  <h6>10:00 am&ndash;1:00 pm IST</h6>

<h6>Problem 1 : Sequence game</h6>

<p>You are given a sequence of <em>N</em> positive
  integers <em>i<sub>1</sub></em>,
  <em>i<sub>2</sub></em>, &hellip;, <em>i<sub>N</sub></em>.  In
  addition, you are given a starting integer <em>b</em> and lower
  and upper integer limits <em>min</em> and <em>max</em>,
  respectively.  Note that 0&nbsp;&le;&nbsp;<em>min</em>&nbsp;&le;&nbsp;<em>b</em>&nbsp;&le;&nbsp;<em>max</em> always.
</p>

<p>The sequence game is played as follows.  Initially, your score
  is <em>b</em>.  In step 1, you can either add 
  <em>i<sub>1</sub></em> to <em>b</em> or
  subtract <em>i<sub>1</sub></em> from <em>b</em> to get a new
  score <em>b<sub>1</sub></em>.  In step 2, you
  update <em>b<sub>1</sub></em> by adding or
  subtracting <em>i<sub>2</sub></em> to get a new
  score <em>b<sub>2</sub></em>.  Proceeding in this way, in
  step <em>j</em>, you update <em>b<sub>j-1</sub></em> by adding
  or subtracting <em>i<sub>j</sub></em> to get a new
  score <em>b<sub>j</sub></em>.  The rule is that each
  score <em>b<sub>j</sub></em> should always lie
  between <em>min</em> and <em>max</em>, inclusive: that is,
  for each <em>j</em>, 1 &nbsp;&le;&nbsp; <em>j</em>
  &nbsp;&le;&nbsp; <em>N</em>, it should be the case that <em>min &nbsp;&le;&nbsp;
  b<sub>j</sub> &nbsp;&le;&nbsp; max</em>.  Your final score
  is <em>b<sub>N</sub></em>, after using the last number in the
  sequence.
</p>

<p>Your aim is to maximise your final score while playing
  according to the rules.  If there is no way to complete
  all <em>N</em> steps without going outside the
  bounds <em>min</em> and <em>max</em>, your score is -1.
</p>

<p>For example, suppose the sequence of numbers you have is
  [2,3,4], <em>b</em> is 5, <em>min</em> is 0 and <em>max</em> is
  8.  After step 1, the score can be 3 or 7.  After step 2, the
  score can be 0, 4, or 6.  A score of 10 is not allowed
  since <em>max</em> is 8.  After step 3, the score can be 0, 2,
  4, or 8.  Thus, in this game, the maximum score you can obtain
  at the end of the sequence is 8.
</p>

<h6>Input format</h6>

<p>The first line of the input contains four integers <em>N</em>,
  <em>b</em>, <em>min</em> and <em>max</em>, whose meaning is as
  explained above.  The second line of input contains <em>N</em>
  space separated integers, the sequence over which the game is
  played.
</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the maximum final score that you can achieve.</p>

<h6>Testdata</h6>

<p>In all cases, N&nbsp;&le;&nbsp;10<sup>3</sup> and
  0&nbsp;&le;&nbsp;<em>min</em>&nbsp;&le;&nbsp;<em>b</em>&nbsp;&le;&nbsp;<em>max</em>&nbsp;&le;&nbsp;10<sup>3</sup>.

<h6>Sample Input</h6>
<pre style="margin:15px">
3 5 0 8
2 3 4
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
8
</pre>

</div>

<h5>Library Committee</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2010, 12 Dec 2009</h6>
  <h6>10:00 am&ndash;1:00 pm IST</h6>

<h6>Problem 2 : Library Committee</h6>

<p>The Siruseri Public Library has a Library Committee with
  three members.  The financial year is coming to an end and
  there is a mad rush to spend this year's budget.  Each
  committee member has independently drawn up a list of books
  that he wants to order for the library.</p>

<p>For simplicity, each book is identified by a unique number, so
  each committee member's recommendation is a list of numbers, in
  some arbitrary order.  It is possible that two or more
  committee members have recommended the same book.  The numbers
  have the same meaning across lists, so if the same number
  appears in multiple lists, it denotes the same book.</p>

<p>For example, the three lists may be as follows:</p>

<ul>

<li> <p><em>Member 1:</em> [12,387,15,162,5]</p>

<li> <p><em>Member 2:</em> [14,162,92,387,7,748]</p>

<li> <p><em>Member 3:</em> [14,5,12,387]</p>

</ul>

<p>In this case, all three members have recommended book 387, only
  member 1 has recommended book 15, two members have recommended
  book 162 and so on.</p>

<p>There is enough money to buy all the books that have been
  recommended, but only one copy of each book may be purchased.
  Your task is to to calculate how many books, overall, are to be
  bought, given the three lists of recommended books. In this
  example, the answer is 9: the list of books to be ordered
  overall is [12,387,15,162,5,14,92,7,748]</p>

<h6>Input format</h6>

<p>The first line of the input contains three
  integers <em>N<sub>1</sub></em>, <em>N<sub>2</sub></em>
  and <em>N<sub>3</sub></em>, where <em>N<sub>j</sub></em> is the
  number of books recommended by committee member <em>j</em>, 1
  &le; <em>j</em> &le; 3.  This is followed by three lines of
  space separated integers.</p>

  <ul>

  <li> Line 2 of the input has <em>N<sub>1</sub></em> integers
    representing the recommendations of Member 1.

  <li> Line 3 of the input has <em>N<sub>2</sub></em> integers
    representing the recommendations of Member 2.

  <li> Line 4 of the input has <em>N<sub>3</sub></em> integers
    representing the recommendations of Member 3.

  </ul>
  
</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the total number of books to be ordered for the library.</p>

<h6>Testdata</h6>

<p>In all cases,
  1&nbsp;&le;&nbsp;<em>N</em><sub>1</sub>, <em>N</em><sub>2</sub>, <em>N</em><sub>3</sub>&nbsp;&le;&nbsp;10<sup>6</sup>. Also,
  each individual list is guaranteed to be free of duplicate
  entries.
</p>


<h6>Sample Input</h6>
<pre style="margin:15px">
5 6 4
12 387 15 162 5
14 162 92 387 7 748
14 5 12 387
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
9
</pre>


<h5 style="font-weight: bold;"> Session 2, 1:00 pm&ndash;4:00 pm IST</h5> <hr>
<br>

<h5>Cheapest Path in a Grid</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2010, 12 Dec 2009</h6>
  <h6>1:00 pm&ndash;4:00 pm IST</h6>

<h6>Problem 1 : Cheapest Path in a Grid</h6>

<p>You are given an <em>N &times; N</em> grid of numbers.  You
  start at the top left corner of the grid.  Your goal is to move
  to the bottom right corner, constrained by the rules below.</p>

<p>At each step you are allowed to perform one of the following
  moves, provided you stay within the grid:</p>

<ul>

<li> <p>Move right one step to the next column in the grid.</p>

<li> <p>Move down one step to the next row in the grid.</p>

<li> <p>One of the columns from 2 to <em>N</em> is special.  Let
    this column be <em>K</em>.  If you are currently in
    row <em>i</em> on column <em>K-1</em>, you can move right to
    any row <em>j</em> on column <em>K</em> in one step. </p>

</ul>

<p>The cost of your path is calculated as follows:</p>

<ul>

<li> <p>Add each number that you visit on the grid to your cost.</p>

<li> <p>When you make a special move
    from row <em>i</em> on
    column <em>K-1</em> to row <em>j</em>
    on column <em>K</em>, you incur an additional cost equal to
    the absolute value of
    <em>i-j</em>.</p>

</ul>

<p>Your aim is to compute the minimum cost required to reach the
  bottom right corner of the grid.</p>

<p>For instance, suppose you have the following grid, where
  column 3 is the special column.</p>

<table>
<tr>
<td align=right>  2</td>
<td align=right>  4</td>
<td align=right> -5</td>
<td align=right>  4</td>
</tr>
<tr>
<td align=right>  1</td>
<td align=right> -3</td>
<td align=right>  1</td>
<td align=right> -3</td>
</tr>
<tr>
<td align=right> -3</td>
<td align=right>  2</td>
<td align=right>  1</td>
<td align=right>  4</td>
</tr>
<tr>
<td align=right>  9</td>
<td align=right>  8</td>
<td align=right>  2</td>
<td align=right>  1</td>
</tr>

</table>

<p>In this grid, the cheapest path has cost -1. To achieve this,
  move as follows:</p>

<ol>

<li> Start at top left corner, cost 2.

<li> Move down one row, add 1, current cost 3.

<li> Move right one column, add -3, current cost 0.

<li> Jump to top row on column 3 (special move), add -5 + 1,
  current cost -4.

<li> Move down one row, add 1, current cost -3.

<li> Move right one column, add -3, current cost -6.

<li> Move down one row, add 4, current cost -2.

<li> Move down one row to bottom right corner, add 1, final cost -1.

</ol>


<h6>Input format</h6>

<p>The first line of the input contains two integers <em>N</em>
  and <em>K</em>, where <em>N</em> is the number of rows and
  columns in the grid and <em>K</em>, 2 &le <em>K</em>
  &le; <em>N</em>, is the special column.  This is followed
  by <em>N</em> lines of input, each containing <em>N</em> space
  separated integers.  Line <em>i+1</em> of the input describes
  the numbers in row <em>i</em> of the grid.</p>
</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
 the cost of cheapest path from the top left corner to the bottom
 right corner.</p>

<h6>Testdata</h6>

<p>In all cases, N &le; 10<sup>3</sup>.</p>


<h6>Sample Input</h6>
<pre style="margin:15px">
4 3
2 4 -5 4
1 -3 1 -3
-3 2 1 4
9 8 2 1
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
-1
</pre>


<h5>Voting</h5><hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2010, 12 Dec 2009</h6>
  <h6>1:00 pm&ndash;4:00 pm IST</h6>

<h6>Problem 2 : Voting</h6>

<p>Elections are on for the Siruseri Town Council.  Elections
  in Siruseri work in a rather odd manner.  Each candidate is
  assigned a unique identification number.  The town is divided
  into five zones and each zone proposes a list of candidates, in
  some arbitrary order, that it would like to nominate to the
  Council.  Any candidate who is proposed by three or more zones
  is elected.  There is no lower limit or upper limit on the size
  of the Council.
</p>

<p>Your task is to to calculate how many candidates are elected
  to the Council, given the lists proposed by the five zones.</p>

<p>For example, suppose the candidates proposed by the five zones
  are as follows:</p>

<ul>

<li> <p><em>Zone 1:</em> [12,387,15,162,5]</p>

<li> <p><em>Zone 2:</em> [14,162,92,387,7,748]</p>

<li> <p><em>Zone 3:</em> [14,5,12,387]</p>

<li> <p><em>Zone 4:</em> [17,952,12,92,398,849]</p>

<li> <p><em>Zone 5:</em> [14,5,92,12,387]</p>

</ul>

<p>In this example, 5 candidates are elected: these are
  [12,387,5,14,92].</p>

<h6>Input format</h6>

<p>The first line of the input contains five
  integers <em>N<sub>1</sub></em>, <em>N<sub>2</sub></em>
  <em>N<sub>3</sub></em>, <em>N<sub>4</sub></em>
  and <em>N<sub>5</sub></em>, where <em>N<sub>j</sub></em> is the
  number of candidates proposed by zone <em>j</em>, 1
  &le; <em>j</em> &le; 5.  This is followed by five lines of
  space separated integers. For 1 &le; <em>j</em> &le; 5,
  line <em>j</em>+1 of the input has <em>N<sub>j</sub></em>
  integers representing the list of candidates proposed by
  zone <em>j</em>.</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the total number of candidates elected to the Town Council.</p>

<h6>Testdata</h6>

<p>In all cases, 1&nbsp;&le;&nbsp;<em>N</em><sub>1</sub>, <em>N</em><sub>2</sub>, <em>N</em><sub>3</sub>,
  <em>N</em><sub>4</sub>, <em>N</em><sub>5</sub>&nbsp;&le;&nbsp;10<sup>6</sup>.
  Also, each individual list is guaranteed to be free of
  duplicate entries.
</p>


<h6>Sample Input</h6>
<pre style="margin:15px">
5 6 4 6 5
12 387 15 162 5
14 162 92 387 7 748
14 5 12 387
17 952 12 92 398 849
14 5 92 12 387
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
5
</pre>


