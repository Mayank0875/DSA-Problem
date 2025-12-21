## Title
Zombie Horde

## Slug
zombie-horde

## Difficulty
Hard

## Description
Zombies gather in swarms. The mutation type of a swarm is determined by the most common zombie variant ID in the group.

Survivor Rick has a collection of $n$ zombies, where each zombie is represented by an integer ID.

To analyze the threat, Survivor Rick must partition these zombies into several non-empty swarms. Every zombie from the original collection must belong to exactly one swarm. From each swarm, a "mutation type" is extracted. The mutation type is defined as the **mode** (most frequent element) of the zombies in that swarm. If a swarm has multiple zombies tied for the most frequent appearance, any one of them can be chosen as the mutation type.

Survivor Rick collects all the extracted mutation types to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> mutation type is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> mutation types 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> mutation types 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> mutation types 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of zombies.
- The second line contains $n$ space-separated integers representing the zombie IDs.

## Output Format
- Return a single integer representing the number of different multisets of mutation types possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
