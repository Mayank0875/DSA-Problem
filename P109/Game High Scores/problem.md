## Title
Game High Scores

## Slug
game-high-scores

## Difficulty
Easy

## Description
A leaderboard updates. It checks if a Player ID is already present before inserting a new score entry.

Your task is to determine if any player ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The player ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All player IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of scores.
- The second line contains n space-separated integers, representing the player IDs.

## Output Format
- Return `Yes` if any player ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
