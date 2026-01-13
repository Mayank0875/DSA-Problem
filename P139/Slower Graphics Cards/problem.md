## Title
Slower Graphics Cards

## Slug
slower-graphics-cards

## Difficulty
Medium

## Description
A gamer compares GPUs.

You have a list of $n$ GPUs. Each GPU has two main properties: **VRAM** and **clock speed**. You are given a 2D integer array `properties` where `properties[i] = [VRAM_i, clock speed_i]` represents the attributes of the $i$-th GPU.

A GPU is considered **slower** if there exists another GPU that has **both** strictly greater VRAM and strictly greater clock speed.

More formally, the $i$-th GPU is slower if there exists an index $j$ such that `VRAM_j > VRAM_i` and `clock speed_j > clock speed_i`.

Your task is to return the number of slower GPUs.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No GPU has strictly greater VRAM and clock speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first GPU (2, 2) is slower because the second GPU (3, 3) has strictly greater VRAM and clock speed.

## Input Format
- The first line contains an integer $n$, the number of GPUs.
- The next $n$ lines each contain two space-separated integers, representing the VRAM and clock speed of a GPU.

## Output Format
- Return a single integer representing the number of slower GPUs.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ VRAM, clock speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
