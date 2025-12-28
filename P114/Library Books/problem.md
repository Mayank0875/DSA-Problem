## Title
Library Books

## Slug
library-books

## Difficulty
Medium

## Description
A reader follows references. A book's bibliography points to books several shelves away.

You start at the **first book** (index 0). Each book has a specific reference reach, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can jump forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can jump to any book at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last book** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Jump 1 step from index 0 to 1, then jump 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum jump length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of books.
- The second line contains `n` space-separated integers representing the `nums` array.

## Output Format
- Return `true` if the last index is reachable, `false` otherwise.

## Constraints
- 1 ≤ n ≤ 10^4
- 0 ≤ nums[i] ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
