## Title
Video Game Combo

## Slug
video-game-combo

## Difficulty
Easy

## Description
A gamer is analyzing their combat logs. A 'Combo' is formed by landing hits where each hit deals strictly more damage than the previous one.

The Gamer is analyzing a sequence of hits represented by an array of integers `nums`, where `nums[i]` represents the damage point at index `i`.

The Gamer wants to find the maximum total damage point obtained during a single "**Combo Chain**". A "Combo Chain" is defined as a contiguous subarray of hits where the damage point of each hit is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of damage points possible from one such Combo Chain. The Combo Chain must include at least one hit.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Gamer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Combo Chain starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of hits.
- The second line contains `n` space-separated integers, representing the damage points.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
