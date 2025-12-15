## Title
Cable Management

## Slug
cable-management

## Difficulty
Hard

## Description
An electrician bundles `n` wires into `k` conduits. Wires have different thicknesses. They must be bundled in sequence. The 'heat generation' of a conduit is the square of the total thickness of wires inside.

You must partition the sequence of wires into exactly `k` non-empty contiguous bundles.
Each bundle corresponds to a conduit.
The "heat generation" for a conduit is calculated as the **square of the sum** of the thicknesses of the wires in that bundle.

Your goal is to minimize the total heat generation (the sum of the heat generation values of all `k` bundles).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the wires into 3 bundles: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total heat generation is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 bundle is allowed, containing all wires. Sum = 15. heat generation = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of wires and the required number of bundles.
- The second line contains `n` integers representing the thicknesses of each wire.

## Output Format
- Return one integer: the minimum total heat generation.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
