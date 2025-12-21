## Title
Movie Frame Sequence

## Slug
movie-frame-sequence

## Difficulty
Hard

## Description
An editor assembles frames for a scene.

The Editor is designing a film strip composed of $n$ frames.

Each frame must have a **positive integer** brightness, and the total brightness across all frames must be exactly $k$.

However, placing frames with overlapping binary signatures next to each other causes visual flicker. The visual flicker between two adjacent frames with brightnesss $x$ and $y$ is defined as:
$$ x \ \& \ y \ (\text{bitwise AND}) $$

The total visual flicker of the system is the sum of the visual flickers between all adjacent pairs in the array:
$$ \text{Total Cost} = \sum_{i=2}^{n} (a_i \ \& \ a_{i-1}) $$

Your task is to determine the **minimum** possible visual flicker that can be achieved by choosing appropriate brightnesss for the array of size $n$ such that the sum of all elements is exactly $k$.

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
