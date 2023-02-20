---
draft: false
title: "Question Paper ZCO 2011"
job_nature: ""
category: ""
---

<div id="cont">
<h5 align="left">Zonal Computing Olympiad, 2011</h5>
 <br>
  

  <p>The Zonal Computing Olympiad, 2011 was held in two sessions on Saturday, December 4, 2010.  Students could take part in either session.  The questions for the two sessions were as follows.</p>

<h5 style="font-weight: bold;"> Session 1, 10:00 am&ndash;1:00 pm IST</h5> <hr>

 <h5>  Hyper Mall</h5> <hr>
  <div id="cont">
<h6>Zonal Computing Olympiad 2011, 4 Dec 2010</h6>
  <h6>10:00 am&ndash;1:00 pm IST</h6>

<h6>Problem 1 : Hyper Mall</h6>


<p>
There are <em>M</em> shoppers, numbered 1,2,&hellip;,<em>M</em>
at the Siruseri HyperMall today.  We have information on the
precise time at which each shopper will complete his/her shopping
and arrive at the billing centre.  No two shoppers arrive at the
billing centre at the same time.  At the billing centre they
enter at the rear end of a queue.
</p>

<p>
There are <em>C</em> counters, numbered 1,2,&hellip;,<em>C</em>
at the billing centre.  When a shopper reaches the head of the
queue he waits for some counter to be available and then moves to
such a counter. If multiple counters are available he chooses the
one with lowest number.  We also have information on the amount
of time each shopper takes at the billing counter.
</p>


<p>
Let <em>t<sub>i</sub></em> be the time at which
shopper <em>i</em> finishes his/her shopping and arrives at the
billing centre and let <em>b<sub>i</sub></em> be the amount of
time he/she will take at the billing counter, where both
<em>t<sub>i</sub></em> and <em>b<sub>i</sub></em> are integers.
Your task is to determine the time at which the last shopper
leaves the HyperMall.
</p>

<p>
Here is an example with 4 shoppers and 2 counters. The table
below lists the values <em>t<sub>i</sub></em>
and <em>b<sub>i</sub></em> for the 4 shoppers.
</p>

<table border cellpadding=5 align=center>
  <tr>
    <td align=center> <em>i</em> </td><td align=right> 1 </td><td align=right> 2 </td><td align=right> 3 </td><td align=right> 4 </td>
  </tr>
  </tr>
    <td align=center> <em>t<sub>i</sub></em> </td><td align=right> 9 </td><td align=right> 7 </td><td align=right> 8 </td><td align=right>  10 </td>
  </tr>
  </tr>
    <td align=center> <em>b<sub>i</sub></em> </td><td align=right>  20  </td><td align=right> 14  </td><td align=right>  12  </td><td align=right>  11 </td>
  </tr>
  </tr>
</table>

<p>
The first to arrive at the billing center is shopper 2, who goes
to counter 1. The next to arrive is shopper 3, who immediately
goes to counter 2.  When the next shopper, shopper 1, arrives,
both the counters are occupied and hence he stands in the
queue. Subsequently, shopper 4 arrives and finds both counters
occupied, and hence stands behind 1 in the queue. At time 20,
shopper 3 finishes and so shopper 1 moves to counter 2. At time
21, shopper 2 finishes his billing and shopper 4 moves to counter
1.  Shopper 4 leaves at time 32 and, finally, shopper 1 leaves at
time 40.
</p>

<h6>Input format</h6>

<p>
The first line of input contains two integers giving the number
of shoppers <em>N</em> and the number of
counters <em>C</em>. This is followed by <em>N</em> lines each
containing two integers, the values <em>t<sub>i</sub></em>
and <em>b<sub>i</sub></em> for the
<em>N</em> shoppers.
</p>

<h6>Output format</h6>

<p>
A single line with a single integer indicating the time at which
the last shopper leaves the HyperMall.
</p>

<h6>Testdata</h6>

<p>
You may assume that 1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;100 and
1&nbsp;&le;&nbsp;<em>C</em>&nbsp;&le;&nbsp;50. You may assume that all input data and the
final answer can be stored in variables of type <tt>int</tt>.
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
4 2
9 20
7 14
8 12
10 11
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
40
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.</p>


<br>
<h5>   Number Game</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2011, 4 Dec 2010</h6>
  <h6>10:00 am&ndash;1:00 pm IST</h6>

<h6>Problem 2 : Number Game</h6>

<p>
Here is a game that you play against a friend.  You are given a
list of numbers. You move first and pick either the first or the
last number from the list, which is then removed from the
list. Your friend moves next and again picks either the first or
the last number from the list that remains.  You move alternately
in this manner till all the numbers in the list have been picked.
</p>

<p>
Your score at the end of the game is the sum of numbers
that you have picked.  Your friend is a master of the game and
will always play to ensure that your total score is as small as
possible.  Your aim is to compute your maximum score under these
circumstances. 
</p>

<p>
For instance, suppose that the sequence of numbers is the
following.
</p>

<blockquote>
2,5,3,3,2,1
</blockquote>

<p>
In this case, the maximum score you can obtain is 9.  To achieve
this, you pick 1 in the first round.  This forces your opponent
to pick one of the 2's.  Depending on which 2 he picks, you can
either pick 5 in the second round and 3 in the third round or 3
in the second round and 5 in the third round.
</p>

<h6>Input format</h6>

<p>
The first line of input is an integer <em>N</em>, the length of
the sequence.  The second line contains <em>N</em> integers, the
sequence on which the game is played.
</p>

<h6>Output format</h6>

<p>
A single line with a single integer indicating the maximum score
you can achieve.
</p>

<h6>Testdata</h6>

<p>
You may assume that 1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;2000.
Each number in the sequence is in the range [-2000,2000].
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
6
2 5 3 3 2 1
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
9
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 2 seconds.  The memory limit is
64MB.
</p>




 <br>
<h5 style="font-weight: bold;"> Session 2, 1:00 pm&ndash;4:00 pm IST</h5> <hr>
 
<br>
<h5>  Suitcase swappers</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2011, 4 Dec 2010</h6>
  <h6>2:00 pm&ndash;5:00 pm IST</h6>

<h6>Problem 1 : Suitcase swappers</h6>

<p>
T&pi;, the all new international terminal at Siruseri's
international airport, has recently been opened for service.  One
of its marvels is its baggage delivery system.
</p>

<p>
There are <em>N</em> conveyor belts that run in parallel from the
plane's parking position into the building, carrying bags from
the plane to the baggage delivery hall.  The loaders place one
bag on each of these <em>N</em> belts at the plane and these bags
move along the belt at the same rate and eventually emerge in the
baggage hall at the same time.
</p>

<p>
Unfortunately, there are some mischievous monkeys who have
sneaked into the airport and positioned themselves in between
some of the conveyor belts.  When a monkey sees bags pass by on
the two belts on either side of it, it swaps the bags.  As a
result, the order in which the bags reach the end of the line is
different from the order in which they were placed originally.
That is, if <em>b<sub>j</sub></em> is the bag that was originally
placed on conveyor belt <em>j</em>, it may arrive at the other
end on a different belt <em>k</em>,
where <em>k&nbsp;&ne;&nbsp;j</em>.
</p>

<p>
There are a number of such monkeys positioned at various places
along the route.  Each monkey swaps bags between a pair of
adjacent belts, but no two monkeys are at the same distance along
the route from the plane to the baggage hall.
</p>

<p>
Here is picture showing 5 conveyor belts and 5 monkeys positioned
along the route, and the effect that they have on the flow of the
bags.  The belts move from left to right.  The monkeys are M1,
M2, M3, M4 and M5, located at distances 10, 20, 30, 40 and 50,
respectively.  Monkey M1 swaps bags 2 and 3.  Monkey M2 swaps
bags 4 and 5.  Monkey M3 swaps bags 1 and 3.  Monkey M4 swaps
bags 2 and 5 and Monkey M5 swaps the same two bags back.
</p>

<img style="margin:15px" align=center width=40% src="swapper.jpg"/>

<p>
You will be given information about the locations of the monkeys
along the conveyor belts.  Assume that the bags placed on
the <em>N</em> belts are originally numbered
1,2,&hellip;,<em>N</em>, with bag <em>j</em> placed on
belt <em>j</em>.  Your task is to compute the order of the bags
in the output.  For instance, in the example above, the final
order of the bags is 3&nbsp;1&nbsp;2&nbsp;5&nbsp;4.
</p>


<h6>Input format</h6>

<p>
The first line of input contains two integers <em>N</em>
and <em>M</em>, where <em>N</em> is the number of conveyor belts
and <em>M</em> is the number of monkeys.  The next <em>M</em>
lines describe the location of the monkeys.  Each of the lines
has two integers <em>D</em> and <em>B</em> where <em>D</em> is
the distance in metres of the monkey from the start of the belts
and 1&nbsp;&le;&nbsp;B&nbsp;&le;&nbsp;N-1 is a belt number,
indicating that this monkey is standing between belts <em>B</em>
and <em>B</em>+1.  The monkeys need not be listed in the same
order as their distance from the start of the belts.
</p>

<h6>Output format</h6>

<p>
A single line with <em>N</em> numbers, describing the order in
which bags 1,2,&hellip;<em>N</em> emerge in the baggage hall.
</p>

<h6>Testdata</h6>

<p>
You may assume that
1&nbsp;&le;&nbsp;<em>M</em>&nbsp;&le;&nbsp;1000,
1&nbsp;&le;&nbsp;<em>N</em>&nbsp;&le;&nbsp;20000 and for each
monkey, its distance <em>D</em> is is in the range [1,10<sup>9</sup>].
No two monkeys are located at the same distance <em>D</em>.
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
5 5
50 3
30 1
20 4
40 3
10 2
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
3 1 2 5 4
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 1 second.  The memory limit is
32MB.
</p>


<br>
<h5>     Balancing Act</h5> <hr>

<div id="cont">
<h6>Zonal Computing Olympiad 2011, 4 Dec 2010</h6>
  <h6>2:00 pm&ndash;5:00 pm IST</h6>

<h6>Problem 2 : Balancing Act</h6>

<p>
Your team is playing a chess tournament against a visiting team.
Your opponents have arrived with a team of <em>M</em> players,
numbered 1,2,&hellip;,<em>M</em>.  You have <em>N</em> players,
numbered 1,2,&hellip;,<em>N</em> from which to choose your team,
where <em>N&nbsp;&ge;&nbsp;M</em>.
</p>

<p>
Each of the <em>M</em> players from the visiting team must be
paired up with one of your <em>N</em> players.  The tournament
rules insist that the pairings must respect the order that has
been fixed for both teams.  That is, when you pick
players <em>i<sub>1</sub></em>, 
<em>i<sub>2</sub></em>,&hellip;,<em>i<sub>M</sub></em>, 
to play against opponents numbered 1,2,&hellip;,<em>M</em>, it
must be the case that
<em>i<sub>1</sub>&lt;i<sub>2</sub>&lt;&hellip;&lt;i<sub>M</sub></em>,
in terms of the order 1,2,&hellip;,<em>N</em> in which your
players are listed.
</p>

<p>
You want to ensure a good fight, so you plan to pick your team so
that the teams are as evenly balanced as possible.  Each
player <em>j</em> on your team has a numerical
score <em>YS(j)</em> that represents his or her playing ability.
Likewise, each player <em>i</em> in the opponent team has a
playing ability indicated by a numerical
score <em>OS(i)</em>. The difference in strength between a
player <em>i<sub>j</sub></em> from your team and his or her
opponent <em>j</em> on the visiting team is the absolute value
|<em>YS(i<sub>j</sub>) - OS(j)</em>|.  The imbalance of a pairing
is the sum of these differences across all <em>M</em> match-ups
in the pairing.  Your aim is to minimize this imbalance.
</p>

<p>
For instance suppose you have six players, whose strengths are as
follows.
</p>

<table border cellpadding=5 align=center>
  <tr>
    <td colspan=7 align=center><em>Home Team</em></td>
  </tr>
  <tr>
    <td align=center> <em>i</em> </td><td align=right> 1 </td><td align=right> 2 </td><td align=right> 3 </td><td align=right> 4 </td><td align=right> 5 </td><td align=right> 6 </td>
  </tr>
  </tr>
    <td align=center> <em>YS(i)</em> </td><td align=right> 2 </td><td align=right> 3 </td><td align=right> 4 </td><td align=right>  1 </td><td align=right>  5 </td><td align=right>  7 </td>
  </tr>
</table>

<p>
Also, suppose that the visiting team has three players, whose
strengths are as follows.

<table border cellpadding=5 align=center>
  <tr>
    <td colspan=4 align=center><em>Visiting Team</em></td>
  </tr>
  <tr>
    <td align=center> <em>i</em> </td><td align=right> 1 </td><td align=right> 2 </td><td align=right> 3 </td>
  </tr>
  </tr>
    <td align=center> <em>OS(i)</em> </td><td align=right> 2 </td><td align=right> 9 </td><td align=right> 2 </td>
  </tr>
</table>

<p>
In this situation, the most balanced pairing is (1,1), (3,2) and (4,3),
which yields an imbalance of 
|<em>YS(1)-OS(1)</em>|+|<em>YS(3)-OS(2)</em>|+|<em>YS(4)-OS(3)</em>|=
|2-2|+|4-9|+|1-2| = 6.
</p>

<p>
Your task is to read a description of the two teams and calculate
the overall imbalance in the most balanced pairing.
</p>

<h6>Input format</h6>

<p>
The first line of input contains two integers <em>N</em>
and <em>M</em>, <em>N&nbsp;&ge;&nbsp;M</em>, the number of
players on the home team and the visiting team, respectively.
The second line of input contains <em>N</em> positive integers,
the strengths of the home team players in the order
1,2,&hellip;,<em>N</em>.  The third line of input
contains <em>M</em> integers, the strengths of the visiting
team players in the order 1,2,&hellip;,<em>M</em>.
</p>

<h6>Output format</h6>

<p>
A single line with a single integer indicating the sum of the
differences in strengths in the most balanced pairing.
</p>

<h6>Testdata</h6>

<p>
You may assume that
1&nbsp;&le;&nbsp;<em>M&nbsp;&le;&nbsp;N</em>&nbsp;&le;&nbsp;2000.
All players' strengths are in the range [1,2000].
</p>

<h6>Sample Input</h6>
<pre style="margin:15px">
6 3
2 3 4 1 5 7
2 9 2
</pre>

<h6>Sample Output</h6>
<pre style="margin:15px">
6
</pre>

<h6>Time and memory limits</h6>

<p>
The time limit for this task is 2 seconds.  The memory limit is
64MB.
</p>



