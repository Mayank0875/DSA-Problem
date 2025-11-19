## Title
Inventory Pallet Block

## Slug
inventory-pallet-block

## Difficulty
Easy

## Description
A forklift driver is organizing pallets into a square block on the loading dock. You are given the total number of pallets to be shipped. Calculate the maximum number of pallets that can make up one side of this square block.

## Examples

### 1

#### Input
10

#### Output
3

#### Explanation
3² = 9 ≤ 10, 4² = 16 > 10

### 2

#### Input
25

#### Output
5

#### Explanation
5² = 25 ≤ 25, 6² = 36 > 25

## Input Format
- A single integer x — the total number of pallets available.

## Output Format
- Return single integer — the maximum possible side length r of the square block that can be built using those pallets.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
