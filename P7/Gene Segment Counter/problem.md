## Title

Gene Segment Counter

## Slug

gene-segment-counter

## Difficulty

Easy

## Description

A geneticist is studying a strand of synthetic DNA of length N, represented by an array A (0 and 1 are two base types). They need to answer Q queries about this strand. Each query (L, R, Val) asks for the total count of base type `Val` (0 or 1) in the segment from L to R, inclusive. After answering all queries, the lab's computer must output the XOR of all the counts.

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