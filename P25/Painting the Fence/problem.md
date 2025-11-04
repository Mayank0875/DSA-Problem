## Title

Painting the Fence

## Slug

painting-the-fence

## Difficulty

Medium

## Description

You have `n` fence sections, arranged side-by-side, that need painting. Each section `i` has a length of `x[i]`. You have `k` painters. To be efficient, each painter must be assigned a contiguous block of fence sections (e.g., painter 1 gets sections 1 to `j`, painter 2 gets `j+1` to `m`, etc.). You want to finish the job as fast as possible, so you must minimize the workload of the busiest painter. Find the minimum possible value for the maximum total length assigned to any single painter.

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

- The first line contains