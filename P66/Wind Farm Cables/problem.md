## Title
Wind Farm Cables

## Slug
wind-farm-cables

## Difficulty
Medium

## Description
Two rows of wind turbines need redundant cabling to the grid.

Two parallel rows, Offshore Row and Inshore Row, each contain n turbines arranged in a line.
Offshore Row has an array `a` representing the power output of each turbine.
Inshore Row has an array `b` representing the power output of each turbine.

Inside each row, adjacent turbines are already connected by internal feeder cables.

You must establish inter-row redundancy lines connecting some turbines of Offshore Row to some turbines of Inshore Row.

The cost to create a line between turbine i of Offshore Row and turbine j of Inshore Row is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single turbine is removed (from either Offshore Row or Inshore Row).
If one turbine fails and disappears along with all its connections, the remaining turbines must still form a single connected network.

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
It's optimal to connect four pairs of turbines:
1. turbine 1 from Offshore Row with turbine 2 from Inshore Row: cost |1-4| = 3.
2. turbine 3 from Offshore Row with turbine 2 from Inshore Row: cost |1-4| = 3.
3. turbine 2 from Offshore Row with turbine 1 from Inshore Row: cost |10-20| = 10.
4. turbine 2 from Offshore Row with turbine 3 from Inshore Row: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first turbine of Offshore Row with the first of Inshore Row, and the last turbine of Offshore Row with the last of Inshore Row, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of turbines in each row.
- The second line contains n integers representing the power outputs of Offshore Row.
- The third line contains n integers representing the power outputs of Inshore Row.

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
