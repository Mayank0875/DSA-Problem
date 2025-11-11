## Title

Recursive Tide

## Slug

recursive-tide

## Difficulty

Easy

## Description

The tide has risen, and the coastal village needs to fill exactly **n** water barrels before the next low tide. The chief tidekeeper has one full barrel of seawater and can use two magical pumps to duplicate water.  
The first pump can fill a barrel in **x** seconds, and the second pump can fill a barrel in **y** seconds. A pump can work on the original barrel or any barrel that has already been filled, and both pumps may operate simultaneously.  

Help the tidekeeper determine the minimum amount of time required to have at least **n** filled barrels, starting with just the original one.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 barrels. Assume pump 1 takes 1 s, pump 2 takes 2 s.
    1. Use pump 1 on the original barrel (1 s elapsed). Now we have 2 barrels. Need 4 more.
    2. Use pump 1 on the original, pump 2 on a copy (2 s elapsed total, 1 s more). Pump 1 finishes. Now have 3 barrels. Need 3 more.
    3. Use pump 1 on the original (3 s elapsed total, 1 s more). Pump 2 finishes its first fill. Now have 4 barrels. Need 2 more.
    4. Use pump 1 on the original, pump 2 on a copy (4 s elapsed total, 1 s more). Pump 1 finishes. Now have 5 barrels. Need 1 more. Pump 2 finishes. Now have 6 barrels. We have enough barrels.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 barrels. Both pumps take 1 s.
    1. Use pump 1 on original (1 s). Have 2 barrels. Need 3 more.
    2. Use pump 1 and 2 on the available barrels (2 s). Have 4 barrels. Need 1 more.
    3. Use pump 1 and 2 again (3 s). Have 6 barrels. We have enough.
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