## Title
Space Debris Cleanup

## Slug
space-debris-cleanup

## Difficulty
Easy

## Description
A space station's garbage disposal system uses a magnetic tractor beam. Valuable scrap metal (represented by non-zero integers) needs to be pulled to the airlock at the front of the queue for recovery. Empty space or dust pockets (represented by `0`) should be pushed to the back for ejection. Given a scan of the debris field, reorder the items so all scrap comes first, maintaining relative order, followed by the empty pockets.

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
