## Title

Neural Maze Replication

## Slug

neural-maze

## Difficulty

Easy

## Description

In the sprawling Neural Maze, a central neuron holds a crucial activation pattern that must be propagated throughout the network before the next processing cycle begins. The master neuron needs to generate exactly **n** additional copies of this pattern. Two specialized replicator neurons are available:
the first replicator can copy a pattern in **x** seconds, and the second replicator can do it in **y** seconds. Both replicators can work on the original pattern or on any copy that already exists, and they may operate simultaneously.
Determine the minimum amount of time required for the master neuron to have at least **n** new copies of the activation pattern, starting with only the original one.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume replicator 1 takes 1 s, replicator 2 takes 2 s.
    1. Use replicator 1 on the original (1 s elapsed). Now we have 2 patterns. Need 4 more.
    2. Use replicator 1 on the original, replicator 2 on a copy (2 s elapsed total, 1 s more). Replicator 1 finishes. Now have 3 patterns. Need 3 more.
    3. Use replicator 1 on the original (3 s elapsed total, 1 s more). Replicator 2 finishes its first copy. Now have 4 patterns. Need 2 more.
    4. Use replicator 1 on the original, replicator 2 on a copy (4 s elapsed total, 1 s more). Replicator 1 finishes. Now have 5 patterns. Need 1 more. Replicator 2 finishes. Now have 6 patterns. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both replicators take 1 s.
    1. Use replicator 1 on original (1 s). Have 2 patterns. Need 3 more.
    2. Use replicator 1 and 2 on the available patterns (2 s). Have 4 patterns. Need 1 more.
    3. Use replicator 1 and 2 again (3 s). Have 6 patterns. We have enough.
Minimum time is 3 seconds.
  
## Input Format  

- Three space-separated integers n, x, and y.

## Output Format  

- Return single integer representing the minimum time in seconds required.
  

## Constraints  

- 1 ≤ n ≤ 1e8
- 1 ≤ x, y ≤ 10

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory