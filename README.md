Download Link: https://assignmentchef.com/product/solved-geneticalgorithms-assignment-1-weapon-target-assignment-problem-wta
<br>



<strong><em>About the problem: </em></strong>

The WTA is a well-known optimization problem. Given a set of weapons of various types and a set of targets, we want to find the optimal assignment of the weapons to the targets in order to minimize the total expected threat coming from the targets. A target can have more than one weapon (of the same or a different type) assigned to it. On the other hand, a single weapon instance can only be assigned to one target (explained in the example).




<strong><em>What you are required to do: </em></strong>

Write a genetic algorithm to solve the WTA problem.

<strong><em>What the input looks like: </em></strong>

You’ll be given the weapon types, the number of each weapon type, the number of targets, the threat coefficient (V) of each target and a matrix containing the success probabilities of each weapon type against each target.

<strong><em>Example: </em></strong>

<table width="622">

 <tbody>

  <tr>

   <td width="622">Enter the weapon types and the number of instances of each type: (Enter“x” when you’re done)Tank 2Aircraft 1 Grenade 2 x Enter the number of targets:3 Enter the threat coefficient of each target:16510 Enter the weapons’ success probabilities matrix:0.3 0.6 0.50.4 0.5 0.40.1 0.2 0.2 Please wait while running the GA… The final WTA solution is:Tank #1 is assigned to target #1,Tank #2 is assigned to target #3,Aircraft #1 is assigned to target #1,Grenade #1 is assigned to target #2,Grenade #2 is assigned to target #2, The expected total threat of the surviving targets is 14.92</td>

  </tr>

 </tbody>

</table>

The weapons’ success probabilities matrix in this example means that:

<ul>

 <li>A tank has a 0.3 probability of damaging target #1, a 0.6 probability of damaging target #2 and a 0.5 probability of damaging target #3.</li>

 <li>An aircraft has a 0.4 probability of damaging target #1, a 0.5 probability of damaging target #2 and a 0.4 probability of damaging target #3.</li>

 <li>A grenade has a 0.1 probability of damaging target #1, a 0.2 probability of damaging target #2 and a 0.2 probability of damaging target #3.</li>

</ul>

<em>Note 1: </em>Your final solution doesn’t have to match the one in this example, but it should produce low threat. You could also display the output in a different format.

<em>Note 2: </em><strong>A single weapon instance can only be assigned to one target</strong>, so for example, grenade #1 is assigned to only one target (target #2) but target #2 has more than one weapon assigned to it (whatever the weapon type is).

<strong><em>Important remarks to help you solve the problem: </em></strong>

<ol>

 <li>The first thing you need to do is to think about how you will encode the solution in your chromosome. Formulate the problem with the objective function and constraints to help you figure out the next steps.</li>

 <li>You should use a <strong>binary, one-dimensional</strong></li>

 <li>The population size and initialization method you use are up to you. You can actually try different population sizes to see how this will affect your results. The maximum number of generations is also up to you.</li>

 <li>Think about your fitness function. It should be a function that measures the objective: <strong>minimize the expected total threat of the surviving targets</strong>.</li>

</ol>

<em>Note: </em>You are given the probability of target damage in a matrix which means that you can get the probability of target survival and use it in your equation!

<ol start="5">

 <li>Think about how you will handle <strong>infeasible solutions</strong>. Infeasible solutions are solutions that violate the constraints of the problem; therefore, they are not allowed.</li>

 <li>Choose the methods and parameters of selection, crossover, mutation and replacement that you find appropriate.</li>

</ol>