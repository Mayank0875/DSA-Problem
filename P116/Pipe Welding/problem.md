## Title
Pipe Welding

## Slug
pipe-welding

## Difficulty
Medium

## Description
A plumber connects pipes. Each pipe segment has a diameter at the male end and female end.

The truck has list of pipes, each defined by a male dia and an female dia, represented as a pair `[male, female]`.

To fit inside, the female diameter of the first pipe must be strictly less than the male diameter of the next pipe (telescoping fit). Specifically, to transition from pipe `[a, b]` to a subsequent pipe `[c, d]`, the female of the first pipe must be **strictly less than** the male of the second pipe (i.e., `b < c`).

You can select pipes in any order you like to form a valid pipeline. Your goal is to determine the maximum number of pipes that can be included in a single pipeline.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest pipeline is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The pipes can be reordered to form the pipeline `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available pipes.
- The next `n` lines each contain two integers, representing the `male` and `female` of an pipe.

## Output Format
- Return a single integer representing the maximum length of the pipeline.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ male < female ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
