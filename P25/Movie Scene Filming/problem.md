## Title

Movie Scene Filming

## Slug

movie-scene-filming

## Difficulty

Medium

## Description

A movie director has `n` scenes to film, which must be shot in order. Each scene `i` has an estimated filming time of `x[i]` hours. The director has `k` film crews. Each crew must be assigned a contiguous block of scenes (e.g., Crew 1 films scenes 1-4, Crew 2 films 5-6, etc.). To make the schedule efficient, the director wants to minimize the maximum number of hours any single crew works. Find this minimum time.

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of scenes and the number of crews.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the time for the i-th scene.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy