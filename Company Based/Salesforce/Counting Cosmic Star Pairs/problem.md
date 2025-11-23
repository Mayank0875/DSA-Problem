## Title

The Curator's Artifact Collection

## Slug

the-curators-artifact-collection

## Difficulty

Medium

## Description

The Royal Museum is preparing for a grand exhibition. The head curator has brought out a vast collection of ancient artifacts from the archives. Each artifact is identified by a specific integer ID.

However, the display cases have limited space. To ensure the exhibit is not too cluttered, the curator must remove exactly $k$ artifacts from the collection. The goal is to make the exhibit as thematic and focused as possible by **minimizing the number of unique artifact types** remaining on display.

You are given an integer array `artifacts` representing the IDs of the available items and an integer $k$. Your task is to determine the least number of unique artifact IDs left after removing exactly $k$ items.

## Examples

### 1

#### Input

3 1
5 5 4

#### Output

1

#### Explanation

Remove the single artifact with ID 4. The remaining artifacts are [5, 5]. The only unique ID left is 5. The count of unique types is 1.

### 2

#### Input

7 3
4 3 1 1 3 3 2


#### Output

2

#### Explanation

The remaining artifacts are [1, 3, 3, 3]. The unique IDs left are 1 and 3. The answer is 2.

## Input Format

- The first line contains an integer $n$ and $k$, the number of artifacts.
- The second line contains $n$ space-separated integers representing the `artifacts` array.


## Output Format

- Return a single integer representing the least number of unique artifact types remaining.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ k ≤ 10^9
- 0 ≤ artifacts[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hash-table, greedy
