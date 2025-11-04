## Title

Train Car Grouping

## Slug

train-car-grouping

## Difficulty

Medium

## Description

A train has `n` cars in a row, with car `i` containing `x[i]` passengers. The train needs to be split into `k` smaller trains (sub-trains). Each sub-train must consist of a contiguous block of cars from the original train. The goal is to minimize the maximum number of passengers on any single sub-train. Find this minimum value.

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

- The first line contains two integers `n` and `k`: the number of cars and the number of sub-trains.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the passenger count of the i-th car.

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