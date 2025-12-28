## Title
Tech Scrap Salvage

## Slug
tech-scrap-salvage

## Difficulty
Medium

## Description
Old tech is scavenged. The Military takes advanced chips, the Research Lab (you) takes functional parts, and the Junkyard gets the rust.

There are $3n$ components of varying utility available. The distribution follows a strict protocol. In each round, you must select any 3 components. The parties then claim them based on the following rules:

1. The **Military** takes the component with the **maximum** utility from the triplet.
2. You, the **Lab**, take the component with the **second maximum** utility.
3. The **Junkyard** takes the remaining component (the one with the minimum utility).

This process repeats until all components are distributed. Your goal as the Lab is to maximize the total utility of the components you acquire.

Given an array of integers `components`, where `components[i]` represents the utility of the $i$-th component, return the maximum total utility you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 components. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Military takes `8`, you take `7`, Junkyard takes `2`.
2. Pick the remaining `(1, 2, 4)`. Military takes `4`, you take `2`, Junkyard takes `1`.
Total utility = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Military takes `5`, you take `4`, Junkyard takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of components.
- The second line contains $3n$ space-separated integers representing the `components` array.

## Output Format
- Return a single integer representing the maximum total utility you can collect.

## Constraints
- 1 ≤ components.length ≤ 10^5
- `components.length` is divisible by 3.
- 1 ≤ components[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
