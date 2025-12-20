## Title
Supply Chain Logistics

## Slug
supply-chain-logistics

## Difficulty
Medium

## Description
A manager tracks the ID of packages moving through a conveyor belt.

The package line is represented as an array `a` of length `n`, consisting of non-negative integers.

To analyze this, we define the "batch ID" of a segment from index `l` to `r` as the bitwise XOR sum of all elements in that segment:
$$f(l, r) = a_l \oplus a_{l+1} \oplus \dots \oplus a_r$$

However, the shipping cost is calculated based on the batch size. The "shipping cost" of a segment is the product of its batch ID `f(l, r)` and its length `(r - l + 1)`.

Your task is to calculate the sum of the shipping cost for all possible subsegments `[l, r]` of the array.
Formally, compute:
$$ \sum_{l=1}^{n} \sum_{r=l}^{n} (f(l, r) \times (r - l + 1)) $$

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
- The first line contains one integer `n` — the length of the array.
- The second line contains `n` integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer — the total weighted XOR sum modulo 998244353.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
