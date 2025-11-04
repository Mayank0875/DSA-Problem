## Title

Printing Press Deadline

## Slug

printing-press-deadline

## Difficulty

Medium

## Description

A publishing house needs to print `t` copies of a new book before a major deadline. They have `n` different printing presses. Each press `i` works at its own pace, taking `k[i]` seconds to print one book. All presses can run in parallel. What is the shortest amount of time they need to print all `t` books?

## Examples

### 1

#### Input

3 7 
3 2 5


#### Output

8

#### Explanation

In 8 seconds:
    Machine 1 (3s/toy) makes floor(8/3) = 2 toys.
    Machine 2 (2s/toy) makes floor(8/2) = 4 toys.
    Machine 3 (5s/toy) makes floor(8/5) = 1 toy.
Total toys = 2 + 4 + 1 = 7.
It's impossible to make 7 toys in less than 8 seconds.

### 2

#### Input

1 1000000000
1

#### Output

1000000000


#### Explanation

It's impossible to make 1000000000 toys in less than 1000000000 seconds.

## Input Format

- The first line contains two integers n and t, the number of machines (elves) and the total number of toys required.
- The second line contains n integers k[1], k[2] ... k[n] , where k[i] is the time in seconds it takes for the i-th machine to produce one toy.
## Output Format

- Return a single integer representing the minimum time required to produce at least t toys.

## Constraints

- 1 ≤ n ≤ 2e5
- 1 ≤ t, k[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy