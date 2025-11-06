## Title

Adventurer's Treasure Hunt

## Slug

adventurers-treasure-hunt

## Difficulty

Medium

## Description

A group of adventurers has found `n` ancient artifacts, and each artifact has a specific gold value. Your team needs to pay a dragon a tribute of `sum` gold. You must determine if it is possible to select a group (a subset) of these artifacts whose values add up exactly to `sum`. You can only use each artifact once. Return true if a subset with the given sum exists. Otherwise false
## Examples

### 1

#### Input

6 9
[3, 34, 4, 12, 5, 2]

#### Output

Yes

#### Explanation

You can select the artifacts with values 4, 3, and 2. Their total value is 4 + 3 + 2 = 9.
    
### 2

#### Input

6 30
[3, 34, 4, 12, 5, 2]

#### Output

No

#### Explanation
No combination of these artifacts adds up to exactly 30.

## Input Format  

- The first line contains two integers, `n` and `sum`, separated by a space. `n` is the number of artifacts, and `sum` is the target value.
- The second line contains `n` space-separated integers, representing the gold values of the artifacts in `arr`.

## Output Format  

- Return `true` if a subset with the given `sum` exists. Otherwise `false`.
  

## Constraints  

- 1 ≤ n ≤ 20
- 1 ≤ sum ≤ 1e9
- 1 ≤ arr[i] ≤ 20

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion