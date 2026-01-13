## Title

Weak Characters Count

## Slug

weak-characters-count

## Difficulty

Medium

## Description

You are playing a game that contains $n$ characters. Each character has two main properties: **attack** and **defense**. You are given a 2D integer array `properties` where `properties[i] = [attack_i, defense_i]` represents the properties of the $i$-th character.

A character is considered **weak** if there exists another character who has **both** strictly greater attack and strictly greater defense.

More formally, a character $i$ is weak if there exists another character $j$ such that `attack_j > attack_i` and `defense_j > defense_i`.

Your task is to return the number of weak characters in the game.

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

No character has strictly greater attack and defense than another.

### 2

#### Input

2
2 2
3 3

#### Output

1

#### Explanation

The first character (2, 2) is weak because the second character (3, 3) has strictly greater attack and defense.
  

## Input Format  

- The first line contains an integer $n$, the number of characters.
- The next $n$ lines each contain two space-separated integers, representing the attack and defense of a character.

## Output Format  

- Return a single integer representing the number of weak characters.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 <= attack[i], defense[i] <= 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, greedy
