## Title
Mountain Ridge Ziplines

## Slug
mountain-ridge-ziplines

## Difficulty
Medium

## Description
An adventure park spans two parallel mountain ridges and needs ziplines for access redundancy.

Two parallel ridges, North Ridge and South Ridge, each contain n platforms arranged in a line.
North Ridge has an array `a` representing the altitude of each platform.
South Ridge has an array `b` representing the altitude of each platform.

Inside each ridge, adjacent platforms are already connected by internal hiking trails.

You must establish inter-ridge ziplines connecting some platforms of North Ridge to some platforms of South Ridge.

The cost to create a zipline between platform i of North Ridge and platform j of South Ridge is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single platform is removed (from either North Ridge or South Ridge).
If one platform fails and disappears along with all its connections, the remaining platforms must still form a single connected network.

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
It's optimal to connect four pairs of platforms:
1. platform 1 from North Ridge with platform 2 from South Ridge: cost |1-4| = 3.
2. platform 3 from North Ridge with platform 2 from South Ridge: cost |1-4| = 3.
3. platform 2 from North Ridge with platform 1 from South Ridge: cost |10-20| = 10.
4. platform 2 from North Ridge with platform 3 from South Ridge: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first platform of North Ridge with the first of South Ridge, and the last platform of North Ridge with the last of South Ridge, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of platforms in each ridge.
- The second line contains n integers representing the altitudes of North Ridge.
- The third line contains n integers representing the altitudes of South Ridge.

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
