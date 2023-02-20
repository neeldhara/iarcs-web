---
draft: false
title: "Question Papper ZCO 2009"
job_nature: ""
category: ""
---

<div id="cont">
<h6 align="left">Zonal Computing Olympiad, 2009</h6>

  <p>The Zonal Computing Olympiad, 2009 was held in two sessions on Saturday, December 20, 2008.  Students could take part in either session.  The questions for the two sessions were as follows.</p>

<h5 style="font-weight: bold;">Session 1, 10:00 am&ndash;1:00 pm IST</h5> <hr>

<h5>Grid Game</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2009, 20 Dec 2008</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 1 : Grid game</h6>


<p>You are given a square grid of positive and negative numbers.
  You have to start at the top left corner of the grid and find a
  path to the bottom-right corner.  In each step, you are only
  allowed to move one position to the right or one position down.
  As a special bonus, you are allowed at most one move that can
  be either to the left or up.  Note that you are allowed to
  visit a position more than once as a result of this special
  move.</p>

<p>Your aim is to find such a path that has the maximum weight,
  where the weight of a path is the sum of all the numbers
  visited along the path.</p>


<h6>Input format</h6>

<p>The first line of the input contains one integer N, the number
  of rows and columns in the grid.  Lines 2 to N+1 describe the N
  rows of the grid.  Each of these N lines of input consists of N
  space separated integers, corresponding to the numbers in one
  row.</p>

<h6>Notes</h6>

<p>In all cases, N &le; 2000.  Each number in the grid is
  guaranteed to be less than 1000.</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the sum of the values on the path of maximum weight.</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
4
12 -16 10 -12
-16 13 -14 7
7 -4 16 -15
-7 16 -9 8 
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
32
</pre>



<h5>Choosing Chocolates</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2009, 20 Dec 2008</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 2 : Choosing chocolates</h6>


<p>Santa Claus has lined up a row of bowls, each containing some
  chocolates.  Nikhil has been told that he can pick up as many
  of these bowls as he wants, provided that he never picks two
  consecutive bowls.</p>

<p>Your aim is to help Nikhil choose a set of bowls so that he
  maximizes the number of chocolates that he picks up.

<h6>Input format</h6>


<p>The first line of the input contains one integer N, the number
  of bowls.  This is followed by a line containing N integers,
  describing the number of chocolates in each of the N bowls.</p>

<h6>Notes</h6>

<p>In all cases, N &le; 100,000.</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the maximum number of chocolates that Nikhil can collect.</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
10
30 10 8 20 11 12 25 13 20 19
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
95
</pre>





<br>
<h5 style="font-weight: bold;"> Session 2, 2:00 pm&ndash;5:00 pm IST</h5> <hr>


<h5>Grid Game</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2009, 20 Dec 2008</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 1 : Grid game</h6>


<p>You are given a square grid of positive and negative numbers.
  You have to start at the top left corner of the grid and find a
  path to the bottom-right corner.  In each step, you are only
  allowed to move one position to the right or one position down.
  As a special bonus, you are allowed at most one move in which
  you can jump and skip over one position, either when going
  right or when going down. When you skip poisitions. you are not
  allowed to go beyond the grid boundary.  Also, you
  are <em>not</em> allowed to skip over the starting position,
  the top left square, or the ending position, the bottom right
  square.</p>

<p>Your aim is to find such a path that has the maximum weight,
  where the weight of a path is the sum of all the numbers
  visited along the path.</p>


<h6>Input format</h6>


<p>The first line of the input contains one integer N, the number
  of rows and columns in the grid.  Lines 2 to N+1 describe the N
  rows of the grid.  Each of these N lines of input consists of N
  space separated integers, corresponding to the numbers in one
  row.</p>

<h6>Notes</h6>

<p>In all cases, N &le; 2000.  Each number in the grid is
  guaranteed to be less than 1000.</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the sum of the values on the path of maximum weight.</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
4
12 -16 10 -12
-16 13 -14 7
7 -4 16 -15
-7 16 -9 8 
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
30
</pre>



<h5>Choosing Chocolates</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2009, 20 Dec 2008</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 2 : Choosing chocolates</h6>


<p>Santa Claus has lined up a row of bowls, each containing some
  chocolates.  Nikhil has been told that he can pick up as many
  of these bowls as he wants, provided that he never picks three
  consecutive bowls.</p>

<p>Your aim is to help Nikhil choose a set of bowls so that he
  maximizes the number of chocolates that he picks up.

<h6>Input format</h6>


<p>The first line of the input contains one integer N, the number
  of bowls.  This is followed by a line containing N integers,
  describing the number of chocolates in each of the N bowls.</p>

<h6>Notes</h6>

<p>In all cases, N &le; 100,000.</p>

<h6>Output format</h6>

<p>Your output should be a single line consisting of one integer,
the maximum number of chocolates that Nikhil can collect.</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
10
30 10 8 20 11 12 25 13 20 19
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
136
</pre>




