# pancake_Astar_search

Made by Ben Lam October 2024

Project aims to recreate the Astar search algorithm to solve the pancake problem, by using the gap heuristic. 

I will be treating this problem like a search algorithm, with the details as following:
* the set of states will be all the possible combinations that our stack of pancakes can assume.
* the goal state is the state where all the pancakes are stacked in order of size, with the largest at the bottom and the smallest at the top.
* the possible actions will be all the places that we can use to flip the pancakes at a certain "level". The order of the pancakes above the level will be reverse, while the order of the rest of the pancakes will remain untouched.
* a possible cost function would be the amount of stacks that it has taken for us to get to the current state, since we ideally would want to solve this question in as little flips as possible.
* a possible forward cost function could be the sum of the difference is sizes of our current stack when compared to the goal stack: e.g. what is the difference in size between the pancake at each level of our current stack compared to each level of the goal stack.
* However, I will be using the gap heuristic to solve the pancake problem. The gap heuristic essentially just involves counting the number of "gaps" in our stack, where a gap is defined when two consecutive levels are more than 1 size apart.

    