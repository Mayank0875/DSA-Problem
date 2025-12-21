## Title
Ant Colony Pheromones

## Slug
ant-colony-pheromones

## Difficulty
Hard

## Description
Ants are organized into task forces. Each force emits a composite pheromone signal determined by the most common worker type in the group.

The Queen has a collection of $n$ ants, where each ant is represented by an integer ID.

To communicate with the colony, The Queen must partition these ants into several non-empty task forces. Every ant from the original collection must belong to exactly one task force. From each task force, a "pheromone signal" is extracted. The pheromone signal is defined as the **mode** (most frequent element) of the ants in that task force. If a task force has multiple ants tied for the most frequent appearance, any one of them can be chosen as the pheromone signal.

The Queen collects all the extracted pheromone signals to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

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
1. Partition into {1, 2, 2} -> pheromone signal is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> pheromone signals 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> pheromone signals 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> pheromone signals 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of ants.
- The second line contains $n$ space-separated integers representing the ant IDs.

## Output Format
- Return a single integer representing the number of different multisets of pheromone signals possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
