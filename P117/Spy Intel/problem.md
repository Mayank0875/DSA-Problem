## Title
Spy Intel

## Slug
spy-intel

## Difficulty
Medium

## Description
Information is classified. The Director sees Top Secret, the Field Agent (you) sees Secret, and the Analyst sees Public info.

There are $3n$ files of varying importance available. The distribution follows a strict protocol. In each round, you must select any 3 files. The parties then claim them based on the following rules:

1. The **Director** takes the file with the **maximum** importance from the triplet.
2. You, the **Field Agent**, take the file with the **second maximum** importance.
3. The **Analyst** takes the remaining file (the one with the minimum importance).

This process repeats until all files are distributed. Your goal as the Field Agent is to maximize the total importance of the files you acquire.

Given an array of integers `files`, where `files[i]` represents the importance of the $i$-th file, return the maximum total importance you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 files. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Director takes `8`, you take `7`, Analyst takes `2`.
2. Pick the remaining `(1, 2, 4)`. Director takes `4`, you take `2`, Analyst takes `1`.
Total importance = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Director takes `5`, you take `4`, Analyst takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of files.
- The second line contains $3n$ space-separated integers representing the `files` array.

## Output Format
- Return a single integer representing the maximum total importance you can collect.

## Constraints
- 1 ≤ files.length ≤ 10^5
- `files.length` is divisible by 3.
- 1 ≤ files[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
