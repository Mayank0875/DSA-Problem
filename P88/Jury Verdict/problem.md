## Title
Jury Verdict

## Slug
jury-verdict

## Difficulty
Medium

## Description
In a weighted jury system, jurors have different 'credibility scores'. A verdict is reached only if the supporting jurors represent a strict majority of the total credibility score.

Your task is to count the number of **verdict groupss**. A verdict group is considered valid if it satisfies two specific criteria:
1.  **Guilty Verdict:** The total credibility of the verdict group is strictly greater than half of the total credibility across all jurors.
2.  **No Superfluous jurors:** The verdict group is minimal. This means that removing **any one** juror from the verdict group would cause the remaining total to drop to half or less of the total credibility (losing the Guilty Verdict).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total credibility is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total credibility = 10. Half = 5.
Valid verdict groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of jurors.
- The second line contains n integers: the credibility of each juror.

## Output Format
- Return one integer: the total number of valid verdict groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ credibility ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
