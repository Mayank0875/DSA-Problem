## Title
The Anti-Gravity Chamber

## Slug
the-anti-gravity-chamber

## Difficulty
Easy

## Description
In a futuristic laboratory, scientists are testing a new linear anti-gravity chamber. A series of test containers are lined up in a row, represented by an array of integers. Some containers hold dense matter (represented by non-zero integers), while others are empty (represented by `0`).

To prepare for the experiment, the scientists need to activate a unidirectional gravity field that pulls all containers with dense matter to the front of the chamber, causing all empty containers (`0`s) to float to the very end.

It is vital for the experiment that the relative order of the dense matter containers remains exactly as it was originally. Additionally, due to the delicate calibration of the chamber sensors, you must perform this rearrangement in-place without using extra storage for a new array.

## Examples
### 1
#### Input
5
0 1 0 3 12
#### Output
1 3 12 0 0
#### Explanation
The non-zero elements are 1, 3, and 12. They are moved to the front while maintaining their order, and the two 0s are pushed to the end.

### 2
#### Input
1
0
#### Output
0
#### Explanation
There is only one element, which is 0, so no changes are needed.

## Input Format
- The first line contains a single integer $n$, the number of containers.
- The second line contains $n$ space-separated integers representing the `nums` array.

## Output Format
- Print the modified array of integers separated by spaces.

## Constraints
- 1 ≤ x ≤ 1e4
- -1e9 ≤ nums[i] ≤ 1e9

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array