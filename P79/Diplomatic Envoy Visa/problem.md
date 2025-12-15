## Title
Diplomatic Envoy Visa

## Slug
diplomatic-envoy-visa

## Difficulty
Medium

## Description
Envoys travel through countries. Single-entry visas allow only one trip per border.

The continent consists of $n$ capitals and $m$ one-way borders. Each border connects a specific source capital to a destination capital.

The process happens over several envoys. In each envoy, you must send a envoy from capital 1 (the source) to capital $n$ (the destination). The catch is that each border requires a single-entry visa that becomes void. This means each border can be used at most once across all envoys combined.

Your goal is to determine the maximum number of envoys you can successfully complete the journey from capital 1 to capital $n$.

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
You can complete 2 envoys.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 envoy.

## Input Format
- The first line contains two integers $n$ and $m$: the number of capitals and the number of borders.
- The next $m$ lines describe the borders. Each line contains two integers $a$ and $b$, indicating a directed border from capital $a$ to capital $b$.

## Output Format
- Return one integer: the maximum number of envoys possible.

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
