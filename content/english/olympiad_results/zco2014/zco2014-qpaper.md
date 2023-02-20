---
draft: false
title: "Question Paper ZCO 2014"
job_nature: ""
category: ""
---

<div id="cont">
<h4 align="left">Zonal Computing Olympiad, 2013</h6>
  

  <p>The Zonal Computing Olympiad, 2014 was held in two sessions
  on Saturday, November 30, 2013.  Students could take part in
  either session.  The questions for the two sessions were as
  follows.</p>

<h5 style="font-weight: bold;">
  Session 1, 10:00 am&ndash;1:00 pm IST</h5>



 <h5> Video Game</h5>

<div id="cont">
<h6>Zonal Computing Olympiad 2014, 30 Nov 2013</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 1 : Video fGame</h6>

<p>You are playing a video game in which several stacks of boxes
are lined up on the floor, with a crane on top to rearrange the
boxes, as shown in the picture below.</p>

<img style="margin:15px" align=center width=300 src=https://www.iarcs.org.in/inoi/2014/zco2014/videogame.png>

<p> The crane supports the following commands: </p>

<ul>

  <li> <p>Move one position left (does nothing if already at the
  leftmost position)</p>

  <li> <p>Move one position right (does nothing if already at the
rightmost position)</p>

  <li> <p>Pick up a box from the current stack (does nothing if the
crane already has a box)</p>

  <li> <p>Drop a box on the current stack (does nothing if the
crane doesn't already have a box)</p>

</ul>

<p> Further, there is a limit <em>H</em> on the number of boxes
on each stack. If a 'drop' command would result in a stack having
more than <em>H</em> boxes, the crane ignores this drop command.
If the current stack has no boxes, a 'pick up' command is ignored.
</p>

<p>You are given the initial number of boxes in each stack and
the sequence of operations performed by the crane.  You have to
compute the final number of boxes in each stack.  </p>

<p>For example, suppose the initial configuration of the game is
as shown in the figure above, with 7 stacks and <em>H</em>=4.
Then, after the following sequence of instructions,</p>

<ol style="margin:15px">
  <li> Pick up box
  <li> Move right
  <li> Move right
  <li> Move right
  <li> Move right
  <li> Drop box
  <li> Move left
  <li> Pick up box
  <li> Move left
  <li> Drop box
</ol>

<p>The number of boxes in each stack from left to right would be 2,1,3,1,4,0,1.</p>
   
<h6>Input format</h6>

<ul style="margin:15px">

<li>
Line 1 : The width of the game (the number of stacks of boxes), <em>N</em>, followed by the max height <em>H</em> of each stack.

<li>
Line 2 : <em>N</em> integers, the initial number of boxes in
each stack, from left to right. Each number is &le; <em>H</em>.

<li>
Line 3 : A sequence of integers, each encoding a commmand
  to the crane.

The commands are encoded as follows:</b>

1 : Move left<br>
2 : Move right<br>
3 : Pick up box<br>
4 : Drop box<br>
0 : Quit

The command Quit (0) appears exactly once, and is the last
command.

<li>
The initial position of the crane is above the leftmost stack,
with the crane not holding any box.

</ul>



<h6>Output format</h6>

<p>A single line with <em>N</em> integers,
the number of boxes in each stack, from left to right.</p>
 

<h6>Sample input 1</h6>
<pre style="margin:15px">>
7 4
3 1 2 1 4 0 1
3 2 2 2 2 4 1 3 1 4 0
</pre>

<h6>Sample output 1</h6>
<pre style="margin:15px">>
2 1 3 1 4 0 1
</pre>

<h6>Sample input 2</h6>
<pre style="margin:15px">>
3 5
2 5 2
3 2 4 2 2 2 1 4 1 1 1 1 0
</pre>

<h6>Sample output 2</h6>
<pre style="margin:15px">>
1 5 2 
</pre>

<h6>Test data</h6>

<p>There is only one subtask worth 100 marks.  In all inputs:

<ul>

<li> The number of commands is between 1 and 10<sup>5</sup>, inclusive.
<li> 1 &leq; <em>N</em> &leq; 10<sup>5</sup>
<li> 1 &leq; <em>H</em> &leq; 10<sup>8</sup>.

</ul>  

<h6>Live evaluation data</h6>

<p>There are 18 test inputs on the server during the exam.</p>


<h6>Limits</h6>
<p>Time limit : 1s</p>
<p>Memory limit: 32 MB</p>

<br>

 <h5>SUPW</h5>
  <div id="cont">
<h6>Zonal Computing Olympiad 2014, 30 Nov 2013</h6>
<h6>10:00 am-1:00 pm IST</h6>


<h6>Problem 2: SUPW</h6>

<p> In ICO School, all students have to participate regularly in
SUPW.  There is a different SUPW activity each day, and each
activity has its own duration.  The SUPW schedule for the next
term has been announced, including information about the number
of minutes taken by each activity.</p>

<p> Nikhil has been designated SUPW coordinator.  His task is to
assign SUPW duties to students, including himself.  The school's
rules say that no student can go three days in a row without any
SUPW duty.</p>

<p> Nikhil wants to find an assignment of SUPW duty for himself
that minimizes the number of minutes he spends overall on SUPW.
</p>


<h6>Input format</h6>

<p>Line 1: A single integer <em>N</em>, the number of days in the
future for which SUPW data is available.</p>

<p>Line 2: <em>N</em> non-negative integers, where the integer in
position <em>i</em> represents the number of minutes required for
SUPW work on day <em>i</em>.</p>

<h6>Output format</h6>

<p> The output consists of a single non-negative integer, the
minimum number of minutes that Nikhil needs to spend on SUPW duties
this term.</p>

<h6>Sample Input 1</h6>

<pre style="margin:15px">
10
3 2 1 1 2 3 1 3 2 1
</pre>

<h6>Sample Output 1</h6>

<pre style="margin:15px">
4

(Explanation: 1+1+1+1)
</pre>

<h6>Sample Input 2</h6>

<pre style="margin:15px">
8
3 2 3 2 3 5 1 3
</pre>

<h6>Sample Output 2</h6>
<pre style="margin:15px">
5

(Explanation: 2+2+1)
</pre>

<h6>Test data</h6>

<p>There is only one subtask worth 100 marks.  In all inputs:

<ul>

<li> 1 &leq; <em>N</em> &leq; 2&times;10<sup>5</sup>
<li> The number of minutes of SUPW each day is between 0 and
  10<sup>4</sup>, inclusive.

</ul>  

<h6>Live evaluation data</h6>

<p>There are 12 test inputs on the server during the exam.</p>

<h6>Limits</h6>
<p>Time limit : 1s</p>
<p>Memory limit: 32 MB</p>


<br>
<hr>
<h5 style="font-weight: bold;">
  Session 2, 2:00 pm&ndash;5:00 pm IST</h5>

 <h5>Smart Phone</h4>

 <div id="cont">
<h6>Zonal Computing Olympiad 2014, 30 Nov 2013</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 1: Smart Phone</h6>

<p> You are developing a smartphone app. You have a list of
potential customers for your app. Each customer has a budget and
will buy the app at your declared price if and only if the price
is less than or equal to the customer's budget.</p>

<p> You want to fix a price so that the revenue you earn from the
app is maximized. Find this maximum possible revenue.</p>

<p> For instance, suppose you have 4 potential customers and
their budgets are 30, 20, 53 and 14.  In this case, the maximum
revenue you can get is 60.</p>

<h6>Input format</h6>

<p>Line 1 : <em>N</em>, the total number of potential customers.</p>

<p>Lines 2 to <em>N</em>+1: Each line has the budget of a
potential customer.</p>

<h6>Output format</h6>

<p> The output consists of a single integer, the maximum possible
revenue you can earn from selling your app.</p>

<h6>Sample Input 1</h6>

<pre style="margin:15px">
4
30
20
53
14
</pre>

<h6>Sample Output 1</h6>

<pre style="margin:15px">
60
</pre>

<h6>Sample Input 2</h6>

<pre style="margin:15px">
5
40
3
65
33
21
</pre>

<h6>Sample Output 2</h6>

<pre style="margin:15px">
99
</pre>


<h6>Test data</h6>

<p>Each customers' budget is between 1 and 10<sup>8</sup>, inclusive.</p>

<p><b>Subtask 1 (30 marks)</b> : 1 &le; <em>N</em> &le; 5000.</p>
<p><b>Subtask 2 (70 marks)</b> : 1 &le; <em>N</em> &le; 5&times;10<sup>5</sup>.</p>

<h6>Live evaluation data</h6>

<p>There are 15 test inputs on the server during the exam. The
grouping into subtasks is as follows.</p>

<ul>
<li><p><b>Subtask 1:</b> Test inputs 0,&hellip;,5</p>
<li><p><b>Subtask 2:</b> Test inputs 6,&hellip;,14</p>
</ul>

<h6>Limits</h6>
<p>Time limit : 1s</p>
<p>Memory limit: 32 MB</p>

<h6>Note</h6>

<p>The answer might not fit in a variable of type
<tt>int</tt>. We recommend that you use variables of type
<tt>long&nbsp;long</tt> to read the input and compute the
answer.  If you use <tt>printf</tt> and <tt>scanf</tt>, you can
use <tt>%lld</tt> for <tt>long&nbsp;long</tt>. </p>

<br>

 <h5> IPL</h5>

<div id="cont">
<h6>Zonal Computing Olympiad 2014, 30 Nov 2013</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 2: IPL</h6>

<p> In IPL 2025, the amount that each player is paid varies from
match to match.  The match fee depends on the quality of
opposition, the venue etc.</p>

<p>The match fees for each match in the new season have been
announced in advance.  Each team has to enforce a mandatory
rotation policy so that no player ever plays three matches in a
row during the season.</p>

<p> Nikhil is the captain and chooses the team for each match.
He wants to allocate a playing schedule for himself to maximize
his earnings through match fees during the season.  </p>


<h6>Input format</h6>

<p>Line 1: A single integer <em>N</em>, the number of games in
the IPL season.</p>

<p>Line 2: <em>N</em> non-negative integers, where the integer in
position <em>i</em> represents the fee for match <em>i</em>.</p>

<h6>Output format</h6>

<p> The output consists of a single non-negative integer, the
maximum amount of money that Nikhil can earn during this IPL
season. </p>

<h6>Sample Input 1</h6>

<pre style="margin:15px">
5 
10 3 5 7 3 
</pre>

<h6>Sample Output 1</h6>

<pre style="margin:15px">
23

(Explanation: 10+3+7+3)
</pre>

<h6>Sample Input 2</h6>

<pre style="margin:15px">
8
3 2 3 2 3 5 1 3
</pre>

<h6>Sample Output 2</h6>

<pre style="margin:15px">
17

(Explanation: 3+3+3+5+3)
</pre>

<h6>Test data</h6>

<p>There is only one subtask worth 100 marks.  In all inputs:

<ul>

<li> 1 &leq; <em>N</em> &leq; 2&times;10<sup>5</sup><br><br>
<li> The fee for each match is between 0 and 10<sup>4</sup>, inclusive.

</ul>  

<h6>Live evaluation data</h6>

<p>There are 12 test inputs on the server during the exam.</p>


<h6>Limits</h6>
<p>Time limit : 1s</p>
<p>Memory limit: 32 MB</p>


</div>




