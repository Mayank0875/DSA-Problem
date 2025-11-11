## Title

Digital Mirage Replication

## Slug

digital-mirage-replication

## Difficulty

Easy

## Description

In the sprawling cyber‑city of Neonopolis, a rogue AI has created a coveted piece of code known as the *Digital Mirage*. To spread it across the network before the authorities intervene, a master hacker must generate exactly n additional copies of the Mirage. Two high‑speed servers are at the hacker’s disposal.

The first server can duplicate one instance of the Mirage (whether it’s the original or any copy) in x seconds, while the second server takes y seconds per copy. The hacker may operate either server alone or both simultaneously.

Determine the minimum amount of time required to produce at least n new copies of the Digital Mirage, starting with just the original instance.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume server 1 takes 1 s, server 2 takes 2 s.
    1. Use server 1 on the original (1 s elapsed). Now we have 2 instances. Need 4 more.
    2. Use server 1 on the original, server 2 on a copy (2 s elapsed total, 1 s more). Server 1 finishes. Now have 3 instances. Need 3 more.
    3. Use server 1 on the original (3 s elapsed total, 1 s more). Server 2 finishes its first copy. Now have 4 instances. Need 2 more.
    4. Use server 1 on the original, server 2 on a copy (4 s elapsed total, 1 s more). Server 1 finishes. Now have 5 instances. Need 1 more. Server 2 finishes. Now have 6 instances. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both servers take 1 s.
    1. Use server 1 on the original (1 s). Have 2 instances. Need 3 more.
    2. Use server 1 and 2 on the available instances (2 s). Have 4 instances. Need 1 more.
    3. Use server 1 and 2 again (3 s). Have 6 instances. We have enough.
Minimum time is 3 seconds.
  
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