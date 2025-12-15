## Title
Bank Heist Escape

## Slug
bank-heist-escape

## Difficulty
Medium

## Description
Robbers flee the vault. Escape routes are blocked by police immediately after use.

The city map consists of $n$ intersections and $m$ one-way streets. Each street connects a specific source intersection to a destination intersection.

The process happens over several cars. In each car, you must send a getaway car from intersection 1 (the source) to intersection $n$ (the destination). The catch is that each street is barricaded by police after a car passes. This means each street can be used at most once across all cars combined.

Your goal is to determine the maximum number of cars you can successfully complete the journey from intersection 1 to intersection $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 cars.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 car.

## Input Format
- The first line contains two integers $n$ and $m$: the number of intersections and the number of streets.
- The next $m$ lines describe the streets. Each line contains two integers $a$ and $b$, indicating a directed street from intersection $a$ to intersection $b$.

## Output Format
- Return one integer: the maximum number of cars possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
