## Title
Hiking Trail Erosion

## Slug
hiking-trail-erosion

## Difficulty
Medium

## Description
Hikers race to the summit. Trails are crumbling and disappear after one person walks them.

The mountain consists of $n$ camps and $m$ one-way trails. Each trail connects a specific source camp to a destination camp.

The process happens over several hikers. In each hiker, you must send a hiker from camp 1 (the source) to camp $n$ (the destination). The catch is that each trail crumbles away due to erosion after use. This means each trail can be used at most once across all hikers combined.

Your goal is to determine the maximum number of hikers you can successfully complete the journey from camp 1 to camp $n$.

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
You can complete 2 hikers.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 hiker.

## Input Format
- The first line contains two integers $n$ and $m$: the number of camps and the number of trails.
- The next $m$ lines describe the trails. Each line contains two integers $a$ and $b$, indicating a directed trail from camp $a$ to camp $b$.

## Output Format
- Return one integer: the maximum number of hikers possible.

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
