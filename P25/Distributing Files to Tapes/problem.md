## Title

Distributing Files to Tapes

## Slug

distributing-files-to-tapes

## Difficulty

Medium

## Description

You have `n` files, arranged in order, with sizes `x[i]`. You need to store these files on `k` old-fashioned magnetic tapes. Each tape can only store a contiguous block of files from the original list. You want to buy `k` tapes that are all the same size, so you need to find the smallest possible capacity for these tapes. This means you must minimize the maximum total size of files stored on any single tape.

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

- The first line contains two integers `n` and `k`: the number of files and the number of tapes.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the size of the i-th file.

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