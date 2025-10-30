## Title

Binary Signal Analysis

## Slug

binary-signal-analysis

## Difficulty

Easy

## Description

A communication device receives a binary signal of length N, stored in array A (0s and 1s). You need to process Q analysis queries on this signal. Each query (L, R, Val) asks for the frequency of the bit `Val` (0 or 1) in the signal segment from index L to R. To verify the integrity of the analysis, you must output the XOR sum of all query answers.

## Examples

### 1

#### Input

6
[1, 0, 1, 1, 0, 0]
3
[[1, 3, 1], [2, 5, 0], [3, 6, 1]]

#### Output

2

#### Explanation
    •   Query 1 → Range [1, 3] → [1, 0, 1] → frequency of 1 = 2
    •   Query 2 → Range [2, 5] → [0, 1, 1, 0] → frequency of 0 = 2
    •   Query 3 → Range [3, 6] → [1, 1, 0, 0] → frequency of 1 = 2
    Now Xor of these frequency is 2.


### 2

#### Input

5
[0, 1, 1, 1, 0]
2
[[1, 1, 0], [2, 2, 1]]

#### Output

0

#### Explanation

Frequency are 1, 1 so Xor of 1 and 1 is 0.

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 or 1).
- The third line contains an integer Q, the number of queries.
- The next Q lines each contain three integers L, R, and Val.

## Output Format

- Return a single integer — the XOR of the answers to all queries.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1
- 1 ≤ q ≤ 10^5
- 1 ≤ L ≤ R ≤ N
- 0 ≤ Val ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum