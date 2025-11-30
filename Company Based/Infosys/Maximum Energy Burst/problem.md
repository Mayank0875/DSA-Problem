## Title

Maximum Energy Burst

## Slug

maximum-energy-burst

## Difficulty

Medium

## Description

A scientist is monitoring a new energy source. They have recorded a sequence of energy readings over N consecutive seconds. These readings can be positive (energy gain), negative (energy drain), or zero. The scientist wants to find the most powerful 'burst' of energy. A burst is defined as the `product` of all readings in a contiguous, non-empty period. Your task is to analyze the full sequence of readings and find the maximum product that can be achieved from any single contiguous subarray.

## Examples

### 1

#### Input

4 
[2, 3, -2, 4]

#### Output

6

#### Explanation

The contiguous subarray `[2, 3]` yields the largest product of 6.
    
### 2

#### Input

3 
[-2, 0, -1]


#### Output

0

#### Explanation

The subarray `[-2, -1]` is not contiguous and thus invalid. The subarray `[0]` yields a product of 0, which is the highest possible value in this case. 

## Input Format  

- The first line contains a single integer N, the number of energy readings.
- The second line contains N space-separated integers, nums_i, representing the energy reading at each second.

## Output Format  

- Return single integer representing the maximum product of any contiguous subarray.

  

## Constraints  

- 1 ≤ n ≤ 1e4
- -10 ≤ nums[i] ≤ 10
- The product of any subarray is guaranteed to fit in a 32-bit integer.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, dynamic-programming


## Companies
infosys