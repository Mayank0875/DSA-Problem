## Title
Archive Storage

## Slug
archive-storage

## Difficulty
Medium

## Description
An archivist puts documents into folders.

The archivist has prepared $n$ documents arranged in a sequence. The $i$-th document has a value of $a_i$.

These documents need to be grouped into folders. Every folder must hold the exact same number of documents, denoted by $k$. The grouping happens sequentially:
- The first $k$ documents go into the first folder.
- The second $k$ documents go into the second folder.
- ...
- The last $k$ documents go into the $(n/k)$-th folder.

Since every folder must have exactly $k$ documents, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The archivist wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the folders is maximized. If there is only one folder (i.e., $k=n$), the difference is 0.

Your task is to calculate this maximum possible difference over all valid choices of $k$.

## Examples

### 1

#### Input
2
1 2

#### Output
1

#### Explanation
Possible values for $k$ are divisors of 2: 1, 2.
- $k=1$: folder 1 has sum 1, folder 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one folder with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All documents are equal. Regardless of $k$, all folders will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of documents.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the documents.

## Output Format
- Return a single integer — the maximum absolute difference.

## Constraints
- 1 ≤ n ≤ 1.5 * 10^5
- 1 ≤ a[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, math, number-theory


