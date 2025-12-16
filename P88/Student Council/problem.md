## Title
Student Council

## Slug
student-council

## Difficulty
Medium

## Description
Classes have different numbers of students. A proposal passes if classes supporting it contain a majority of the student body.

Your task is to count the number of **voting blockss**. A voting block is considered valid if it satisfies two specific criteria:
1.  **Proposal Pass:** The total student count of the voting block is strictly greater than half of the total student count across all classes.
2.  **No Superfluous classes:** The voting block is minimal. This means that removing **any one** class from the voting block would cause the remaining total to drop to half or less of the total student count (losing the Proposal Pass).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total student count is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total student count = 10. Half = 5.
Valid voting blockss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of classes.
- The second line contains n integers: the student count of each class.

## Output Format
- Return one integer: the total number of valid voting blockss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ student count ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
