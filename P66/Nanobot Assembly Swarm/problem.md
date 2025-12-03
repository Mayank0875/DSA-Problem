## Title
Nanobot Assembly Swarm

## Slug
nanobot-assembly-swarm

## Difficulty
Medium

## Description
Two lines of nanobots need to link up to form a rigid structure.

Two parallel lines, Line Alpha and Line Beta, each contain n bots arranged in a line.
Line Alpha has an array `a` representing the charge of each bot.
Line Beta has an array `b` representing the charge of each bot.

Inside each line, adjacent bots are already connected by internal magnetic fields.

You must establish inter-line physical links connecting some bots of Line Alpha to some bots of Line Beta.

The cost to create a link between bot i of Line Alpha and bot j of Line Beta is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single bot is removed (from either Line Alpha or Line Beta).
If one bot fails and disappears along with all its connections, the remaining bots must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of bots:
1. bot 1 from Line Alpha with bot 2 from Line Beta: cost |1-4| = 3.
2. bot 3 from Line Alpha with bot 2 from Line Beta: cost |1-4| = 3.
3. bot 2 from Line Alpha with bot 1 from Line Beta: cost |10-20| = 10.
4. bot 2 from Line Alpha with bot 3 from Line Beta: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first bot of Line Alpha with the first of Line Beta, and the last bot of Line Alpha with the last of Line Beta, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of bots in each line.
- The second line contains n integers representing the charges of Line Alpha.
- The third line contains n integers representing the charges of Line Beta.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
