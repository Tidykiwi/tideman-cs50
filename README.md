# tideman-cs50
Console application that runs a "ranked-pairs" style election.<br><br>
Completed as part of studying CS50 - Introduction to Computer Science from Harvard University<br><br>

In a ranked-choice system, voters can vote for more than one candidate. Instead of just voting for their top choice, they can rank the candidates in order of preference. Here, each voter, in addition to specifying their first preference candidate, can also indicate their second and third choices. <br>
In such an election, a “Condorcet winner” of an election is the person who would have won any head-to-head matchup against another candidate.<br>

The Tideman voting method (also known as “ranked pairs”) is a ranked-choice voting method that’s guaranteed to produce the Condorcet winner of the election if one exists.

Generally speaking, the Tideman method works by constructing a “graph” of candidates, where an arrow (i.e. edge) from candidate A to candidate B indicates that candidate A wins against candidate B in a head-to-head matchup.


Implement a program that runs a Tideman election, per the below.<br>

./tideman Alice Bob Charlie<br>
Number of voters: 5<br><br>
Rank 1: Alice
Rank 2: Charlie
Rank 3: Bob

Rank 1: Alice
Rank 2: Charlie
Rank 3: Bob

Rank 1: Bob
Rank 2: Charlie
Rank 3: Alice

Rank 1: Bob
Rank 2: Charlie
Rank 3: Alice

Rank 1: Charlie
Rank 2: Alice
Rank 3: Bob

Charlie
