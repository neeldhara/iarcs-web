---
draft: false
title: "Question Paper ZCO 2013"
job_nature: ""
category: ""
---

<div id="cont">
<h4 align="left">Zonal Computing Olympiad, 2013</h4>

  <p>The Zonal Computing Olympiad, 2013 was held in two sessions
  on Saturday, November 10, 2012.  Students could take part in
  either session.  The questions for the two sessions were as
  follows.</p>

<h5 style="font-weight: bold;">
  Session 1, 10:00 am&ndash;1:00 pm IST</h5>


<h5> Tournament</h5> 

<div id="cont">
<h6>Zonal Computing Olympiad 2013, 10 Nov 2012</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 1 : Tournament</h6>

<p><em>N</em> teams participate in a league cricket tournament on
Mars, where each pair of distinct teams plays each other exactly
once. Thus, there are a total of <em>(N &times; (N-1))/2</em> matches. An
expert has assigned a strength to each team, a positive
integer. Strangely, the Martian crowds love one-sided matches and
the advertising revenue earned from a match is the absolute value
of the difference between the strengths of the two matches. Given
the strengths of the <em>N</em> teams, find the total advertising
revenue earned from all the matches.</p>

<p>For example, suppose <em>N</em> is 4 and the team strengths for
teams 1, 2, 3, and 4 are 3, 10, 3, and 5 respectively. Then the
advertising revenues from the 6 matches are as follows:</p>

<table border="1" style="margin:15px">
<tr>
<th>Match</th> <th>Team A</th> <th>Team B</th> <th>Ad revenue</th>
</tr>
<tr> <td align=center>1</td>  <td align=center>1</td>  <td align=center>2</td>   <td align=center>7</td>  </tr>
<tr> <td align=center>2</td>  <td align=center>1</td>  <td align=center>3</td>   <td align=center>0</td>  </tr>
<tr> <td align=center>3</td>  <td align=center>1</td>  <td align=center>4</td>   <td align=center>2</td>  </tr>
<tr> <td align=center>4</td>  <td align=center>2</td>  <td align=center>3</td>   <td align=center>7</td>  </tr>
<tr> <td align=center>5</td>  <td align=center>2</td>  <td align=center>4</td>   <td align=center>5</td>  </tr>
<tr> <td align=center>6</td>  <td align=center>3</td>  <td align=center>4</td>   <td align=center>2</td>  </tr>
</table>

<p>Thus the total advertising revenue is 23.</p>

<h6>Input format</h6>
<p>Line 1 : A single integer, <em>N</em>.</p>
<p>Line 2 : <em>N</em> space-separated integers, the strengths of the <em>N</em> teams.</p>

<h6>Output format</h6>
<p>A single integer, the total advertising revenue from the tournament.</p>

<h6>Sample input</h6>
<pre style="margin:15px">
4
3 10 3 5
</pre>

<h6>Sample output</h6>
<pre style="margin:15px">
23
</pre>

<h6>Test data</h6>
<p>In all subtasks, the strength of each team is an integer
between 1 and 1,000 inclusive.</p> 
<p><b>Subtask 1 (30 marks)</b> : 2 &leq; <em>N</em> &leq; 1,000.</p>
<p><b>Subtask 2 (70 marks)</b> : 2 &leq; <em>N</em> &leq; 200,000.</p>

<h6>Limits</h6>
<p>Time limit : 3s</p>
<p>Memory limit: 64 MB</p>

<h6>Note</h6>

<p>The answer might not fit in a variable of type
<tt>int</tt>. We recommend that type
<tt>long&nbsp;long</tt> be used for computing all advertising
revenues.  If you use <tt>printf</tt> and <tt>scanf</tt>, you can
use <tt>%lld</tt> for <tt>long&nbsp;long</tt>. </p>




<br>
<h5>  Little Red Riding Hood</h5> 

<div id="cont">
<h6>Zonal Computing Olympiad 2013, 10 Nov 2012</h6>
<h6>10:00 am-1:00 pm IST</h6>

<h6>Problem 2: Little Red Riding Hood</h6>

<p>Little Red Riding Hood is carrying a basket with berries
through the forest to her grandmother's house.  The forest is
arranged in the form of a square <em>N &times; N</em> grid of
cells.  The top left corner cell, where Little Red Riding Hood
starts her journey, is numbered (1,1) and the bottom
right corner cell, where her grandmother lives, is numbered
<em>(N,N)</em>.  In each step, she can move either one position
right or one position down.</p>

<p> The forest is full of dangerous wolves and she is looking for
a safe path to reach her destination.  Little Red Riding Hood's
fairy godmother has placed some special anti-wolf magical charms
in some of the cells in the grid.  Each charm has a strength.  If
the charm in cell <em>(i,j)</em> has strength <em>k</em> then its
zone of influence is all the cells within <em>k</em> steps of
<em>(i,j)</em>; that is, all cells <em>(i',j')</em> such that
|<em>i</em> - <em>i'</em>| + |<em>j</em> - <em>j'</em>| &leq;
<em>k</em>.  A cell within the zone of influence of a charm is
safe from wolves.  A safe path from (1,1) to <em>(N,N)</em> is
one in which every cell along the path is safe.</p>

<p>Little Red Riding Hood is carrying a basket with berries.  In
each cell, she drops some berries while pushing her way through
the thick forest.  However, sometimes she is also able to pick up
fresh berries.  Each cell is labelled with an integer that
indicates the net change in the number of berries in her basket
on passing through the cell; that is, the number of berries she
picks up in that cell minus the number of berries she drops.  You
can assume that there are enough berries in her basket to start
with so that the basket never becomes empty.</p>

<p>Little Red Riding Hood knows the positions and strengths of
all the magic charms and is looking for a safe path along which
the number of berries she has in the basket when she reaches her
grandmother's house is maximized.</p>

<p>As an example consider the following grid:</p>

<pre style="margin:15px">
 3  3  2  4  3 
 2  1 -1 -2  2  
-1  2  4  3 -3  
-2  2  3  2  1  
 3 -1  2 -1  2  
</pre>

<p> Suppose there are 3 magic charms, at position (1,2) with
strength 2, at position (4,5) with strength 2 and one at position
(4,2) with strength 1.  The positions within the zone of
influence of these three charms are indicated in the three grids
below using <tt>X</tt>'s.  </p>

<pre style="margin:15px">
X  X  X  X  .         .  .  .  .  .         .  .  .  .  .
X  X  X  .  .         .  .  .  .  X         .  .  .  .  .
.  X  .  .  .         .  .  .  X  X         .  X  .  .  .
.  .  .  .  .         .  .  X  X  X         X  X  X  .  .
.  .  .  .  .         .  .  .  X  X         .  X  .  .  .
</pre>

<p> Putting these together, the cells that are under the zone of
influence of at least one charm are marked with <tt>X</tt> below.
</p>

<pre style="margin:15px">
X  X  X  X  .
X  X  X  .  X
.  X  .  X  X
X  X  X  X  X
.  X  .  X  X
</pre>

<p> Here are two examples of safe paths in this grid, marked
using <tt>Y</tt>'s.  </p>

<pre style="margin:15px">
Y  Y  X  X  .          Y  X  X  X  .
X  Y  X  .  X          Y  Y  X  .  X
.  Y  .  X  X          .  Y  .  X  X
X  Y  Y  Y  Y          X  Y  Y  Y  X
.  X  .  X  Y          .  X  .  Y  Y
</pre>

<p> Along the first path, she accumulates 19 berries while on the
second path she collects 16 berries.  You can verify that among all safe
paths, the maximum number of berries she can collect is 19.  </p>

<p> Your task is to help Little Red Riding Hood find out if there
is at least one safe path and, if so, compute the maximum number
of berries she can collect among all safe paths (which may be a
negative number, in which case it is the minimum number of
berries she will lose among all safe paths).</p>


<h6>Input format</h6>

<p>Line 1: Two space separated integers <em>N</em> and
<em>M</em>, giving the dimension of the grid and the number of
magic charms, respectively

<p>Lines 2 to <em>N</em>+1: These <em>N</em> lines desribe the
grid.  Line <em>i</em>+1 contains <em>N</em> space separated
integers, describing the net change in berries in the <em>N</em>
cells along row <em>i</em> of the grid.</p>

<p>Lines <em>N</em>+2 to <em>N</em>+<em>M</em>+1: These
<em>M</em> lines describe the magic charms.  Each of these lines
has 3 integers: the first two integers describe the position of
the charm in the grid and the third integer describes its
strength.</p>

<h6>Output format</h6>

<p> The first line of output must either consist of the word
<tt>YES</tt>, if there are safe paths, or the word <tt>NO</tt>,
if there are no safe paths. If the output on the first line is
<tt>YES</tt> then the second line should contain a single integer
giving the maximum number of berries Little Red Riding Hood can
collect among all safe paths.  </p>

<h6>Sample Input</h6>

<pre style="margin:15px">
5 3
3 3 2 4 3 
2 1 -1 -2 2  
-1 2 4 3 -3  
-2 2 3 2 1  
3 -1 2 -1 2  
1 2 2
4 5 2
4 2 1
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
YES
19
</pre>

<h6>Test data</h6>

<p>In all subtasks, you may assume that 2 &le; <em>N</em> &le;
500.  Each value on the grid is guaranteed to have absolute value
not more than 1000. </p>

<p>Let <em>K</em> denote the maximum strength among all the magic
charms.</p>

<p><b>Subtask 1 (30 marks)</b> : 1 &le; <em>M</em> &le; 10, 1
&le; <em>K</em> &le; 1,000.</p>
<p><b>Subtask 2 (70 marks)</b> : 1 &le; <em>M</em> &le; 10,000, 1
&le; <em>K</em> &le; 10.</p>

<h6>Limits</h6>
<p>Time limit : 3s</p>
<p>Memory limit: 128 MB</p>



<br>
<hr>
<h5 style="font-weight: bold;">
  Session 2, 2:00 pm&ndash;5:00 pm IST</h5>

<h5> Chewing</h5>

<div id="cont">
<h6>Zonal Computing Olympiad 2013, 10 Nov 2012</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 1: Chewing</h6>

<p>Hobbes has challenged Calvin to display his chewing skills and
chew two different types of <em>Chewing Magazine</em>'s Diabolic
Jawlockers chewing gum at the same time. Being a generous sort of
tiger, Hobbes allows Calvin to pick the two types of gum he will
chew.</p>

<p>Each type of chewing gum has a hardness quotient, given by a
non-negative integer.  If Calvin chews two pieces of gum at the
same time, the total hardness quotient is the sum of the
individual hardness quotients of the two pieces of gum.</p>

<p>Calvin knows that he cannot chew any gum combination whose
hardness quotient is <em>K</em> or more. He is given a list with
the hardness quotient of each type of gum in the Diabolic
Jawlockers collection.  How many different pairs of chewing gum
can Calvin choose from so that the total hardness quotient
remains strictly below his hardness limit <em>K</em>?</p>

<p>For instance, suppose there are 7 types of chewing gum as
follows:

<table border="1" style="margin:15px">
<tr>

</tr>
<tr> <td align=center>&nbsp;Chewing gum type&nbsp;</td>
     <td align=center>&nbsp;1&nbsp;</td>
     <td align=center>&nbsp;2&nbsp;</td>
     <td align=center>&nbsp;3&nbsp;</td>
     <td align=center>&nbsp;4&nbsp;</td>
     <td align=center>&nbsp;5&nbsp;</td>
     <td align=center>&nbsp;6&nbsp;</td>
     <td align=center>&nbsp;7&nbsp;</td>
</tr>
<tr> <td align=center>&nbsp;Hardness quotient&nbsp;</td>
     <td align=center>&nbsp;10&nbsp;</td>
     <td align=center>&nbsp;1&nbsp;</td>
     <td align=center>&nbsp;3&nbsp;</td>
     <td align=center>&nbsp;1&nbsp;</td>
     <td align=center>&nbsp;5&nbsp;</td>
     <td align=center>&nbsp;5&nbsp;</td>
     <td align=center>&nbsp;0&nbsp;</td>
</tr>
</table>

<p>
If Calvin's hardness
limit is 4, there are 4 possible pairs he can choose:
type 2 and 7 (1+0 &lt; 4), type 3 and 7 (3+0 &lt; 4),
type 2 and 4 (1+1 &lt; 4) and type 4 and 7 (1+0 &lt; 4).
</p>

<h6>Input format</h6>

<p>Line 1 : Two space separated integers <em>N</em> and
<em>K</em>, where <em>N</em> is the number of different types of
chewing gum and <em>K</em> is Calvin's hardness limit.</p>

<p>Line 2: <em>N</em> space separated non-negative integers,
which are the hardness quotients of each of the <em>N</em>
types of chewing gum.</p>

<h6>Output format</h6>

<p> The output consists of a single non-negative integer, the
number of pairs of chewing gum with total hardness quotient strictly
less than <em>K</em>.  </p>

<h6>Sample Input</h6>

<pre style="margin:15px">
7 4
10 1 3 1 5 5 0
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
4
</pre>


<h6>Test data</h6>

<p>In all subtasks, you may assume that all the hardness
quotients as well as the hardness limit <em>K</em> are between 0
and 1,000,000, inclusive.</p>

<p><b>Subtask 1 (30 marks)</b> : 2 &le; <em>N</em> &le; 2,000.</p>
<p><b>Subtask 2 (70 marks)</b> : 2 &le; <em>N</em> &le; 100,000.</p>

<h6>Limits</h6>
<p>Time limit : 3s</p>
<p>Memory limit: 64 MB</p>

<h6>Note</h6>

<p>The answer might not fit in a variable of type
<tt>int</tt>. We recommend that type
<tt>long&nbsp;long</tt> be used for computing the
answer.  If you use <tt>printf</tt> and <tt>scanf</tt>, you can
use <tt>%lld</tt> for <tt>long&nbsp;long</tt>. </p>




<br>
<h5>Save Spaceman Spiff</h5>

<div id="cont">
<h6>Zonal Computing Olympiad 2013, 10 Nov 2012</h6>
<h6>2:00 pm-5:00 pm IST</h6>

<h6>Problem 2: Save Spaceman Spiff</h6>

<p>Spaceman Spiff has crash landed on Planet Quorg. He has to
reach his ship quickly. But the evil Yukbarfs have stolen many
Death Ray Blasters and have placed them along the way. You'll
have to help him out!</p>

<p>Spaceman Spiff is initially at the top left corner (1,1) of a
rectangular <em>N &times; M</em> grid . He needs to reach the
bottom right corner <em>(N,M)</em>. He can only move down or
right. He moves at the speed of 1 cell per second. He has to move
every second&mdash;that is, he cannot stop and wait at any cell.</p>

<p>There are <em>K</em> special cells that contain the Death Ray
Blasters planted by the Yukbarfs. Each Blaster has a starting
time <em>t</em> and a frequency <em>f</em>.  It first fires at
time <em>t</em> seconds, followed by another round at time
<em>t+f</em> seconds, then at time <em>t+2f</em> seconds
&hellip;.  When a Blaster fires, it simultaneously emits four
pulses, one in each of the four directions: up, down, left and
right.  The pulses travel at 1 cell per second.

<p>Suppose a blaster is located at <em>(x,y)</em> with starting
time <em>t</em> and frequency <em>f</em>.  At time <em>t</em>
seconds, it shoots its first set of pulses. The pulse travelling
upwards will be at the cell <em>(x,y-s)</em> at time <em>t+s</em>
seconds.  At this time, the pulse travelling left will be at cell
<em>(x-s,y)</em>, the pulse travelling right will be at cell
<em>(x+s,y)</em> and the pulse travelling down will be at cell
<em>(x,y+s)</em>.  It will fire next at time <em>t+f</em>
seconds.  If a pulse crosses an edge of the grid, it
disappears. Pulses do not affect each other if they meet. They
continue along their original path. At any time, if Spaceman
Spiff and a pulse are in the same cell, he dies. That is the only
way pulses interact with Spaceman Spiff. Given these, you should
find the least time (in seconds) in which Spaceman Spiff can
reach his ship safely.  </p>


<p> As an example consider a 4&times;4 grid that has only one
Blaster, at (3,2), with starting time 1 and frequency 3.  In the
grids below, <tt>S</tt> denotes Spaceman Spiff, <tt>B</tt>
denotes the blaster and <tt>P</tt> denotes a pulse.  The sequence
of grids describes a successful attempt to reach his ship that
takes 6 seconds.</p>

<pre style="margin:15px">
   t=0                t=1                t=2                t=3  
S  .  .  .         .  S  .  .         .  .  S  .         .  P  .  S
.  .  .  .         .  .  .  .         .  P  .  .         .  .  .  .
.  B  .  .         .  P  .  .         P  B  P  .         .  B  .  P
.  .  .  .         .  .  .  .         .  P  .  .         .  .  .  .
</pre>


<pre style="margin:15px">
   t=4                t=5                t=6
.  .  .  .         .  .  .  .         .  P  .  .
.  .  .  S         .  P  .  .         .  .  .  .
.  P  .  .         P  B  P  S         .  B  .  P
.  .  .  .         .  P  .  .         .  .  .  S
</pre>


<h6>Input format</h6>

<p>Line 1: Three space separated integers <em>N</em>, <em>M</em>
and <em>K</em>, describing the number of rows and columns in the
grid and the number of Blasters, respectively.</p>

<p>Lines 2 to <em>K</em>+1: These lines describe the <em>K</em>
blasters.  Each line has four space separated integers. The first
two integers on the line denote the row and column where the
Blaster is located, the third integer is its starting time, and
the fourth integer is its frequency.</p>

<h6>Output format</h6>

<p> The first line of output must either consist of the word
<tt>YES</tt>, if Spaceman Spiff can reach his ship safely, or the
word <tt>NO</tt>, if he cannot do so. If the output on the first
line is <tt>YES</tt> then the second line should contain a single
integer giving the least time, in seconds, that it takes him to
reach his ship safely.</p>

<h6>Sample Input 1</h6>

<pre style="margin:15px">
4 4 1
3 2 1 3
</pre>

<h6>Sample Output 1</h6>
<pre style="margin:15px">
YES
6
</pre>


<h6>Sample Input 2</h6>

<pre style="margin:15px">
5 5 2
5 1 1 2
4 4 1 2
</pre>

<h6>Sample Output 2</h6>
<pre style="margin:15px">
YES
8
</pre>



<h6>Test data</h6>


<p>In all subtasks, you may assume that:</p>
  
<ul>

<li> <p>2 &le; <em>N</em>,<em>M</em> &le; 2500. </p>

<li><p>All the frequencies are guaranteed to be integers between
1 and 3000, inclusive.</p>

<li><p>All the starting times are guaranteed to be integers
between 0 and 3000, inclusive.</p>

<li><p>All the coordinates of the Blasters are guaranteed to be
valid cells in the <em>N&times;M</em> grid. No two Blasters will
be on the same cell.</p>

</ul>

<p><b>Subtask 1 (30 marks)</b> : <em>K</em> = 1.</p>
<p><b>Subtask 2 (70 marks)</b> : 1 &le; <em>K</em> &le; 2500.</p>

<h6>Limits</h6>
<p>Time limit : 3s</p>
<p>Memory limit: 128 MB</p>


