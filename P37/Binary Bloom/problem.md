## Title

Binary Bloom

## Slug

binary-bloom

## Difficulty

Easy

## Description

The garden of Binary Bloom needs to produce exactly **n** new blossoms before sunrise. The master gardener has a single original blossom and can use two enchanted sprayers to create more.  
The first sprayer takes **x** seconds to sprout a new blossom from any existing one, and the second sprayer takes **y** seconds. The gardener may operate either sprayer alone or both at the same time.  
Determine the minimum amount of time required to have at least **n** additional blossoms, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 blossoms. Assume sprayer 1 takes 1 s, sprayer 2 takes 2 s.
    1. Use sprayer 1 on the original (1 s elapsed). Now we have 2 blossoms. Need 4 more.
    2. Use sprayer 1 on the original, sprayer 2 on a blossom (2 s elapsed total, 1 s more). Sprayer 1 finishes. Now have 3 blossoms. Need 3 more.
    3. Use sprayer 1 on the original (3 s elapsed total, 1 s more). Sprayer 2 finishes its first sprout. Now have 4 blossoms. Need 2 more.
    4. Use sprayer 1 on the original, sprayer 2 on a blossom (4 s elapsed total, 1 s more). Sprayer 1 finishes. Now have 5 blossoms. Need 1 more. Sprayer 2 finishes. Now have 6 blossoms. We have enough blossoms.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 blossoms. Both sprayers take 1 s.
    1. Use sprayer 1 on the original (1 s). Have 2 blossoms. Need 3 more.
    2. Use sprayer 1 and 2 on the available blossoms (2 s). Have 4 blossoms. Need 1 more.
    3. Use sprayer 1 and 2 again (3 s). Have 6 blossoms. We have enough.
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