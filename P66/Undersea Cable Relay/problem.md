## Title
Undersea Cable Relay

## Slug
undersea-cable-relay

## Difficulty
Medium

## Description
Two transoceanic fiber cables running parallel need interconnects to reroute data if a repeater fails.

Two parallel cables, Cable Alpha and Cable Omega, each contain n repeaters arranged in a line.
Cable Alpha has an array `a` representing the signal integrity of each repeater.
Cable Omega has an array `b` representing the signal integrity of each repeater.

Inside each cable, adjacent repeaters are already connected by internal fiber optics.

You must establish inter-cable bridge links connecting some repeaters of Cable Alpha to some repeaters of Cable Omega.

The cost to create a link between repeater i of Cable Alpha and repeater j of Cable Omega is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single repeater is removed (from either Cable Alpha or Cable Omega).
If one repeater fails and disappears along with all its connections, the remaining repeaters must still form a single connected network.

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
It's optimal to connect four pairs of repeaters:
1. repeater 1 from Cable Alpha with repeater 2 from Cable Omega: cost |1-4| = 3.
2. repeater 3 from Cable Alpha with repeater 2 from Cable Omega: cost |1-4| = 3.
3. repeater 2 from Cable Alpha with repeater 1 from Cable Omega: cost |10-20| = 10.
4. repeater 2 from Cable Alpha with repeater 3 from Cable Omega: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first repeater of Cable Alpha with the first of Cable Omega, and the last repeater of Cable Alpha with the last of Cable Omega, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of repeaters in each cable.
- The second line contains n integers representing the signal integritys of Cable Alpha.
- The third line contains n integers representing the signal integritys of Cable Omega.

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
