## Title
Solar Panel Strings

## Slug
solar-panel-strings

## Difficulty
Hard

## Description
A solar farm has `n` panels in a row. They are wired into `k` strings. The 'inverter load' for a string is the square of the total wattage of panels connected to it.

You must partition the sequence of panels into exactly `k` non-empty contiguous strings.
Each string corresponds to a inverter.
The "inverter load" for a inverter is calculated as the **square of the sum** of the wattages of the panels in that string.

Your goal is to minimize the total inverter load (the sum of the inverter load values of all `k` strings).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the panels into 3 strings: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total inverter load is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 string is allowed, containing all panels. Sum = 15. inverter load = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of panels and the required number of strings.
- The second line contains `n` integers representing the wattages of each panel.

## Output Format
- Return one integer: the minimum total inverter load.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
