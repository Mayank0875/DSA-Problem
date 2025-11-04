## Title

Perfect Sandwich

## Slug

perfect-sandwich

## Difficulty

Medium

## Description

You are making a sandwich and have `n` possible ingredients. Each ingredient has a "flavor score." For the "perfect sandwich," the total flavor score must be *exactly* `sum`. You must determine if it's possible to choose a combination (a subset) of your `n` ingredients to reach this exact flavor score. You can only use each ingredient once.
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