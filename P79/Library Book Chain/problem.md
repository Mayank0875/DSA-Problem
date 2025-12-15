## Title
Library Book Chain

## Slug
library-book-chain

## Difficulty
Medium

## Description
Books are passed between readers. Fragile bindings fall apart after one reading.

The club consists of $n$ readers and $m$ one-way loans. Each loan connects a specific source reader to a destination reader.

The process happens over several readings. In each reading, you must send a book from reader 1 (the source) to reader $n$ (the destination). The catch is that each loan causes the binding to fall apart. This means each loan can be used at most once across all readings combined.

Your goal is to determine the maximum number of readings you can successfully complete the journey from reader 1 to reader $n$.

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
You can complete 2 readings.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 reading.

## Input Format
- The first line contains two integers $n$ and $m$: the number of readers and the number of loans.
- The next $m$ lines describe the loans. Each line contains two integers $a$ and $b$, indicating a directed loan from reader $a$ to reader $b$.

## Output Format
- Return one integer: the maximum number of readings possible.

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
