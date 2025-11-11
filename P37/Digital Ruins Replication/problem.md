## Title

Digital Ruins Replication

## Slug

digital-ruins-replication

## Difficulty

Easy

## Description

Archaeologists have uncovered a priceless digital artifact stored in the ruins of an ancient server. The lead researcher possesses the original file and must create exactly n additional copies before the excavation ends. Two high‑speed data replicators are at their disposal.
The first replicator can duplicate a file in x seconds (whether from the original or any copy), and the second replicator takes y seconds. The team may operate either replicator alone or both at the same time.  
Determine the minimum amount of time required to produce at least n new copies of the artifact, starting with just the original file.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume replicator 1 takes 1s, replicator 2 takes 2s.
    1. Use replicator 1 on the original (1s elapsed). Now we have 2 files. Need 4 more.
    2. Use replicator 1 on original, replicator 2 on a copy (2s elapsed total, 1s more). Replicator 1 finishes. Now have 3 files. Need 3 more.
    3. Use replicator 1 on original (3s elapsed total, 1s more). Replicator 2 finishes its first copy. Now have 4 files. Need 2 more.
    4. Use replicator 1 on original, replicator 2 on a copy (4s elapsed total, 1s more). Replicator 1 finishes. Now have 5 files. Need 1 more. Replicator 2 finishes. Now have 6 files. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both replicators take 1s.
    1. Use replicator 1 on original (1s). Have 2 files. Need 3 more.
    2. Use replicator 1 and 2 on the available files (2s). Have 4 files. Need 1 more.
    3. Use replicator 1 and 2 again (3s). Have 6 files. We have enough.
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