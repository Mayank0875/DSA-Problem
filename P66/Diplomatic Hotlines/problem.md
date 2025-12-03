## Title
Diplomatic Hotlines

## Slug
diplomatic-hotlines

## Difficulty
Medium

## Description
Two alliances need secure hotlines between their capitals to prevent war.

Two parallel alliances, NATO and Warsaw Pact, each contain n capitals arranged in a line.
NATO has an array `a` representing the GDP of each capital.
Warsaw Pact has an array `b` representing the GDP of each capital.

Inside each alliance, adjacent capitals are already connected by internal treaties.

You must establish inter-alliance hotlines connecting some capitals of NATO to some capitals of Warsaw Pact.

The cost to create a hotline between capital i of NATO and capital j of Warsaw Pact is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single capital is removed (from either NATO or Warsaw Pact).
If one capital fails and disappears along with all its connections, the remaining capitals must still form a single connected network.

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
It's optimal to connect four pairs of capitals:
1. capital 1 from NATO with capital 2 from Warsaw Pact: cost |1-4| = 3.
2. capital 3 from NATO with capital 2 from Warsaw Pact: cost |1-4| = 3.
3. capital 2 from NATO with capital 1 from Warsaw Pact: cost |10-20| = 10.
4. capital 2 from NATO with capital 3 from Warsaw Pact: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first capital of NATO with the first of Warsaw Pact, and the last capital of NATO with the last of Warsaw Pact, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of capitals in each alliance.
- The second line contains n integers representing the GDPs of NATO.
- The third line contains n integers representing the GDPs of Warsaw Pact.

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
