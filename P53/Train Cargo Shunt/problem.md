## Title
Train Cargo Shunt

## Slug
train-cargo-shunt

## Difficulty
Easy

## Description
A freight train consists of loaded cars (non-zero weights) and empty flatbeds (`0`). At the railyard, a shunting locomotive pushes all the loaded cars to the front of the train assembly so they are together, moving all empty flatbeds to the rear.

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
