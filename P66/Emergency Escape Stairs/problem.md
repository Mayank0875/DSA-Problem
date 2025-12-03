## Title
Emergency Escape Stairs

## Slug
emergency-escape-stairs

## Difficulty
Medium

## Description
Two stairwells in a building need cross-passages for fire safety.

Two parallel stairwells, East Stairs and West Stairs, each contain n landings arranged in a line.
East Stairs has an array `a` representing the floor level of each landing.
West Stairs has an array `b` representing the floor level of each landing.

Inside each stairwell, adjacent landings are already connected by internal stairs.

You must establish inter-stairwell fire doors connecting some landings of East Stairs to some landings of West Stairs.

The cost to create a door between landing i of East Stairs and landing j of West Stairs is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single landing is removed (from either East Stairs or West Stairs).
If one landing fails and disappears along with all its connections, the remaining landings must still form a single connected network.

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
It's optimal to connect four pairs of landings:
1. landing 1 from East Stairs with landing 2 from West Stairs: cost |1-4| = 3.
2. landing 3 from East Stairs with landing 2 from West Stairs: cost |1-4| = 3.
3. landing 2 from East Stairs with landing 1 from West Stairs: cost |10-20| = 10.
4. landing 2 from East Stairs with landing 3 from West Stairs: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first landing of East Stairs with the first of West Stairs, and the last landing of East Stairs with the last of West Stairs, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of landings in each stairwell.
- The second line contains n integers representing the floor levels of East Stairs.
- The third line contains n integers representing the floor levels of West Stairs.

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
