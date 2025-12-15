## Title
Data Packet Stream

## Slug
data-packet-stream

## Difficulty
Medium

## Description
A server receives a file of size `n` KB. The file arrives in packets of size 1 to 6 KB.

File size is `n` KB.
Packets arrive in a stream. The sequence of packet sizes distinguishes the transmission flow.

Your task is to calculate the total number of distinct ways to receive the stream such that the total data size is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

## Examples

### 1

#### Input
8

#### Output
125

#### Explanation
There are 125 distinct sequences.

### 2

#### Input
3

#### Output
4

#### Explanation
There are 4 distinct sequences:
1+1+1
1+2
2+1
3

## Input Format
- The only input line has an integer `n`: the target data size.

## Output Format
- Return one integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
