## Title

Market Equilibrium Period

## Slug

market-equilibrium-period

## Difficulty

Easy

## Description

An analyst tracks daily stock market movements, marking a day as '0' if the market went down and '1' if it went up compared to the previous day. They are looking for the longest continuous period where the market experienced an equal number of up days and down days, signifying a period of equilibrium. Given the sequence of daily market movements, find the length of the longest such equilibrium period.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The period [0, 1] (Down, Up) is the longest with an equal number of up and down days.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

Periods [0, 1] (Down, Up) and [1, 0] (Up, Down) are the longest equilibrium periods.

## Input Format

- The first line contains a single integer N, the number of days tracked.
- The second line contains N space-separated integers, where 0 represents a down day and 1 represents an up day.

## Output Format

- Return a single integer representing the length of the longest contiguous period with an equal number of 0s and 1s.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap, finance