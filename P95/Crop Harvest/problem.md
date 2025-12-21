## Title
Crop Harvest

## Slug
crop-harvest

## Difficulty
Hard

## Description
Vegetables are packed into crates. The type of a crate is the most frequent vegetable ID inside.

Farmer John has a collection of $n$ vegetables, where each vegetable is represented by an integer ID.

To prepare for market, Farmer John must partition these vegetables into several non-empty crates. Every vegetable from the original collection must belong to exactly one crate. From each crate, a "crate type" is extracted. The crate type is defined as the **mode** (most frequent element) of the vegetables in that crate. If a crate has multiple vegetables tied for the most frequent appearance, any one of them can be chosen as the crate type.

Farmer John collects all the extracted crate types to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> crate type is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> crate types 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> crate types 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> crate types 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of vegetables.
- The second line contains $n$ space-separated integers representing the vegetable IDs.

## Output Format
- Return a single integer representing the number of different multisets of crate types possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
