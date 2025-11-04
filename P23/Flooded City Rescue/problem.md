## Title

Flooded City Rescue

## Slug

flooded-city-rescue

## Difficulty

Medium

## Description

A city is flooding, and you need to pump `t` gallons of water out. You have `n` different pumps. Each pump `i` works at a constant rate, taking `k[i]` seconds to remove one gallon. All pumps can run in parallel. What is the minimum time required to pump at least `t` gallons of water?

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