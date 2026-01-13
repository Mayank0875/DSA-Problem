## Title
Gap in the Wall

## Slug
gap-in-the-wall

## Difficulty
Medium

## Description
Bricks in a wall are numbered sequentially. Some bricks have fallen out. A mason needs to replace the first missing brick (lowest number).

You are given an unsorted integer array `ids` representing the Brick Numbers currently in the system. Some Brick Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Brick Number that is **missing** from the list. This will be the number of the brick to replace first.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Brick Numbers 1 and 2 are present. The smallest missing positive Brick Number is 3.

### 2

#### Input
4
3 4 -1 1

#### Output
2

#### Explanation
1 is present, but 2 is missing.

## Input Format
- The first line contains an integer $n$, the size of the array.
- The second line contains $n$ space-separated integers `ids`.

## Output Format
- Return a single integer representing the smallest missing positive Brick Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

