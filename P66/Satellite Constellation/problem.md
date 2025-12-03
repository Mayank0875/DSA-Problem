## Title
Satellite Constellation

## Slug
satellite-constellation

## Difficulty
Medium

## Description
Two orbital planes of satellites need laser interlinks to maintain the network if a satellite is lost.

Two parallel planes, Polar Orbit and Equatorial Orbit, each contain n satellites arranged in a line.
Polar Orbit has an array `a` representing the orbital altitude of each satellite.
Equatorial Orbit has an array `b` representing the orbital altitude of each satellite.

Inside each plane, adjacent satellites are already connected by internal radio signals.

You must establish inter-plane laser links connecting some satellites of Polar Orbit to some satellites of Equatorial Orbit.

The cost to create a link between satellite i of Polar Orbit and satellite j of Equatorial Orbit is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single satellite is removed (from either Polar Orbit or Equatorial Orbit).
If one satellite fails and disappears along with all its connections, the remaining satellites must still form a single connected network.

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
It's optimal to connect four pairs of satellites:
1. satellite 1 from Polar Orbit with satellite 2 from Equatorial Orbit: cost |1-4| = 3.
2. satellite 3 from Polar Orbit with satellite 2 from Equatorial Orbit: cost |1-4| = 3.
3. satellite 2 from Polar Orbit with satellite 1 from Equatorial Orbit: cost |10-20| = 10.
4. satellite 2 from Polar Orbit with satellite 3 from Equatorial Orbit: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first satellite of Polar Orbit with the first of Equatorial Orbit, and the last satellite of Polar Orbit with the last of Equatorial Orbit, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of satellites in each plane.
- The second line contains n integers representing the orbital altitudes of Polar Orbit.
- The third line contains n integers representing the orbital altitudes of Equatorial Orbit.

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
