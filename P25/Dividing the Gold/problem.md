## Title

Dividing the Gold

## Slug

dividing-the-gold

## Difficulty

Medium

## Description

A band of `k` adventurers has found a treasure trove of `n` gold piles, arranged in a line. Pile `i` contains `x[i]` gold coins. They must split the treasure fairly. Each adventurer must take a contiguous block of piles (e.g., adventurer 1 takes piles 1-2, adventurer 2 takes 3-4, etc.). To prevent squabbling, they agree to minimize the maximum amount of gold any single adventurer takes. Find this minimum-maximum amount.

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of gold piles and the number of adventurers.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the gold in the i-th pile.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy