## Title

Conveyor Belt Rotation

## Slug

conveyor-belt-rotation

## Difficulty

Easy

## Description

You are an engineer at a factory. Items are placed on a conveyor belt, represented by an array. At the end of the shift, the belt rotates $k$ steps to the right. A rotation to the right means the last item on the belt moves to the first position, and all other items shift one spot to the right. This process is repeated $k$ times, where $k$ is non-negative.

Your task is to determine the final arrangement of the items on the belt. You must modify the array in-place, without creating a new belt.

## Examples

### 1

#### Input

7 3 
[1, 2, 3, 4, 5, 6, 7]

#### Output

[5, 6, 7, 1, 2, 3, 4]

#### Explanation

After 1 rotation: `[7, 1, 2, 3, 4, 5, 6]`
After 2 rotations: `[6, 7, 1, 2, 3, 4, 5]`
After 3 rotations: `[5, 6, 7, 1, 2, 3, 4]`
    
### 2

#### Input

4 2 
[-1, -100, 3, 99]

#### Output

[3, 99, -1, -100]

#### Explanation

After 1 rotation: `[99, -1, -100, 3]`
After 2 rotations: `[3, 99, -1, -100]`
  

## Input Format  

- The first line contains two integers, n and k, the number of items on the belt and the number of rotations.
- The second line contains n space-separated integers, nums_i, representing the items.

## Output Format  

- Return array containing the n integers in their new order.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ k ≤ 1e5
- -1e9 ≤ nums[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers

## Company
facebook