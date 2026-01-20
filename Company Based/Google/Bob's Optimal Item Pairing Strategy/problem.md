## Title

Bob's Optimal Item Pairing Strategy

## Slug

bobs-optimal-item-pairing-strategy

## Difficulty

Medium

## Description

Bob works in a large warehouse. He has a collection of $n$ items, where each item has a specific weight. The total number of items, $n$, is always an even number.

Bob needs to pack these items into boxes. Each box must contain exactly two items. His goal is to arrange the items into pairs such that the weight of the heaviest box is minimized. He wants to avoid having any single box that is too heavy.

Your task is to help Bob. You must calculate the minimized maximum weight of any pair after optimally grouping all the items.

## Examples

### 1

#### Input

4 
3 5 2 3

#### Output

7

#### Explanation

The elements can be paired as (3,3) and (5,2).
The sums are 3+3=6 and 5+2=7. The maximum is 7.
    
### 2

#### Input

6 
3 5 4 2 4 6

#### Output

8

#### Explanation

The elements can be paired as (3,5), (4,4), and (6,2).
The sums are 8, 8, and 8. The maximum is 8.

## Input Format  

- The first line contains an integer $n$, representing the number of items.
- The second line contains $n$ space-separated integers, representing the weights of the items.

## Output Format  

- Return a single integer representing the minimized maximum pair sum.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- $n$ is even
- 1 ≤ nums[i] ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, greedy, two-pointers, sorting