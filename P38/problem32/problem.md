## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Easy

## Description

In the realm of enchanted programming, a mysterious loop appears on a sequence of enchanted stones. Each stone bears a magical number. For every stone, you must discover the number on the nearest previous stone where the magic value is **strictly lower** than the current stone's value. If no such stone exists (either because it is the first stone or all earlier stones have values that are higher or equal), the loop vanishes and you should indicate this with `-1`. Determining these values helps unravel the pattern of the vanishing loop across the sequence.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Stone 0 (100): No previous stone, output -1.  
Stone 1 (80): Value 100 on stone 0 is not lower, output -1.  
Stone 2 (60): Values 100, 80 are not lower, output -1.  
Stone 3 (70): Value 60 on stone 2 is lower, output 60.  
Stone 4 (60): Values 100, 80, 60, 70. None are strictly lower, output -1.  
Stone 5 (75): Value 60 on stone 4 is the nearest lower, output 60.  
Stone 6 (85): Value 75 on stone 5 is the nearest lower, output 75.  
Stone 7 (110): Value 85 on stone 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All values are equal, so no strictly lower previous value exists for any stone.

## Input Format

The first line contains a single integer n, the number of stones.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the magical value on each stone.

## Output Format

Return array of integers. The i‑th integer should be the value on the nearest stone j < i such that p_j < p_i. If no such stone exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array