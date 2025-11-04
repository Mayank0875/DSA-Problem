## Title

Museum Exhibit Weight

## Slug

museum-exhibit-weight

## Difficulty

Medium

## Description

A museum curator is setting up a new exhibit on an antique display stand. The stand is very sensitive and will only activate if the items placed on it have a combined weight of *exactly* `sum`. The curator has `n` items to choose from. Can they select a subset of these items that perfectly matches the required weight?
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