## Title

Counting Cosmic Star Pairs

## Slug

counting-cosmic-star-pairs

## Difficulty

Medium

## Description

In the vast observatory of the Galactic Federation, astronomers study the luminosity of distant stars. A "Binary Star System" is formed when two distinct stars exert a gravitational pull on each other that results in perfect stability.

For a system to be stable, the sum of the luminosity values of the two stars must exactly equal a specific cosmic constant, known as the `target`.

You are given an integer array `luminosity` representing the brightness of available stars and an integer `target`. Your task is to count the total number of unique pairs of stars $(i, j)$ such that $i < j$ and their combined luminosity equals the `target`.

## Examples

### 1

#### Input

6 6
1 5 7 -1 5 1

#### Output

6

#### Explanation

Total 6 pair whose sum is 6.

### 2

#### Input

4 2
1 1 1 1

#### Output

6

#### Explanation

Every combination of two '1's sums to 2. The number of ways to choose 2 items from 4 is 6.

## Input Format

- The first line contains an integer $n$ and `target`, the number of stars and target.
- The second line contains $n$ space-separated integers representing `luminosity`.


## Output Format

- Return a single integer — total number of valid pairs.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ target ≤ 10^9
- 0 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array
