## Title
Computer Chip Layout

## Slug
computer-chip-layout

## Difficulty
Hard

## Description
A designer places transistors on a chip.

The Designer is designing a logic gate composed of $n$ transistors.

Each transistor must have a **positive integer** clock speed, and the total clock speed across all transistors must be exactly $k$.

However, placing transistors with overlapping binary signatures next to each other causes signal noise. The signal noise between two adjacent transistors with clock speeds $x$ and $y$ is defined as:
$$ x \ \& \ y \ (\text{bitwise AND}) $$

The total signal noise of the system is the sum of the signal noises between all adjacent pairs in the array:
$$ \text{Total Cost} = \sum_{i=2}^{n} (a_i \ \& \ a_{i-1}) $$

Your task is to determine the **minimum** possible signal noise that can be achieved by choosing appropriate clock speeds for the array of size $n$ such that the sum of all elements is exactly $k$.

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
