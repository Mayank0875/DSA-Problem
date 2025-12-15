## Title
Forestry Logging

## Slug
forestry-logging

## Difficulty
Hard

## Description
A forest tract has `n` groves. `k` logging teams are assigned contiguous sectors. The 'ecological impact' of a sector is the square of the total biomass harvested there.

You must partition the sequence of groves into exactly `k` non-empty contiguous sectors.
Each sector corresponds to a team.
The "ecological impact" for a team is calculated as the **square of the sum** of the biomass values of the groves in that sector.

Your goal is to minimize the total ecological impact (the sum of the ecological impact values of all `k` sectors).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the groves into 3 sectors: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total ecological impact is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 sector is allowed, containing all groves. Sum = 15. ecological impact = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of groves and the required number of sectors.
- The second line contains `n` integers representing the biomass values of each grove.

## Output Format
- Return one integer: the minimum total ecological impact.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
