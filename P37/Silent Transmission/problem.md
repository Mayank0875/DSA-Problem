## Title

Silent Transmission

## Slug

silent-transmission

## Difficulty

Easy

## Description

A covert agency must disseminate a secret message before the operation begins. The lead operative holds the original message and needs to create exactly **n** additional copies of it. Two encrypted transmitters are available.
The first transmitter can send one copy of the message (from the original or any existing copy) in **x** seconds, and the second transmitter can do the same in **y** seconds. The operatives may use either transmitter alone or both at the same time.
Determine the minimum amount of time required to produce at least **n** new copies of the secret message, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume copier 1 takes 1s, copier 2 takes 2s.
    1. Use copier 1 on the original (1s elapsed). Now we have 2 blueprints. Need 4 more.
    2. Use copier 1 on original, copier 2 on copy (2s elapsed total, 1s more). Copier 1 finishes. Now have 3 blueprints. Need 3 more.
    3. Use copier 1 on original (3s elapsed total, 1s more). Copier 2 finishes its first copy. Now have 4 blueprints. Need 2 more.
    4. Use copier 1 on original, copier 2 on a copy (4s elapsed total, 1s more). Copier 1 finishes. Now have 5 blueprints. Need 1 more. Copier 2 finishes. Now have 6 blueprints. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both copiers take 1s.
    1. Use copier 1 on original (1s). Have 2 blueprints. Need 3 more.
    2. Use copier 1 and 2 on the available blueprints (2s). Have 4 blueprints. Need 1 more.
    3. Use copier 1 and 2 again (3s). Have 6 blueprints. We have enough.
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