## Title
Server Rack Floor Plan

## Slug
server-rack-floor-plan

## Difficulty
Easy

## Description
A data center engineer is planning the layout of server racks in a new room. The cooling system works best if the racks are arranged in a perfect square. Given the total number of server racks available for installation, find the maximum width (in racks) of this square arrangement.

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
- A single integer x — the total number of server racks available.

## Output Format
- Return single integer — the maximum possible side length r of the square layout that can be built using those server racks.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
