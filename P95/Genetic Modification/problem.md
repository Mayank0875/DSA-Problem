## Title
Genetic Modification

## Slug
genetic-modification

## Difficulty
Hard

## Description
A geneticist splices gene sequences. Genes are grouped into strands, and the dominant trait of a strand is the most frequent gene ID within it.

Dr. Mendel has a collection of $n$ genes, where each gene is represented by an integer ID.

To create a new organism, Dr. Mendel must partition these genes into several non-empty strands. Every gene from the original collection must belong to exactly one strand. From each strand, a "dominant trait" is extracted. The dominant trait is defined as the **mode** (most frequent element) of the genes in that strand. If a strand has multiple genes tied for the most frequent appearance, any one of them can be chosen as the dominant trait.

Dr. Mendel collects all the extracted dominant traits to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> dominant trait is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> dominant traits 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> dominant traits 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> dominant traits 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of genes.
- The second line contains $n$ space-separated integers representing the gene IDs.

## Output Format
- Return a single integer representing the number of different multisets of dominant traits possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
