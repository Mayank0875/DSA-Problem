## Title
Archive Box Storage

## Slug
archive-box-storage

## Difficulty
Hard

## Description
A librarian stores `n` historical scrolls into `k` protective boxes. Scrolls vary in thickness and must stay in chronological order. The 'pressure' on a box is the square of the total thickness of scrolls inside it.

You must partition the sequence of scrolls into exactly `k` non-empty contiguous collections.
Each collection corresponds to a box.
The "pressure" for a box is calculated as the **square of the sum** of the thicknesses of the scrolls in that collection.

Your goal is to minimize the total pressure (the sum of the pressure values of all `k` collections).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the scrolls into 3 collections: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total pressure is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 collection is allowed, containing all scrolls. Sum = 15. pressure = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of scrolls and the required number of collections.
- The second line contains `n` integers representing the thicknesses of each scroll.

## Output Format
- Return one integer: the minimum total pressure.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
