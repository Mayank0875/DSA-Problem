## Title
Film Editing Scenes

## Slug
film-editing-scenes

## Difficulty
Hard

## Description
A movie has `n` raw clips. The director groups them into `k` scenes. Clips must remain chronological. The 'emotional intensity' variance of a scene is modeled as the square of the total duration of clips in it.

You must partition the sequence of clips into exactly `k` non-empty contiguous scenes.
Each scene corresponds to a scene.
The "intensity variance" for a scene is calculated as the **square of the sum** of the durations of the clips in that scene.

Your goal is to minimize the total intensity variance (the sum of the intensity variance values of all `k` scenes).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the clips into 3 scenes: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total intensity variance is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 scene is allowed, containing all clips. Sum = 15. intensity variance = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of clips and the required number of scenes.
- The second line contains `n` integers representing the durations of each clip.

## Output Format
- Return one integer: the minimum total intensity variance.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
