## Title
Military Platoon March

## Slug
military-platoon-march

## Difficulty
Hard

## Description
A regiment has `n` squads. They march in `k` columns. Squads stay in formation order. The 'ground vibration' caused by a column is the square of the total weight of soldiers in that column.

You must partition the sequence of squads into exactly `k` non-empty contiguous columns.
Each column corresponds to a column.
The "ground vibration" for a column is calculated as the **square of the sum** of the weights of the squads in that column.

Your goal is to minimize the total ground vibration (the sum of the ground vibration values of all `k` columns).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the squads into 3 columns: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total ground vibration is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 column is allowed, containing all squads. Sum = 15. ground vibration = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of squads and the required number of columns.
- The second line contains `n` integers representing the weights of each squad.

## Output Format
- Return one integer: the minimum total ground vibration.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
