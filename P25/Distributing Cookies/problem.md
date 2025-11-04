## Title

Distributing Cookies

## Slug

distributing-cookies

## Difficulty

Medium

## Description

You have baked `n` batches of cookies, which are lined up on the counter. Batch `i` has `x[i]` cookies. You need to pack these cookies into `k` boxes for `k` friends. You must pack contiguous batches into each box (e.g., box 1 gets batches 1-2, box 2 gets 3-5, etc.). You want to be fair, so you aim to minimize the maximum number of cookies any single friend receives. Find this minimum possible number.

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

- The first line contains two integers `n` and `k`: the number of batches and the number of boxes.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the number of cookies in the i-th batch.

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