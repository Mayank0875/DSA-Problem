## Title
Satellite Orbit

## Slug
satellite-orbit

## Difficulty
Medium

## Description
Satellites occupy orbital slots 1, 2, 3... Debris (negative) occupies some orbits. Launch control needs the lowest clear slot for a new satellite.

You are given an unsorted integer array `ids` representing the Slot Numbers currently in the system. Some Slot Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Slot Number that is **missing** from the list. This will be the target slot.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Slot Numbers 1 and 2 are present. The smallest missing positive Slot Number is 3.

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
- Return a single integer representing the smallest missing positive Slot Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

