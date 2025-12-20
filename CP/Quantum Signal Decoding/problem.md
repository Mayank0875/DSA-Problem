## Title

Quantum Signal Decoding

## Slug

quantum-signal-decoding

## Difficulty

Medium

## Description

In the year 3042, archeologists discovered a stream of quantum data emitted by an ancient alien artifact. This data stream is represented as an array a of length n, consisting of non-negative integers.

To decode the message, scientists have defined the "energy" of a data segment from index l to r as the bitwise XOR sum of all elements in that segment:

f(l, r) = a_l ⊕ a_{l+1} ⊕ ... ⊕ a_r

However, the artifact's transmission is weighted by the duration of the signal. The "total importance" of a segment is the product of its energy f(l, r) and its length (r − l + 1).
Your task is to calculate the sum of the total importance for all possible subsegments [l, r] of the array.
Formally, compute:

sum over l = 1 to n, sum over r = l to n of
f(l, r) × (r − l + 1)

Since the result can be very large, print it modulo 998244353.

## Examples

### 1

#### Input

3
1 3 2

#### Output

12

#### Explanation

Total Sum is 12.
    
### 2

#### Input

4
39 68 31 80

#### Output

1337

#### Explanation

Total Sum is 1337.
  

## Input Format  

- The first line contains one integer $n$ — the length of the array.
- The second line contains $n$ integers a_1, a_2, ...., a_n.

## Output Format  

- Return a single integer — the total weighted XOR sum modulo $998244353$.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ a_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

maths, dynamic-programming