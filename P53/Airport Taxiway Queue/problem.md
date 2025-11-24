## Title
Airport Taxiway Queue

## Slug
airport-taxiway-queue

## Difficulty
Easy

## Description
Planes (non-zero flight numbers) are lined up on a taxiway. Some flights are cancelled and disappear (`0`). The tower directs the remaining planes to move forward and close the gaps, keeping the queue order, so the empty slots are at the back of the line.

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
- The first line contains a single integer n, the number of elements.
- The second line contains n space-separated integers representing the array.

## Output Format
- Print the modified array of integers separated by spaces.

## Constraints
- 1 ≤ n ≤ 1e4
- -1e9 ≤ nums[i] ≤ 1e9

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array
