## Title
Software Patching

## Slug
software-patching

## Difficulty
Medium

## Description
Exploits move through a system. Vulnerabilities are patched immediately after detection.

The software consists of $n$ modules and $m$ one-way exploits. Each exploit connects a specific source module to a destination module.

The process happens over several attacks. In each attack, you must send a attack from module 1 (the source) to module $n$ (the destination). The catch is that each exploit is patched by security software. This means each exploit can be used at most once across all attacks combined.

Your goal is to determine the maximum number of attacks you can successfully complete the journey from module 1 to module $n$.

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
You can complete 2 attacks.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 attack.

## Input Format
- The first line contains two integers $n$ and $m$: the number of modules and the number of exploits.
- The next $m$ lines describe the exploits. Each line contains two integers $a$ and $b$, indicating a directed exploit from module $a$ to module $b$.

## Output Format
- Return one integer: the maximum number of attacks possible.

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
