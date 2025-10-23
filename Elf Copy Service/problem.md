## Title

Elf Copy Service

## Slug

elf-copy-service

## Difficulty

Easy

## Description

Santa needs more copies of a new toy blueprint! The head elf has the original blueprint and needs to make exactly n additional copies before the workshop starts. There are two magical copiers available.
The first copier takes x seconds to copy one blueprint (from the original or another copy), and the second copier takes y seconds. The elves can use either copier or both simultaneously. 
Help the head elf determine the minimum amount of time required to produce at least n new copies of the blueprint, starting with just the original.


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