## Title
Mining Cart Train

## Slug
mining-cart-train

## Difficulty
Hard

## Description
Miners load ore into a train of carts.

The Foreman is designing a cart train composed of $n$ carts.

Each cart must have a **positive integer** ore weight, and the total ore weight across all carts must be exactly $k$.

However, placing carts with overlapping binary signatures next to each other causes friction heat. The friction heat between two adjacent carts with ore weights $x$ and $y$ is defined as:
$$ x \ \& \ y \ (\text{bitwise AND}) $$

The total friction heat of the system is the sum of the friction heats between all adjacent pairs in the array:
$$ \text{Total Cost} = \sum_{i=2}^{n} (a_i \ \& \ a_{i-1}) $$

Your task is to determine the **minimum** possible friction heat that can be achieved by choosing appropriate ore weights for the array of size $n$ such that the sum of all elements is exactly $k$.

## Examples

### 1

#### Input
2 4

#### Output
1

#### Explanation
For $n = 2$ and $k = 4$, possible arrays are $[1, 3]$ (cost $1 \& 3 = 1$) and $[2, 2]$ (cost $2 \& 2 = 2$). The minimum cost is 1.

### 2

#### Input
2 5

#### Output
0

#### Explanation
We can choose array $[4, 1]$. Sum is $4+1=5$. Cost is $4 \ \& \ 1 = 0$.

## Input Format
- The only input line has two space-separated integers $n$ and $k$.

## Output Format
- Return one integer: representing the minimum cost.

## Constraints
- 1 ≤ n ≤ 10^6
- n ≤ k ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, greedy
