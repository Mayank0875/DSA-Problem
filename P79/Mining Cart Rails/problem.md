## Title
Mining Cart Rails

## Slug
mining-cart-rails

## Difficulty
Medium

## Description
Carts carry ore. Old wooden rails splinter and break under a heavy load.

The mine consists of $n$ junctions and $m$ one-way rails. Each rail connects a specific source junction to a destination junction.

The process happens over several carts. In each cart, you must send a cart from junction 1 (the source) to junction $n$ (the destination). The catch is that each rail splinters and breaks after a cart passes. This means each rail can be used at most once across all carts combined.

Your goal is to determine the maximum number of carts you can successfully complete the journey from junction 1 to junction $n$.

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
You can complete 2 carts.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 cart.

## Input Format
- The first line contains two integers $n$ and $m$: the number of junctions and the number of rails.
- The next $m$ lines describe the rails. Each line contains two integers $a$ and $b$, indicating a directed rail from junction $a$ to junction $b$.

## Output Format
- Return one integer: the maximum number of carts possible.

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
