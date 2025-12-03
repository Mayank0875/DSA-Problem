## Title
Subway Tunnel Ventilation

## Slug
subway-tunnel-ventilation

## Difficulty
Medium

## Description
Two parallel subway tunnels require interconnecting ventilation shafts for safety.

Two parallel tunnels, Line 1 and Line 2, each contain n sections arranged in a line.
Line 1 has an array `a` representing the air pressure of each section.
Line 2 has an array `b` representing the air pressure of each section.

Inside each tunnel, adjacent sections are already connected by internal tracks.

You must establish inter-tunnel air ducts connecting some sections of Line 1 to some sections of Line 2.

The cost to create a duct between section i of Line 1 and section j of Line 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single section is removed (from either Line 1 or Line 2).
If one section fails and disappears along with all its connections, the remaining sections must still form a single connected network.

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
It's optimal to connect four pairs of sections:
1. section 1 from Line 1 with section 2 from Line 2: cost |1-4| = 3.
2. section 3 from Line 1 with section 2 from Line 2: cost |1-4| = 3.
3. section 2 from Line 1 with section 1 from Line 2: cost |10-20| = 10.
4. section 2 from Line 1 with section 3 from Line 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first section of Line 1 with the first of Line 2, and the last section of Line 1 with the last of Line 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of sections in each tunnel.
- The second line contains n integers representing the air pressures of Line 1.
- The third line contains n integers representing the air pressures of Line 2.

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
