---
draft: false
title: "Question Paper ZCO 2012"
job_nature: ""
category: ""
---

<div id="cont">
<h4 align="left">Zonal Computing Olympiad, 2012</h4>
  

  <p>The Zonal Computing Olympiad, 2012 was held in two sessions
  on Saturday, November 26, 2012.  Students could take part in
  either session.  The questions for the two sessions were as
  follows.</p>

<h5 style="font-weight: bold;"> Session 1, 10:00 am&ndash;1:00 pm IST</h5>

<hr>
<h5>  Matched Brackets</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2012, 26 Nov 2011</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 1 : Matched Brackets</h6>

<p>
A sequence of opening and closing brackets is
<em>well-bracketed</em> if we can pair up each opening bracket
with a matching closing bracket in the usual sense.  For
instance, the sequences <tt>()</tt>, <tt>(())</tt> and
<tt>()(())</tt> are well-bracketed, while <tt>(</tt>,
<tt>())</tt>, <tt>(()()</tt>, and <tt>)(</tt>  are not well-bracketed.
</p>

<p> The <em>nesting depth</em> of a well-bracketed sequence tells
us the maximum number of levels of inner matched brackets
enclosed within outer matched brackets.  For instance, the
nesting depth of <tt>()</tt> and <tt>()()()</tt> is 1, the
nesting depth of <tt>(())</tt> and <tt>()(())</tt> is 2, the
nesting depth of <tt>((()))</tt> is 3, and so on.  </p>

<p>
Given a well-bracketed sequence, we are interested in computing
the following:
</p>

<ul>

<li> <p>The nesting depth, and the first position where it
  occurs&ndash;this will be the position of the first opening
  bracket at this nesting depth, where the positions are numbered
  starting with 1.</p>
  
<li> <p>The maximum number of symbols between any pair of matched
  brackets, including both the outer brackets, and the first
  position where this occurs&ndash;that is, the position of the
  first opening bracket of this segment.<p>

</ul>

<p>For instance, the nesting depth of
<tt>()(())()(()())(()())</tt> is 2 and the first position where
this occurs is 4.  The opening bracket at position 10 is also at
nesting depth 2 but we have to report the first position where
this occurs, which is 4.</p>

<p>In this sequence, the maximum number of symbols between a pair
of matched bracket is 6, starting at position 9.  There is
another such sequence of length 6 starting at position 15, but
this is not the first such position.</p>

<h6>Input format</h6>

<p>The input consists of two lines.  The first line is a single
integer <em>N</em>, the length of the bracket sequence.
Positions in the sequence are numbered 1,2,&hellip;,<em>N</em>.
The second line is a sequence of <em>N</em> space-separated
integers that encode the bracket expression as follows: 1 denotes
an opening bracket <tt>(</tt> and 2 denotes a closing bracket
<tt>)</tt>.  Nothing other than 1 or 2 appears in the second line
of input and the corresponding expression is guaranteed to be
well-bracketed.</p>

<h6>Output format</h6>

<p> Your program should print 4 space-separated integers in a
line, denoting the four quantities asked for in the following
order: nesting depth, first position that achieves the nesting
depth, length of the maximum sequence between matching brackets
and the first position where such a maximum length sequence
occurs.  </p>

<h6>Testdata</h6>

<p>
You may assume that
2&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>5</sup>.  In 30% of
the test cases, 2&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>3</sup>.
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
20
1 2 1 1 2 2 1 2 1 1 2 1 2 2 1 1 2 1 2 2
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
2 4 6 9
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.</p>

<br>

<h5>  Wormholes</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2012, 26 Nov 2011</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 2 : Wormholes</h6>

<p> The year is 2102 and today is the day of ZCO. This year there
are <em>N</em> contests and the starting and ending times of each
contest is known to you. You have to participate in exactly one
of these contests. Different contests may overlap. The duration
of different contests might be different. </p>

<p>There is only one examination centre. There is a wormhole
<em>V</em> that transports you from your house to the
examination centre and another wormhole <em>W</em> that
transports you from the examination centre back to your
house. Obviously, transportation through a wormhole does not take
any time; it is instantaneous. But the wormholes can be used at
only certain fixed times, and these are known to you.</p>

<p>So, you use a <em>V</em> wormhole to reach the exam centre,
possibly wait for some time before the next contest begins, take
part in the contest, possibly wait for some more time and then
use a <em>W</em> wormhole to return back home. If you leave
through a <em>V</em> wormhole at time <em>t</em><sub>1</sub> and
come back through a <em>W</em> wormhole at time
<em>t</em><sub>2</sub>, then the total time you have spent is
(<em>t</em><sub>2</sub>&nbsp;-&nbsp;<em>t</em><sub>1</sub>&nbsp;+&nbsp;1). Your
aim is to spend as little time as possible overall while ensuring
that you take part in one of the contests.</p>

<p>You can reach the centre exactly at the starting time of the
contest, if possible. And you can leave the examination centre
the very second the contest ends, if possible. You can assume
that you will always be able to attend at least one
contest&ndash;that is, there will always be a contest
such that there is a <em>V</em> wormhole before it and a
<em>W</em> wormhole after it.</p>

<p> For instance, suppose there are 3 contests with (start,end)
times (15,21), (5,10), and (7,25), respectively.  Suppose the
<em>V</em> wormhole is available at times 4, 14, 25, 2 and the
<em>W</em> wormhole is available at times 13 and 21.  In this
case, you can leave by the <em>V</em> wormhole at time 14, take
part in the contest from time 15 to 21, and then use the
<em>W</em> wormhole at time 21 to get back home.  Therefore the
time you have spent is (21&nbsp;-&nbsp;14&nbsp;+&nbsp;1) = 8. You
can check that you cannot do better than this.  </p>

<h6>Input format</h6>

<p>The first line contains 3 space separated integers <em>N</em>,
<em>X</em>, and <em>Y</em>, where <em>N</em> is the number of
contests, <em>X</em> is the number of time instances when
wormhole <em>V</em> can be used and <em>Y</em> is the number of
time instances when wormhole <em>W</em> can be used.  The next
<em>N</em> lines describe each contest.  Each of these <em>N</em>
lines contains two space separated integers <em>S</em> and
<em>E</em>, where <em>S</em> is the starting time of the
particular contest and <em>E</em> is the ending time of that
contest, with <em>S</em> &lt; <em>E</em>.  The next line contains
<em>X</em> space separated integers which are the time instances
when the wormhole <em>V</em> can be used.  The next line contains
<em>Y</em> space separated integers which are the time instances
when the wormhole <em>W</em> can be used.</p>

<h6>Output format</h6>

<p>Print a single line that contains a single integer, the
minimum time needed to be spent to take part in a contest.</p>

<h6>Testdata</h6>

<p> All the starting and ending times of contests are distinct
and no contest starts at the same time as another contest ends.
The time instances when wormholes are available are all distinct,
but may coincide with starting and ending times of contests.
All the time instances (the contest timings and the wormhole
timings) will be integers between 1 and 1000000 (inclusive).</p>

<p>You may assume that 
1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>5</sup>,
1&nbsp;&le;&nbsp;<em>X</em>&nbsp;&le;&nbsp;10<sup>5</sup>, and
1&nbsp;&le;&nbsp;<em>Y</em>&nbsp;&le;&nbsp;10<sup>5</sup>.
</p>


<p>In 30% of the cases, 
1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>3</sup>,
1&nbsp;&le;&nbsp;<em>X</em>&nbsp;&le;&nbsp;10<sup>3</sup>, and
1&nbsp;&le;&nbsp;<em>Y</em>&nbsp;&le;&nbsp;10<sup>3</sup>.
</p>


<h6>Sample Input</h6>

<pre style="margin:15px">
3 4 2
15 21
5 10
7 25
4 14 25 2
13 21
</pre>

<h6>Sample Output</h6>

<pre style="margin:15px">
8
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.</p>



<br>

<h5 style="font-weight: bold;"> Session 2, 2:00 pm&ndash;5:00 pm IST</h5>

<hr>

<h5>   Matched Brackets</h5> <hr>


<div id="cont">
<h6>Zonal Computing Olympiad 2012, 26 Nov 2011</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 1 : Matched Brackets</h6>

<p> We consider sequences of opening and closing brackets with
two types of brackets, <tt>()</tt> and <tt>[]</tt>.  A bracket
sequence is <em>well-bracketed</em> if we can pair up each
opening bracket with a matching closing bracket in the usual
sense.  For instance, the sequences <tt>()</tt>, <tt>[]</tt>
<tt>([])</tt> and <tt>[]([])</tt> are well-bracketed, while
<tt>(</tt>, <tt>()]</tt>, <tt>(]</tt>, <tt>)(</tt> and
<tt>[(])</tt> are not well-bracketed.  In the last case, each
opening bracket has a matching closing bracket and vice versa,
but the intervals spanned by the different types of brackets
intersect each other instead of being contained one within the
other.</p>

<p> The <em>alternating depth</em> of a well-bracketed sequence
tells us the maximum number of times we switch between the two
types of brackets when we have inner matched brackets enclosed
within outer matched brackets.  For instance, the alternating
depth of <tt>()</tt>, <tt>[[[]]]</tt> and <tt>()[][]</tt> is 1,
the alternating depth of <tt>[()]</tt> and <tt>()([])</tt> is 2,
the alternating depth of <tt>([()])</tt> and <tt>[()][(([]))]</tt>
is 3, and so on.</p>

<p>
Given a well-bracketed sequence, we are interested in computing
three quantities.
</p>

<ul>

<li> <p>The alternating depth of the sequence.</p>
  
<li> <p>The maximum number of symbols between any pair of matched
  brackets of the type <tt>(</tt> and <tt>)</tt>, including both
  the outer brackets.</p>

<li> <p>The maximum number of symbols between any pair of matched
  brackets of the type <tt>[</tt> and <tt>]</tt>, including both
  the outer brackets.</p>
  
</ul>

<p>For instance, the alternating depth of <tt>(([]))[[[()]]]</tt>
is 2, the maximum number of symbols between a matched pair
<tt>()</tt> is 6 and the maximum number of symbols between a
matched pair <tt>[]</tt> is 8.


<h6>Input format</h6>

<p>The input consists of two lines.  The first line is a single
integer <em>N</em>, the length of the bracket sequence.
Positions in the sequence are numbered 1,2,&hellip;,<em>N</em>.
The second line is a sequence of <em>N</em> space-separated
integers that encode the bracket expression as follows: 1 denotes
an opening bracket <tt>(</tt>, 2 denotes a closing bracket
<tt>)</tt>, 3 denotes an opening bracket <tt>[</tt> and 4 denotes
a closing bracket <tt>]</tt>.  Nothing other than 1, 2, 3 or 4
appears in the second line of input and the corresponding
expression is guaranteed to be well-bracketed.</p>

<h6>Output format</h6>

<p> Your program should print 3 space-separated integers in a
line, denoting the three quantities asked for in the following
order: alternating depth, length of the maximum sequence between
matching <tt>()</tt> brackets and length of the maximum sequence
between matching <tt>[]</tt> brackets.  </p>

<h6>Testdata</h6>

<p>
You may assume that
2&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>5</sup>.  In 30% of
the test cases, 2&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>3</sup>.
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
14
1 1 3 4 2 2 3 3 3 1 2 4 4 4
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
2 6 8
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.</p>


<br>

<h5>   Round Table</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2012, 26 Nov 2011</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 2 : Round Table</h6>

<p> It's dinner time in Castle Camelot, and the fearsome Knights
of the Round Table are clamouring for dessert. You, the chef, are
in a soup.  There are <em>N</em> knights, including King Arthur, 
each with a different preference for dessert, but you cannot afford 
to make desserts for all of them.</p>

<p>You are given the cost of manufacturing each Knight's
preferred dessert&ndash;since it is a round table, the list
starts with the cost of King Arthur's dessert, and goes
counter-clockwise.</p>

<p>You decide to pick the cheapest desserts to make, such that
 for every pair of adjacent Knights, at least one gets his dessert.
 This will ensure that the Knights do not protest.</p>

<!--<p>A strange feature of the Knights is that they will not
complain about not getting dessert unless they get support from
both their neighbours.  So, you decide to pick the cheapest
desserts to make, such that for every pair of adjacent Knights,
at least one gets his dessert.</p>-->

<p>What is the minimum cost of tonight's dinner, given this
condition?</p>

<p>For instance, suppose there are 5 Knights and their desserts
cost 1, 2, 1, 2 and 2.  In this case, the minimum cost is 4,
which you can achieve by feeding the first, third and fourth (or
fifth) Knights.  </p>

<h6>Input format</h6>

<p>There are 2 lines of input.  The first line contains a single
integer <em>N</em>, the number of seats at the table.  The next
line contains <em>N</em> space separated integers, each being the
cost of the dessert of a Knight, listed in counterclockwise order
around the table, starting with King Arthur.</p>

<h6>Output format</h6>

<p>The output should be a single line containing a single
integer, the minimum possible cost for you, the chef.</p>

<h6>Testdata</h6>

<p>Each Knight's dessert costs strictly more than 0 and strictly
less than 1000.  You may assume that
1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>6</sup>.  In
30% of the test cases,
1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;10<sup>3</sup>.  </p>



<h6>Sample Input</h6>

<pre style="margin:15px">
5
1 2 1 2 2
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
4
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.</p>






