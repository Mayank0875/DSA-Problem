## Title
Laser Tag Mirrors

## Slug
laser-tag-mirrors

## Difficulty
Medium

## Description
Beams bounce to the target. Fragile mirrors shatter when hit by a high-power beam.

The arena consists of $n$ turrets and $m$ one-way lines of sight. Each line of sight connects a specific source turret to a destination turret.

The process happens over several shots. In each shot, you must send a beam from turret 1 (the source) to turret $n$ (the destination). The catch is that each line of sight shatters the reflecting mirror. This means each line of sight can be used at most once across all shots combined.

Your goal is to determine the maximum number of shots you can successfully complete the journey from turret 1 to turret $n$.

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
You can complete 2 shots.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 shot.

## Input Format
- The first line contains two integers $n$ and $m$: the number of turrets and the number of lines of sight.
- The next $m$ lines describe the lines of sight. Each line contains two integers $a$ and $b$, indicating a directed line of sight from turret $a$ to turret $b$.

## Output Format
- Return one integer: the maximum number of shots possible.

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
