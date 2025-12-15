## Title
Radio Frequency Allocation

## Slug
radio-frequency-allocation

## Difficulty
Medium

## Description
A regulator assigns `n` stations to `m` frequencies.

However, not every station is compatible with every frequency due to broadcast range.
You are given a list of `k` compatible pairs, where a specific station can work with a specific frequency.

Your task is to determine the maximum number of licenses that can be formed simultaneously. Each station and each frequency can be assigned to at most one license.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 stations and 2 frequencies.
Possible valid matching could be:
- station 1 with frequency 2
- station 2 with frequency 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only station 1 and frequency 1 are compatible. The maximum number of operational licenses is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of stations, frequencies, and compatible pairs.
- The stations are numbered `1` to `n` and the frequencies are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that station `a` and frequency `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
