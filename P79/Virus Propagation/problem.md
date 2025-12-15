## Title
Virus Propagation

## Slug
virus-propagation

## Difficulty
Medium

## Description
A biological virus spreads. Transmission vectors are blocked by immunity after one infection event.

The population consists of $n$ hosts and $m$ one-way vectors. Each vector connects a specific source host to a destination host.

The process happens over several waves. In each wave, you must send a infection from host 1 (the source) to host $n$ (the destination). The catch is that each vector triggers immunity and cannot be used again. This means each vector can be used at most once across all waves combined.

Your goal is to determine the maximum number of waves you can successfully complete the journey from host 1 to host $n$.

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
You can complete 2 waves.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 wave.

## Input Format
- The first line contains two integers $n$ and $m$: the number of hosts and the number of vectors.
- The next $m$ lines describe the vectors. Each line contains two integers $a$ and $b$, indicating a directed vector from host $a$ to host $b$.

## Output Format
- Return one integer: the maximum number of waves possible.

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
