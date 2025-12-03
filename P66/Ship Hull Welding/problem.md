## Title
Ship Hull Welding

## Slug
ship-hull-welding

## Difficulty
Medium

## Description
A shipwright is welding two steel plates together with cross-beams for structural integrity.

Two parallel plates, Port Plate and Starboard Plate, each contain n rivets arranged in a line.
Port Plate has an array `a` representing the stress load of each rivet.
Starboard Plate has an array `b` representing the stress load of each rivet.

Inside each plate, adjacent rivets are already connected by internal welds.

You must establish inter-plate cross-beams connecting some rivets of Port Plate to some rivets of Starboard Plate.

The cost to create a beam between rivet i of Port Plate and rivet j of Starboard Plate is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single rivet is removed (from either Port Plate or Starboard Plate).
If one rivet fails and disappears along with all its connections, the remaining rivets must still form a single connected network.

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
It's optimal to connect four pairs of rivets:
1. rivet 1 from Port Plate with rivet 2 from Starboard Plate: cost |1-4| = 3.
2. rivet 3 from Port Plate with rivet 2 from Starboard Plate: cost |1-4| = 3.
3. rivet 2 from Port Plate with rivet 1 from Starboard Plate: cost |10-20| = 10.
4. rivet 2 from Port Plate with rivet 3 from Starboard Plate: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first rivet of Port Plate with the first of Starboard Plate, and the last rivet of Port Plate with the last of Starboard Plate, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of rivets in each plate.
- The second line contains n integers representing the stress loads of Port Plate.
- The third line contains n integers representing the stress loads of Starboard Plate.

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
