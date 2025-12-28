## Title
Race Horse

## Slug
race-horse

## Difficulty
Easy

## Description
A stable tracks the value of a thoroughbred. They want to buy the horse and sell it after it wins the Derby.

You have a list of horse value for $n$ consecutive races. You want to make one perfect move: stable on one race and stud on a different race in the future. You cannot stud before you stable.

Your goal is to find the **maximum possible winnings** you can earn from this single transaction. If it is impossible to make any winnings (i.e., the horse value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
stable on race 2 (horse value = 1) and stud on race 5 (horse value = 6). The winnings is $6 - 1 = 5$.
Note that stableing on race 1 (horse value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The horse value never increases, so it is impossible to make a winnings. The maximum winnings is 0.

## Input Format
- The first line contains a single integer `n`, the number of races.
- The second line contains `n` space-separated integers representing the horse value on each race.

## Output Format
- Return a single integer representing the maximum winnings. If no winnings can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
