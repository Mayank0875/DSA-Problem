## Title
Battery Pack Assembly

## Slug
battery-pack-assembly

## Difficulty
Hard

## Description
Cells with `n` capacities are assembled into `k` modules. Cells are placed in order. The 'thermal runaway risk' of a module is the square of its total capacity.

You must partition the sequence of cells into exactly `k` non-empty contiguous modules.
Each module corresponds to a module.
The "thermal runaway risk" for a module is calculated as the **square of the sum** of the capacities of the cells in that module.

Your goal is to minimize the total thermal runaway risk (the sum of the thermal runaway risk values of all `k` modules).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the cells into 3 modules: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total thermal runaway risk is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 module is allowed, containing all cells. Sum = 15. thermal runaway risk = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of cells and the required number of modules.
- The second line contains `n` integers representing the capacities of each cell.

## Output Format
- Return one integer: the minimum total thermal runaway risk.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
