## Title

Previous Lower Encryption Level

## Slug

previous-lower-encryption-level

## Difficulty

Easy

## Description

You are exploring the mysterious Encrypted Valley, where each location records an encryption strength value. For every location, you need to determine the encryption strength of the nearest previous location that had a strictly lower value than the current one. If no such previous location exists (either because it’s the first location or all earlier values are higher or equal), you should indicate this. This information helps map out the valley’s security gradients. Your task is to compute this value for every location given the sequence of encryption strengths.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Location 0 (100): No previous location, output -1.  
Location 1 (80): Strength 100 at location 0 is not lower, output -1.  
Location 2 (60): Strengths 100, 80 are not lower, output -1.  
Location 3 (70): Strength 60 at location 2 is lower, output 60.  
Location 4 (60): Strengths 100, 80, 60, 70. None are strictly lower, output -1.  
Location 5 (75): Strength 60 at location 4 is the nearest lower, output 60.  
Location 6 (85): Strength 75 at location 5 is the nearest lower, output 75.  
Location 7 (110): Strength 85 at location 6 is the nearest lower, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All strengths are equal, so no strictly lower previous strength exists for any location.

## Input Format

The first line contains a single integer n, the number of locations.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the encryption strength for each location.

## Output Format

Return array of integers. The i-th integer should be the encryption strength at the nearest location j < i such that p_j < p_i. If no such location exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array