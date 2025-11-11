## Title

Data Rift Replication

## Slug

data-rift-replication

## Difficulty

Easy

## Description

A critical data rift has been detected, and the central server holds the original data file. Before the rift expands, the system must produce exactly n additional copies of this file. Two replication nodes are available.
The first node can replicate a file (from the original or any existing copy) in x seconds, and the second node can do it in y seconds. The nodes may operate independently or simultaneously.
Determine the minimum amount of time required to have at least n new copies of the file, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume node 1 takes 1s, node 2 takes 2s.
    1. Use node 1 on the original (1s elapsed). Now we have 2 files. Need 4 more.
    2. Use node 1 on original, node 2 on a copy (2s elapsed total, 1s more). Node 1 finishes. Now have 3 files. Need 3 more.
    3. Use node 1 on original (3s elapsed total, 1s more). Node 2 finishes its first copy. Now have 4 files. Need 2 more.
    4. Use node 1 on original, node 2 on a copy (4s elapsed total, 1s more). Node 1 finishes. Now have 5 files. Need 1 more. Node 2 finishes. Now have 6 files. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both nodes take 1s.
    1. Use node 1 on original (1s). Have 2 files. Need 3 more.
    2. Use node 1 and 2 on the available files (2s). Have 4 files. Need 1 more.
    3. Use node 1 and 2 again (3s). Have 6 files. We have enough.
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