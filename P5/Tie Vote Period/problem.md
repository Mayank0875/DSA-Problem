## Title

Tie Vote Period

## Slug

tie-vote-period

## Difficulty

Easy

## Description

A voting record tracks N consecutive votes on a proposal, where '1' means a 'Yes' vote and '0' means a 'No' vote. We want to find the longest continuous sequence of votes where the number of 'Yes' votes exactly equals the number of 'No' votes. This identifies the longest period where opinion was perfectly split. Given the voting record, find the length of the longest such "tie period".

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The sequence [0, 1] (No, Yes) is the longest tie period.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (No, Yes) and [1, 0] (Yes, No) are the longest tie periods.

## Input Format

- The first line contains a single integer N, the total number of votes.
- The second line contains N space-separated integers, representing the votes (0 for No, 1 for Yes).

## Output Format

- Return a single integer representing the length of the longest contiguous tie period.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap
