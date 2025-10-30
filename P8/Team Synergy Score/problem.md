## Title

Team Synergy Score

## Slug

team-synergy-score

## Difficulty

Medium

## Description

A team for a programming contest has N members. Each member `i` has a "skill rating" `A[i]`. The "team synergy" is calculated as the greatest common divisor (GCD) of all members' skill ratings. The coach can swap out exactly one member of the team for a new "prospect" player. This prospect can have any skill rating from 1 to 10⁹. What is the maximum possible team synergy score the coach can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the coach replaces the member with rating 7 with a prospect rated 4, the team's ratings become [4, 6, 8]. The GCD is 2, which is the maximum.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The coach can "swap" a player with a prospect who has the exact same rating.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math