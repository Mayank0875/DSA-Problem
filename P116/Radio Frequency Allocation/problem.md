## Title
Radio Frequency Allocation

## Slug
radio-frequency-allocation

## Difficulty
Medium

## Description
Stations broadcast on frequency bands. Each station has a min Hz and max Hz.

The chart lists list of stations, each defined by a min Hz and an max Hz, represented as a pair `[min, max]`.

To prevent interference, the max frequency of one station must be strictly less than the min frequency of the next channel. Specifically, to transition from station `[a, b]` to a subsequent station `[c, d]`, the max of the first station must be **strictly less than** the min of the second station (i.e., `b < c`).

You can select stations in any order you like to form a valid spectrum allocation. Your goal is to determine the maximum number of stations that can be included in a single spectrum allocation.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest spectrum allocation is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The stations can be reordered to form the spectrum allocation `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available stations.
- The next `n` lines each contain two integers, representing the `min` and `max` of an station.

## Output Format
- Return a single integer representing the maximum length of the spectrum allocation.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
