## Title
Treasure Chest Keys

## Slug
treasure-chest-keys

## Difficulty
Medium

## Description
Keys have different magic values. To open the chest, a combination of keys must be inserted whose magic sum exceeds half the total magic of all existing keys.

Your task is to count the number of **keyringss**. A keyring is considered valid if it satisfies two specific criteria:
1.  **Unlock Threshold:** The total magic value of the keyring is strictly greater than half of the total magic value across all keys.
2.  **No Superfluous keys:** The keyring is minimal. This means that removing **any one** key from the keyring would cause the remaining total to drop to half or less of the total magic value (losing the Unlock Threshold).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total magic value is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total magic value = 10. Half = 5.
Valid keyringss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of keys.
- The second line contains n integers: the magic value of each key.

## Output Format
- Return one integer: the total number of valid keyringss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ magic value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
