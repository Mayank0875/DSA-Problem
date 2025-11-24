## Title
Alien Species Count

## Slug
alien-species-count

## Difficulty
Medium

## Description
A xenobiologist tracks populations of alien species. A rare phenomenon only affects species with an even population count. As births and deaths occur, modifying the counts, report the total number of individuals belonging to the affected species.

## Examples

### 1

#### Input
4
1 2 3 4
4
1 0
-3 1
-4 0
2 3

#### Output
8 6 2 4

#### Explanation
Initially, the array is `[1, 2, 3, 4]`.
1. Add 1 to index 0: Array becomes `[2, 2, 3, 4]`. Sum of evens: 2 + 2 + 4 = 8.
2. Add -3 to index 1: Array becomes `[2, -1, 3, 4]`. Sum of evens: 2 + 4 = 6.
3. Add -4 to index 0: Array becomes `[-2, -1, 3, 4]`. Sum of evens: -2 + 4 = 2.
4. Add 2 to index 3: Array becomes `[-2, -1, 3, 6]`. Sum of evens: -2 + 6 = 4.

### 2

#### Input
1
1
1
4 0

#### Output
0

#### Explanation
Initially, the array is `[1]`.
1. Add 4 to index 0: Array becomes `[5]`. Sum of evens: 0.

## Input Format
- The first line contains an integer n, the number of elements.
- The second line contains n space-separated integers representing the initial state.
- The third line contains an integer q, the number of updates.
- The next q lines each contain two space-separated integers representing the `val` (amount to add) and `index` for each update.

## Output Format
- Return an array of size q representing the sum of even values after each update.

## Constraints
- 1 ≤ n ≤ 10^4
- -10^4 ≤ arr[i] ≤ 10^4
- 1 ≤ q ≤ 10^4
- -10^4 ≤ val ≤ 10^4
- 0 ≤ index < n

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array
