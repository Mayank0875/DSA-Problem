## Title
Telecom Signal Towers

## Slug
telecom-signal-towers

## Difficulty
Hard

## Description
A region has `n` settlements. `k` signal towers are placed to cover contiguous groups of settlements. The 'signal interference' for a tower is the square of the total population it serves.

You must partition the sequence of settlements into exactly `k` non-empty contiguous coverage areas.
Each area corresponds to a tower.
The "signal interference" for a tower is calculated as the **square of the sum** of the populations of the settlements in that area.

Your goal is to minimize the total signal interference (the sum of the signal interference values of all `k` coverage areas).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the settlements into 3 coverage areas: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total signal interference is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 area is allowed, containing all settlements. Sum = 15. signal interference = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of settlements and the required number of coverage areas.
- The second line contains `n` integers representing the populations of each settlement.

## Output Format
- Return one integer: the minimum total signal interference.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
