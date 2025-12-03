## Title
Chain Mail Armor

## Slug
chain-mail-armor

## Difficulty
Medium

## Description
Two rows of rings in chain mail need interconnecting rings to stop a sword thrust.

Two parallel rows, Top Row and Bottom Row, each contain n rings arranged in a line.
Top Row has an array `a` representing the diameter of each ring.
Bottom Row has an array `b` representing the diameter of each ring.

Inside each row, adjacent rings are already connected by internal interlocks.

You must establish inter-row connectors connecting some rings of Top Row to some rings of Bottom Row.

The cost to create a connector between ring i of Top Row and ring j of Bottom Row is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single ring is removed (from either Top Row or Bottom Row).
If one ring fails and disappears along with all its connections, the remaining rings must still form a single connected network.

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
It's optimal to connect four pairs of rings:
1. ring 1 from Top Row with ring 2 from Bottom Row: cost |1-4| = 3.
2. ring 3 from Top Row with ring 2 from Bottom Row: cost |1-4| = 3.
3. ring 2 from Top Row with ring 1 from Bottom Row: cost |10-20| = 10.
4. ring 2 from Top Row with ring 3 from Bottom Row: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first ring of Top Row with the first of Bottom Row, and the last ring of Top Row with the last of Bottom Row, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of rings in each row.
- The second line contains n integers representing the diameters of Top Row.
- The third line contains n integers representing the diameters of Bottom Row.

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
