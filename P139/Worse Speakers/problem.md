## Title
Worse Speakers

## Slug
worse-speakers

## Difficulty
Medium

## Description
An audiophile rates speakers.

You have a list of $n$ speakers. Each speaker has two main properties: **max volume** and **clarity**. You are given a 2D integer array `properties` where `properties[i] = [max volume_i, clarity_i]` represents the attributes of the $i$-th speaker.

A speaker is considered **worse** if there exists another speaker that has **both** strictly greater max volume and strictly greater clarity.

More formally, the $i$-th speaker is worse if there exists an index $j$ such that `max volume_j > max volume_i` and `clarity_j > clarity_i`.

Your task is to return the number of worse speakers.

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
No speaker has strictly greater max volume and clarity than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first speaker (2, 2) is worse because the second speaker (3, 3) has strictly greater max volume and clarity.

## Input Format
- The first line contains an integer $n$, the number of speakers.
- The next $n$ lines each contain two space-separated integers, representing the max volume and clarity of a speaker.

## Output Format
- Return a single integer representing the number of worse speakers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ max volume, clarity ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
