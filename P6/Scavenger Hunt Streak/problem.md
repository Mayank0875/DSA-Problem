## Title

Scavenger Hunt Streak

## Slug

scavenger-hunt-streak

## Difficulty

Medium

## Description

You are on a scavenger hunt with N clues lined up. Finding clue `i` gives you a "time bonus" of `A[i]` minutes (an integer from 0 to 9).
A "fast streak" is a contiguous sequence of clues, from L to R, where the total time bonus gained (`A[L] + ... + A[R]`) is exactly equal to the number of clues found in that streak (R - L + 1).
How many different fast streaks are there in the scavenger hunt?

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 fast streaks: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 fast streaks: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of fast streaks.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map