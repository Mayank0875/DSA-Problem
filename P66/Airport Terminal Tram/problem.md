## Title
Airport Terminal Tram

## Slug
airport-terminal-tram

## Difficulty
Medium

## Description
Two parallel airport concourses need shuttle walkways to ensure passenger flow if a section closes.

Two parallel concourses, Concourse A and Concourse B, each contain n gates arranged in a line.
Concourse A has an array `a` representing the passenger capacity of each gate.
Concourse B has an array `b` representing the passenger capacity of each gate.

Inside each concourse, adjacent gates are already connected by internal moving walkways.

You must establish inter-concourse shuttle trams connecting some gates of Concourse A to some gates of Concourse B.

The cost to create a tram between gate i of Concourse A and gate j of Concourse B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single gate is removed (from either Concourse A or Concourse B).
If one gate fails and disappears along with all its connections, the remaining gates must still form a single connected network.

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
It's optimal to connect four pairs of gates:
1. gate 1 from Concourse A with gate 2 from Concourse B: cost |1-4| = 3.
2. gate 3 from Concourse A with gate 2 from Concourse B: cost |1-4| = 3.
3. gate 2 from Concourse A with gate 1 from Concourse B: cost |10-20| = 10.
4. gate 2 from Concourse A with gate 3 from Concourse B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first gate of Concourse A with the first of Concourse B, and the last gate of Concourse A with the last of Concourse B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of gates in each concourse.
- The second line contains n integers representing the passenger capacitys of Concourse A.
- The third line contains n integers representing the passenger capacitys of Concourse B.

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
